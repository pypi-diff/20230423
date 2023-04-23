# Comparing `tmp/auth_lib_profcomff-2023.4.19.tar.gz` & `tmp/auth_lib_profcomff-2023.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_lib_profcomff-2023.4.19.tar", last modified: Wed Apr 19 12:02:16 2023, max compression
+gzip compressed data, was "auth_lib_profcomff-2023.4.23.tar", last modified: Sun Apr 23 12:30:17 2023, max compression
```

## Comparing `auth_lib_profcomff-2023.4.19.tar` & `auth_lib_profcomff-2023.4.23.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/auth_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/aiomethods.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/auth_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/testing/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/auth_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/aiomethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/auth_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/auth_lib/testing/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 12:30:17.000000 auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 12:30:17.892802 auth_lib_profcomff-2023.4.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-23 12:30:06.000000 auth_lib_profcomff-2023.4.23/setup.py
```

### Comparing `auth_lib_profcomff-2023.4.19/LICENSE` & `auth_lib_profcomff-2023.4.23/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.4.19/PKG-INFO` & `auth_lib_profcomff-2023.4.23/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,107 +1,97 @@
-Metadata-Version: 2.1
-Name: auth_lib_profcomff
-Version: 2023.4.19
-Home-page: https://github.com/profcomff/auth-lib
-Author: Semyon Grigoriev
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: fastapi
-Provides-Extra: testing
-License-File: LICENSE
-
 # auth-lib
 Библиотека функций авторизации для микросервисов Твой ФФ!
 
+[![pypi](https://img.shields.io/pypi/dm/auth-lib-profcomff?label=PIP%20INSTALLS&style=for-the-badge)](https://pypi.org/project/auth-lib-profcomff)
+[![tg](https://img.shields.io/badge/telegram-Viribus%20unitis-brightgreen?style=for-the-badge&logo=telegram)](https://t.me/+eIMtCymYDepmN2Ey)
 
 ## Примеры использования
+### FastAPI
 ```python
 from auth_lib.fastapi import UnionAuth
 from fastapi import APIRouter, Depends
 router = APIRouter(prefix="/...")
 
 ## Чтобы дернуть ручку нужен один скоуп, авторизация обязательна
 ## Юзкейс https://github.com/profcomff/timetable-api/blob/a374c74cd960941100f6c923ff9c3ff706a1ed09/calendar_backend/routes/room/room.py#L45
 @router.smth("/")
 async def foo(_=Depends(UnionAuth(scopes=["service.resource.method"], allow_none=False, auto_error=True))):
   pass
-  
+
 ## Чтобы дернуть ручку нужно два скоупа, авторизация обязательна
 ## Юзкейс https://github.com/profcomff/print-api/blob/775f36fdd185eec8d9096d3472b7730cf5ac9798/print_service/routes/user.py#L78
 @router.smth("/")
 async def bar(_=Depends(UnionAuth(scopes=["scope1", "scope2"], allow_none=False, auto_error=True))):
   pass
-  
+
 ## Чтобы дернуть ручку не нужны скоупы, авторизация необязательна, но если передана недействительная сессия, то кинет ошибку
 @router.smth("/")
 async def baz(_=Depends(UnionAuth(scopes=[], allow_none=True, auto_error=True))):
   pass
 
 
 ## Чтобы дернуть ручку не нужны скоупы, авторизация обязательна
 @router.smth("/")
 async def foo(_=Depends(UnionAuth(scopes=[], allow_none=False, auto_error=True))):
   pass
 
 ```
 Depends вызывает инстанс класса с нужными параметрами и возвращает словарь со всеми полями отсюда https://api.test.profcomff.com/#/Logout/me_me_get
 
-Описание класса UnionAuth
-Поля
-```
-scopes: list[str] - список имен скоупов, которые нужны в данной ручке. Например ["printer.user.create", "printer.user.delete"]
-allow_none: bool - Если true, то при отсутствии нужного заголовка в запросе ручка будет доступна юзеру, если заголовк передан, то обработка идет в зависимости от следующего параметра
-auto_error: bool - если true, то при несовпадении скоупов/завершенной сессии и тд(на запрос GET /me не 200) - кинет 401, если false, то не будет кидать ошибки, но будет возвращать None
-```
+#### Параметры конструктора UnionAuth
+- `scopes: list[str]` - список имен скоупов, которые нужны в данной ручке. Например `["printer.user.create", "printer.user.delete"]`
+- `allow_none: bool` - Если true, то при отсутствии нужного заголовка в запросе ручка будет доступна юзеру, если заголовк передан, то обработка идет в зависимости от следующего параметра
+- `auto_error: bool` - если `True`, то при несовпадении скоупов/завершенной сессии и т.д. (на запрос `GET /me` не 200) - кинет 401, если `False`, то не будет кидать ошибки, но будет возвращать `None`
+
 Чтобы задать хост авторизации надо в переменные окружения или в .env файл прописать AUTH_URL="..."
 
-Defaults 
+#### Настройки
 ```python
 auth_url="https://api.test.profcomff.com/auth/"
 AUTH_AUTO_ERROR: bool = True
 AUTH_ALLOW_NONE: bool = False
 
 ```
 
-Пример мока библиотеки:
-
+## Тестирование сервисов
 Установите нужные завивсимости
 ```shell
 pip install 'auth-lib-profcomff[testing]'
 ```
 
+Используйте маркировку для тестирования
 ```python
 import pytest
 from fastapi.testclient import TestClient
 from fastapi import FastAPI
 
 @pytest.fixture
 def client(auth_mock):
     yield TestClient(FastAPI())
 
-@pytest.mark.authenticated("scope1", "scope2", ...)
+@pytest.mark.authenticated("scope1", "scope2", ..., user_id=5)
 def test1(client):
     """
-    В этом тесте будут выданы скоупы scope1, scope2,
+    В этом тесте будут выданы скоупы scope1, scope2, user_id в ответе будет равен 5
     библиотека не будет проверять токен через АПИ, будет просто возвращать
     нужный словарь, как будто пользователь авторизован с нужными скоупами
     """
     assert 2*2 == 4
 
-    
+
 @pytest.mark.authenticated()
 def test2(client):
     """
-    В этом тесте скоупов выдано не будет,
+    В этом тесте скоупов выдано не будет, user_id будет равен 0
     но библиотека не будет проверять токен через АПИ, будет просто возвращать
     нужный словарь, как будто пользователь авторизован с нужными скоупами
     """
     assert 2*2 == 4
 
 
 def test3(client):
     """
-    В этом тесте скоупов выдано не будет, библиотека будет проверять 
+    В этом тесте скоупов выдано не будет, библиотека будет проверять
     токен через АПИ
     """
     assert 2*2 == 4
 ```
```

### Comparing `auth_lib_profcomff-2023.4.19/README.md` & `auth_lib_profcomff-2023.4.23/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,108 @@
+Metadata-Version: 2.1
+Name: auth_lib_profcomff
+Version: 2023.4.23
+Home-page: https://github.com/profcomff/auth-lib
+Author: Semyon Grigoriev
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+Provides-Extra: fastapi
+Provides-Extra: testing
+License-File: LICENSE
+
 # auth-lib
 Библиотека функций авторизации для микросервисов Твой ФФ!
 
+[![pypi](https://img.shields.io/pypi/dm/auth-lib-profcomff?label=PIP%20INSTALLS&style=for-the-badge)](https://pypi.org/project/auth-lib-profcomff)
+[![tg](https://img.shields.io/badge/telegram-Viribus%20unitis-brightgreen?style=for-the-badge&logo=telegram)](https://t.me/+eIMtCymYDepmN2Ey)
 
 ## Примеры использования
+### FastAPI
 ```python
 from auth_lib.fastapi import UnionAuth
 from fastapi import APIRouter, Depends
 router = APIRouter(prefix="/...")
 
 ## Чтобы дернуть ручку нужен один скоуп, авторизация обязательна
 ## Юзкейс https://github.com/profcomff/timetable-api/blob/a374c74cd960941100f6c923ff9c3ff706a1ed09/calendar_backend/routes/room/room.py#L45
 @router.smth("/")
 async def foo(_=Depends(UnionAuth(scopes=["service.resource.method"], allow_none=False, auto_error=True))):
   pass
-  
+
 ## Чтобы дернуть ручку нужно два скоупа, авторизация обязательна
 ## Юзкейс https://github.com/profcomff/print-api/blob/775f36fdd185eec8d9096d3472b7730cf5ac9798/print_service/routes/user.py#L78
 @router.smth("/")
 async def bar(_=Depends(UnionAuth(scopes=["scope1", "scope2"], allow_none=False, auto_error=True))):
   pass
-  
+
 ## Чтобы дернуть ручку не нужны скоупы, авторизация необязательна, но если передана недействительная сессия, то кинет ошибку
 @router.smth("/")
 async def baz(_=Depends(UnionAuth(scopes=[], allow_none=True, auto_error=True))):
   pass
 
 
 ## Чтобы дернуть ручку не нужны скоупы, авторизация обязательна
 @router.smth("/")
 async def foo(_=Depends(UnionAuth(scopes=[], allow_none=False, auto_error=True))):
   pass
 
 ```
 Depends вызывает инстанс класса с нужными параметрами и возвращает словарь со всеми полями отсюда https://api.test.profcomff.com/#/Logout/me_me_get
 
-Описание класса UnionAuth
-Поля
-```
-scopes: list[str] - список имен скоупов, которые нужны в данной ручке. Например ["printer.user.create", "printer.user.delete"]
-allow_none: bool - Если true, то при отсутствии нужного заголовка в запросе ручка будет доступна юзеру, если заголовк передан, то обработка идет в зависимости от следующего параметра
-auto_error: bool - если true, то при несовпадении скоупов/завершенной сессии и тд(на запрос GET /me не 200) - кинет 401, если false, то не будет кидать ошибки, но будет возвращать None
-```
+#### Параметры конструктора UnionAuth
+- `scopes: list[str]` - список имен скоупов, которые нужны в данной ручке. Например `["printer.user.create", "printer.user.delete"]`
+- `allow_none: bool` - Если true, то при отсутствии нужного заголовка в запросе ручка будет доступна юзеру, если заголовк передан, то обработка идет в зависимости от следующего параметра
+- `auto_error: bool` - если `True`, то при несовпадении скоупов/завершенной сессии и т.д. (на запрос `GET /me` не 200) - кинет 401, если `False`, то не будет кидать ошибки, но будет возвращать `None`
+
 Чтобы задать хост авторизации надо в переменные окружения или в .env файл прописать AUTH_URL="..."
 
-Defaults 
+#### Настройки
 ```python
 auth_url="https://api.test.profcomff.com/auth/"
 AUTH_AUTO_ERROR: bool = True
 AUTH_ALLOW_NONE: bool = False
 
 ```
 
-Пример мока библиотеки:
-
+## Тестирование сервисов
 Установите нужные завивсимости
 ```shell
 pip install 'auth-lib-profcomff[testing]'
 ```
 
+Используйте маркировку для тестирования
 ```python
 import pytest
 from fastapi.testclient import TestClient
 from fastapi import FastAPI
 
 @pytest.fixture
 def client(auth_mock):
     yield TestClient(FastAPI())
 
-@pytest.mark.authenticated("scope1", "scope2", ...)
+@pytest.mark.authenticated("scope1", "scope2", ..., user_id=5)
 def test1(client):
     """
-    В этом тесте будут выданы скоупы scope1, scope2,
+    В этом тесте будут выданы скоупы scope1, scope2, user_id в ответе будет равен 5
     библиотека не будет проверять токен через АПИ, будет просто возвращать
     нужный словарь, как будто пользователь авторизован с нужными скоупами
     """
     assert 2*2 == 4
 
-    
+
 @pytest.mark.authenticated()
 def test2(client):
     """
-    В этом тесте скоупов выдано не будет,
+    В этом тесте скоупов выдано не будет, user_id будет равен 0
     но библиотека не будет проверять токен через АПИ, будет просто возвращать
     нужный словарь, как будто пользователь авторизован с нужными скоупами
     """
     assert 2*2 == 4
 
 
 def test3(client):
     """
-    В этом тесте скоупов выдано не будет, библиотека будет проверять 
+    В этом тесте скоупов выдано не будет, библиотека будет проверять
     токен через АПИ
     """
     assert 2*2 == 4
 ```
```

### Comparing `auth_lib_profcomff-2023.4.19/auth_lib/aiomethods.py` & `auth_lib_profcomff-2023.4.23/auth_lib/aiomethods.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.4.19/auth_lib/exceptions.py` & `auth_lib_profcomff-2023.4.23/auth_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.4.19/auth_lib/fastapi.py` & `auth_lib_profcomff-2023.4.23/auth_lib/fastapi.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.4.19/auth_lib/methods.py` & `auth_lib_profcomff-2023.4.23/auth_lib/methods.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.4.19/auth_lib/testing/testutils.py` & `auth_lib_profcomff-2023.4.23/auth_lib/testing/testutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     if not marker:
         return (yield)
     scopes: tuple[str] = marker.args
     session_scopes = []
     for cnt, scope in enumerate(scopes):
         session_scopes.append({"id": cnt, "name": scope, "comment": ""})
     _return_val: dict[str, int | list[dict[str, str | int]]] = {
-        "user_id": 0,
+        "user_id": marker.kwargs.get("user_id", 0),
         "id": 0,
         "session_scopes": session_scopes,
         "user_scopes": session_scopes,
     }
     patcher = patch(
         "auth_lib.fastapi.UnionAuth.__call__",
         new=MagicMock(return_value=_return_val),
```

### Comparing `auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/PKG-INFO` & `auth_lib_profcomff-2023.4.23/auth_lib_profcomff.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,108 @@
 Metadata-Version: 2.1
 Name: auth-lib-profcomff
-Version: 2023.4.19
+Version: 2023.4.23
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: fastapi
 Provides-Extra: testing
 License-File: LICENSE
 
 # auth-lib
 Библиотека функций авторизации для микросервисов Твой ФФ!
 
+[![pypi](https://img.shields.io/pypi/dm/auth-lib-profcomff?label=PIP%20INSTALLS&style=for-the-badge)](https://pypi.org/project/auth-lib-profcomff)
+[![tg](https://img.shields.io/badge/telegram-Viribus%20unitis-brightgreen?style=for-the-badge&logo=telegram)](https://t.me/+eIMtCymYDepmN2Ey)
 
 ## Примеры использования
+### FastAPI
 ```python
 from auth_lib.fastapi import UnionAuth
 from fastapi import APIRouter, Depends
 router = APIRouter(prefix="/...")
 
 ## Чтобы дернуть ручку нужен один скоуп, авторизация обязательна
 ## Юзкейс https://github.com/profcomff/timetable-api/blob/a374c74cd960941100f6c923ff9c3ff706a1ed09/calendar_backend/routes/room/room.py#L45
 @router.smth("/")
 async def foo(_=Depends(UnionAuth(scopes=["service.resource.method"], allow_none=False, auto_error=True))):
   pass
-  
+
 ## Чтобы дернуть ручку нужно два скоупа, авторизация обязательна
 ## Юзкейс https://github.com/profcomff/print-api/blob/775f36fdd185eec8d9096d3472b7730cf5ac9798/print_service/routes/user.py#L78
 @router.smth("/")
 async def bar(_=Depends(UnionAuth(scopes=["scope1", "scope2"], allow_none=False, auto_error=True))):
   pass
-  
+
 ## Чтобы дернуть ручку не нужны скоупы, авторизация необязательна, но если передана недействительная сессия, то кинет ошибку
 @router.smth("/")
 async def baz(_=Depends(UnionAuth(scopes=[], allow_none=True, auto_error=True))):
   pass
 
 
 ## Чтобы дернуть ручку не нужны скоупы, авторизация обязательна
 @router.smth("/")
 async def foo(_=Depends(UnionAuth(scopes=[], allow_none=False, auto_error=True))):
   pass
 
 ```
 Depends вызывает инстанс класса с нужными параметрами и возвращает словарь со всеми полями отсюда https://api.test.profcomff.com/#/Logout/me_me_get
 
-Описание класса UnionAuth
-Поля
-```
-scopes: list[str] - список имен скоупов, которые нужны в данной ручке. Например ["printer.user.create", "printer.user.delete"]
-allow_none: bool - Если true, то при отсутствии нужного заголовка в запросе ручка будет доступна юзеру, если заголовк передан, то обработка идет в зависимости от следующего параметра
-auto_error: bool - если true, то при несовпадении скоупов/завершенной сессии и тд(на запрос GET /me не 200) - кинет 401, если false, то не будет кидать ошибки, но будет возвращать None
-```
+#### Параметры конструктора UnionAuth
+- `scopes: list[str]` - список имен скоупов, которые нужны в данной ручке. Например `["printer.user.create", "printer.user.delete"]`
+- `allow_none: bool` - Если true, то при отсутствии нужного заголовка в запросе ручка будет доступна юзеру, если заголовк передан, то обработка идет в зависимости от следующего параметра
+- `auto_error: bool` - если `True`, то при несовпадении скоупов/завершенной сессии и т.д. (на запрос `GET /me` не 200) - кинет 401, если `False`, то не будет кидать ошибки, но будет возвращать `None`
+
 Чтобы задать хост авторизации надо в переменные окружения или в .env файл прописать AUTH_URL="..."
 
-Defaults 
+#### Настройки
 ```python
 auth_url="https://api.test.profcomff.com/auth/"
 AUTH_AUTO_ERROR: bool = True
 AUTH_ALLOW_NONE: bool = False
 
 ```
 
-Пример мока библиотеки:
-
+## Тестирование сервисов
 Установите нужные завивсимости
 ```shell
 pip install 'auth-lib-profcomff[testing]'
 ```
 
+Используйте маркировку для тестирования
 ```python
 import pytest
 from fastapi.testclient import TestClient
 from fastapi import FastAPI
 
 @pytest.fixture
 def client(auth_mock):
     yield TestClient(FastAPI())
 
-@pytest.mark.authenticated("scope1", "scope2", ...)
+@pytest.mark.authenticated("scope1", "scope2", ..., user_id=5)
 def test1(client):
     """
-    В этом тесте будут выданы скоупы scope1, scope2,
+    В этом тесте будут выданы скоупы scope1, scope2, user_id в ответе будет равен 5
     библиотека не будет проверять токен через АПИ, будет просто возвращать
     нужный словарь, как будто пользователь авторизован с нужными скоупами
     """
     assert 2*2 == 4
 
-    
+
 @pytest.mark.authenticated()
 def test2(client):
     """
-    В этом тесте скоупов выдано не будет,
+    В этом тесте скоупов выдано не будет, user_id будет равен 0
     но библиотека не будет проверять токен через АПИ, будет просто возвращать
     нужный словарь, как будто пользователь авторизован с нужными скоупами
     """
     assert 2*2 == 4
 
 
 def test3(client):
     """
-    В этом тесте скоупов выдано не будет, библиотека будет проверять 
+    В этом тесте скоупов выдано не будет, библиотека будет проверять
     токен через АПИ
     """
     assert 2*2 == 4
 ```
```

### Comparing `auth_lib_profcomff-2023.4.19/setup.py` & `auth_lib_profcomff-2023.4.23/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="auth_lib_profcomff",
-    version="2023.04.19",
+    version="2023.04.23",
     author="Semyon Grigoriev",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/profcomff/auth-lib",
     packages=find_packages(),
     install_requires=["requests", "aiohttp", "setuptools"],
     extras_require={
```

