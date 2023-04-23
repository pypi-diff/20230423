# Comparing `tmp/XMLCit-0.0.7.tar.gz` & `tmp/XMLCit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XMLCit-0.0.7.tar", last modified: Fri Apr 21 20:47:34 2023, max compression
+gzip compressed data, was "XMLCit-0.0.8.tar", last modified: Sun Apr 23 18:24:40 2023, max compression
```

## Comparing `XMLCit-0.0.7.tar` & `XMLCit-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 20:47:34.155805 XMLCit-0.0.7/
--rw-rw-rw-   0        0        0     1086 2023-04-20 02:25:43.000000 XMLCit-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2498 2023-04-21 20:47:34.155805 XMLCit-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1901 2023-04-21 20:46:21.000000 XMLCit-0.0.7/README.md
--rw-rw-rw-   0        0        0       88 2023-04-21 20:44:49.000000 XMLCit-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      743 2023-04-21 20:47:34.155805 XMLCit-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 20:47:34.120909 XMLCit-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 20:47:34.129357 XMLCit-0.0.7/src/XMLCit/
--rw-rw-rw-   0        0        0        0 2023-04-20 03:24:00.000000 XMLCit-0.0.7/src/XMLCit/__init__.py
--rw-rw-rw-   0        0        0    15638 2023-04-21 20:46:24.000000 XMLCit-0.0.7/src/XMLCit/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:47:34.155805 XMLCit-0.0.7/src/XMLCit.egg-info/
--rw-rw-rw-   0        0        0     2498 2023-04-21 20:47:34.000000 XMLCit-0.0.7/src/XMLCit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-04-21 20:47:34.000000 XMLCit-0.0.7/src/XMLCit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 20:47:34.000000 XMLCit-0.0.7/src/XMLCit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 20:47:34.000000 XMLCit-0.0.7/src/XMLCit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 18:24:40.530737 XMLCit-0.0.8/
+-rw-rw-rw-   0        0        0     1086 2023-04-20 02:25:43.000000 XMLCit-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4453 2023-04-23 18:24:40.530737 XMLCit-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3854 2023-04-23 18:22:55.000000 XMLCit-0.0.8/README.md
+-rw-rw-rw-   0        0        0       88 2023-04-21 20:44:49.000000 XMLCit-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      743 2023-04-23 18:24:40.537824 XMLCit-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-23 18:24:40.503575 XMLCit-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-23 18:24:40.511571 XMLCit-0.0.8/src/XMLCit/
+-rw-rw-rw-   0        0        0        0 2023-04-20 03:24:00.000000 XMLCit-0.0.8/src/XMLCit/__init__.py
+-rw-rw-rw-   0        0        0    15638 2023-04-21 20:46:24.000000 XMLCit-0.0.8/src/XMLCit/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:24:40.529756 XMLCit-0.0.8/src/XMLCit.egg-info/
+-rw-rw-rw-   0        0        0     4453 2023-04-23 18:24:40.000000 XMLCit-0.0.8/src/XMLCit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-04-23 18:24:40.000000 XMLCit-0.0.8/src/XMLCit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 18:24:40.000000 XMLCit-0.0.8/src/XMLCit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-23 18:24:40.000000 XMLCit-0.0.8/src/XMLCit.egg-info/top_level.txt
```

### Comparing `XMLCit-0.0.7/LICENSE` & `XMLCit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `XMLCit-0.0.7/PKG-INFO` & `XMLCit-0.0.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,73 @@
-Metadata-Version: 2.1
-Name: XMLCit
-Version: 0.0.7
-Summary: This package was made to edit XML files ( particularly TEI-XML files). The main purpose is to facilitate the tagging and edit of repeated citations and the inclusion of VIAF records
-Home-page: https://github.com/hernandezj1/XMLCit
-Author: Jose Hernandez
-Author-email: jose.hndz.prz@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # XMLCit package
 
 ## Purpose
  
-  This packages was developed by staff of the Research Computing Center to serve the needs of our digital humanities community. Therefore the classes and functions in this package were develop with ease of use and to be applicable to TEI-XML standards. TEI-XML specifications can be found here <a href='https://tei-c.org/'>TEI</a>
+  This packages was developed by staff of the Research Computing Center at Florida State University to serve the needs of our digital humanities community. Therefore the methods and functions in this package were developed with ease of use in mind and to be specifically applicable to TEI-XML standards. TEI-XML specifications can be found here <a href='https://tei-c.org/'>TEI</a>
+
+  The functions and methods here encompassed modify XMl documents on a large scale to avoid tedious work by the researcher. The main goald of this package was to provide a way to do the following: 
+
+  1. Tag a specific word within every instance of a specific node of the TEI-XMl document. In our case this was specific citations within the __note__ node.
+  
+  2. Add attributes to every instance of a specific node based on the presence of an ID number attribute or a specific collection of words inside said node. These attributes where:
+
+      a. A VIAF number, webscraped from the VIAF website
+
+      b. an ID number
+
+      c. A completed citation. 
+    
+
+  __Usage guidelines:__
+
+  To import the libary please use the next few lines in your code. It is key that for the methods inside the Insert class you define an instance of this class beforehand.
+
+    ```
+    from XMLCit import functions # After this all functions can be found by doing the following: 
+    functions.AddVIAF
+    functions.Addtag
+    functions.RepeatCitation
+
+    #To use the class methods do the following:
+    instance = functions.Insert()
+    #then you can use this instance to call each of the methods and not include the self parameter
+    instance.ID()
+    instance.CitbyID()
+    instance.CitbyText()
+
+    ```
+
+
+
 ## Structure
-  Due to the brevity of this package only a single module was made to hold one class( with 3 methoods) and 3 additional functions.
+  Due to the brevity of this package only a single module was made to hold one class( with 3 methods) and the 3 additional functions.
 ## Class description : Insert
 
-  This class focuses on the insertion of attributes into tags in the XML.
+  This class focuses on the Insertion of attributes into tags in the XML documents.
 
 ### Method descriptions
 
 1.  __ID__
-      inserts an 'ID' attribute inside the selected tag based on text inside XML tag
+  - Inserts an 'ID' attribute inside the selected tag based on text inside XML tag. 
 
 2.  __CitbyID__
-  - inserts a text( in this case meant to be a full citation) in an attrribute by the ID attribute
+  - Inserts a text( in this case meant to be a full citation) in an attribute by checking for the specified ID number.
 
 3.  __CitbyText__
-- inserts a text( in this case meant to be a full citation) in an attrribute by seacrhing for matching text
+  - Inserts a text( in this case meant to be a full citation) in an attrribute by seacrhing for matching text inside the selected tag (node)
 
 ## Additional Functions descriptions
 
 4.  __AddVIAF__
-        This function identifies those nodes (citations) in which a repeated non-written out citation happens like Ibid. and op. cit. 
-        It will then transfer the closest fullcitation attribute from a node that has: the same ID number AND a FullCitation attribute. 
+      This function adds an attribute with the <a href='https://viaf.org/'>VIAF</a> (Virtual International Authority File) number of the cited text. To do this it searches the first 4 words of the citation in the VIAF database using the __selenium__ webdriver.
 
+      *Additional Requirements:*
+        This function will need a filepath argument to be filled in directing the fucntion to find a chromedriver executable file to run the __selenium__ webdriver. This version of the function only works with the Chrome web browser. Future updates shall expand to the Firefox webdriver.       
+
+      
 5.  __Addtag__
-        This function adds an attribute with the VIAF ( Virtual International Authority File) number  of the citation. To do this it searches the first 4 words of the citation in the VIAF database using the selenium webdriver.
-        
-        
+
+      This function adds a tag on a specified word inside an existing tag (node) in the XML. The Initial purpose of the function (and the one contained in defaults) is to tag a specific word with the __cit__ tag that is inside a specific tag  for further inclusion of attributes with other functions in this package.
+
 6. __RepeatCitation__
-        This function adds a tag on a specified word inside an existing tag (node) in the XML. The Initial purpose of the function ( and the one contained in defaults) is to tag repeated citation with the cit tag for further inclusion of attributes with other functions in package
+
+      This function identifies those nodes (in this case __cit__ tags) in which a repeated non-written out citation happens like Ibid. and op. cit. It will then transfer the closest Full Citation attribute from a node that has: the same ID number AND a completed FullCitation attribute. It can also be used to transfer the VIAF attributes as well by changing the FullCitation default
```

#### html2text {}

```diff
@@ -1,31 +1,47 @@
-Metadata-Version: 2.1 Name: XMLCit Version: 0.0.7 Summary: This package was
-made to edit XML files ( particularly TEI-XML files). The main purpose is to
-facilitate the tagging and edit of repeated citations and the inclusion of VIAF
-records Home-page: https://github.com/hernandezj1/XMLCit Author: Jose Hernandez
-Author-email: jose.hndz.prz@gmail.com Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE # XMLCit package ## Purpose This
-packages was developed by staff of the Research Computing Center to serve the
-needs of our digital humanities community. Therefore the classes and functions
-in this package were develop with ease of use and to be applicable to TEI-XML
-standards. TEI-XML specifications can be found here TEI ## Structure Due to the
-brevity of this package only a single module was made to hold one class( with 3
-methoods) and 3 additional functions. ## Class description : Insert This class
-focuses on the insertion of attributes into tags in the XML. ### Method
-descriptions 1. __ID__ inserts an 'ID' attribute inside the selected tag based
-on text inside XML tag 2. __CitbyID__ - inserts a text( in this case meant to
-be a full citation) in an attrribute by the ID attribute 3. __CitbyText__ -
-inserts a text( in this case meant to be a full citation) in an attrribute by
-seacrhing for matching text ## Additional Functions descriptions 4. __AddVIAF__
-This function identifies those nodes (citations) in which a repeated non-
-written out citation happens like Ibid. and op. cit. It will then transfer the
-closest fullcitation attribute from a node that has: the same ID number AND a
-FullCitation attribute. 5. __Addtag__ This function adds an attribute with the
-VIAF ( Virtual International Authority File) number of the citation. To do this
-it searches the first 4 words of the citation in the VIAF database using the
-selenium webdriver. 6. __RepeatCitation__ This function adds a tag on a
-specified word inside an existing tag (node) in the XML. The Initial purpose of
-the function ( and the one contained in defaults) is to tag repeated citation
-with the cit tag for further inclusion of attributes with other functions in
-package
+# XMLCit package ## Purpose This packages was developed by staff of the
+Research Computing Center at Florida State University to serve the needs of our
+digital humanities community. Therefore the methods and functions in this
+package were developed with ease of use in mind and to be specifically
+applicable to TEI-XML standards. TEI-XML specifications can be found here TEI
+The functions and methods here encompassed modify XMl documents on a large
+scale to avoid tedious work by the researcher. The main goald of this package
+was to provide a way to do the following: 1. Tag a specific word within every
+instance of a specific node of the TEI-XMl document. In our case this was
+specific citations within the __note__ node. 2. Add attributes to every
+instance of a specific node based on the presence of an ID number attribute or
+a specific collection of words inside said node. These attributes where: a. A
+VIAF number, webscraped from the VIAF website b. an ID number c. A completed
+citation. __Usage guidelines:__ To import the libary please use the next few
+lines in your code. It is key that for the methods inside the Insert class you
+define an instance of this class beforehand. ``` from XMLCit import functions #
+After this all functions can be found by doing the following: functions.AddVIAF
+functions.Addtag functions.RepeatCitation #To use the class methods do the
+following: instance = functions.Insert() #then you can use this instance to
+call each of the methods and not include the self parameter instance.ID()
+instance.CitbyID() instance.CitbyText() ``` ## Structure Due to the brevity of
+this package only a single module was made to hold one class( with 3 methods)
+and the 3 additional functions. ## Class description : Insert This class
+focuses on the Insertion of attributes into tags in the XML documents. ###
+Method descriptions 1. __ID__ - Inserts an 'ID' attribute inside the selected
+tag based on text inside XML tag. 2. __CitbyID__ - Inserts a text( in this case
+meant to be a full citation) in an attribute by checking for the specified ID
+number. 3. __CitbyText__ - Inserts a text( in this case meant to be a full
+citation) in an attrribute by seacrhing for matching text inside the selected
+tag (node) ## Additional Functions descriptions 4. __AddVIAF__ This function
+adds an attribute with the VIAF (Virtual International Authority File) number
+of the cited text. To do this it searches the first 4 words of the citation in
+the VIAF database using the __selenium__ webdriver. *Additional Requirements:
+* This function will need a filepath argument to be filled in directing the
+fucntion to find a chromedriver executable file to run the __selenium__
+webdriver. This version of the function only works with the Chrome web browser.
+Future updates shall expand to the Firefox webdriver. 5. __Addtag__ This
+function adds a tag on a specified word inside an existing tag (node) in the
+XML. The Initial purpose of the function (and the one contained in defaults) is
+to tag a specific word with the __cit__ tag that is inside a specific tag for
+further inclusion of attributes with other functions in this package. 6.
+__RepeatCitation__ This function identifies those nodes (in this case __cit__
+tags) in which a repeated non-written out citation happens like Ibid. and op.
+cit. It will then transfer the closest Full Citation attribute from a node that
+has: the same ID number AND a completed FullCitation attribute. It can also be
+used to transfer the VIAF attributes as well by changing the FullCitation
+default
```

### Comparing `XMLCit-0.0.7/setup.cfg` & `XMLCit-0.0.8/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2058 4d4c 4369 740d 0a76 6572 7369   = XMLCit..versi
-00000020: 6f6e 203d 2030 2e30 2e37 0d0a 6175 7468  on = 0.0.7..auth
+00000020: 6f6e 203d 2030 2e30 2e38 0d0a 6175 7468  on = 0.0.8..auth
 00000030: 6f72 203d 204a 6f73 6520 4865 726e 616e  or = Jose Hernan
 00000040: 6465 7a0d 0a61 7574 686f 725f 656d 6169  dez..author_emai
 00000050: 6c20 3d20 6a6f 7365 2e68 6e64 7a2e 7072  l = jose.hndz.pr
 00000060: 7a40 676d 6169 6c2e 636f 6d0d 0a64 6573  z@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2054 6869 7320  cription = This 
 00000080: 7061 636b 6167 6520 7761 7320 6d61 6465  package was made
 00000090: 2074 6f20 6564 6974 2058 4d4c 2066 696c   to edit XML fil
```

### Comparing `XMLCit-0.0.7/src/XMLCit/functions.py` & `XMLCit-0.0.8/src/XMLCit/functions.py`

 * *Files identical despite different names*

