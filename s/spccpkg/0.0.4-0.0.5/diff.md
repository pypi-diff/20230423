# Comparing `tmp/spccpkg-0.0.4.tar.gz` & `tmp/spccpkg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spccpkg-0.0.4.tar", last modified: Sun Apr 23 17:48:43 2023, max compression
+gzip compressed data, was "spccpkg-0.0.5.tar", last modified: Sun Apr 23 18:06:31 2023, max compression
```

## Comparing `spccpkg-0.0.4.tar` & `spccpkg-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 17:48:43.175546 spccpkg-0.0.4/
--rw-rw-rw-   0        0        0      451 2023-04-23 17:48:43.174546 spccpkg-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-23 17:48:43.175546 spccpkg-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      698 2023-04-23 17:48:15.000000 spccpkg-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 17:48:43.151545 spccpkg-0.0.4/spcc/
--rw-rw-rw-   0        0        0       29 2023-04-23 10:20:37.000000 spccpkg-0.0.4/spcc/__init__.py
--rw-rw-rw-   0        0        0    30490 2023-04-23 17:26:06.000000 spccpkg-0.0.4/spcc/code.py
-drwxrwxrwx   0        0        0        0 2023-04-23 17:48:43.172545 spccpkg-0.0.4/spccpkg.egg-info/
--rw-rw-rw-   0        0        0      451 2023-04-23 17:48:42.000000 spccpkg-0.0.4/spccpkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-23 17:48:43.000000 spccpkg-0.0.4/spccpkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 17:48:42.000000 spccpkg-0.0.4/spccpkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 17:48:42.000000 spccpkg-0.0.4/spccpkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 18:06:31.523142 spccpkg-0.0.5/
+-rw-rw-rw-   0        0        0      451 2023-04-23 18:06:31.522142 spccpkg-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-23 18:06:31.524156 spccpkg-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      698 2023-04-23 18:06:24.000000 spccpkg-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:06:31.505142 spccpkg-0.0.5/spcc/
+-rw-rw-rw-   0        0        0       29 2023-04-23 10:20:37.000000 spccpkg-0.0.5/spcc/__init__.py
+-rw-rw-rw-   0        0        0    30418 2023-04-23 17:57:30.000000 spccpkg-0.0.5/spcc/code.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:06:31.521143 spccpkg-0.0.5/spccpkg.egg-info/
+-rw-rw-rw-   0        0        0      451 2023-04-23 18:06:31.000000 spccpkg-0.0.5/spccpkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-04-23 18:06:31.000000 spccpkg-0.0.5/spccpkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 18:06:31.000000 spccpkg-0.0.5/spccpkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-23 18:06:31.000000 spccpkg-0.0.5/spccpkg.egg-info/top_level.txt
```

### Comparing `spccpkg-0.0.4/setup.py` & `spccpkg-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'A basic hello package'
 
 # Setting up
 setup(
     name="spccpkg",
     version=VERSION,
     author="yashbrid03",
```

### Comparing `spccpkg-0.0.4/spcc/code.py` & `spccpkg-0.0.5/spcc/code.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 print("{: ^20}{: ^20}{: ^20}".format('Non Terminals','First','Follow'))
 print(FIRST)
 print(FOLLOW)
 for non_terminal in non_terminals:
     print("{: ^20}{: ^20}{: ^20}".format(non_terminal,str(FIRST[non_terminal]),str(FOLLOW[non_terminal])))
 
         '''
-        print(repr(string))
+        print(string)
 
     def lexical():
         string = '''import re
 
 tokens = []
 
 string = ''
@@ -148,15 +148,15 @@
         else:
             tokens.append(["INTEGER", word])
     elif word in ['(',')','{','}','[',']',',',':',';','"']:    
         tokens.append(['DELIMITER', word])
 
 for token in tokens:
     print(token)'''
-        print(repr(string))
+        print(string)
 
     def PP():
         string = '''
         import java.util.*;
 
 class PredictiveParser {
     public static void main(String args[]) {
@@ -215,15 +215,15 @@
                 System.out.println("Error");
                 break;
             }
         }
     }
 }       
         '''
-        print(repr(string))
+        print(string)
 
     def flex():
         string = '''
         %{
     #include<stdio.h>       //header files and declaration
     int v = 0, c = 0;
 %}
@@ -270,15 +270,15 @@
 
 flex filename.l
 gcc lex.yy.c -o filename.exe
 filename.exe
 
 
         '''
-        print(repr(string))
+        print(string)
 
     def OP():
         string = '''
         import numpy as np
 def stringcheck():
     a = list(input("Enter the operators and non terminals used --> "))
     a.append('$')
@@ -393,15 +393,15 @@
         print("String is accepted")
     else:
         print("String is not accepted")
 else:
     print("Grammar is not accepted ")
 
         '''
-        print(repr(string))
+        print(string)
 
     def DSP1():
         string = '''
         import java.util.*;
 
 public class DSP1 {
     public static int evaluateOperand(String operand, Map<String, Integer> symtab) throws IllegalArgumentException {
@@ -484,15 +484,15 @@
         System.out.println("\nSymbol Table: " + symtab);
         System.out.println("Literal Table: " + littab);
         System.out.println("Pool Table: " + pooltab);
     }
 }
 
         '''
-        print(repr(string))
+        print(string)
 
     def P2():
         string = '''
         import java.io.BufferedReader;
 import java.io.FileReader;
 import java.io.FileWriter;
 import java.io.IOException;
@@ -587,15 +587,15 @@
 LOOP 202 1
 B 212 1
 NEXT 208 1
 BACK 202 1
 LAST 210 1
 
         '''
-        print(repr(string))
+        print(string)
 
     def macro():
         string = '''
         Macro.txt
 #include<stdio.h>
 #include<conio.h>
 MACRO
@@ -657,15 +657,15 @@
 print("\n\nMNT\nIndex\tMacro Name MDT Index")
 for i in range (len(mnt)):
    print(mnt[i],"\t ", end="")
 print("\n\nMDT\nIndex\tCard")
 for i in range (1, len(mdt)+1):
    print(i,"\t", mdt.get(i))
         '''
-        print(repr(string))
+        print(string)
 
     def yacc():
         string = '''
         calci.l file
 %{
 	#include "y.tab.h"
 	#include<math.h>
@@ -843,25 +843,25 @@
     if(valid)
     {
         printf("\nIt is a identifier!\n");
     }
 }
 
         '''
-        print(repr(string))
+        print(string)
 
     def commands():
         string = '''
         flex filename.l
         bison filename.y
         bison -dy filename.y
         gcc lex.yy.c y.tab.c -o filename.exe
         filename.exe
         '''
-        print(repr(string))
+        print(string)
 
     def ICG():
         string = '''
         Lex File
         %{
             #include"y.tab.h"
             extern char yyval;
@@ -979,15 +979,15 @@
             threeAdd();
             printf("Four Address Code:\n");
             fouradd();
             printf("Triple Address Code:\n");
             triple();
         '''
 
-        print(repr(string))
+        print(string)
 
     def main():
         string = '''
         ICG()
         commands()
         yacc()
         macro()
@@ -995,8 +995,8 @@
         DSP1()
         OP()
         flex()
         PP()
         lexical()
         ff()
         '''
-        print(repr(string))
+        print(string)
```

