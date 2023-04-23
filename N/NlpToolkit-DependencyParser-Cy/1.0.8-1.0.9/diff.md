# Comparing `tmp/NlpToolkit-DependencyParser-Cy-1.0.8.tar.gz` & `tmp/NlpToolkit-DependencyParser-Cy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NlpToolkit-DependencyParser-Cy-1.0.8.tar", last modified: Sat Oct 16 14:33:20 2021, max compression
+gzip compressed data, was "dist/NlpToolkit-DependencyParser-Cy-1.0.9.tar", last modified: Sat Oct 30 19:04:16 2021, max compression
```

## Comparing `NlpToolkit-DependencyParser-Cy-1.0.8.tar` & `NlpToolkit-DependencyParser-Cy-1.0.9.tar`

### file list

```diff
@@ -1,49 +1,57 @@
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-10-16 14:33:20.000000 NlpToolkit-DependencyParser-Cy-1.0.8/
--rw-r--r--   0 olcay      (501) staff       (20)      300 2021-10-16 14:33:20.000000 NlpToolkit-DependencyParser-Cy-1.0.8/PKG-INFO
--rw-r--r--   0 olcay      (501) staff       (20)     1111 2021-10-16 14:33:16.000000 NlpToolkit-DependencyParser-Cy-1.0.8/setup.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-10-16 14:33:20.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/
--rw-r--r--   0 olcay      (501) staff       (20)      570 2020-10-09 08:23:14.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/DependencyRelation.pyx
--rw-r--r--   0 olcay      (501) staff       (20)      299 2021-10-16 14:27:05.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/ParserEvaluationScore.pxd
--rw-r--r--   0 olcay      (501) staff       (20)   201365 2020-10-09 08:23:15.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/DependencyRelation.c
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-10-16 14:33:20.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/
--rw-r--r--   0 olcay      (501) staff       (20)     1705 2021-10-12 20:43:43.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankWord.pyx
--rw-r--r--   0 olcay      (501) staff       (20)      174 2021-10-12 20:42:58.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankFeatures.pxd
--rw-r--r--   0 olcay      (501) staff       (20)   281662 2021-10-12 20:42:58.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankFeatures.c
--rw-r--r--   0 olcay      (501) staff       (20)   263282 2021-10-16 14:31:52.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankSentence.c
--rw-r--r--   0 olcay      (501) staff       (20)   317917 2021-10-16 14:33:02.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankCorpus.c
--rw-r--r--   0 olcay      (501) staff       (20)   351803 2021-10-16 14:31:52.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankWord.c
--rw-r--r--   0 olcay      (501) staff       (20)        0 2020-10-29 09:34:05.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/__init__.py
--rw-r--r--   0 olcay      (501) staff       (20)     8228 2021-10-16 14:31:51.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyRelation.pyx
--rw-r--r--   0 olcay      (501) staff       (20)      334 2021-10-16 14:31:51.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankSentence.pxd
--rw-r--r--   0 olcay      (501) staff       (20)     1312 2021-09-22 17:01:10.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyType.py
--rw-r--r--   0 olcay      (501) staff       (20)     1142 2021-10-16 14:31:51.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankSentence.pyx
--rw-r--r--   0 olcay      (501) staff       (20)      375 2020-11-01 13:29:42.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyPosType.py
--rw-r--r--   0 olcay      (501) staff       (20)      339 2021-10-16 14:31:51.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyRelation.pxd
--rw-r--r--   0 olcay      (501) staff       (20)     3231 2021-10-16 14:33:02.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankCorpus.pyx
--rw-r--r--   0 olcay      (501) staff       (20)     1233 2021-10-12 20:42:58.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankFeatures.pyx
--rw-r--r--   0 olcay      (501) staff       (20)      901 2021-10-12 20:43:43.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankWord.pxd
--rw-r--r--   0 olcay      (501) staff       (20)   371902 2021-10-16 14:31:52.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyRelation.c
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-10-16 14:33:20.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Stanford/
--rw-r--r--   0 olcay      (501) staff       (20)     4434 2021-02-08 20:14:22.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Stanford/StanfordDependencyRelation.pyx
--rw-r--r--   0 olcay      (501) staff       (20)      998 2019-12-13 06:32:09.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Stanford/StanfordDependencyType.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2020-10-29 09:33:45.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Stanford/__init__.py
--rw-r--r--   0 olcay      (501) staff       (20)   295862 2021-02-08 20:14:22.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Stanford/StanfordDependencyRelation.c
--rw-r--r--   0 olcay      (501) staff       (20)      191 2021-02-08 20:06:37.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Stanford/StanfordDependencyRelation.pxd
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-12-13 06:24:54.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-10-16 14:33:20.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/
--rw-r--r--   0 olcay      (501) staff       (20)      990 2020-10-29 09:34:50.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankCorpus.pyx
--rw-r--r--   0 olcay      (501) staff       (20)   249193 2020-11-01 16:24:18.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankCorpus.c
--rw-r--r--   0 olcay      (501) staff       (20)      137 2020-10-09 08:50:22.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankSentence.pxd
--rw-r--r--   0 olcay      (501) staff       (20)   349871 2021-09-22 17:07:22.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankWord.c
--rw-r--r--   0 olcay      (501) staff       (20)     3774 2020-10-09 08:47:25.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankWord.pyx
--rw-r--r--   0 olcay      (501) staff       (20)     3942 2021-02-08 20:02:53.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyRelation.pyx
--rw-r--r--   0 olcay      (501) staff       (20)        0 2020-10-29 09:32:42.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/__init__.py
--rw-r--r--   0 olcay      (501) staff       (20)   257594 2021-09-22 17:07:21.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankSentence.c
--rw-r--r--   0 olcay      (501) staff       (20)      263 2020-10-09 08:44:26.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyRelation.pxd
--rw-r--r--   0 olcay      (501) staff       (20)   287967 2021-02-08 20:02:53.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyRelation.c
--rw-r--r--   0 olcay      (501) staff       (20)      605 2020-10-29 09:34:50.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankWord.pxd
--rw-r--r--   0 olcay      (501) staff       (20)     1384 2020-10-29 09:34:50.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankSentence.pyx
--rw-r--r--   0 olcay      (501) staff       (20)      647 2019-12-13 06:33:36.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyType.py
--rw-r--r--   0 olcay      (501) staff       (20)   246190 2021-10-16 14:27:06.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/ParserEvaluationScore.c
--rw-r--r--   0 olcay      (501) staff       (20)     1128 2021-10-16 14:27:05.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/ParserEvaluationScore.pyx
--rw-r--r--   0 olcay      (501) staff       (20)       76 2020-10-09 08:23:14.000000 NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/DependencyRelation.pxd
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/
+-rw-r--r--   0 olcay      (501) staff       (20)   201365 2020-10-09 08:23:15.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/DependencyRelation.c
+-rw-r--r--   0 olcay      (501) staff       (20)       76 2020-10-09 08:23:14.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/DependencyRelation.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)      570 2020-10-09 08:23:14.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/DependencyRelation.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)   246190 2021-10-16 14:27:06.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/ParserEvaluationScore.c
+-rw-r--r--   0 olcay      (501) staff       (20)      299 2021-10-16 14:27:05.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/ParserEvaluationScore.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)     1128 2021-10-16 14:27:05.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/ParserEvaluationScore.pyx
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Stanford/
+-rw-r--r--   0 olcay      (501) staff       (20)   295862 2021-02-08 20:14:22.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Stanford/StanfordDependencyRelation.c
+-rw-r--r--   0 olcay      (501) staff       (20)      191 2021-02-08 20:06:37.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Stanford/StanfordDependencyRelation.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)     4434 2021-02-08 20:14:22.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Stanford/StanfordDependencyRelation.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)      998 2019-12-13 06:32:09.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Stanford/StanfordDependencyType.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2020-10-29 09:33:45.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Stanford/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/
+-rw-r--r--   0 olcay      (501) staff       (20)   287967 2021-02-08 20:02:53.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyRelation.c
+-rw-r--r--   0 olcay      (501) staff       (20)      263 2020-10-09 08:44:26.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyRelation.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)     3942 2021-02-08 20:02:53.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyRelation.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)   249341 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankCorpus.c
+-rw-r--r--   0 olcay      (501) staff       (20)      990 2020-10-29 09:34:50.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankCorpus.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)   257594 2021-09-22 17:07:21.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankSentence.c
+-rw-r--r--   0 olcay      (501) staff       (20)      137 2020-10-09 08:50:22.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankSentence.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)     1384 2020-10-29 09:34:50.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankSentence.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)   349871 2021-09-22 17:07:22.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankWord.c
+-rw-r--r--   0 olcay      (501) staff       (20)      605 2020-10-29 09:34:50.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankWord.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)     3774 2020-10-09 08:47:25.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankWord.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)      647 2019-12-13 06:33:36.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyType.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2020-10-29 09:32:42.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/
+-rw-r--r--   0 olcay      (501) staff       (20)      375 2020-11-01 13:29:42.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyPosType.py
+-rw-r--r--   0 olcay      (501) staff       (20)   371902 2021-10-16 14:31:52.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyRelation.c
+-rw-r--r--   0 olcay      (501) staff       (20)      339 2021-10-16 14:31:51.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyRelation.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)     8228 2021-10-16 14:31:51.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyRelation.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)   317917 2021-10-16 14:33:02.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankCorpus.c
+-rw-r--r--   0 olcay      (501) staff       (20)     3231 2021-10-16 14:33:02.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankCorpus.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)   281662 2021-10-12 20:42:58.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankFeatures.c
+-rw-r--r--   0 olcay      (501) staff       (20)      174 2021-10-12 20:42:58.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankFeatures.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)     1233 2021-10-12 20:42:58.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankFeatures.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)   263282 2021-10-16 14:31:52.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankSentence.c
+-rw-r--r--   0 olcay      (501) staff       (20)      334 2021-10-16 14:31:51.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankSentence.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)     1142 2021-10-16 14:31:51.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankSentence.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)   351803 2021-10-16 14:31:52.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankWord.c
+-rw-r--r--   0 olcay      (501) staff       (20)      901 2021-10-12 20:43:43.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankWord.pxd
+-rw-r--r--   0 olcay      (501) staff       (20)     1705 2021-10-12 20:43:43.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankWord.pyx
+-rw-r--r--   0 olcay      (501) staff       (20)     1312 2021-09-22 17:01:10.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyType.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2020-10-29 09:34:05.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/__init__.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-12-13 06:24:54.000000 NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/NlpToolkit_DependencyParser_Cy.egg-info/
+-rw-r--r--   0 olcay      (501) staff       (20)     5160 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/NlpToolkit_DependencyParser_Cy.egg-info/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)     2590 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/NlpToolkit_DependencyParser_Cy.egg-info/SOURCES.txt
+-rw-r--r--   0 olcay      (501) staff       (20)        1 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/NlpToolkit_DependencyParser_Cy.egg-info/dependency_links.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       36 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/NlpToolkit_DependencyParser_Cy.egg-info/requires.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       17 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/NlpToolkit_DependencyParser_Cy.egg-info/top_level.txt
+-rw-r--r--   0 olcay      (501) staff       (20)     5160 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)     4283 2021-03-31 18:21:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/README.md
+-rw-r--r--   0 olcay      (501) staff       (20)       38 2021-10-30 19:04:16.000000 NlpToolkit-DependencyParser-Cy-1.0.9/setup.cfg
+-rw-r--r--   0 olcay      (501) staff       (20)     1324 2021-10-30 19:04:12.000000 NlpToolkit-DependencyParser-Cy-1.0.9/setup.py
```

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/setup.py` & `NlpToolkit-DependencyParser-Cy-1.0.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-from distutils.core import setup
+from setuptools import setup
+
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 from Cython.Build import cythonize
 
 setup(
     ext_modules=cythonize(["DependencyParser/*.pyx", "DependencyParser/Stanford/*.pyx",
                            "DependencyParser/Turkish/*.pyx", "DependencyParser/Universal/*.pyx"],
                           compiler_directives={'language_level': "3"}),
     name='NlpToolkit-DependencyParser-Cy',
-    version='1.0.8',
+    version='1.0.9',
     packages=['DependencyParser', 'DependencyParser.Turkish', 'DependencyParser.Universal', 'DependencyParser.Stanford'],
     package_data={'DependencyParser': ['*.pxd', '*.pyx', '*.c', '*.py'],
                   'DependencyParser.Turkish': ['*.pxd', '*.pyx', '*.c', '*.py'],
                   'DependencyParser.Universal': ['*.pxd', '*.pyx', '*.c', '*.py'],
                   'DependencyParser.Stanford': ['*.pxd', '*.pyx', '*.c', '*.py']},
     url='https://github.com/StarlangSoftware/TurkishDependencyParser-Cy',
     license='',
     author='olcaytaner',
     author_email='olcay.yildiz@ozyegin.edu.tr',
     description='Turkish Dependency Parser',
-    install_requires=['NlpToolkit-MorphologicalAnalysis-Cy']
+    install_requires=['NlpToolkit-MorphologicalAnalysis-Cy'],
+    long_description=long_description,
+    long_description_content_type='text/markdown'
 )
```

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/DependencyRelation.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/DependencyRelation.pyx`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/DependencyRelation.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/DependencyRelation.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankWord.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankWord.pyx`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankFeatures.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankFeatures.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankSentence.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankSentence.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankCorpus.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankCorpus.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankWord.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankWord.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyRelation.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyRelation.pyx`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyType.py` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyType.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankSentence.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankSentence.pyx`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankCorpus.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankCorpus.pyx`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankFeatures.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankFeatures.pyx`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyTreeBankWord.pxd` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyTreeBankWord.pxd`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Universal/UniversalDependencyRelation.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Universal/UniversalDependencyRelation.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Stanford/StanfordDependencyRelation.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Stanford/StanfordDependencyRelation.pyx`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Stanford/StanfordDependencyType.py` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Stanford/StanfordDependencyType.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Stanford/StanfordDependencyRelation.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Stanford/StanfordDependencyRelation.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankCorpus.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankCorpus.pyx`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankCorpus.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankCorpus.c`

 * *Files 0% similar despite different names*

```diff
@@ -995,14 +995,15 @@
   struct __pyx_obj_10Dictionary_4Word_Word *(*getWord)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, int, int __pyx_skip_dispatch);
   PyObject *(*getWords)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch);
   PyObject *(*getStrings)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch);
   int (*getIndex)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   int (*wordCount)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch);
   PyObject *(*addWord)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   int (*charCount)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch);
+  PyObject *(*insertWord)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, int, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   PyObject *(*replaceWord)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, int, struct __pyx_obj_10Dictionary_4Word_Word *, int __pyx_skip_dispatch);
   int (*safeIndex)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, int, int __pyx_skip_dispatch);
   PyObject *(*toString)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, int __pyx_skip_dispatch);
   PyObject *(*writeToFile)(struct __pyx_obj_6Corpus_8Sentence_Sentence *, PyObject *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_6Corpus_8Sentence_Sentence *__pyx_vtabptr_6Corpus_8Sentence_Sentence;
```

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankWord.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankWord.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankWord.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankWord.pyx`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyRelation.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyRelation.pyx`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankSentence.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankSentence.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyRelation.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyRelation.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankWord.pxd` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankWord.pxd`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyTreeBankSentence.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyTreeBankSentence.pyx`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/Turkish/TurkishDependencyType.py` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/Turkish/TurkishDependencyType.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/ParserEvaluationScore.c` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/ParserEvaluationScore.c`

 * *Files identical despite different names*

### Comparing `NlpToolkit-DependencyParser-Cy-1.0.8/DependencyParser/ParserEvaluationScore.pyx` & `NlpToolkit-DependencyParser-Cy-1.0.9/DependencyParser/ParserEvaluationScore.pyx`

 * *Files identical despite different names*

