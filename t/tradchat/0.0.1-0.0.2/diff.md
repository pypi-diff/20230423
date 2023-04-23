# Comparing `tmp/tradchat-0.0.1.tar.gz` & `tmp/tradchat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradchat-0.0.1.tar", last modified: Wed Apr 19 02:17:18 2023, max compression
+gzip compressed data, was "tradchat-0.0.2.tar", last modified: Sun Apr 23 19:22:25 2023, max compression
```

## Comparing `tradchat-0.0.1.tar` & `tradchat-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 02:17:18.310807 tradchat-0.0.1/
--rw-rw-rw-   0        0        0      394 2023-04-19 02:17:18.306207 tradchat-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-19 02:17:18.313322 tradchat-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-04-19 02:16:57.000000 tradchat-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 02:17:18.222141 tradchat-0.0.1/tradchat/
--rw-rw-rw-   0        0        0    19813 2023-04-19 00:55:15.000000 tradchat-0.0.1/tradchat/Server.py
--rw-rw-rw-   0        0        0  6082053 2023-04-19 02:10:08.000000 tradchat-0.0.1/tradchat/zip.py
-drwxrwxrwx   0        0        0        0 2023-04-19 02:17:18.304877 tradchat-0.0.1/tradchat.egg-info/
--rw-rw-rw-   0        0        0      394 2023-04-19 02:17:17.000000 tradchat-0.0.1/tradchat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-19 02:17:18.000000 tradchat-0.0.1/tradchat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 02:17:17.000000 tradchat-0.0.1/tradchat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 02:17:17.000000 tradchat-0.0.1/tradchat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-19 02:17:17.000000 tradchat-0.0.1/tradchat.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-23 19:22:25.718331 tradchat-0.0.2/
+-rw-rw-rw-   0        0        0      350 2023-04-23 19:22:25.715103 tradchat-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-23 19:22:25.718844 tradchat-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      483 2023-04-23 19:22:00.000000 tradchat-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 19:22:25.639362 tradchat-0.0.2/tradchat/
+-rw-rw-rw-   0        0        0    19832 2023-04-23 19:01:37.000000 tradchat-0.0.2/tradchat/Server.py
+-rw-rw-rw-   0        0        0  4165371 2023-04-23 19:20:49.000000 tradchat-0.0.2/tradchat/zip.py
+drwxrwxrwx   0        0        0        0 2023-04-23 19:22:25.708480 tradchat-0.0.2/tradchat.egg-info/
+-rw-rw-rw-   0        0        0      350 2023-04-23 19:22:25.000000 tradchat-0.0.2/tradchat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-23 19:22:25.000000 tradchat-0.0.2/tradchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 19:22:25.000000 tradchat-0.0.2/tradchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-23 19:22:25.000000 tradchat-0.0.2/tradchat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-23 19:22:25.000000 tradchat-0.0.2/tradchat.egg-info/zip-safe
```

### Comparing `tradchat-0.0.1/tradchat/Server.py` & `tradchat-0.0.2/tradchat/Server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from flask import Flask, render_template, request, redirect, session
 from flask_socketio import SocketIO
 import secrets
 from datetime import*
-import os
 from flask_wtf import FlaskForm
 from wtforms import FileField
 from contextlib import suppress
 import shutil
 import smtplib
 from email.message import EmailMessage
 import ssl
@@ -338,15 +337,15 @@
 def Recv(msg):
     T(target=recv, args=(msg,)).start()
 
 def recv(msg):
     try:
         message = eval(msg)
     except Exception:
-        print('Error')
+        print(f'Error: {msg}')
         return
     if message[0] == "making sure it is alright to send a email":
         if message[1] in accounts:
             email = accounts[message[1]][7]
             password = accounts[message[1]][0]
             try:
                 send_email(email, password)
@@ -389,20 +388,20 @@
         return
     if message[0] == 'Requesting to delete a room':
         for password in rooms:
             if rooms[password][1].lower() == message[1].lower():
                 if rooms[password][0] == message[2]:
                     with suppress(KeyError):del messages[rooms[password][1]]
                     del rooms[password]
-                    Server.send(str(['Sucsessfuul delete', message[2]]), boadcast=True)
+                    Server.send(str(['Sucsessfuul delete', message[2], message[1]]), broadcast=True)
                     return
                 else:
-                    Server.send(str(['Requesting to delete a room', message[2], 'you shoshonuko not delete a room that does not belong to you']), boadcast=True)
+                    Server.send(str(['Requesting to delete a room', message[2], 'you should not delete a room that does not belong to you']), broadcast=True)
                     return
-        Server.send(str(['Requesting to delete a room', message[2], 'you shoshonuko not delete a room that does not even EXIST']), boadcast=True)
+        Server.send(str(['Requesting to delete a room', message[2], 'you should not delete a room that does not even EXIST']), broadcast=True)
         return
     if message[0] == "Then you better give me my messages buster":
         accounts[message[1]][6] = message[2]
         file = open('accounts.txt', 'w')
         for thing in list(str(accounts)):
             try:
                 file.write(thing)
@@ -414,34 +413,35 @@
     if message[0] == 'Requesting to make a new room':
         count = 0
         for password in rooms:
             name = rooms[password][0]
             if name == message[2]:
                 count += 1
         if count > 2:
-            Server.send(str(['Requesting to make a new room', message[2], 'you shoshonuko not make more than 2 rooms']), boadcast=True)
+            Server.send(str(['Requesting to make a new room', message[2], 'you should not make more than 2 rooms']), broadcast=True)
             return
         for room in rooms:
             if room.lower() == message[1].lower():
-                Server.send(str(['Requesting to make a new room', message[2], 'you shoshonuko not take that claimed room']), boadcast=True)
+                Server.send(str(['Requesting to make a new room', message[2], 'you should not take that claimed room']), broadcast=True)
                 return
         for password in rooms:
             if rooms[password][1] == message[3]:
-                Server.send(str(['Requesting to make a new room', message[2], 'you shoshonuko not take that claimed room name']), boadcast=True)
+                Server.send(str(['Requesting to make a new room', message[2], 'you should not take that claimed room name']), broadcast=True)
                 return
         messages[message[3]] = []
-        rooms[message[1]] = [message[2], message[3].replace("'", "").replace('"', '')]
+        rooms[message[1]] = [message[2], message[3]]
         file = open('rooms.txt', 'w')
         for thing in list(str(rooms)):
             try:
                 file.write(thing)
             except UnicodeEncodeError:
                 file.write(' _emoji_ ')
         file.close()
-        Server.send(str(['Successful make', message[2], message[3]]), boadcast=True)
+        Server.send(str(['Successful make', message[2], message[3]]), broadcast=True)
+        print('hey hey')
         return
     if message[1] == 'PrivateText':
         day = date.today()
         time = datetime.today()
         compounded = ['PrivateText', [[message[0], message[3]], f'{months[int(day.month)-1]} {day.day}, {day.year} at {time.hour}:{time.minute}'], message[2]]
         messages['mainroom'].append(compounded)
         Server.send(str(['mainroom', compounded]), broadcast=True)
@@ -453,14 +453,15 @@
                 file.write(' _emoji_ ')
         file.close()
     if message[1] == 'Public':
         day = date.today()
         time = datetime.today()
         compounded = ['Public', [[message[0], message[3]], f'{months[int(day.month)-1]} {day.day}, {day.year} at {time.hour}:{time.minute}']]
         try:
+            print(message[2])
             messages[message[2]].append(compounded)
         except KeyError:
             Server.send(str(['you better switch to this room', message[0], 'mainroom']), broadcast=True)
             return
         Server.send(str([message[2], compounded]), broadcast=True)
         file = open('chat.txt', 'w')
         for thing in list(str(messages)):
```

