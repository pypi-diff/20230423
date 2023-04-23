# Comparing `tmp/blacksheep-2.0a4.tar.gz` & `tmp/blacksheep-2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacksheep-2.0a4.tar", last modified: Sun Mar 19 21:08:31 2023, max compression
+gzip compressed data, was "blacksheep-2.0a5.tar", last modified: Sun Apr  2 15:04:54 2023, max compression
```

## Comparing `blacksheep-2.0a4.tar` & `blacksheep-2.0a5.tar`

### file list

```diff
@@ -1,174 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.037614 blacksheep-2.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-19 21:05:53.000000 blacksheep-2.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-19 21:05:53.000000 blacksheep-2.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-03-19 21:08:31.037614 blacksheep-2.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-03-19 21:05:53.000000 blacksheep-2.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.021614 blacksheep-2.0a4/blacksheep/
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/asgi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   706640 2023-03-19 21:07:08.000000 blacksheep-2.0a4/blacksheep/baseapp.c
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/baseapp.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/baseapp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/baseapp.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.025614 blacksheep-2.0a4/blacksheep/client/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13126 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/client/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/client/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    15695 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/client/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.025614 blacksheep-2.0a4/blacksheep/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.025614 blacksheep-2.0a4/blacksheep/common/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/common/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/common/files/asyncfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/common/files/info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      679 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/common/files/pathsutils.py
--rw-r--r--   0 runner    (1001) docker     (123)   964597 2023-03-19 21:07:06.000000 blacksheep-2.0a4/blacksheep/contents.c
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/contents.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/contents.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/contents.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   707655 2023-03-19 21:07:05.000000 blacksheep-2.0a4/blacksheep/cookies.c
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/cookies.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/cookies.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   699417 2023-03-19 21:07:04.000000 blacksheep-2.0a4/blacksheep/exceptions.c
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/exceptions.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/exceptions.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   588643 2023-03-19 21:07:05.000000 blacksheep-2.0a4/blacksheep/headers.c
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/headers.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/headers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/headers.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.025614 blacksheep-2.0a4/blacksheep/includes/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/includes/consts.pxi
--rw-r--r--   0 runner    (1001) docker     (123)  1173870 2023-03-19 21:07:06.000000 blacksheep-2.0a4/blacksheep/messages.c
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/messages.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/messages.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18246 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/messages.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/multipart.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)   627408 2023-03-19 21:07:07.000000 blacksheep-2.0a4/blacksheep/scribe.c
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/scribe.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/scribe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/scribe.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.025614 blacksheep-2.0a4/blacksheep/server/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.029614 blacksheep-2.0a4/blacksheep/server/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/authentication/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/authentication/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)    37634 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/authentication/oidc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.029614 blacksheep-2.0a4/blacksheep/server/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27177 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/cors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/csrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/dataprotection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/di.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.029614 blacksheep-2.0a4/blacksheep/server/files/
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/files/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/files/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.029614 blacksheep-2.0a4/blacksheep/server/headers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/headers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.029614 blacksheep-2.0a4/blacksheep/server/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/openapi/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/openapi/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/openapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/openapi/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    37219 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/openapi/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.029614 blacksheep-2.0a4/blacksheep/server/remotes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/remotes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/remotes/forwarding.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/remotes/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.029614 blacksheep-2.0a4/blacksheep/server/rendering/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/rendering/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/rendering/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/rendering/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.029614 blacksheep-2.0a4/blacksheep/server/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/res/error.css
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/res/error.html
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/res/fileslist.html
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/res/redoc-ui.html
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/res/swagger-ui.html
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)    18590 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.029614 blacksheep-2.0a4/blacksheep/server/security/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/security/hsts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.029614 blacksheep-2.0a4/blacksheep/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/sessions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.033614 blacksheep-2.0a4/blacksheep/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/settings/di.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/settings/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/settings/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.033614 blacksheep-2.0a4/blacksheep/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/testing/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/testing/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/testing/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)   405591 2023-03-19 21:07:04.000000 blacksheep-2.0a4/blacksheep/url.c
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/url.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/url.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/url.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.033614 blacksheep-2.0a4/blacksheep/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-19 21:05:53.000000 blacksheep-2.0a4/blacksheep/utils/aio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.021614 blacksheep-2.0a4/blacksheep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-03-19 21:08:30.000000 blacksheep-2.0a4/blacksheep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-03-19 21:08:30.000000 blacksheep-2.0a4/blacksheep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 21:08:30.000000 blacksheep-2.0a4/blacksheep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 21:08:30.000000 blacksheep-2.0a4/blacksheep.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-19 21:08:30.000000 blacksheep-2.0a4/blacksheep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-19 21:08:30.000000 blacksheep-2.0a4/blacksheep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 21:08:31.037614 blacksheep-2.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-03-19 21:05:53.000000 blacksheep-2.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 21:08:31.037614 blacksheep-2.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   113290 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_auth_cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)    19745 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)    25552 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_cors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_csrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_dataprotection.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_files_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    25887 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_files_serving.py
--rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_multipart.py
--rw-r--r--   0 runner    (1001) docker     (123)    19342 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    28307 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_openapi_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    65012 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_openapi_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_pathutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)    16338 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    28976 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)    20776 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-03-19 21:05:53.000000 blacksheep-2.0a4/tests/test_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.937207 blacksheep-2.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-02 15:02:14.000000 blacksheep-2.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-02 15:02:14.000000 blacksheep-2.0a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-02 15:04:54.937207 blacksheep-2.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-02 15:02:14.000000 blacksheep-2.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.925207 blacksheep-2.0a5/blacksheep/
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/asgi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   701131 2023-04-02 15:03:30.000000 blacksheep-2.0a5/blacksheep/baseapp.c
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/baseapp.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/baseapp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/baseapp.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.925207 blacksheep-2.0a5/blacksheep/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13126 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/client/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/client/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/client/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.925207 blacksheep-2.0a5/blacksheep/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.925207 blacksheep-2.0a5/blacksheep/common/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/common/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/common/files/asyncfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/common/files/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      679 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/common/files/pathsutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)   964597 2023-04-02 15:03:29.000000 blacksheep-2.0a5/blacksheep/contents.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/contents.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/contents.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/contents.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   707655 2023-04-02 15:03:28.000000 blacksheep-2.0a5/blacksheep/cookies.c
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/cookies.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/cookies.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   699417 2023-04-02 15:03:27.000000 blacksheep-2.0a5/blacksheep/exceptions.c
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/exceptions.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/exceptions.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   588643 2023-04-02 15:03:27.000000 blacksheep-2.0a5/blacksheep/headers.c
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/headers.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/headers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/headers.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.925207 blacksheep-2.0a5/blacksheep/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/includes/consts.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)  1182750 2023-04-02 15:03:29.000000 blacksheep-2.0a5/blacksheep/messages.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/messages.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/messages.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/messages.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/multipart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)   627544 2023-04-02 15:03:30.000000 blacksheep-2.0a5/blacksheep/scribe.c
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/scribe.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/scribe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/scribe.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.929207 blacksheep-2.0a5/blacksheep/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28718 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.929207 blacksheep-2.0a5/blacksheep/server/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/authentication/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/authentication/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37888 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/authentication/oidc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.929207 blacksheep-2.0a5/blacksheep/server/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27177 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/csrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/dataprotection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/di.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.929207 blacksheep-2.0a5/blacksheep/server/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/files/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/files/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.929207 blacksheep-2.0a5/blacksheep/server/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/headers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.929207 blacksheep-2.0a5/blacksheep/server/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/openapi/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16431 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/openapi/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/openapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/openapi/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37219 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/openapi/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.929207 blacksheep-2.0a5/blacksheep/server/remotes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/remotes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/remotes/forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/remotes/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.929207 blacksheep-2.0a5/blacksheep/server/rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/rendering/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/rendering/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/rendering/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.933207 blacksheep-2.0a5/blacksheep/server/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/res/error.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/res/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/res/fileslist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/res/redoc-ui.html
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/res/swagger-ui.html
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26785 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/routing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.933207 blacksheep-2.0a5/blacksheep/server/security/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/security/hsts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.933207 blacksheep-2.0a5/blacksheep/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/sessions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.933207 blacksheep-2.0a5/blacksheep/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/settings/di.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/settings/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/settings/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.933207 blacksheep-2.0a5/blacksheep/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/testing/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/testing/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/testing/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)   417831 2023-04-02 15:03:26.000000 blacksheep-2.0a5/blacksheep/url.c
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/url.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/url.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/url.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.933207 blacksheep-2.0a5/blacksheep/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-02 15:02:14.000000 blacksheep-2.0a5/blacksheep/utils/aio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.925207 blacksheep-2.0a5/blacksheep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-02 15:04:54.000000 blacksheep-2.0a5/blacksheep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-02 15:04:54.000000 blacksheep-2.0a5/blacksheep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 15:04:54.000000 blacksheep-2.0a5/blacksheep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 15:04:54.000000 blacksheep-2.0a5/blacksheep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-02 15:04:54.000000 blacksheep-2.0a5/blacksheep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-02 15:04:54.000000 blacksheep-2.0a5/blacksheep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 15:04:54.937207 blacksheep-2.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-02 15:02:14.000000 blacksheep-2.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:04:54.937207 blacksheep-2.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   113290 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18585 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_auth_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19745 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26270 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_csrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_dataprotection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_files_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25887 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_files_serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_multipart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19342 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28307 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_openapi_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65012 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_openapi_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_pathutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16338 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28976 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26915 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-04-02 15:02:14.000000 blacksheep-2.0a5/tests/test_websocket.py
```

### Comparing `blacksheep-2.0a4/LICENSE` & `blacksheep-2.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/PKG-INFO` & `blacksheep-2.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacksheep
-Version: 2.0a4
+Version: 2.0a5
 Summary: Fast web framework for Python asyncio
 Home-page: https://github.com/Neoteroi/BlackSheep
 Author: Roberto Prevato
 Author-email: roberto.prevato@gmail.com
 License: MIT
 Keywords: BlackSheep web framework
 Platform: *nix
```

### Comparing `blacksheep-2.0a4/README.md` & `blacksheep-2.0a5/README.md`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/__init__.py` & `blacksheep-2.0a5/blacksheep/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/baseapp.c` & `blacksheep-2.0a5/blacksheep/baseapp.c`

 * *Files 0% similar despite different names*

```diff
@@ -1401,16 +1401,16 @@
   PyObject_HEAD
   PyObject *__pyx_v_exc;
   PyObject *__pyx_v_request;
   struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self;
 };
 
 
-/* "blacksheep/baseapp.pyx":74
- *         return self.router.get_match(request.method, request._path)
+/* "blacksheep/baseapp.pyx":71
+ *             )
  * 
  *     async def handle(self, Request request):             # <<<<<<<<<<<<<<
  *         cdef object route
  *         cdef Response response
  */
 struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_5_handle {
   PyObject_HEAD
@@ -1424,30 +1424,30 @@
   PyObject *__pyx_t_2;
   PyObject *__pyx_t_3;
   PyObject *__pyx_t_4;
   PyObject *__pyx_t_5;
 };
 
 
-/* "blacksheep/baseapp.pyx":97
+/* "blacksheep/baseapp.pyx":94
  *         return response or Response(204)
  * 
  *     async def handle_request_handler_exception(self, request, exc):             # <<<<<<<<<<<<<<
  *         if isinstance(exc, HTTPException):
  *             await self.log_handled_exc(request, exc)
  */
 struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception {
   PyObject_HEAD
   PyObject *__pyx_v_exc;
   PyObject *__pyx_v_request;
   struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self;
 };
 
 
-/* "blacksheep/baseapp.pyx":119
+/* "blacksheep/baseapp.pyx":116
  *         return None
  * 
  *     async def handle_internal_server_error(self, Request request, Exception exc):             # <<<<<<<<<<<<<<
  *         """
  *         Handles an unhandled exception.
  */
 struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error {
@@ -1457,15 +1457,15 @@
   struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self;
   PyObject *__pyx_t_0;
   PyObject *__pyx_t_1;
   PyObject *__pyx_t_2;
 };
 
 
-/* "blacksheep/baseapp.pyx":137
+/* "blacksheep/baseapp.pyx":134
  *         return Response(500, content=TextContent("Internal server error."))
  * 
  *     async def _apply_exception_handler(self, Request request, Exception exc, object exception_handler):             # <<<<<<<<<<<<<<
  *         try:
  *             return await exception_handler(self, request, exc)
  */
 struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler {
@@ -1480,15 +1480,15 @@
   PyObject *__pyx_t_2;
   PyObject *__pyx_t_3;
   PyObject *__pyx_t_4;
   PyObject *__pyx_t_5;
 };
 
 
-/* "blacksheep/baseapp.pyx":143
+/* "blacksheep/baseapp.pyx":140
  *             return await self.handle_exception(request, server_ex)
  * 
  *     async def handle_http_exception(self, Request request, HTTPException http_exception):             # <<<<<<<<<<<<<<
  *         exception_handler = self.get_http_exception_handler(http_exception)
  *         if exception_handler:
  */
 struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception {
@@ -1496,15 +1496,15 @@
   PyObject *__pyx_v_exception_handler;
   struct __pyx_obj_10blacksheep_10exceptions_HTTPException *__pyx_v_http_exception;
   struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request;
   struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self;
 };
 
 
-/* "blacksheep/baseapp.pyx":150
+/* "blacksheep/baseapp.pyx":147
  *         return await self.handle_exception(request, http_exception)
  * 
  *     async def handle_exception(self, request, exc):             # <<<<<<<<<<<<<<
  *         exception_handler = self.get_exception_handler(exc)
  *         if exception_handler:
  */
 struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception {
@@ -1554,14 +1554,15 @@
  */
 
 struct __pyx_vtabstruct_10blacksheep_3url_URL {
   struct __pyx_obj_10blacksheep_3url_URL *(*join)(struct __pyx_obj_10blacksheep_3url_URL *, struct __pyx_obj_10blacksheep_3url_URL *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*base_url)(struct __pyx_obj_10blacksheep_3url_URL *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*with_host)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*with_scheme)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
+  struct __pyx_obj_10blacksheep_3url_URL *(*with_query)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_10blacksheep_3url_URL *__pyx_vtabptr_10blacksheep_3url_URL;
 
 
 /* "messages.pxd":18
  * 
  * 
@@ -2363,15 +2364,14 @@
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_HTTP_s_s_s_s[] = "HTTP %s - \"%s %s\". %s";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_http_exception[] = "http_exception";
 static const char __pyx_k_BaseApplication[] = "BaseApplication";
-static const char __pyx_k_get_route_match[] = "get_route_match";
 static const char __pyx_k_log_handled_exc[] = "log_handled_exc";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_application_json[] = "application/json";
 static const char __pyx_k_handle_exception[] = "handle_exception";
 static const char __pyx_k_handle_not_found[] = "handle_not_found";
 static const char __pyx_k_produce_response[] = "produce_response";
@@ -2450,15 +2450,14 @@
 static PyObject *__pyx_n_s_exception;
 static PyObject *__pyx_n_s_exception_handler;
 static PyObject *__pyx_n_s_get;
 static PyObject *__pyx_n_s_getLogger;
 static PyObject *__pyx_n_s_get_class_instance_hierarchy;
 static PyObject *__pyx_n_s_get_logger;
 static PyObject *__pyx_n_s_get_match;
-static PyObject *__pyx_n_s_get_route_match;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_handle;
 static PyObject *__pyx_n_s_handle_bad_request;
 static PyObject *__pyx_n_s_handle_exception;
 static PyObject *__pyx_n_s_handle_http_exception;
 static PyObject *__pyx_n_s_handle_internal_server_error;
 static PyObject *__pyx_n_s_handle_not_found;
@@ -2513,30 +2512,29 @@
 static PyObject *__pyx_pf_10blacksheep_7baseapp_3handle_bad_request(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_app, CYTHON_UNUSED struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, struct __pyx_obj_10blacksheep_10exceptions_HTTPException *__pyx_v_http_exception); /* proto */
 static PyObject *__pyx_pf_10blacksheep_7baseapp_6common_http_exception_handler(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_app, CYTHON_UNUSED struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, struct __pyx_obj_10blacksheep_10exceptions_HTTPException *__pyx_v_http_exception); /* proto */
 static PyObject *__pyx_pf_10blacksheep_7baseapp_9get_logger(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static int __pyx_pf_10blacksheep_7baseapp_15BaseApplication___init__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, int __pyx_v_show_error_details, PyObject *__pyx_v_router); /* proto */
 static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_2init_exceptions_handlers(CYTHON_UNUSED struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_4log_unhandled_exc(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_request, PyObject *__pyx_v_exc); /* proto */
 static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_7log_handled_exc(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_request, PyObject *__pyx_v_exc); /* proto */
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_10get_route_match(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request); /* proto */
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_12handle(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request); /* proto */
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_15handle_request_handler_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_request, PyObject *__pyx_v_exc); /* proto */
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_18handle_internal_server_error(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, PyObject *__pyx_v_exc); /* proto */
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_21_apply_exception_handler(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, PyObject *__pyx_v_exc, PyObject *__pyx_v_exception_handler); /* proto */
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_24handle_http_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, struct __pyx_obj_10blacksheep_10exceptions_HTTPException *__pyx_v_http_exception); /* proto */
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_27handle_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_request, PyObject *__pyx_v_exc); /* proto */
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_10handle(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request); /* proto */
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_13handle_request_handler_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_request, PyObject *__pyx_v_exc); /* proto */
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_16handle_internal_server_error(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, PyObject *__pyx_v_exc); /* proto */
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_19_apply_exception_handler(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, PyObject *__pyx_v_exc, PyObject *__pyx_v_exception_handler); /* proto */
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_22handle_http_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, struct __pyx_obj_10blacksheep_10exceptions_HTTPException *__pyx_v_http_exception); /* proto */
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_25handle_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_request, PyObject *__pyx_v_exc); /* proto */
 static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_18show_error_details___get__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self); /* proto */
 static int __pyx_pf_10blacksheep_7baseapp_15BaseApplication_18show_error_details_2__set__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_6router___get__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_6logger___get__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_19exceptions_handlers___get__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self); /* proto */
 static int __pyx_pf_10blacksheep_7baseapp_15BaseApplication_19exceptions_handlers_2__set__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_10blacksheep_7baseapp_15BaseApplication_19exceptions_handlers_4__del__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_30__reduce_cython__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_32__setstate_cython__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_28__reduce_cython__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_30__setstate_cython__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_10blacksheep_7baseapp_11__pyx_unpickle_BaseApplication(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_10blacksheep_7baseapp_BaseApplication(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_10blacksheep_7baseapp___pyx_scope_struct__handle_not_found(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_10blacksheep_7baseapp___pyx_scope_struct_1_handle_bad_request(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_10blacksheep_7baseapp___pyx_scope_struct_2_common_http_exception_handler(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_10blacksheep_7baseapp___pyx_scope_struct_3_log_unhandled_exc(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_10blacksheep_7baseapp___pyx_scope_struct_4_log_handled_exc(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -4466,192 +4464,69 @@
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_12generator5(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
 /* "blacksheep/baseapp.pyx":71
  *             )
  * 
- *     def get_route_match(self, Request request):             # <<<<<<<<<<<<<<
- *         return self.router.get_match(request.method, request._path)
- * 
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_11get_route_match(PyObject *__pyx_v_self, PyObject *__pyx_v_request); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_11get_route_match(PyObject *__pyx_v_self, PyObject *__pyx_v_request) {
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("get_route_match (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 71, __pyx_L1_error)
-  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_10get_route_match(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), ((struct __pyx_obj_10blacksheep_8messages_Request *)__pyx_v_request));
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_10get_route_match(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_route_match", 0);
-
-  /* "blacksheep/baseapp.pyx":72
- * 
- *     def get_route_match(self, Request request):
- *         return self.router.get_match(request.method, request._path)             # <<<<<<<<<<<<<<
- * 
- *     async def handle(self, Request request):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->router, __pyx_n_s_get_match); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  __pyx_t_4 = 0;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-      __pyx_t_4 = 1;
-    }
-  }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_request->method, __pyx_v_request->_path};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_request->method, __pyx_v_request->_path};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_4, 2+__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
-  } else
-  #endif
-  {
-    __pyx_t_5 = PyTuple_New(2+__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (__pyx_t_3) {
-      __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
-    }
-    __Pyx_INCREF(__pyx_v_request->method);
-    __Pyx_GIVEREF(__pyx_v_request->method);
-    PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_4, __pyx_v_request->method);
-    __Pyx_INCREF(__pyx_v_request->_path);
-    __Pyx_GIVEREF(__pyx_v_request->_path);
-    PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_4, __pyx_v_request->_path);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "blacksheep/baseapp.pyx":71
- *             )
- * 
- *     def get_route_match(self, Request request):             # <<<<<<<<<<<<<<
- *         return self.router.get_match(request.method, request._path)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("blacksheep.baseapp.BaseApplication.get_route_match", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_14generator5(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
-
-/* "blacksheep/baseapp.pyx":74
- *         return self.router.get_match(request.method, request._path)
- * 
  *     async def handle(self, Request request):             # <<<<<<<<<<<<<<
  *         cdef object route
  *         cdef Response response
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_13handle(PyObject *__pyx_v_self, PyObject *__pyx_v_request); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_13handle(PyObject *__pyx_v_self, PyObject *__pyx_v_request) {
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_11handle(PyObject *__pyx_v_self, PyObject *__pyx_v_request); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_11handle(PyObject *__pyx_v_self, PyObject *__pyx_v_request) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("handle (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 74, __pyx_L1_error)
-  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_12handle(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), ((struct __pyx_obj_10blacksheep_8messages_Request *)__pyx_v_request));
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_10handle(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), ((struct __pyx_obj_10blacksheep_8messages_Request *)__pyx_v_request));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_12handle(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request) {
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_10handle(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request) {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_5_handle *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("handle", 0);
   __pyx_cur_scope = (struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_5_handle *)__pyx_tp_new_10blacksheep_7baseapp___pyx_scope_struct_5_handle(__pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_5_handle, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_5_handle *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 74, __pyx_L1_error)
+    __PYX_ERR(0, 71, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_request = __pyx_v_request;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_request);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_request);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_14generator5, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_handle, __pyx_n_s_BaseApplication_handle, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_12generator5, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_handle, __pyx_n_s_BaseApplication_handle, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4659,15 +4534,15 @@
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_14generator5(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_12generator5(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_5_handle *__pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_5_handle *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
@@ -4699,105 +4574,105 @@
     case 2: goto __pyx_L19_resume_from_await;
     case 3: goto __pyx_L24_resume_from_await;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 71, __pyx_L1_error)
 
-  /* "blacksheep/baseapp.pyx":78
+  /* "blacksheep/baseapp.pyx":75
  *         cdef Response response
  * 
- *         route = self.get_route_match(request)             # <<<<<<<<<<<<<<
+ *         route = self.router.get_match(request)             # <<<<<<<<<<<<<<
  * 
  *         if route:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_get_route_match); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self->router, __pyx_n_s_get_match); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_cur_scope->__pyx_v_request)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_cur_scope->__pyx_v_request));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_route = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "blacksheep/baseapp.pyx":80
- *         route = self.get_route_match(request)
+  /* "blacksheep/baseapp.pyx":77
+ *         route = self.router.get_match(request)
  * 
  *         if route:             # <<<<<<<<<<<<<<
  *             request.route_values = route.values
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_route); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_route); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 77, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "blacksheep/baseapp.pyx":81
+    /* "blacksheep/baseapp.pyx":78
  * 
  *         if route:
  *             request.route_values = route.values             # <<<<<<<<<<<<<<
  * 
  *             try:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_route, __pyx_n_s_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_route, __pyx_n_s_values); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_request->route_values);
     __Pyx_DECREF(__pyx_cur_scope->__pyx_v_request->route_values);
     __pyx_cur_scope->__pyx_v_request->route_values = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "blacksheep/baseapp.pyx":83
+    /* "blacksheep/baseapp.pyx":80
  *             request.route_values = route.values
  * 
  *             try:             # <<<<<<<<<<<<<<
  *                 response = await route.handler(request)
  *             except Exception as exc:
  */
     {
       __Pyx_ExceptionSave(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
       /*try:*/ {
 
-        /* "blacksheep/baseapp.pyx":84
+        /* "blacksheep/baseapp.pyx":81
  * 
  *             try:
  *                 response = await route.handler(request)             # <<<<<<<<<<<<<<
  *             except Exception as exc:
  *                 response = await self.handle_request_handler_exception(request, exc)
  */
-        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_route, __pyx_n_s_handler); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L5_error)
+        __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_route, __pyx_n_s_handler); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_2);
         __pyx_t_3 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
           if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_2, function);
           }
         }
         __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_cur_scope->__pyx_v_request)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_cur_scope->__pyx_v_request));
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L5_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_1);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XGOTREF(__pyx_r);
         if (likely(__pyx_r)) {
           __Pyx_XGIVEREF(__pyx_t_5);
@@ -4818,27 +4693,27 @@
           __Pyx_XGOTREF(__pyx_t_5);
           __pyx_t_6 = __pyx_cur_scope->__pyx_t_1;
           __pyx_cur_scope->__pyx_t_1 = 0;
           __Pyx_XGOTREF(__pyx_t_6);
           __pyx_t_7 = __pyx_cur_scope->__pyx_t_2;
           __pyx_cur_scope->__pyx_t_2 = 0;
           __Pyx_XGOTREF(__pyx_t_7);
-          if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 84, __pyx_L5_error)
+          if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 81, __pyx_L5_error)
           __pyx_t_1 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_1);
         } else {
           __pyx_t_1 = NULL;
-          if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 84, __pyx_L5_error)
+          if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 81, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_1);
         }
-        if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_10blacksheep_8messages_Response))))) __PYX_ERR(0, 84, __pyx_L5_error)
+        if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_10blacksheep_8messages_Response))))) __PYX_ERR(0, 81, __pyx_L5_error)
         __Pyx_GIVEREF(__pyx_t_1);
         __pyx_cur_scope->__pyx_v_response = ((struct __pyx_obj_10blacksheep_8messages_Response *)__pyx_t_1);
         __pyx_t_1 = 0;
 
-        /* "blacksheep/baseapp.pyx":83
+        /* "blacksheep/baseapp.pyx":80
  *             request.route_values = route.values
  * 
  *             try:             # <<<<<<<<<<<<<<
  *                 response = await route.handler(request)
  *             except Exception as exc:
  */
       }
@@ -4847,41 +4722,41 @@
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L10_try_end;
       __pyx_L5_error:;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "blacksheep/baseapp.pyx":85
+      /* "blacksheep/baseapp.pyx":82
  *             try:
  *                 response = await route.handler(request)
  *             except Exception as exc:             # <<<<<<<<<<<<<<
  *                 response = await self.handle_request_handler_exception(request, exc)
  *         else:
  */
       __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_8) {
         __Pyx_AddTraceback("blacksheep.baseapp.BaseApplication.handle", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3) < 0) __PYX_ERR(0, 85, __pyx_L7_except_error)
+        if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3) < 0) __PYX_ERR(0, 82, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_GIVEREF(__pyx_t_2);
         __pyx_cur_scope->__pyx_v_exc = __pyx_t_2;
         /*try:*/ {
 
-          /* "blacksheep/baseapp.pyx":86
+          /* "blacksheep/baseapp.pyx":83
  *                 response = await route.handler(request)
  *             except Exception as exc:
  *                 response = await self.handle_request_handler_exception(request, exc)             # <<<<<<<<<<<<<<
  *         else:
  *             response = await self.exceptions_handlers.get(404)(self, request, None)
  */
-          __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_request_handler_exception); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 86, __pyx_L17_error)
+          __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_request_handler_exception); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 83, __pyx_L17_error)
           __Pyx_GOTREF(__pyx_t_10);
           __pyx_t_11 = NULL;
           __pyx_t_8 = 0;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
             __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_10);
             if (likely(__pyx_t_11)) {
               PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
@@ -4890,40 +4765,40 @@
               __Pyx_DECREF_SET(__pyx_t_10, function);
               __pyx_t_8 = 1;
             }
           }
           #if CYTHON_FAST_PYCALL
           if (PyFunction_Check(__pyx_t_10)) {
             PyObject *__pyx_temp[3] = {__pyx_t_11, ((PyObject *)__pyx_cur_scope->__pyx_v_request), __pyx_cur_scope->__pyx_v_exc};
-            __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 86, __pyx_L17_error)
+            __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 83, __pyx_L17_error)
             __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
             __Pyx_GOTREF(__pyx_t_9);
           } else
           #endif
           #if CYTHON_FAST_PYCCALL
           if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
             PyObject *__pyx_temp[3] = {__pyx_t_11, ((PyObject *)__pyx_cur_scope->__pyx_v_request), __pyx_cur_scope->__pyx_v_exc};
-            __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 86, __pyx_L17_error)
+            __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 83, __pyx_L17_error)
             __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
             __Pyx_GOTREF(__pyx_t_9);
           } else
           #endif
           {
-            __pyx_t_12 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 86, __pyx_L17_error)
+            __pyx_t_12 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 83, __pyx_L17_error)
             __Pyx_GOTREF(__pyx_t_12);
             if (__pyx_t_11) {
               __Pyx_GIVEREF(__pyx_t_11); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_11); __pyx_t_11 = NULL;
             }
             __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
             __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
             PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_8, ((PyObject *)__pyx_cur_scope->__pyx_v_request));
             __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
             __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
             PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_8, __pyx_cur_scope->__pyx_v_exc);
-            __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_12, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 86, __pyx_L17_error)
+            __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_12, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 83, __pyx_L17_error)
             __Pyx_GOTREF(__pyx_t_9);
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           }
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_9);
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_XGOTREF(__pyx_r);
@@ -4961,29 +4836,29 @@
             __Pyx_XGOTREF(__pyx_t_5);
             __pyx_t_6 = __pyx_cur_scope->__pyx_t_4;
             __pyx_cur_scope->__pyx_t_4 = 0;
             __Pyx_XGOTREF(__pyx_t_6);
             __pyx_t_7 = __pyx_cur_scope->__pyx_t_5;
             __pyx_cur_scope->__pyx_t_5 = 0;
             __Pyx_XGOTREF(__pyx_t_7);
-            if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 86, __pyx_L17_error)
+            if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 83, __pyx_L17_error)
             __pyx_t_9 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_9);
           } else {
             __pyx_t_9 = NULL;
-            if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_9) < 0) __PYX_ERR(0, 86, __pyx_L17_error)
+            if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_9) < 0) __PYX_ERR(0, 83, __pyx_L17_error)
             __Pyx_GOTREF(__pyx_t_9);
           }
-          if (!(likely(((__pyx_t_9) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_9, __pyx_ptype_10blacksheep_8messages_Response))))) __PYX_ERR(0, 86, __pyx_L17_error)
+          if (!(likely(((__pyx_t_9) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_9, __pyx_ptype_10blacksheep_8messages_Response))))) __PYX_ERR(0, 83, __pyx_L17_error)
           __Pyx_XGOTREF(((PyObject *)__pyx_cur_scope->__pyx_v_response));
           __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_response, ((struct __pyx_obj_10blacksheep_8messages_Response *)__pyx_t_9));
           __Pyx_GIVEREF(__pyx_t_9);
           __pyx_t_9 = 0;
         }
 
-        /* "blacksheep/baseapp.pyx":85
+        /* "blacksheep/baseapp.pyx":82
  *             try:
  *                 response = await route.handler(request)
  *             except Exception as exc:             # <<<<<<<<<<<<<<
  *                 response = await self.handle_request_handler_exception(request, exc)
  *         else:
  */
         /*finally:*/ {
@@ -5035,15 +4910,15 @@
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         goto __pyx_L6_exception_handled;
       }
       goto __pyx_L7_except_error;
       __pyx_L7_except_error:;
 
-      /* "blacksheep/baseapp.pyx":83
+      /* "blacksheep/baseapp.pyx":80
  *             request.route_values = route.values
  * 
  *             try:             # <<<<<<<<<<<<<<
  *                 response = await route.handler(request)
  *             except Exception as exc:
  */
       __Pyx_XGIVEREF(__pyx_t_5);
@@ -5055,37 +4930,37 @@
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_XGIVEREF(__pyx_t_6);
       __Pyx_XGIVEREF(__pyx_t_7);
       __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_6, __pyx_t_7);
       __pyx_L10_try_end:;
     }
 
-    /* "blacksheep/baseapp.pyx":80
- *         route = self.get_route_match(request)
+    /* "blacksheep/baseapp.pyx":77
+ *         route = self.router.get_match(request)
  * 
  *         if route:             # <<<<<<<<<<<<<<
  *             request.route_values = route.values
  * 
  */
     goto __pyx_L4;
   }
 
-  /* "blacksheep/baseapp.pyx":88
+  /* "blacksheep/baseapp.pyx":85
  *                 response = await self.handle_request_handler_exception(request, exc)
  *         else:
  *             response = await self.exceptions_handlers.get(404)(self, request, None)             # <<<<<<<<<<<<<<
  *             if not response:
  *                 response = Response(404)
  */
   /*else*/ {
     if (unlikely(__pyx_cur_scope->__pyx_v_self->exceptions_handlers == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "get");
-      __PYX_ERR(0, 88, __pyx_L1_error)
+      __PYX_ERR(0, 85, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyDict_GetItemDefault(__pyx_cur_scope->__pyx_v_self->exceptions_handlers, __pyx_int_404, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_GetItemDefault(__pyx_cur_scope->__pyx_v_self->exceptions_handlers, __pyx_int_404, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = NULL;
     __pyx_t_13 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -5094,43 +4969,43 @@
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_13 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[4] = {__pyx_t_1, ((PyObject *)__pyx_cur_scope->__pyx_v_self), ((PyObject *)__pyx_cur_scope->__pyx_v_request), Py_None};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_13, 3+__pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_13, 3+__pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
       PyObject *__pyx_temp[4] = {__pyx_t_1, ((PyObject *)__pyx_cur_scope->__pyx_v_self), ((PyObject *)__pyx_cur_scope->__pyx_v_request), Py_None};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_13, 3+__pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_13, 3+__pyx_t_13); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
-      __pyx_t_9 = PyTuple_New(3+__pyx_t_13); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __pyx_t_9 = PyTuple_New(3+__pyx_t_13); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 85, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       if (__pyx_t_1) {
         __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_1); __pyx_t_1 = NULL;
       }
       __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_self));
       __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_self));
       PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_13, ((PyObject *)__pyx_cur_scope->__pyx_v_self));
       __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
       __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
       PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_13, ((PyObject *)__pyx_cur_scope->__pyx_v_request));
       __Pyx_INCREF(Py_None);
       __Pyx_GIVEREF(Py_None);
       PyTuple_SET_ITEM(__pyx_t_9, 2+__pyx_t_13, Py_None);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XGOTREF(__pyx_r);
@@ -5138,90 +5013,90 @@
       __Pyx_XGIVEREF(__pyx_r);
       __Pyx_RefNannyFinishContext();
       __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
       /* return from generator, awaiting value */
       __pyx_generator->resume_label = 3;
       return __pyx_r;
       __pyx_L24_resume_from_await:;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 88, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 85, __pyx_L1_error)
       __pyx_t_3 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_3);
     } else {
       __pyx_t_3 = NULL;
-      if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_3) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
+      if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_3) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
     }
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_10blacksheep_8messages_Response))))) __PYX_ERR(0, 88, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_10blacksheep_8messages_Response))))) __PYX_ERR(0, 85, __pyx_L1_error)
     __Pyx_GIVEREF(__pyx_t_3);
     __pyx_cur_scope->__pyx_v_response = ((struct __pyx_obj_10blacksheep_8messages_Response *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "blacksheep/baseapp.pyx":89
+    /* "blacksheep/baseapp.pyx":86
  *         else:
  *             response = await self.exceptions_handlers.get(404)(self, request, None)
  *             if not response:             # <<<<<<<<<<<<<<
  *                 response = Response(404)
  *         # if the request handler didn't return an object,
  */
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_cur_scope->__pyx_v_response)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_cur_scope->__pyx_v_response)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 86, __pyx_L1_error)
     __pyx_t_21 = ((!__pyx_t_4) != 0);
     if (__pyx_t_21) {
 
-      /* "blacksheep/baseapp.pyx":90
+      /* "blacksheep/baseapp.pyx":87
  *             response = await self.exceptions_handlers.get(404)(self, request, None)
  *             if not response:
  *                 response = Response(404)             # <<<<<<<<<<<<<<
  *         # if the request handler didn't return an object,
  *         # and since the request was handled successfully, return success status code No Content
  */
-      __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8messages_Response), __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8messages_Response), __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_GOTREF(((PyObject *)__pyx_cur_scope->__pyx_v_response));
       __Pyx_DECREF_SET(__pyx_cur_scope->__pyx_v_response, ((struct __pyx_obj_10blacksheep_8messages_Response *)__pyx_t_3));
       __Pyx_GIVEREF(__pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "blacksheep/baseapp.pyx":89
+      /* "blacksheep/baseapp.pyx":86
  *         else:
  *             response = await self.exceptions_handlers.get(404)(self, request, None)
  *             if not response:             # <<<<<<<<<<<<<<
  *                 response = Response(404)
  *         # if the request handler didn't return an object,
  */
     }
   }
   __pyx_L4:;
 
-  /* "blacksheep/baseapp.pyx":95
+  /* "blacksheep/baseapp.pyx":92
  *         # for example, a user might return "None" from an handler
  *         # this might be ambiguous, if a programmer thinks to return None for "Not found"
  *         return response or Response(204)             # <<<<<<<<<<<<<<
  * 
  *     async def handle_request_handler_exception(self, request, exc):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_21 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_cur_scope->__pyx_v_response)); if (unlikely(__pyx_t_21 < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_cur_scope->__pyx_v_response)); if (unlikely(__pyx_t_21 < 0)) __PYX_ERR(0, 92, __pyx_L1_error)
   if (!__pyx_t_21) {
   } else {
     __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_response));
     __pyx_t_3 = ((PyObject *)__pyx_cur_scope->__pyx_v_response);
     goto __pyx_L26_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8messages_Response), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8messages_Response), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_t_2);
   __pyx_t_3 = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_L26_bool_binop_done:;
   __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   goto __pyx_L0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "blacksheep/baseapp.pyx":74
- *         return self.router.get_match(request.method, request._path)
+  /* "blacksheep/baseapp.pyx":71
+ *             )
  * 
  *     async def handle(self, Request request):             # <<<<<<<<<<<<<<
  *         cdef object route
  *         cdef Response response
  */
 
   /* function exit code */
@@ -5240,27 +5115,27 @@
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_17generator6(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_15generator6(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "blacksheep/baseapp.pyx":97
+/* "blacksheep/baseapp.pyx":94
  *         return response or Response(204)
  * 
  *     async def handle_request_handler_exception(self, request, exc):             # <<<<<<<<<<<<<<
  *         if isinstance(exc, HTTPException):
  *             await self.log_handled_exc(request, exc)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_16handle_request_handler_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_16handle_request_handler_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_14handle_request_handler_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_14handle_request_handler_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_request = 0;
   PyObject *__pyx_v_exc = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5284,71 +5159,71 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_request)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_request_handler_exception", 1, 2, 2, 1); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_request_handler_exception", 1, 2, 2, 1); __PYX_ERR(0, 94, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_request_handler_exception") < 0)) __PYX_ERR(0, 97, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_request_handler_exception") < 0)) __PYX_ERR(0, 94, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_request = values[0];
     __pyx_v_exc = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("handle_request_handler_exception", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 97, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("handle_request_handler_exception", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 94, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("blacksheep.baseapp.BaseApplication.handle_request_handler_exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_15handle_request_handler_exception(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), __pyx_v_request, __pyx_v_exc);
+  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_13handle_request_handler_exception(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), __pyx_v_request, __pyx_v_exc);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_15handle_request_handler_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_request, PyObject *__pyx_v_exc) {
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_13handle_request_handler_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_request, PyObject *__pyx_v_exc) {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("handle_request_handler_exception", 0);
   __pyx_cur_scope = (struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception *)__pyx_tp_new_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception(__pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 97, __pyx_L1_error)
+    __PYX_ERR(0, 94, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_request = __pyx_v_request;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_request);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_request);
   __pyx_cur_scope->__pyx_v_exc = __pyx_v_exc;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_17generator6, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_handle_request_handler_exception, __pyx_n_s_BaseApplication_handle_request_h, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_15generator6, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_handle_request_handler_exception, __pyx_n_s_BaseApplication_handle_request_h, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5356,15 +5231,15 @@
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_17generator6(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_15generator6(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception *__pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -5384,35 +5259,35 @@
     case 4: goto __pyx_L9_resume_from_await;
     case 5: goto __pyx_L10_resume_from_await;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 94, __pyx_L1_error)
 
-  /* "blacksheep/baseapp.pyx":98
+  /* "blacksheep/baseapp.pyx":95
  * 
  *     async def handle_request_handler_exception(self, request, exc):
  *         if isinstance(exc, HTTPException):             # <<<<<<<<<<<<<<
  *             await self.log_handled_exc(request, exc)
  *             return await self.handle_http_exception(request, exc)
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_cur_scope->__pyx_v_exc, __pyx_ptype_10blacksheep_10exceptions_HTTPException); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "blacksheep/baseapp.pyx":99
+    /* "blacksheep/baseapp.pyx":96
  *     async def handle_request_handler_exception(self, request, exc):
  *         if isinstance(exc, HTTPException):
  *             await self.log_handled_exc(request, exc)             # <<<<<<<<<<<<<<
  *             return await self.handle_http_exception(request, exc)
  * 
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_log_handled_exc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_log_handled_exc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -5421,40 +5296,40 @@
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
-      __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 99, __pyx_L1_error)
+      __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_request);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_request);
       PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_cur_scope->__pyx_v_request);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
       PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_cur_scope->__pyx_v_exc);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XGOTREF(__pyx_r);
@@ -5462,32 +5337,32 @@
       __Pyx_XGIVEREF(__pyx_r);
       __Pyx_RefNannyFinishContext();
       __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
       /* return from generator, awaiting value */
       __pyx_generator->resume_label = 1;
       return __pyx_r;
       __pyx_L5_resume_from_await:;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 99, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 96, __pyx_L1_error)
     } else {
       PyObject* exc_type = __Pyx_PyErr_Occurred();
       if (exc_type) {
         if (likely(exc_type == PyExc_StopIteration || (exc_type != PyExc_GeneratorExit && __Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))) PyErr_Clear();
-        else __PYX_ERR(0, 99, __pyx_L1_error)
+        else __PYX_ERR(0, 96, __pyx_L1_error)
       }
     }
 
-    /* "blacksheep/baseapp.pyx":100
+    /* "blacksheep/baseapp.pyx":97
  *         if isinstance(exc, HTTPException):
  *             await self.log_handled_exc(request, exc)
  *             return await self.handle_http_exception(request, exc)             # <<<<<<<<<<<<<<
  * 
  *         if type(exc) in self.exceptions_handlers:
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_http_exception); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_http_exception); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_7 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -5496,40 +5371,40 @@
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_7) {
         __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_request);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_request);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_6, __pyx_cur_scope->__pyx_v_request);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_6, __pyx_cur_scope->__pyx_v_exc);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XGOTREF(__pyx_r);
@@ -5537,57 +5412,57 @@
       __Pyx_XGIVEREF(__pyx_r);
       __Pyx_RefNannyFinishContext();
       __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
       /* return from generator, awaiting value */
       __pyx_generator->resume_label = 2;
       return __pyx_r;
       __pyx_L6_resume_from_await:;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 100, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 97, __pyx_L1_error)
       __pyx_t_3 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_3);
     } else {
       __pyx_t_3 = NULL;
-      if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_3) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
+      if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_3) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
     }
     __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "blacksheep/baseapp.pyx":98
+    /* "blacksheep/baseapp.pyx":95
  * 
  *     async def handle_request_handler_exception(self, request, exc):
  *         if isinstance(exc, HTTPException):             # <<<<<<<<<<<<<<
  *             await self.log_handled_exc(request, exc)
  *             return await self.handle_http_exception(request, exc)
  */
   }
 
-  /* "blacksheep/baseapp.pyx":102
+  /* "blacksheep/baseapp.pyx":99
  *             return await self.handle_http_exception(request, exc)
  * 
  *         if type(exc) in self.exceptions_handlers:             # <<<<<<<<<<<<<<
  *             await self.log_handled_exc(request, exc)
  *         else:
  */
   if (unlikely(__pyx_cur_scope->__pyx_v_self->exceptions_handlers == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 102, __pyx_L1_error)
+    __PYX_ERR(0, 99, __pyx_L1_error)
   }
-  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(((PyObject *)Py_TYPE(__pyx_cur_scope->__pyx_v_exc)), __pyx_cur_scope->__pyx_v_self->exceptions_handlers, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 102, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(((PyObject *)Py_TYPE(__pyx_cur_scope->__pyx_v_exc)), __pyx_cur_scope->__pyx_v_self->exceptions_handlers, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 99, __pyx_L1_error)
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "blacksheep/baseapp.pyx":103
+    /* "blacksheep/baseapp.pyx":100
  * 
  *         if type(exc) in self.exceptions_handlers:
  *             await self.log_handled_exc(request, exc)             # <<<<<<<<<<<<<<
  *         else:
  *             await self.log_unhandled_exc(request, exc)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_log_handled_exc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 103, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_log_handled_exc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -5596,40 +5471,40 @@
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
-      __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 103, __pyx_L1_error)
+      __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_request);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_request);
       PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_cur_scope->__pyx_v_request);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
       PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_cur_scope->__pyx_v_exc);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XGOTREF(__pyx_r);
@@ -5637,42 +5512,42 @@
       __Pyx_XGIVEREF(__pyx_r);
       __Pyx_RefNannyFinishContext();
       __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
       /* return from generator, awaiting value */
       __pyx_generator->resume_label = 3;
       return __pyx_r;
       __pyx_L8_resume_from_await:;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 103, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 100, __pyx_L1_error)
     } else {
       PyObject* exc_type = __Pyx_PyErr_Occurred();
       if (exc_type) {
         if (likely(exc_type == PyExc_StopIteration || (exc_type != PyExc_GeneratorExit && __Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))) PyErr_Clear();
-        else __PYX_ERR(0, 103, __pyx_L1_error)
+        else __PYX_ERR(0, 100, __pyx_L1_error)
       }
     }
 
-    /* "blacksheep/baseapp.pyx":102
+    /* "blacksheep/baseapp.pyx":99
  *             return await self.handle_http_exception(request, exc)
  * 
  *         if type(exc) in self.exceptions_handlers:             # <<<<<<<<<<<<<<
  *             await self.log_handled_exc(request, exc)
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "blacksheep/baseapp.pyx":105
+  /* "blacksheep/baseapp.pyx":102
  *             await self.log_handled_exc(request, exc)
  *         else:
  *             await self.log_unhandled_exc(request, exc)             # <<<<<<<<<<<<<<
  * 
  *         return await self.handle_exception(request, exc)
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_log_unhandled_exc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_log_unhandled_exc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_7 = NULL;
     __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -5681,40 +5556,40 @@
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_6 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_3);
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 105, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 102, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (__pyx_t_7) {
         __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_request);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_request);
       PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_6, __pyx_cur_scope->__pyx_v_request);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
       PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_6, __pyx_cur_scope->__pyx_v_exc);
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XGOTREF(__pyx_r);
@@ -5722,34 +5597,34 @@
       __Pyx_XGIVEREF(__pyx_r);
       __Pyx_RefNannyFinishContext();
       __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
       /* return from generator, awaiting value */
       __pyx_generator->resume_label = 4;
       return __pyx_r;
       __pyx_L9_resume_from_await:;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 105, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 102, __pyx_L1_error)
     } else {
       PyObject* exc_type = __Pyx_PyErr_Occurred();
       if (exc_type) {
         if (likely(exc_type == PyExc_StopIteration || (exc_type != PyExc_GeneratorExit && __Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))) PyErr_Clear();
-        else __PYX_ERR(0, 105, __pyx_L1_error)
+        else __PYX_ERR(0, 102, __pyx_L1_error)
       }
     }
   }
   __pyx_L7:;
 
-  /* "blacksheep/baseapp.pyx":107
+  /* "blacksheep/baseapp.pyx":104
  *             await self.log_unhandled_exc(request, exc)
  * 
  *         return await self.handle_exception(request, exc)             # <<<<<<<<<<<<<<
  * 
  *     cdef object get_http_exception_handler(self, HTTPException http_exception):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_exception); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_exception); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -5758,40 +5633,40 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_5) {
       __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
     }
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_request);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_request);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_cur_scope->__pyx_v_request);
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_cur_scope->__pyx_v_exc);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_XGOTREF(__pyx_r);
@@ -5799,27 +5674,27 @@
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
     /* return from generator, awaiting value */
     __pyx_generator->resume_label = 5;
     return __pyx_r;
     __pyx_L10_resume_from_await:;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 107, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 104, __pyx_L1_error)
     __pyx_t_3 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_3);
   } else {
     __pyx_t_3 = NULL;
-    if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_3) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+    if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_3) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
   }
   __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   goto __pyx_L0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "blacksheep/baseapp.pyx":97
+  /* "blacksheep/baseapp.pyx":94
  *         return response or Response(204)
  * 
  *     async def handle_request_handler_exception(self, request, exc):             # <<<<<<<<<<<<<<
  *         if isinstance(exc, HTTPException):
  *             await self.log_handled_exc(request, exc)
  */
 
@@ -5837,15 +5712,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/baseapp.pyx":109
+/* "blacksheep/baseapp.pyx":106
  *         return await self.handle_exception(request, exc)
  * 
  *     cdef object get_http_exception_handler(self, HTTPException http_exception):             # <<<<<<<<<<<<<<
  *         return self.exceptions_handlers.get(http_exception.status, common_http_exception_handler)
  * 
  */
 
@@ -5856,39 +5731,39 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_http_exception_handler", 0);
 
-  /* "blacksheep/baseapp.pyx":110
+  /* "blacksheep/baseapp.pyx":107
  * 
  *     cdef object get_http_exception_handler(self, HTTPException http_exception):
  *         return self.exceptions_handlers.get(http_exception.status, common_http_exception_handler)             # <<<<<<<<<<<<<<
  * 
  *     cdef object get_exception_handler(self, Exception exception):
  */
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(__pyx_v_self->exceptions_handlers == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "get");
-    __PYX_ERR(0, 110, __pyx_L1_error)
+    __PYX_ERR(0, 107, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_http_exception->status); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_http_exception->status); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_common_http_exception_handler); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_common_http_exception_handler); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyDict_GetItemDefault(__pyx_v_self->exceptions_handlers, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_GetItemDefault(__pyx_v_self->exceptions_handlers, __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/baseapp.pyx":109
+  /* "blacksheep/baseapp.pyx":106
  *         return await self.handle_exception(request, exc)
  * 
  *     cdef object get_http_exception_handler(self, HTTPException http_exception):             # <<<<<<<<<<<<<<
  *         return self.exceptions_handlers.get(http_exception.status, common_http_exception_handler)
  * 
  */
 
@@ -5901,15 +5776,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/baseapp.pyx":112
+/* "blacksheep/baseapp.pyx":109
  *         return self.exceptions_handlers.get(http_exception.status, common_http_exception_handler)
  * 
  *     cdef object get_exception_handler(self, Exception exception):             # <<<<<<<<<<<<<<
  *         for current_class_in_hierarchy in get_class_instance_hierarchy(exception):
  *             if current_class_in_hierarchy in self.exceptions_handlers:
  */
 
@@ -5925,146 +5800,146 @@
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_exception_handler", 0);
 
-  /* "blacksheep/baseapp.pyx":113
+  /* "blacksheep/baseapp.pyx":110
  * 
  *     cdef object get_exception_handler(self, Exception exception):
  *         for current_class_in_hierarchy in get_class_instance_hierarchy(exception):             # <<<<<<<<<<<<<<
  *             if current_class_in_hierarchy in self.exceptions_handlers:
  *                 return self.exceptions_handlers[current_class_in_hierarchy]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_get_class_instance_hierarchy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_get_class_instance_hierarchy); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_exception) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_exception);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 110, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 110, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 110, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_5(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 113, __pyx_L1_error)
+          else __PYX_ERR(0, 110, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_current_class_in_hierarchy, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "blacksheep/baseapp.pyx":114
+    /* "blacksheep/baseapp.pyx":111
  *     cdef object get_exception_handler(self, Exception exception):
  *         for current_class_in_hierarchy in get_class_instance_hierarchy(exception):
  *             if current_class_in_hierarchy in self.exceptions_handlers:             # <<<<<<<<<<<<<<
  *                 return self.exceptions_handlers[current_class_in_hierarchy]
  * 
  */
     if (unlikely(__pyx_v_self->exceptions_handlers == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 114, __pyx_L1_error)
+      __PYX_ERR(0, 111, __pyx_L1_error)
     }
-    __pyx_t_6 = (__Pyx_PyDict_ContainsTF(__pyx_v_current_class_in_hierarchy, __pyx_v_self->exceptions_handlers, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __pyx_t_6 = (__Pyx_PyDict_ContainsTF(__pyx_v_current_class_in_hierarchy, __pyx_v_self->exceptions_handlers, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
     __pyx_t_7 = (__pyx_t_6 != 0);
     if (__pyx_t_7) {
 
-      /* "blacksheep/baseapp.pyx":115
+      /* "blacksheep/baseapp.pyx":112
  *         for current_class_in_hierarchy in get_class_instance_hierarchy(exception):
  *             if current_class_in_hierarchy in self.exceptions_handlers:
  *                 return self.exceptions_handlers[current_class_in_hierarchy]             # <<<<<<<<<<<<<<
  * 
  *         return None
  */
       __Pyx_XDECREF(__pyx_r);
       if (unlikely(__pyx_v_self->exceptions_handlers == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 115, __pyx_L1_error)
+        __PYX_ERR(0, 112, __pyx_L1_error)
       }
-      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_self->exceptions_handlers, __pyx_v_current_class_in_hierarchy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_self->exceptions_handlers, __pyx_v_current_class_in_hierarchy); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_r = __pyx_t_1;
       __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       goto __pyx_L0;
 
-      /* "blacksheep/baseapp.pyx":114
+      /* "blacksheep/baseapp.pyx":111
  *     cdef object get_exception_handler(self, Exception exception):
  *         for current_class_in_hierarchy in get_class_instance_hierarchy(exception):
  *             if current_class_in_hierarchy in self.exceptions_handlers:             # <<<<<<<<<<<<<<
  *                 return self.exceptions_handlers[current_class_in_hierarchy]
  * 
  */
     }
 
-    /* "blacksheep/baseapp.pyx":113
+    /* "blacksheep/baseapp.pyx":110
  * 
  *     cdef object get_exception_handler(self, Exception exception):
  *         for current_class_in_hierarchy in get_class_instance_hierarchy(exception):             # <<<<<<<<<<<<<<
  *             if current_class_in_hierarchy in self.exceptions_handlers:
  *                 return self.exceptions_handlers[current_class_in_hierarchy]
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "blacksheep/baseapp.pyx":117
+  /* "blacksheep/baseapp.pyx":114
  *                 return self.exceptions_handlers[current_class_in_hierarchy]
  * 
  *         return None             # <<<<<<<<<<<<<<
  * 
  *     async def handle_internal_server_error(self, Request request, Exception exc):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
 
-  /* "blacksheep/baseapp.pyx":112
+  /* "blacksheep/baseapp.pyx":109
  *         return self.exceptions_handlers.get(http_exception.status, common_http_exception_handler)
  * 
  *     cdef object get_exception_handler(self, Exception exception):             # <<<<<<<<<<<<<<
  *         for current_class_in_hierarchy in get_class_instance_hierarchy(exception):
  *             if current_class_in_hierarchy in self.exceptions_handlers:
  */
 
@@ -6077,28 +5952,28 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_current_class_in_hierarchy);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_20generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_18generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "blacksheep/baseapp.pyx":119
+/* "blacksheep/baseapp.pyx":116
  *         return None
  * 
  *     async def handle_internal_server_error(self, Request request, Exception exc):             # <<<<<<<<<<<<<<
  *         """
  *         Handles an unhandled exception.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_19handle_internal_server_error(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_10blacksheep_7baseapp_15BaseApplication_18handle_internal_server_error[] = "\n        Handles an unhandled exception.\n        ";
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_19handle_internal_server_error(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_17handle_internal_server_error(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10blacksheep_7baseapp_15BaseApplication_16handle_internal_server_error[] = "\n        Handles an unhandled exception.\n        ";
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_17handle_internal_server_error(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request = 0;
   PyObject *__pyx_v_exc = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -6122,77 +5997,77 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_request)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_internal_server_error", 1, 2, 2, 1); __PYX_ERR(0, 119, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_internal_server_error", 1, 2, 2, 1); __PYX_ERR(0, 116, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_internal_server_error") < 0)) __PYX_ERR(0, 119, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_internal_server_error") < 0)) __PYX_ERR(0, 116, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_request = ((struct __pyx_obj_10blacksheep_8messages_Request *)values[0]);
     __pyx_v_exc = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("handle_internal_server_error", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 119, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("handle_internal_server_error", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 116, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("blacksheep.baseapp.BaseApplication.handle_internal_server_error", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 119, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_exc), (&((PyTypeObject*)PyExc_Exception)[0]), 1, "exc", 0))) __PYX_ERR(0, 119, __pyx_L1_error)
-  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_18handle_internal_server_error(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), __pyx_v_request, __pyx_v_exc);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_exc), (&((PyTypeObject*)PyExc_Exception)[0]), 1, "exc", 0))) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_16handle_internal_server_error(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), __pyx_v_request, __pyx_v_exc);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_18handle_internal_server_error(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, PyObject *__pyx_v_exc) {
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_16handle_internal_server_error(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, PyObject *__pyx_v_exc) {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("handle_internal_server_error", 0);
   __pyx_cur_scope = (struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error *)__pyx_tp_new_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error(__pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 119, __pyx_L1_error)
+    __PYX_ERR(0, 116, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_request = __pyx_v_request;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_request);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_request);
   __pyx_cur_scope->__pyx_v_exc = __pyx_v_exc;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_20generator7, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_handle_internal_server_error, __pyx_n_s_BaseApplication_handle_internal, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_18generator7, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_handle_internal_server_error, __pyx_n_s_BaseApplication_handle_internal, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 116, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6200,15 +6075,15 @@
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_20generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_18generator7(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error *__pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -6229,58 +6104,58 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L11_resume_from_await;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 119, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 116, __pyx_L1_error)
 
-  /* "blacksheep/baseapp.pyx":123
+  /* "blacksheep/baseapp.pyx":120
  *         Handles an unhandled exception.
  *         """
  *         if 500 in self.exceptions_handlers:             # <<<<<<<<<<<<<<
  *             # give a chance to run to the custom exception handler - but if it
  *             # fails, handle the failure (otherwise the
  */
   if (unlikely(__pyx_cur_scope->__pyx_v_self->exceptions_handlers == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 123, __pyx_L1_error)
+    __PYX_ERR(0, 120, __pyx_L1_error)
   }
-  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_int_500, __pyx_cur_scope->__pyx_v_self->exceptions_handlers, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_int_500, __pyx_cur_scope->__pyx_v_self->exceptions_handlers, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 120, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "blacksheep/baseapp.pyx":126
+    /* "blacksheep/baseapp.pyx":123
  *             # give a chance to run to the custom exception handler - but if it
  *             # fails, handle the failure (otherwise the
  *             try:             # <<<<<<<<<<<<<<
  *                 return await self.exceptions_handlers[500](self, request, exc)
  *             except Exception:
  */
     {
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "blacksheep/baseapp.pyx":127
+        /* "blacksheep/baseapp.pyx":124
  *             # fails, handle the failure (otherwise the
  *             try:
  *                 return await self.exceptions_handlers[500](self, request, exc)             # <<<<<<<<<<<<<<
  *             except Exception:
  *                 self.logger.exception(
  */
         __Pyx_XDECREF(__pyx_r);
         if (unlikely(__pyx_cur_scope->__pyx_v_self->exceptions_handlers == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 127, __pyx_L5_error)
+          __PYX_ERR(0, 124, __pyx_L5_error)
         }
-        __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_cur_scope->__pyx_v_self->exceptions_handlers, __pyx_int_500); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 127, __pyx_L5_error)
+        __pyx_t_7 = __Pyx_PyDict_GetItem(__pyx_cur_scope->__pyx_v_self->exceptions_handlers, __pyx_int_500); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 124, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_7);
         __pyx_t_8 = NULL;
         __pyx_t_9 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
           __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
           if (likely(__pyx_t_8)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
@@ -6289,43 +6164,43 @@
             __Pyx_DECREF_SET(__pyx_t_7, function);
             __pyx_t_9 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_7)) {
           PyObject *__pyx_temp[4] = {__pyx_t_8, ((PyObject *)__pyx_cur_scope->__pyx_v_self), ((PyObject *)__pyx_cur_scope->__pyx_v_request), __pyx_cur_scope->__pyx_v_exc};
-          __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 127, __pyx_L5_error)
+          __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 124, __pyx_L5_error)
           __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_GOTREF(__pyx_t_6);
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
           PyObject *__pyx_temp[4] = {__pyx_t_8, ((PyObject *)__pyx_cur_scope->__pyx_v_self), ((PyObject *)__pyx_cur_scope->__pyx_v_request), __pyx_cur_scope->__pyx_v_exc};
-          __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 127, __pyx_L5_error)
+          __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 3+__pyx_t_9); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 124, __pyx_L5_error)
           __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_GOTREF(__pyx_t_6);
         } else
         #endif
         {
-          __pyx_t_10 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 127, __pyx_L5_error)
+          __pyx_t_10 = PyTuple_New(3+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 124, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_10);
           if (__pyx_t_8) {
             __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
           }
           __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_self));
           __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_self));
           PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, ((PyObject *)__pyx_cur_scope->__pyx_v_self));
           __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
           __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
           PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, ((PyObject *)__pyx_cur_scope->__pyx_v_request));
           __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
           __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
           PyTuple_SET_ITEM(__pyx_t_10, 2+__pyx_t_9, __pyx_cur_scope->__pyx_v_exc);
-          __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 127, __pyx_L5_error)
+          __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 124, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         }
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_6);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_XGOTREF(__pyx_r);
@@ -6348,108 +6223,108 @@
           __Pyx_XGOTREF(__pyx_t_3);
           __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
           __pyx_cur_scope->__pyx_t_1 = 0;
           __Pyx_XGOTREF(__pyx_t_4);
           __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
           __pyx_cur_scope->__pyx_t_2 = 0;
           __Pyx_XGOTREF(__pyx_t_5);
-          if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 127, __pyx_L5_error)
+          if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 124, __pyx_L5_error)
           __pyx_t_6 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_6);
         } else {
           __pyx_t_6 = NULL;
-          if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_6) < 0) __PYX_ERR(0, 127, __pyx_L5_error)
+          if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_6) < 0) __PYX_ERR(0, 124, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_6);
         }
         __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         goto __pyx_L9_try_return;
 
-        /* "blacksheep/baseapp.pyx":126
+        /* "blacksheep/baseapp.pyx":123
  *             # give a chance to run to the custom exception handler - but if it
  *             # fails, handle the failure (otherwise the
  *             try:             # <<<<<<<<<<<<<<
  *                 return await self.exceptions_handlers[500](self, request, exc)
  *             except Exception:
  */
       }
       __pyx_L5_error:;
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "blacksheep/baseapp.pyx":128
+      /* "blacksheep/baseapp.pyx":125
  *             try:
  *                 return await self.exceptions_handlers[500](self, request, exc)
  *             except Exception:             # <<<<<<<<<<<<<<
  *                 self.logger.exception(
  *                     "An exception occurred while trying to apply a custom 500 Internal Server Error handler!"
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_9) {
         __Pyx_AddTraceback("blacksheep.baseapp.BaseApplication.handle_internal_server_error", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_10) < 0) __PYX_ERR(0, 128, __pyx_L7_except_error)
+        if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_10) < 0) __PYX_ERR(0, 125, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_10);
 
-        /* "blacksheep/baseapp.pyx":129
+        /* "blacksheep/baseapp.pyx":126
  *                 return await self.exceptions_handlers[500](self, request, exc)
  *             except Exception:
  *                 self.logger.exception(             # <<<<<<<<<<<<<<
  *                     "An exception occurred while trying to apply a custom 500 Internal Server Error handler!"
  *                 )
  */
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self->logger, __pyx_n_s_exception); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 129, __pyx_L7_except_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_self->logger, __pyx_n_s_exception); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 126, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_12 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
           __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
           if (likely(__pyx_t_12)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
             __Pyx_INCREF(__pyx_t_12);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_11, function);
           }
         }
         __pyx_t_8 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_12, __pyx_kp_u_An_exception_occurred_while_tryi) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_kp_u_An_exception_occurred_while_tryi);
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 129, __pyx_L7_except_error)
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 126, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-        /* "blacksheep/baseapp.pyx":132
+        /* "blacksheep/baseapp.pyx":129
  *                     "An exception occurred while trying to apply a custom 500 Internal Server Error handler!"
  *                 )
  *                 return Response(500, content=TextContent('Internal Server Error'))             # <<<<<<<<<<<<<<
  *         if self.show_error_details:
  *             return self.server_error_details_handler.produce_response(request, exc)
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 132, __pyx_L7_except_error)
+        __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 129, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_11 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8contents_TextContent), __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 132, __pyx_L7_except_error)
+        __pyx_t_11 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8contents_TextContent), __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 129, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_11);
-        if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_content, __pyx_t_11) < 0) __PYX_ERR(0, 132, __pyx_L7_except_error)
+        if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_content, __pyx_t_11) < 0) __PYX_ERR(0, 129, __pyx_L7_except_error)
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __pyx_t_11 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8messages_Response), __pyx_tuple__8, __pyx_t_8); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 132, __pyx_L7_except_error)
+        __pyx_t_11 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8messages_Response), __pyx_tuple__8, __pyx_t_8); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 129, __pyx_L7_except_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         goto __pyx_L8_except_return;
       }
       goto __pyx_L7_except_error;
       __pyx_L7_except_error:;
 
-      /* "blacksheep/baseapp.pyx":126
+      /* "blacksheep/baseapp.pyx":123
  *             # give a chance to run to the custom exception handler - but if it
  *             # fails, handle the failure (otherwise the
  *             try:             # <<<<<<<<<<<<<<
  *                 return await self.exceptions_handlers[500](self, request, exc)
  *             except Exception:
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -6467,44 +6342,44 @@
       __Pyx_XGIVEREF(__pyx_t_3);
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       goto __pyx_L0;
     }
 
-    /* "blacksheep/baseapp.pyx":123
+    /* "blacksheep/baseapp.pyx":120
  *         Handles an unhandled exception.
  *         """
  *         if 500 in self.exceptions_handlers:             # <<<<<<<<<<<<<<
  *             # give a chance to run to the custom exception handler - but if it
  *             # fails, handle the failure (otherwise the
  */
   }
 
-  /* "blacksheep/baseapp.pyx":133
+  /* "blacksheep/baseapp.pyx":130
  *                 )
  *                 return Response(500, content=TextContent('Internal Server Error'))
  *         if self.show_error_details:             # <<<<<<<<<<<<<<
  *             return self.server_error_details_handler.produce_response(request, exc)
  *         return Response(500, content=TextContent("Internal server error."))
  */
   __pyx_t_2 = (__pyx_cur_scope->__pyx_v_self->show_error_details != 0);
   if (__pyx_t_2) {
 
-    /* "blacksheep/baseapp.pyx":134
+    /* "blacksheep/baseapp.pyx":131
  *                 return Response(500, content=TextContent('Internal Server Error'))
  *         if self.show_error_details:
  *             return self.server_error_details_handler.produce_response(request, exc)             # <<<<<<<<<<<<<<
  *         return Response(500, content=TextContent("Internal server error."))
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_server_error_details_handler); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_server_error_details_handler); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_produce_response); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_produce_response); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
@@ -6514,80 +6389,80 @@
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_9 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, ((PyObject *)__pyx_cur_scope->__pyx_v_request), __pyx_cur_scope->__pyx_v_exc};
-      __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 134, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 131, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_10);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_7, ((PyObject *)__pyx_cur_scope->__pyx_v_request), __pyx_cur_scope->__pyx_v_exc};
-      __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 134, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 131, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_GOTREF(__pyx_t_10);
     } else
     #endif
     {
-      __pyx_t_11 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 134, __pyx_L1_error)
+      __pyx_t_11 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 131, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       if (__pyx_t_7) {
         __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_7); __pyx_t_7 = NULL;
       }
       __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
       __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
       PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_9, ((PyObject *)__pyx_cur_scope->__pyx_v_request));
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
       PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_9, __pyx_cur_scope->__pyx_v_exc);
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_11, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 134, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_11, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 131, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     goto __pyx_L0;
 
-    /* "blacksheep/baseapp.pyx":133
+    /* "blacksheep/baseapp.pyx":130
  *                 )
  *                 return Response(500, content=TextContent('Internal Server Error'))
  *         if self.show_error_details:             # <<<<<<<<<<<<<<
  *             return self.server_error_details_handler.produce_response(request, exc)
  *         return Response(500, content=TextContent("Internal server error."))
  */
   }
 
-  /* "blacksheep/baseapp.pyx":135
+  /* "blacksheep/baseapp.pyx":132
  *         if self.show_error_details:
  *             return self.server_error_details_handler.produce_response(request, exc)
  *         return Response(500, content=TextContent("Internal server error."))             # <<<<<<<<<<<<<<
  * 
  *     async def _apply_exception_handler(self, Request request, Exception exc, object exception_handler):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8contents_TextContent), __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8contents_TextContent), __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_content, __pyx_t_6) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_content, __pyx_t_6) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8messages_Response), __pyx_tuple__8, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_8messages_Response), __pyx_tuple__8, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   goto __pyx_L0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "blacksheep/baseapp.pyx":119
+  /* "blacksheep/baseapp.pyx":116
  *         return None
  * 
  *     async def handle_internal_server_error(self, Request request, Exception exc):             # <<<<<<<<<<<<<<
  *         """
  *         Handles an unhandled exception.
  */
 
@@ -6606,27 +6481,27 @@
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_23generator8(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_21generator8(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "blacksheep/baseapp.pyx":137
+/* "blacksheep/baseapp.pyx":134
  *         return Response(500, content=TextContent("Internal server error."))
  * 
  *     async def _apply_exception_handler(self, Request request, Exception exc, object exception_handler):             # <<<<<<<<<<<<<<
  *         try:
  *             return await exception_handler(self, request, exc)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_22_apply_exception_handler(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_22_apply_exception_handler(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_20_apply_exception_handler(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_20_apply_exception_handler(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request = 0;
   PyObject *__pyx_v_exc = 0;
   PyObject *__pyx_v_exception_handler = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -6653,71 +6528,71 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_request)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_apply_exception_handler", 1, 3, 3, 1); __PYX_ERR(0, 137, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_apply_exception_handler", 1, 3, 3, 1); __PYX_ERR(0, 134, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exception_handler)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_apply_exception_handler", 1, 3, 3, 2); __PYX_ERR(0, 137, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_apply_exception_handler", 1, 3, 3, 2); __PYX_ERR(0, 134, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_apply_exception_handler") < 0)) __PYX_ERR(0, 137, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_apply_exception_handler") < 0)) __PYX_ERR(0, 134, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_request = ((struct __pyx_obj_10blacksheep_8messages_Request *)values[0]);
     __pyx_v_exc = ((PyObject*)values[1]);
     __pyx_v_exception_handler = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_apply_exception_handler", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 137, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_apply_exception_handler", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 134, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("blacksheep.baseapp.BaseApplication._apply_exception_handler", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 137, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_exc), (&((PyTypeObject*)PyExc_Exception)[0]), 1, "exc", 0))) __PYX_ERR(0, 137, __pyx_L1_error)
-  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_21_apply_exception_handler(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), __pyx_v_request, __pyx_v_exc, __pyx_v_exception_handler);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 134, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_exc), (&((PyTypeObject*)PyExc_Exception)[0]), 1, "exc", 0))) __PYX_ERR(0, 134, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_19_apply_exception_handler(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), __pyx_v_request, __pyx_v_exc, __pyx_v_exception_handler);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_21_apply_exception_handler(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, PyObject *__pyx_v_exc, PyObject *__pyx_v_exception_handler) {
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_19_apply_exception_handler(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, PyObject *__pyx_v_exc, PyObject *__pyx_v_exception_handler) {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_apply_exception_handler", 0);
   __pyx_cur_scope = (struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler *)__pyx_tp_new_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler(__pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 137, __pyx_L1_error)
+    __PYX_ERR(0, 134, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_request = __pyx_v_request;
@@ -6726,15 +6601,15 @@
   __pyx_cur_scope->__pyx_v_exc = __pyx_v_exc;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
   __pyx_cur_scope->__pyx_v_exception_handler = __pyx_v_exception_handler;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exception_handler);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exception_handler);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_23generator8, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_apply_exception_handler, __pyx_n_s_BaseApplication__apply_exception, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_21generator8, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_apply_exception_handler, __pyx_n_s_BaseApplication__apply_exception, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 134, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6742,15 +6617,15 @@
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_23generator8(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_21generator8(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler *__pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -6780,31 +6655,31 @@
     case 1: goto __pyx_L10_resume_from_await;
     case 2: goto __pyx_L18_resume_from_await;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 134, __pyx_L1_error)
 
-  /* "blacksheep/baseapp.pyx":138
+  /* "blacksheep/baseapp.pyx":135
  * 
  *     async def _apply_exception_handler(self, Request request, Exception exc, object exception_handler):
  *         try:             # <<<<<<<<<<<<<<
  *             return await exception_handler(self, request, exc)
  *         except Exception as server_ex:
  */
   {
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "blacksheep/baseapp.pyx":139
+      /* "blacksheep/baseapp.pyx":136
  *     async def _apply_exception_handler(self, Request request, Exception exc, object exception_handler):
  *         try:
  *             return await exception_handler(self, request, exc)             # <<<<<<<<<<<<<<
  *         except Exception as server_ex:
  *             return await self.handle_exception(request, server_ex)
  */
       __Pyx_XDECREF(__pyx_r);
@@ -6820,43 +6695,43 @@
           __Pyx_DECREF_SET(__pyx_t_5, function);
           __pyx_t_7 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[4] = {__pyx_t_6, ((PyObject *)__pyx_cur_scope->__pyx_v_self), ((PyObject *)__pyx_cur_scope->__pyx_v_request), __pyx_cur_scope->__pyx_v_exc};
-        __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L4_error)
+        __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L4_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_4);
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[4] = {__pyx_t_6, ((PyObject *)__pyx_cur_scope->__pyx_v_self), ((PyObject *)__pyx_cur_scope->__pyx_v_request), __pyx_cur_scope->__pyx_v_exc};
-        __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L4_error)
+        __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L4_error)
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_GOTREF(__pyx_t_4);
       } else
       #endif
       {
-        __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 139, __pyx_L4_error)
+        __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 136, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_8);
         if (__pyx_t_6) {
           __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
         }
         __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_self));
         __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_self));
         PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, ((PyObject *)__pyx_cur_scope->__pyx_v_self));
         __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
         __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
         PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, ((PyObject *)__pyx_cur_scope->__pyx_v_request));
         __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
         __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
         PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_cur_scope->__pyx_v_exc);
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L4_error)
+        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_4);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XGOTREF(__pyx_r);
@@ -6879,67 +6754,67 @@
         __Pyx_XGOTREF(__pyx_t_1);
         __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
         __pyx_cur_scope->__pyx_t_1 = 0;
         __Pyx_XGOTREF(__pyx_t_2);
         __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
         __pyx_cur_scope->__pyx_t_2 = 0;
         __Pyx_XGOTREF(__pyx_t_3);
-        if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 139, __pyx_L4_error)
+        if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 136, __pyx_L4_error)
         __pyx_t_4 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_4);
       } else {
         __pyx_t_4 = NULL;
-        if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_4) < 0) __PYX_ERR(0, 139, __pyx_L4_error)
+        if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_4) < 0) __PYX_ERR(0, 136, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_4);
       }
       __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       goto __pyx_L8_try_return;
 
-      /* "blacksheep/baseapp.pyx":138
+      /* "blacksheep/baseapp.pyx":135
  * 
  *     async def _apply_exception_handler(self, Request request, Exception exc, object exception_handler):
  *         try:             # <<<<<<<<<<<<<<
  *             return await exception_handler(self, request, exc)
  *         except Exception as server_ex:
  */
     }
     __pyx_L4_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "blacksheep/baseapp.pyx":140
+    /* "blacksheep/baseapp.pyx":137
  *         try:
  *             return await exception_handler(self, request, exc)
  *         except Exception as server_ex:             # <<<<<<<<<<<<<<
  *             return await self.handle_exception(request, server_ex)
  * 
  */
     __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_7) {
       __Pyx_AddTraceback("blacksheep.baseapp.BaseApplication._apply_exception_handler", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_5, &__pyx_t_8) < 0) __PYX_ERR(0, 140, __pyx_L6_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_5, &__pyx_t_8) < 0) __PYX_ERR(0, 137, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_5);
       __pyx_cur_scope->__pyx_v_server_ex = __pyx_t_5;
       /*try:*/ {
 
-        /* "blacksheep/baseapp.pyx":141
+        /* "blacksheep/baseapp.pyx":138
  *             return await exception_handler(self, request, exc)
  *         except Exception as server_ex:
  *             return await self.handle_exception(request, server_ex)             # <<<<<<<<<<<<<<
  * 
  *     async def handle_http_exception(self, Request request, HTTPException http_exception):
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_exception); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 141, __pyx_L16_error)
+        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_exception); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 138, __pyx_L16_error)
         __Pyx_GOTREF(__pyx_t_9);
         __pyx_t_10 = NULL;
         __pyx_t_7 = 0;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
           __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
           if (likely(__pyx_t_10)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
@@ -6948,40 +6823,40 @@
             __Pyx_DECREF_SET(__pyx_t_9, function);
             __pyx_t_7 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
         if (PyFunction_Check(__pyx_t_9)) {
           PyObject *__pyx_temp[3] = {__pyx_t_10, ((PyObject *)__pyx_cur_scope->__pyx_v_request), __pyx_cur_scope->__pyx_v_server_ex};
-          __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 141, __pyx_L16_error)
+          __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L16_error)
           __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
           __Pyx_GOTREF(__pyx_t_6);
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
         if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
           PyObject *__pyx_temp[3] = {__pyx_t_10, ((PyObject *)__pyx_cur_scope->__pyx_v_request), __pyx_cur_scope->__pyx_v_server_ex};
-          __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 141, __pyx_L16_error)
+          __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L16_error)
           __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
           __Pyx_GOTREF(__pyx_t_6);
         } else
         #endif
         {
-          __pyx_t_11 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 141, __pyx_L16_error)
+          __pyx_t_11 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 138, __pyx_L16_error)
           __Pyx_GOTREF(__pyx_t_11);
           if (__pyx_t_10) {
             __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_10); __pyx_t_10 = NULL;
           }
           __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
           __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
           PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_7, ((PyObject *)__pyx_cur_scope->__pyx_v_request));
           __Pyx_INCREF(__pyx_cur_scope->__pyx_v_server_ex);
           __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_server_ex);
           PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_7, __pyx_cur_scope->__pyx_v_server_ex);
-          __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 141, __pyx_L16_error)
+          __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 138, __pyx_L16_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         }
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_6);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_XGOTREF(__pyx_r);
@@ -7019,30 +6894,30 @@
           __Pyx_XGOTREF(__pyx_t_4);
           __pyx_t_5 = __pyx_cur_scope->__pyx_t_4;
           __pyx_cur_scope->__pyx_t_4 = 0;
           __Pyx_XGOTREF(__pyx_t_5);
           __pyx_t_8 = __pyx_cur_scope->__pyx_t_5;
           __pyx_cur_scope->__pyx_t_5 = 0;
           __Pyx_XGOTREF(__pyx_t_8);
-          if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 141, __pyx_L16_error)
+          if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 138, __pyx_L16_error)
           __pyx_t_6 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_6);
         } else {
           __pyx_t_6 = NULL;
-          if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_6) < 0) __PYX_ERR(0, 141, __pyx_L16_error)
+          if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_6) < 0) __PYX_ERR(0, 138, __pyx_L16_error)
           __Pyx_GOTREF(__pyx_t_6);
         }
         __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L15_return;
       }
 
-      /* "blacksheep/baseapp.pyx":140
+      /* "blacksheep/baseapp.pyx":137
  *         try:
  *             return await exception_handler(self, request, exc)
  *         except Exception as server_ex:             # <<<<<<<<<<<<<<
  *             return await self.handle_exception(request, server_ex)
  * 
  */
       /*finally:*/ {
@@ -7114,15 +6989,15 @@
           goto __pyx_L7_except_return;
         }
       }
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
-    /* "blacksheep/baseapp.pyx":138
+    /* "blacksheep/baseapp.pyx":135
  * 
  *     async def _apply_exception_handler(self, Request request, Exception exc, object exception_handler):
  *         try:             # <<<<<<<<<<<<<<
  *             return await exception_handler(self, request, exc)
  *         except Exception as server_ex:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -7141,15 +7016,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "blacksheep/baseapp.pyx":137
+  /* "blacksheep/baseapp.pyx":134
  *         return Response(500, content=TextContent("Internal server error."))
  * 
  *     async def _apply_exception_handler(self, Request request, Exception exc, object exception_handler):             # <<<<<<<<<<<<<<
  *         try:
  *             return await exception_handler(self, request, exc)
  */
 
@@ -7169,27 +7044,27 @@
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_26generator9(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_24generator9(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "blacksheep/baseapp.pyx":143
+/* "blacksheep/baseapp.pyx":140
  *             return await self.handle_exception(request, server_ex)
  * 
  *     async def handle_http_exception(self, Request request, HTTPException http_exception):             # <<<<<<<<<<<<<<
  *         exception_handler = self.get_http_exception_handler(http_exception)
  *         if exception_handler:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_25handle_http_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_25handle_http_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_23handle_http_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_23handle_http_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request = 0;
   struct __pyx_obj_10blacksheep_10exceptions_HTTPException *__pyx_v_http_exception = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -7213,77 +7088,77 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_request)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_http_exception)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_http_exception", 1, 2, 2, 1); __PYX_ERR(0, 143, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_http_exception", 1, 2, 2, 1); __PYX_ERR(0, 140, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_http_exception") < 0)) __PYX_ERR(0, 143, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_http_exception") < 0)) __PYX_ERR(0, 140, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_request = ((struct __pyx_obj_10blacksheep_8messages_Request *)values[0]);
     __pyx_v_http_exception = ((struct __pyx_obj_10blacksheep_10exceptions_HTTPException *)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("handle_http_exception", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 143, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("handle_http_exception", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 140, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("blacksheep.baseapp.BaseApplication.handle_http_exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 143, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_http_exception), __pyx_ptype_10blacksheep_10exceptions_HTTPException, 1, "http_exception", 0))) __PYX_ERR(0, 143, __pyx_L1_error)
-  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_24handle_http_exception(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), __pyx_v_request, __pyx_v_http_exception);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 140, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_http_exception), __pyx_ptype_10blacksheep_10exceptions_HTTPException, 1, "http_exception", 0))) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_22handle_http_exception(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), __pyx_v_request, __pyx_v_http_exception);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_24handle_http_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, struct __pyx_obj_10blacksheep_10exceptions_HTTPException *__pyx_v_http_exception) {
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_22handle_http_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_request, struct __pyx_obj_10blacksheep_10exceptions_HTTPException *__pyx_v_http_exception) {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("handle_http_exception", 0);
   __pyx_cur_scope = (struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception *)__pyx_tp_new_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception(__pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 143, __pyx_L1_error)
+    __PYX_ERR(0, 140, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_request = __pyx_v_request;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_request);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_request);
   __pyx_cur_scope->__pyx_v_http_exception = __pyx_v_http_exception;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_http_exception);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_http_exception);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_26generator9, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_handle_http_exception, __pyx_n_s_BaseApplication_handle_http_exce, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_24generator9, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_handle_http_exception, __pyx_n_s_BaseApplication_handle_http_exce, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 140, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7291,15 +7166,15 @@
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_26generator9(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_24generator9(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception *__pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -7315,48 +7190,48 @@
     case 1: goto __pyx_L5_resume_from_await;
     case 2: goto __pyx_L6_resume_from_await;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 140, __pyx_L1_error)
 
-  /* "blacksheep/baseapp.pyx":144
+  /* "blacksheep/baseapp.pyx":141
  * 
  *     async def handle_http_exception(self, Request request, HTTPException http_exception):
  *         exception_handler = self.get_http_exception_handler(http_exception)             # <<<<<<<<<<<<<<
  *         if exception_handler:
  *             return await self._apply_exception_handler(request, http_exception, exception_handler)
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_7baseapp_BaseApplication *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->get_http_exception_handler(__pyx_cur_scope->__pyx_v_self, __pyx_cur_scope->__pyx_v_http_exception); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_7baseapp_BaseApplication *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->get_http_exception_handler(__pyx_cur_scope->__pyx_v_self, __pyx_cur_scope->__pyx_v_http_exception); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_exception_handler = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "blacksheep/baseapp.pyx":145
+  /* "blacksheep/baseapp.pyx":142
  *     async def handle_http_exception(self, Request request, HTTPException http_exception):
  *         exception_handler = self.get_http_exception_handler(http_exception)
  *         if exception_handler:             # <<<<<<<<<<<<<<
  *             return await self._apply_exception_handler(request, http_exception, exception_handler)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_exception_handler); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 145, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_exception_handler); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 142, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "blacksheep/baseapp.pyx":146
+    /* "blacksheep/baseapp.pyx":143
  *         exception_handler = self.get_http_exception_handler(http_exception)
  *         if exception_handler:
  *             return await self._apply_exception_handler(request, http_exception, exception_handler)             # <<<<<<<<<<<<<<
  * 
  *         return await self.handle_exception(request, http_exception)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_apply_exception_handler); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_apply_exception_handler); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7365,43 +7240,43 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_5 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_4, ((PyObject *)__pyx_cur_scope->__pyx_v_request), ((PyObject *)__pyx_cur_scope->__pyx_v_http_exception), __pyx_cur_scope->__pyx_v_exception_handler};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_4, ((PyObject *)__pyx_cur_scope->__pyx_v_request), ((PyObject *)__pyx_cur_scope->__pyx_v_http_exception), __pyx_cur_scope->__pyx_v_exception_handler};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
     } else
     #endif
     {
-      __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 146, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       if (__pyx_t_4) {
         __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
       __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
       PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, ((PyObject *)__pyx_cur_scope->__pyx_v_request));
       __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_http_exception));
       __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_http_exception));
       PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, ((PyObject *)__pyx_cur_scope->__pyx_v_http_exception));
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exception_handler);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exception_handler);
       PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_5, __pyx_cur_scope->__pyx_v_exception_handler);
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XGOTREF(__pyx_r);
@@ -7409,43 +7284,43 @@
       __Pyx_XGIVEREF(__pyx_r);
       __Pyx_RefNannyFinishContext();
       __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
       /* return from generator, awaiting value */
       __pyx_generator->resume_label = 1;
       return __pyx_r;
       __pyx_L5_resume_from_await:;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 146, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 143, __pyx_L1_error)
       __pyx_t_1 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_1);
     } else {
       __pyx_t_1 = NULL;
-      if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
+      if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
     }
     __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "blacksheep/baseapp.pyx":145
+    /* "blacksheep/baseapp.pyx":142
  *     async def handle_http_exception(self, Request request, HTTPException http_exception):
  *         exception_handler = self.get_http_exception_handler(http_exception)
  *         if exception_handler:             # <<<<<<<<<<<<<<
  *             return await self._apply_exception_handler(request, http_exception, exception_handler)
  * 
  */
   }
 
-  /* "blacksheep/baseapp.pyx":148
+  /* "blacksheep/baseapp.pyx":145
  *             return await self._apply_exception_handler(request, http_exception, exception_handler)
  * 
  *         return await self.handle_exception(request, http_exception)             # <<<<<<<<<<<<<<
  * 
  *     async def handle_exception(self, request, exc):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_exception); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_exception); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_6 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7454,40 +7329,40 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, ((PyObject *)__pyx_cur_scope->__pyx_v_request), ((PyObject *)__pyx_cur_scope->__pyx_v_http_exception)};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, ((PyObject *)__pyx_cur_scope->__pyx_v_request), ((PyObject *)__pyx_cur_scope->__pyx_v_http_exception)};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
     __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_request));
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_5, ((PyObject *)__pyx_cur_scope->__pyx_v_request));
     __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_v_http_exception));
     __Pyx_GIVEREF(((PyObject *)__pyx_cur_scope->__pyx_v_http_exception));
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_5, ((PyObject *)__pyx_cur_scope->__pyx_v_http_exception));
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_XGOTREF(__pyx_r);
@@ -7495,27 +7370,27 @@
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
     /* return from generator, awaiting value */
     __pyx_generator->resume_label = 2;
     return __pyx_r;
     __pyx_L6_resume_from_await:;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 148, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 145, __pyx_L1_error)
     __pyx_t_1 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_1);
   } else {
     __pyx_t_1 = NULL;
-    if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 148, __pyx_L1_error)
+    if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 145, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
   }
   __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   goto __pyx_L0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "blacksheep/baseapp.pyx":143
+  /* "blacksheep/baseapp.pyx":140
  *             return await self.handle_exception(request, server_ex)
  * 
  *     async def handle_http_exception(self, Request request, HTTPException http_exception):             # <<<<<<<<<<<<<<
  *         exception_handler = self.get_http_exception_handler(http_exception)
  *         if exception_handler:
  */
 
@@ -7532,27 +7407,27 @@
   __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_29generator10(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_27generator10(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "blacksheep/baseapp.pyx":150
+/* "blacksheep/baseapp.pyx":147
  *         return await self.handle_exception(request, http_exception)
  * 
  *     async def handle_exception(self, request, exc):             # <<<<<<<<<<<<<<
  *         exception_handler = self.get_exception_handler(exc)
  *         if exception_handler:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_28handle_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_28handle_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_26handle_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_26handle_exception(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_request = 0;
   PyObject *__pyx_v_exc = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -7576,71 +7451,71 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_request)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_exception", 1, 2, 2, 1); __PYX_ERR(0, 150, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_exception", 1, 2, 2, 1); __PYX_ERR(0, 147, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_exception") < 0)) __PYX_ERR(0, 150, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_exception") < 0)) __PYX_ERR(0, 147, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_request = values[0];
     __pyx_v_exc = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("handle_exception", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 150, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("handle_exception", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 147, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("blacksheep.baseapp.BaseApplication.handle_exception", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_27handle_exception(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), __pyx_v_request, __pyx_v_exc);
+  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_25handle_exception(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), __pyx_v_request, __pyx_v_exc);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_27handle_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_request, PyObject *__pyx_v_exc) {
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_25handle_exception(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v_request, PyObject *__pyx_v_exc) {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception *__pyx_cur_scope;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("handle_exception", 0);
   __pyx_cur_scope = (struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception *)__pyx_tp_new_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception(__pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 150, __pyx_L1_error)
+    __PYX_ERR(0, 147, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_request = __pyx_v_request;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_request);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_request);
   __pyx_cur_scope->__pyx_v_exc = __pyx_v_exc;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_29generator10, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_handle_exception, __pyx_n_s_BaseApplication_handle_exception, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Coroutine_New((__pyx_coroutine_body_t) __pyx_gb_10blacksheep_7baseapp_15BaseApplication_27generator10, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_handle_exception, __pyx_n_s_BaseApplication_handle_exception, __pyx_n_s_blacksheep_baseapp); if (unlikely(!gen)) __PYX_ERR(0, 147, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7648,15 +7523,15 @@
   __pyx_r = NULL;
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_29generator10(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
+static PyObject *__pyx_gb_10blacksheep_7baseapp_15BaseApplication_27generator10(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value) /* generator body */
 {
   struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception *__pyx_cur_scope = ((struct __pyx_obj_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception *)__pyx_generator->closure);
   PyObject *__pyx_r = NULL;
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -7672,49 +7547,49 @@
     case 1: goto __pyx_L5_resume_from_await;
     case 2: goto __pyx_L6_resume_from_await;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 147, __pyx_L1_error)
 
-  /* "blacksheep/baseapp.pyx":151
+  /* "blacksheep/baseapp.pyx":148
  * 
  *     async def handle_exception(self, request, exc):
  *         exception_handler = self.get_exception_handler(exc)             # <<<<<<<<<<<<<<
  *         if exception_handler:
  *             return await self._apply_exception_handler(request, exc, exception_handler)
  */
-  if (!(likely(__Pyx_PyException_Check(__pyx_cur_scope->__pyx_v_exc))||((__pyx_cur_scope->__pyx_v_exc) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "Exception", Py_TYPE(__pyx_cur_scope->__pyx_v_exc)->tp_name), 0))) __PYX_ERR(0, 151, __pyx_L1_error)
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_7baseapp_BaseApplication *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->get_exception_handler(__pyx_cur_scope->__pyx_v_self, ((PyObject*)__pyx_cur_scope->__pyx_v_exc)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+  if (!(likely(__Pyx_PyException_Check(__pyx_cur_scope->__pyx_v_exc))||((__pyx_cur_scope->__pyx_v_exc) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "Exception", Py_TYPE(__pyx_cur_scope->__pyx_v_exc)->tp_name), 0))) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_7baseapp_BaseApplication *)__pyx_cur_scope->__pyx_v_self->__pyx_vtab)->get_exception_handler(__pyx_cur_scope->__pyx_v_self, ((PyObject*)__pyx_cur_scope->__pyx_v_exc)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_exception_handler = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "blacksheep/baseapp.pyx":152
+  /* "blacksheep/baseapp.pyx":149
  *     async def handle_exception(self, request, exc):
  *         exception_handler = self.get_exception_handler(exc)
  *         if exception_handler:             # <<<<<<<<<<<<<<
  *             return await self._apply_exception_handler(request, exc, exception_handler)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_exception_handler); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 152, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_exception_handler); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 149, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "blacksheep/baseapp.pyx":153
+    /* "blacksheep/baseapp.pyx":150
  *         exception_handler = self.get_exception_handler(exc)
  *         if exception_handler:
  *             return await self._apply_exception_handler(request, exc, exception_handler)             # <<<<<<<<<<<<<<
  * 
  *         return await self.handle_internal_server_error(request, exc)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_apply_exception_handler); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_apply_exception_handler); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 150, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7723,43 +7598,43 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_5 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc, __pyx_cur_scope->__pyx_v_exception_handler};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc, __pyx_cur_scope->__pyx_v_exception_handler};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 3+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_GOTREF(__pyx_t_1);
     } else
     #endif
     {
-      __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(3+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 150, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       if (__pyx_t_4) {
         __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
       }
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_request);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_request);
       PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_cur_scope->__pyx_v_request);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
       PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, __pyx_cur_scope->__pyx_v_exc);
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exception_handler);
       __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exception_handler);
       PyTuple_SET_ITEM(__pyx_t_6, 2+__pyx_t_5, __pyx_cur_scope->__pyx_v_exception_handler);
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XGOTREF(__pyx_r);
@@ -7767,41 +7642,41 @@
       __Pyx_XGIVEREF(__pyx_r);
       __Pyx_RefNannyFinishContext();
       __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
       /* return from generator, awaiting value */
       __pyx_generator->resume_label = 1;
       return __pyx_r;
       __pyx_L5_resume_from_await:;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 153, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 150, __pyx_L1_error)
       __pyx_t_1 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_1);
     } else {
       __pyx_t_1 = NULL;
-      if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
+      if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
     }
     __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "blacksheep/baseapp.pyx":152
+    /* "blacksheep/baseapp.pyx":149
  *     async def handle_exception(self, request, exc):
  *         exception_handler = self.get_exception_handler(exc)
  *         if exception_handler:             # <<<<<<<<<<<<<<
  *             return await self._apply_exception_handler(request, exc, exception_handler)
  * 
  */
   }
 
-  /* "blacksheep/baseapp.pyx":155
+  /* "blacksheep/baseapp.pyx":152
  *             return await self._apply_exception_handler(request, exc, exception_handler)
  * 
  *         return await self.handle_internal_server_error(request, exc)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_internal_server_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_handle_internal_server_error); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_6 = NULL;
   __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7810,40 +7685,40 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_5 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_cur_scope->__pyx_v_request, __pyx_cur_scope->__pyx_v_exc};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 155, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_request);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_request);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_5, __pyx_cur_scope->__pyx_v_request);
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_exc);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_exc);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_5, __pyx_cur_scope->__pyx_v_exc);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __Pyx_Coroutine_Yield_From(__pyx_generator, __pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_XGOTREF(__pyx_r);
@@ -7851,27 +7726,27 @@
     __Pyx_XGIVEREF(__pyx_r);
     __Pyx_RefNannyFinishContext();
     __Pyx_Coroutine_ResetAndClearException(__pyx_generator);
     /* return from generator, awaiting value */
     __pyx_generator->resume_label = 2;
     return __pyx_r;
     __pyx_L6_resume_from_await:;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 155, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 152, __pyx_L1_error)
     __pyx_t_1 = __pyx_sent_value; __Pyx_INCREF(__pyx_t_1);
   } else {
     __pyx_t_1 = NULL;
-    if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
+    if (__Pyx_PyGen_FetchStopIterationValue(&__pyx_t_1) < 0) __PYX_ERR(0, 152, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
   }
   __pyx_r = NULL; __Pyx_ReturnWithStopIteration(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   goto __pyx_L0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "blacksheep/baseapp.pyx":150
+  /* "blacksheep/baseapp.pyx":147
  *         return await self.handle_exception(request, http_exception)
  * 
  *     async def handle_exception(self, request, exc):             # <<<<<<<<<<<<<<
  *         exception_handler = self.get_exception_handler(exc)
  *         if exception_handler:
  */
 
@@ -8160,27 +8035,27 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_31__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_31__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_29__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_29__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_30__reduce_cython__(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_28__reduce_cython__(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_30__reduce_cython__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self) {
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_28__reduce_cython__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -8424,27 +8299,27 @@
  *     else:
  *         return __pyx_unpickle_BaseApplication, (type(self), 0xe75049b, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_BaseApplication__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_33__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_33__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_31__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_7baseapp_15BaseApplication_31__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_32__setstate_cython__(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_10blacksheep_7baseapp_15BaseApplication_30__setstate_cython__(((struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_32__setstate_cython__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_10blacksheep_7baseapp_15BaseApplication_30__setstate_cython__(struct __pyx_obj_10blacksheep_7baseapp_BaseApplication *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -10013,23 +9888,22 @@
   }
 }
 
 static PyMethodDef __pyx_methods_10blacksheep_7baseapp_BaseApplication[] = {
   {"init_exceptions_handlers", (PyCFunction)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_3init_exceptions_handlers, METH_NOARGS, 0},
   {"log_unhandled_exc", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_5log_unhandled_exc, METH_VARARGS|METH_KEYWORDS, 0},
   {"log_handled_exc", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_8log_handled_exc, METH_VARARGS|METH_KEYWORDS, 0},
-  {"get_route_match", (PyCFunction)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_11get_route_match, METH_O, 0},
-  {"handle", (PyCFunction)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_13handle, METH_O, 0},
-  {"handle_request_handler_exception", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_16handle_request_handler_exception, METH_VARARGS|METH_KEYWORDS, 0},
-  {"handle_internal_server_error", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_19handle_internal_server_error, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10blacksheep_7baseapp_15BaseApplication_18handle_internal_server_error},
-  {"_apply_exception_handler", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_22_apply_exception_handler, METH_VARARGS|METH_KEYWORDS, 0},
-  {"handle_http_exception", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_25handle_http_exception, METH_VARARGS|METH_KEYWORDS, 0},
-  {"handle_exception", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_28handle_exception, METH_VARARGS|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_31__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_33__setstate_cython__, METH_O, 0},
+  {"handle", (PyCFunction)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_11handle, METH_O, 0},
+  {"handle_request_handler_exception", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_14handle_request_handler_exception, METH_VARARGS|METH_KEYWORDS, 0},
+  {"handle_internal_server_error", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_17handle_internal_server_error, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10blacksheep_7baseapp_15BaseApplication_16handle_internal_server_error},
+  {"_apply_exception_handler", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_20_apply_exception_handler, METH_VARARGS|METH_KEYWORDS, 0},
+  {"handle_http_exception", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_23handle_http_exception, METH_VARARGS|METH_KEYWORDS, 0},
+  {"handle_exception", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_26handle_exception, METH_VARARGS|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_29__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_10blacksheep_7baseapp_15BaseApplication_31__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_10blacksheep_7baseapp_BaseApplication[] = {
   {(char *)"show_error_details", __pyx_getprop_10blacksheep_7baseapp_15BaseApplication_show_error_details, __pyx_setprop_10blacksheep_7baseapp_15BaseApplication_show_error_details, (char *)0, 0},
   {(char *)"router", __pyx_getprop_10blacksheep_7baseapp_15BaseApplication_router, 0, (char *)0, 0},
   {(char *)"logger", __pyx_getprop_10blacksheep_7baseapp_15BaseApplication_logger, 0, (char *)0, 0},
@@ -11569,15 +11443,14 @@
   {&__pyx_n_s_exception, __pyx_k_exception, sizeof(__pyx_k_exception), 0, 0, 1, 1},
   {&__pyx_n_s_exception_handler, __pyx_k_exception_handler, sizeof(__pyx_k_exception_handler), 0, 0, 1, 1},
   {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
   {&__pyx_n_s_getLogger, __pyx_k_getLogger, sizeof(__pyx_k_getLogger), 0, 0, 1, 1},
   {&__pyx_n_s_get_class_instance_hierarchy, __pyx_k_get_class_instance_hierarchy, sizeof(__pyx_k_get_class_instance_hierarchy), 0, 0, 1, 1},
   {&__pyx_n_s_get_logger, __pyx_k_get_logger, sizeof(__pyx_k_get_logger), 0, 0, 1, 1},
   {&__pyx_n_s_get_match, __pyx_k_get_match, sizeof(__pyx_k_get_match), 0, 0, 1, 1},
-  {&__pyx_n_s_get_route_match, __pyx_k_get_route_match, sizeof(__pyx_k_get_route_match), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_handle, __pyx_k_handle, sizeof(__pyx_k_handle), 0, 0, 1, 1},
   {&__pyx_n_s_handle_bad_request, __pyx_k_handle_bad_request, sizeof(__pyx_k_handle_bad_request), 0, 0, 1, 1},
   {&__pyx_n_s_handle_exception, __pyx_k_handle_exception, sizeof(__pyx_k_handle_exception), 0, 0, 1, 1},
   {&__pyx_n_s_handle_http_exception, __pyx_k_handle_http_exception, sizeof(__pyx_k_handle_http_exception), 0, 0, 1, 1},
   {&__pyx_n_s_handle_internal_server_error, __pyx_k_handle_internal_server_error, sizeof(__pyx_k_handle_internal_server_error), 0, 0, 1, 1},
   {&__pyx_n_s_handle_not_found, __pyx_k_handle_not_found, sizeof(__pyx_k_handle_not_found), 0, 0, 1, 1},
@@ -11659,47 +11532,47 @@
  * 
  * 
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_int_400); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "blacksheep/baseapp.pyx":95
+  /* "blacksheep/baseapp.pyx":92
  *         # for example, a user might return "None" from an handler
  *         # this might be ambiguous, if a programmer thinks to return None for "Not found"
  *         return response or Response(204)             # <<<<<<<<<<<<<<
  * 
  *     async def handle_request_handler_exception(self, request, exc):
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_int_204); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_int_204); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "blacksheep/baseapp.pyx":132
+  /* "blacksheep/baseapp.pyx":129
  *                     "An exception occurred while trying to apply a custom 500 Internal Server Error handler!"
  *                 )
  *                 return Response(500, content=TextContent('Internal Server Error'))             # <<<<<<<<<<<<<<
  *         if self.show_error_details:
  *             return self.server_error_details_handler.produce_response(request, exc)
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_int_500); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_int_500); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Internal_Server_Error); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Internal_Server_Error); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "blacksheep/baseapp.pyx":135
+  /* "blacksheep/baseapp.pyx":132
  *         if self.show_error_details:
  *             return self.server_error_details_handler.produce_response(request, exc)
  *         return Response(500, content=TextContent("Internal server error."))             # <<<<<<<<<<<<<<
  * 
  *     async def _apply_exception_handler(self, Request request, Exception exc, object exception_handler):
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Internal_server_error); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Internal_server_error); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xe75049b, 0xc7f976d, 0xa0c2b62):             # <<<<<<<<<<<<<<
@@ -11878,55 +11751,55 @@
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_4_log_handled_exc.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_4_log_handled_exc.tp_dictoffset && __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_4_log_handled_exc.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_4_log_handled_exc.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_4_log_handled_exc = &__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_4_log_handled_exc;
-  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_5_handle) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_5_handle) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_5_handle.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_5_handle.tp_dictoffset && __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_5_handle.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_5_handle.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_5_handle = &__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_5_handle;
-  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception.tp_dictoffset && __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception = &__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_6_handle_request_handler_exception;
-  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error) < 0) __PYX_ERR(0, 119, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error.tp_dictoffset && __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error = &__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_7_handle_internal_server_error;
-  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler.tp_dictoffset && __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler = &__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_8__apply_exception_handler;
-  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception.tp_dictoffset && __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception = &__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_9_handle_http_exception;
-  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception) < 0) __PYX_ERR(0, 150, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception) < 0) __PYX_ERR(0, 147, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception.tp_dictoffset && __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception = &__pyx_type_10blacksheep_7baseapp___pyx_scope_struct_10_handle_exception;
```

### Comparing `blacksheep-2.0a4/blacksheep/baseapp.pxd` & `blacksheep-2.0a5/blacksheep/baseapp.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/baseapp.pyi` & `blacksheep-2.0a5/blacksheep/baseapp.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
 from typing import Awaitable, Callable, Dict, Optional, Type, TypeVar, Union
 
 from blacksheep.exceptions import HTTPException
 from blacksheep.messages import Request, Response
 from blacksheep.server.application import Application
-from blacksheep.server.routing import RouteMatch, Router
+from blacksheep.server.routing import RouteMatch, RouterProtocol
 
 ExcT = TypeVar("ExcT", bound=Exception)
 
 ExceptionHandlersType = Dict[
     Union[int, Type[Exception]],
     Callable[[Application, Request, ExcT], Awaitable[Response]],
 ]
 
 class BaseApplication:
-    def __init__(self, show_error_details: bool, router: Router):
+    def __init__(self, show_error_details: bool, router: RouterProtocol):
         self.router = router
         self.exceptions_handlers = self.init_exceptions_handlers()
         self.show_error_details = show_error_details
     def init_exceptions_handlers(self) -> ExceptionHandlersType: ...
     async def handle(self, request: Request) -> Response: ...
     async def handle_internal_server_error(
         self, request: Request, exc: Exception
```

### Comparing `blacksheep-2.0a4/blacksheep/baseapp.pyx` & `blacksheep-2.0a5/blacksheep/baseapp.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -64,22 +64,19 @@
             self.logger.info(
                 "Handled error: \"%s %s\". %s",
                 request.method,
                 request.url.value.decode(),
                 str(exc)
             )
 
-    def get_route_match(self, Request request):
-        return self.router.get_match(request.method, request._path)
-
     async def handle(self, Request request):
         cdef object route
         cdef Response response
 
-        route = self.get_route_match(request)
+        route = self.router.get_match(request)
 
         if route:
             request.route_values = route.values
 
             try:
                 response = await route.handler(request)
             except Exception as exc:
```

### Comparing `blacksheep-2.0a4/blacksheep/client/connection.py` & `blacksheep-2.0a5/blacksheep/client/connection.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/client/cookies.py` & `blacksheep-2.0a5/blacksheep/client/cookies.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/client/exceptions.py` & `blacksheep-2.0a5/blacksheep/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/client/pool.py` & `blacksheep-2.0a5/blacksheep/client/pool.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/client/session.py` & `blacksheep-2.0a5/blacksheep/client/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,15 @@
 import asyncio
 import ssl
 from asyncio import AbstractEventLoop, TimeoutError
-from typing import (
-    Any,
-    AnyStr,
-    Callable,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-    cast,
-)
+from typing import Any, AnyStr, Callable, Dict, List, Optional, Tuple, Type, Union, cast
 from urllib.parse import urlencode
 
 from blacksheep import URL, Content, InvalidURL, Request, Response
+from blacksheep.common.types import HeadersType, ParamsType, URLType, normalize_headers
 from blacksheep.middlewares import get_middlewares_chain
 from blacksheep.utils.aio import get_running_loop
 
 from .connection import ConnectionClosedError
 from .cookies import CookieJar, cookies_middleware
 from .exceptions import (
     CircularRedirectError,
@@ -28,39 +17,14 @@
     MaximumRedirectsExceededError,
     MissingLocationForRedirect,
     RequestTimeout,
     UnsupportedRedirect,
 )
 from .pool import ClientConnection, ConnectionPools
 
-URLType = Union[str, bytes, URL]
-KeyValuePair = Tuple[AnyStr, AnyStr]
-Headers = Union[Dict[AnyStr, AnyStr], Iterable[KeyValuePair]]
-Params = Union[Dict[AnyStr, AnyStr], Iterable[KeyValuePair]]
-
-
-def _ensure_header_bytes(value: AnyStr) -> bytes:
-    return value if isinstance(value, bytes) else value.encode("ascii")
-
-
-def normalize_headers(
-    headers: Optional[Headers],
-) -> Optional[List[Tuple[bytes, bytes]]]:
-    if headers is None:
-        return None
-    if isinstance(headers, dict):
-        return [
-            (_ensure_header_bytes(key), _ensure_header_bytes(value))
-            for key, value in headers.items()
-        ]
-    return [
-        (_ensure_header_bytes(key), _ensure_header_bytes(value))
-        for key, value in headers
-    ]
-
 
 class RedirectsCache:
     """Used to store permanent redirects urls for later reuse"""
 
     __slots__ = ("_cache",)
 
     def __init__(self):
@@ -90,15 +54,15 @@
 class ClientSession:
     def __init__(
         self,
         loop: Optional[AbstractEventLoop] = None,
         base_url: Union[None, bytes, str, URL] = None,
         ssl: Union[None, bool, ssl.SSLContext] = None,
         pools: Optional[ConnectionPools] = None,
-        default_headers: Optional[Headers] = None,
+        default_headers: Optional[HeadersType] = None,
         follow_redirects: bool = True,
         connection_timeout: float = 10.0,
         request_timeout: float = 60.0,
         maximum_redirects: int = 20,
         redirects_cache_type: Union[Type[RedirectsCache], Any] = None,
         cookie_jar: Union[None, bool, CookieJar] = None,
         middlewares: Optional[List[Callable[..., Any]]] = None,
@@ -148,15 +112,15 @@
         self.delay_before_retry = 0.5
 
     @property
     def default_headers(self) -> Optional[List[Tuple[bytes, bytes]]]:
         return self._default_headers
 
     @default_headers.setter
-    def default_headers(self, value: Optional[Headers]):
+    def default_headers(self, value: Optional[HeadersType]):
         self._default_headers = normalize_headers(value)
 
     @property
     def middlewares(self) -> List[Callable[..., Any]]:
         return self._middlewares
 
     @middlewares.setter
@@ -191,15 +155,15 @@
 
         self._handler = get_middlewares_chain(self._middlewares, root_handler)
 
     def use_standard_redirect(self):
         """Uses specification compliant handling of 301 and 302 redirects"""
         self.non_standard_handling_of_301_302_redirect_method = False
 
-    def get_url(self, url, params: Optional[Params] = None) -> bytes:
+    def get_url(self, url, params: Optional[ParamsType] = None) -> bytes:
         value = self.get_url_value(url)
         if not params:
             return value
         query = urlencode(params).encode("ascii")
         return value + (b"&" if b"?" in value else b"?") + query
 
     def get_url_value(self, url: Union[AnyStr, URL]) -> bytes:
@@ -382,99 +346,99 @@
             raise
         except TimeoutError:
             raise RequestTimeout(request.url, self.request_timeout)
 
     async def get(
         self,
         url: URLType,
-        headers: Optional[Headers] = None,
-        params: Optional[Params] = None,
+        headers: Optional[HeadersType] = None,
+        params: Optional[ParamsType] = None,
     ) -> Response:
         return await self.send(
             Request("GET", self.get_url(url, params), normalize_headers(headers))
         )
 
     async def post(
         self,
         url: URLType,
         content: Optional[Content] = None,
-        headers: Optional[Headers] = None,
-        params: Optional[Params] = None,
+        headers: Optional[HeadersType] = None,
+        params: Optional[ParamsType] = None,
     ) -> Response:
         request = Request("POST", self.get_url(url, params), normalize_headers(headers))
         return await self.send(
             request.with_content(content) if content is not None else request
         )
 
     async def put(
         self,
         url: URLType,
         content: Optional[Content] = None,
-        headers: Optional[Headers] = None,
-        params: Optional[Params] = None,
+        headers: Optional[HeadersType] = None,
+        params: Optional[ParamsType] = None,
     ) -> Response:
         request = Request("PUT", self.get_url(url, params), normalize_headers(headers))
         return await self.send(
             request.with_content(content) if content is not None else request
         )
 
     async def delete(
         self,
         url: URLType,
         content: Optional[Content] = None,
-        headers: Optional[Headers] = None,
-        params: Optional[Params] = None,
+        headers: Optional[HeadersType] = None,
+        params: Optional[ParamsType] = None,
     ) -> Response:
         request = Request(
             "DELETE", self.get_url(url, params), normalize_headers(headers)
         )
         return await self.send(
             request.with_content(content) if content is not None else request
         )
 
     async def trace(
         self,
         url: URLType,
-        headers: Optional[Headers] = None,
-        params: Optional[Params] = None,
+        headers: Optional[HeadersType] = None,
+        params: Optional[ParamsType] = None,
     ) -> Response:
         return await self.send(
             Request("TRACE", self.get_url(url, params), normalize_headers(headers))
         )
 
     async def head(
         self,
         url: URLType,
-        headers: Optional[Headers] = None,
-        params: Optional[Params] = None,
+        headers: Optional[HeadersType] = None,
+        params: Optional[ParamsType] = None,
     ) -> Response:
         return await self.send(
             Request("HEAD", self.get_url(url, params), normalize_headers(headers))
         )
 
     async def patch(
         self,
         url: URLType,
         content: Optional[Content] = None,
-        headers: Optional[Headers] = None,
-        params: Optional[Params] = None,
+        headers: Optional[HeadersType] = None,
+        params: Optional[ParamsType] = None,
     ) -> Response:
         request = Request(
             "PATCH", self.get_url(url, params), normalize_headers(headers)
         )
         return await self.send(
             request.with_content(content) if content is not None else request
         )
 
     async def options(
         self,
         url: URLType,
         content: Optional[Content] = None,
-        headers: Optional[Headers] = None,
-        params: Optional[Params] = None,
+        headers: Optional[HeadersType] = None,
+        params: Optional[ParamsType] = None,
     ) -> Response:
         request = Request(
             "OPTIONS", self.get_url(url, params), normalize_headers(headers)
         )
         return await self.send(
             request.with_content(content) if content is not None else request
         )
```

### Comparing `blacksheep-2.0a4/blacksheep/common/files/asyncfs.py` & `blacksheep-2.0a5/blacksheep/common/files/asyncfs.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/common/files/info.py` & `blacksheep-2.0a5/blacksheep/common/files/info.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/common/files/pathsutils.py` & `blacksheep-2.0a5/blacksheep/common/files/pathsutils.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/contents.c` & `blacksheep-2.0a5/blacksheep/contents.c`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/contents.pxd` & `blacksheep-2.0a5/blacksheep/contents.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/contents.pyi` & `blacksheep-2.0a5/blacksheep/contents.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/contents.pyx` & `blacksheep-2.0a5/blacksheep/contents.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/cookies.c` & `blacksheep-2.0a5/blacksheep/cookies.c`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/cookies.pxd` & `blacksheep-2.0a5/blacksheep/cookies.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/cookies.pyi` & `blacksheep-2.0a5/blacksheep/cookies.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/cookies.pyx` & `blacksheep-2.0a5/blacksheep/cookies.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/exceptions.c` & `blacksheep-2.0a5/blacksheep/exceptions.c`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/exceptions.pyi` & `blacksheep-2.0a5/blacksheep/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/exceptions.pyx` & `blacksheep-2.0a5/blacksheep/exceptions.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/headers.c` & `blacksheep-2.0a5/blacksheep/headers.c`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/headers.pxd` & `blacksheep-2.0a5/blacksheep/headers.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/headers.pyi` & `blacksheep-2.0a5/blacksheep/headers.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/headers.pyx` & `blacksheep-2.0a5/blacksheep/headers.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/messages.c` & `blacksheep-2.0a5/blacksheep/messages.c`

 * *Files 1% similar despite different names*

```diff
@@ -1485,14 +1485,15 @@
  */
 
 struct __pyx_vtabstruct_10blacksheep_3url_URL {
   struct __pyx_obj_10blacksheep_3url_URL *(*join)(struct __pyx_obj_10blacksheep_3url_URL *, struct __pyx_obj_10blacksheep_3url_URL *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*base_url)(struct __pyx_obj_10blacksheep_3url_URL *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*with_host)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*with_scheme)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
+  struct __pyx_obj_10blacksheep_3url_URL *(*with_query)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_10blacksheep_3url_URL *__pyx_vtabptr_10blacksheep_3url_URL;
 
 
 /* "headers.pxd":13
  * 
  * 
@@ -1559,15 +1560,15 @@
 struct __pyx_vtabstruct_10blacksheep_8messages_Request {
   struct __pyx_vtabstruct_10blacksheep_8messages_Message __pyx_base;
   int (*expect_100_continue)(struct __pyx_obj_10blacksheep_8messages_Request *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_10blacksheep_8messages_Request *__pyx_vtabptr_10blacksheep_8messages_Request;
 
 
-/* "blacksheep/messages.pyx":481
+/* "blacksheep/messages.pyx":488
  * 
  * 
  * cdef class Response(Message):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(
  */
 
@@ -2587,25 +2588,27 @@
 static const char __pyx_k_file_name[] = "file_name";
 static const char __pyx_k_headers_2[] = "_headers";
 static const char __pyx_k_multipart[] = "multipart";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_raw_query[] = "_raw_query";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_timedelta[] = "timedelta";
+static const char __pyx_k_urlencode[] = "urlencode";
 static const char __pyx_k_HTTPStatus[] = "HTTPStatus";
 static const char __pyx_k_ISO_8859_1[] = "ISO-8859-1";
 static const char __pyx_k_Response_2[] = "Response";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_add_header[] = "add_header";
 static const char __pyx_k_charset_rx[] = "_charset_rx";
 static const char __pyx_k_has_header[] = "has_header";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_set_cookie[] = "set-cookie";
 static const char __pyx_k_set_header[] = "set_header";
+static const char __pyx_k_with_query[] = "with_query";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_get_cookies[] = "get_cookies";
 static const char __pyx_k_get_headers[] = "get_headers";
 static const char __pyx_k_is_absolute[] = "is_absolute";
 static const char __pyx_k_is_redirect[] = "is_redirect";
 static const char __pyx_k_100_continue[] = "100-continue";
@@ -2836,20 +2839,22 @@
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_text;
 static PyObject *__pyx_n_s_throw;
 static PyObject *__pyx_n_s_timedelta;
 static PyObject *__pyx_n_s_unquote;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_url;
+static PyObject *__pyx_n_s_urlencode;
 static PyObject *__pyx_n_s_urllib_parse;
 static PyObject *__pyx_n_u_user;
 static PyObject *__pyx_n_s_utcnow;
 static PyObject *__pyx_n_u_utf8;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_s_with_content;
+static PyObject *__pyx_n_s_with_query;
 static PyObject *__pyx_n_b_xml;
 static PyObject *__pyx_pf_10blacksheep_8messages_parse_charset(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_value); /* proto */
 static int __pyx_pf_10blacksheep_8messages_7Message___init__(struct __pyx_obj_10blacksheep_8messages_Message *__pyx_v_self, PyObject *__pyx_v_headers); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Message_7headers___get__(struct __pyx_obj_10blacksheep_8messages_Message *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Message_2with_content(struct __pyx_obj_10blacksheep_8messages_Message *__pyx_v_self, struct __pyx_obj_10blacksheep_8contents_Content *__pyx_v_content); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Message_4get_first_header(struct __pyx_obj_10blacksheep_8messages_Message *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Message_6get_headers(struct __pyx_obj_10blacksheep_8messages_Message *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
@@ -2892,14 +2897,15 @@
 static PyObject *__pyx_pf_10blacksheep_8messages_7Request_9client_ip___get__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Request_18original_client_ip___get__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self); /* proto */
 static int __pyx_pf_10blacksheep_8messages_7Request_18original_client_ip_2__set__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Request_7session___get__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self); /* proto */
 static int __pyx_pf_10blacksheep_8messages_7Request_7session_2__set__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Request_2incoming(PyTypeObject *__pyx_v_cls, PyObject *__pyx_v_method, PyObject *__pyx_v_path, PyObject *__pyx_v_query, PyObject *__pyx_v_headers); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Request_5query___get__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self); /* proto */
+static int __pyx_pf_10blacksheep_8messages_7Request_5query_2__set__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Request_3url___get__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self); /* proto */
 static int __pyx_pf_10blacksheep_8messages_7Request_3url_2__set__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Request_4__repr__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Request_7cookies___get__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Request_6get_cookie(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self, PyObject *__pyx_v_name); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Request_8set_cookie(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self, PyObject *__pyx_v_name, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_10blacksheep_8messages_7Request_4etag___get__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self); /* proto */
@@ -11915,15 +11921,15 @@
 }
 
 /* "blacksheep/messages.pyx":376
  * 
  *     @property
  *     def query(self):             # <<<<<<<<<<<<<<
  *         if self._raw_query:
- *             return parse_qs(self._raw_query.decode('utf8'))
+ *             return parse_qs(self._raw_query.decode("utf8"))
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_10blacksheep_8messages_7Request_5query_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_10blacksheep_8messages_7Request_5query_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -11948,24 +11954,24 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "blacksheep/messages.pyx":377
  *     @property
  *     def query(self):
  *         if self._raw_query:             # <<<<<<<<<<<<<<
- *             return parse_qs(self._raw_query.decode('utf8'))
+ *             return parse_qs(self._raw_query.decode("utf8"))
  *         return {}
  */
   __pyx_t_1 = (__pyx_v_self->_raw_query != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_self->_raw_query) != 0);
   if (__pyx_t_1) {
 
     /* "blacksheep/messages.pyx":378
  *     def query(self):
  *         if self._raw_query:
- *             return parse_qs(self._raw_query.decode('utf8'))             # <<<<<<<<<<<<<<
+ *             return parse_qs(self._raw_query.decode("utf8"))             # <<<<<<<<<<<<<<
  *         return {}
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parse_qs); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 378, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (unlikely(__pyx_v_self->_raw_query == Py_None)) {
@@ -11994,39 +12000,39 @@
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
     /* "blacksheep/messages.pyx":377
  *     @property
  *     def query(self):
  *         if self._raw_query:             # <<<<<<<<<<<<<<
- *             return parse_qs(self._raw_query.decode('utf8'))
+ *             return parse_qs(self._raw_query.decode("utf8"))
  *         return {}
  */
   }
 
   /* "blacksheep/messages.pyx":379
  *         if self._raw_query:
- *             return parse_qs(self._raw_query.decode('utf8'))
+ *             return parse_qs(self._raw_query.decode("utf8"))
  *         return {}             # <<<<<<<<<<<<<<
  * 
- *     @property
+ *     @query.setter
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "blacksheep/messages.pyx":376
  * 
  *     @property
  *     def query(self):             # <<<<<<<<<<<<<<
  *         if self._raw_query:
- *             return parse_qs(self._raw_query.decode('utf8'))
+ *             return parse_qs(self._raw_query.decode("utf8"))
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
@@ -12037,14 +12043,194 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "blacksheep/messages.pyx":382
  * 
+ *     @query.setter
+ *     def query(self, value):             # <<<<<<<<<<<<<<
+ *         cdef bytes raw_query
+ *         raw_query = urlencode(value, True).encode("utf8")
+ */
+
+/* Python wrapper */
+static int __pyx_pw_10blacksheep_8messages_7Request_5query_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_10blacksheep_8messages_7Request_5query_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_10blacksheep_8messages_7Request_5query_2__set__(((struct __pyx_obj_10blacksheep_8messages_Request *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_10blacksheep_8messages_7Request_5query_2__set__(struct __pyx_obj_10blacksheep_8messages_Request *__pyx_v_self, PyObject *__pyx_v_value) {
+  PyObject *__pyx_v_raw_query = 0;
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__set__", 0);
+
+  /* "blacksheep/messages.pyx":384
+ *     def query(self, value):
+ *         cdef bytes raw_query
+ *         raw_query = urlencode(value, True).encode("utf8")             # <<<<<<<<<<<<<<
+ *         self._raw_query = raw_query
+ *         self.url = self.url.with_query(raw_query)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_urlencode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 384, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = NULL;
+  __pyx_t_5 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_4);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_5 = 1;
+    }
+  }
+  #if CYTHON_FAST_PYCALL
+  if (PyFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_value, Py_True};
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 384, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_2);
+  } else
+  #endif
+  #if CYTHON_FAST_PYCCALL
+  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
+    PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_v_value, Py_True};
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_5, 2+__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 384, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_GOTREF(__pyx_t_2);
+  } else
+  #endif
+  {
+    __pyx_t_6 = PyTuple_New(2+__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 384, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (__pyx_t_4) {
+      __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
+    }
+    __Pyx_INCREF(__pyx_v_value);
+    __Pyx_GIVEREF(__pyx_v_value);
+    PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_5, __pyx_v_value);
+    __Pyx_INCREF(Py_True);
+    __Pyx_GIVEREF(Py_True);
+    PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_5, Py_True);
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 384, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 384, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_n_u_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_u_utf8);
+  __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 384, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_v_raw_query = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "blacksheep/messages.pyx":385
+ *         cdef bytes raw_query
+ *         raw_query = urlencode(value, True).encode("utf8")
+ *         self._raw_query = raw_query             # <<<<<<<<<<<<<<
+ *         self.url = self.url.with_query(raw_query)
+ * 
+ */
+  __Pyx_INCREF(__pyx_v_raw_query);
+  __Pyx_GIVEREF(__pyx_v_raw_query);
+  __Pyx_GOTREF(__pyx_v_self->_raw_query);
+  __Pyx_DECREF(__pyx_v_self->_raw_query);
+  __pyx_v_self->_raw_query = __pyx_v_raw_query;
+
+  /* "blacksheep/messages.pyx":386
+ *         raw_query = urlencode(value, True).encode("utf8")
+ *         self._raw_query = raw_query
+ *         self.url = self.url.with_query(raw_query)             # <<<<<<<<<<<<<<
+ * 
+ *     @property
+ */
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_url); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_with_query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+    }
+  }
+  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_raw_query) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_raw_query);
+  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_url, __pyx_t_1) < 0) __PYX_ERR(0, 386, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "blacksheep/messages.pyx":382
+ * 
+ *     @query.setter
+ *     def query(self, value):             # <<<<<<<<<<<<<<
+ *         cdef bytes raw_query
+ *         raw_query = urlencode(value, True).encode("utf8")
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("blacksheep.messages.Request.query.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_raw_query);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "blacksheep/messages.pyx":389
+ * 
  *     @property
  *     def url(self):             # <<<<<<<<<<<<<<
  *         if self._url:
  *             return self._url
  */
 
 /* Python wrapper */
@@ -12067,117 +12253,117 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "blacksheep/messages.pyx":383
+  /* "blacksheep/messages.pyx":390
  *     @property
  *     def url(self):
  *         if self._url:             # <<<<<<<<<<<<<<
  *             return self._url
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_self->_url)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_self->_url)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 390, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "blacksheep/messages.pyx":384
+    /* "blacksheep/messages.pyx":391
  *     def url(self):
  *         if self._url:
  *             return self._url             # <<<<<<<<<<<<<<
  * 
  *         if self._raw_query:
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_self->_url));
     __pyx_r = ((PyObject *)__pyx_v_self->_url);
     goto __pyx_L0;
 
-    /* "blacksheep/messages.pyx":383
+    /* "blacksheep/messages.pyx":390
  *     @property
  *     def url(self):
  *         if self._url:             # <<<<<<<<<<<<<<
  *             return self._url
  * 
  */
   }
 
-  /* "blacksheep/messages.pyx":386
+  /* "blacksheep/messages.pyx":393
  *             return self._url
  * 
  *         if self._raw_query:             # <<<<<<<<<<<<<<
  *             self._url = URL(self._path + b'?' + self._raw_query)
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->_raw_query != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_self->_raw_query) != 0);
   if (__pyx_t_1) {
 
-    /* "blacksheep/messages.pyx":387
+    /* "blacksheep/messages.pyx":394
  * 
  *         if self._raw_query:
  *             self._url = URL(self._path + b'?' + self._raw_query)             # <<<<<<<<<<<<<<
  *         else:
  *             self._url = URL(self._path)
  */
-    __pyx_t_2 = PyNumber_Add(__pyx_v_self->_path, __pyx_kp_b__10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_v_self->_path, __pyx_kp_b__10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 394, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_self->_raw_query); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_self->_raw_query); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 394, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 394, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_v_self->_url);
     __Pyx_DECREF(((PyObject *)__pyx_v_self->_url));
     __pyx_v_self->_url = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "blacksheep/messages.pyx":386
+    /* "blacksheep/messages.pyx":393
  *             return self._url
  * 
  *         if self._raw_query:             # <<<<<<<<<<<<<<
  *             self._url = URL(self._path + b'?' + self._raw_query)
  *         else:
  */
     goto __pyx_L4;
   }
 
-  /* "blacksheep/messages.pyx":389
+  /* "blacksheep/messages.pyx":396
  *             self._url = URL(self._path + b'?' + self._raw_query)
  *         else:
  *             self._url = URL(self._path)             # <<<<<<<<<<<<<<
  *         return self._url
  * 
  */
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_v_self->_path); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_v_self->_path); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 396, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_v_self->_url);
     __Pyx_DECREF(((PyObject *)__pyx_v_self->_url));
     __pyx_v_self->_url = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_2);
     __pyx_t_2 = 0;
   }
   __pyx_L4:;
 
-  /* "blacksheep/messages.pyx":390
+  /* "blacksheep/messages.pyx":397
  *         else:
  *             self._url = URL(self._path)
  *         return self._url             # <<<<<<<<<<<<<<
  * 
  *     @url.setter
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self->_url));
   __pyx_r = ((PyObject *)__pyx_v_self->_url);
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":382
+  /* "blacksheep/messages.pyx":389
  * 
  *     @property
  *     def url(self):             # <<<<<<<<<<<<<<
  *         if self._url:
  *             return self._url
  */
 
@@ -12189,15 +12375,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":393
+/* "blacksheep/messages.pyx":400
  * 
  *     @url.setter
  *     def url(self, object value):             # <<<<<<<<<<<<<<
  *         cdef URL _url
  * 
  */
 
@@ -12224,296 +12410,296 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "blacksheep/messages.pyx":396
+  /* "blacksheep/messages.pyx":403
  *         cdef URL _url
  * 
  *         if value:             # <<<<<<<<<<<<<<
  *             if isinstance(value, bytes):
  *                 _url = URL(value)
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 403, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "blacksheep/messages.pyx":397
+    /* "blacksheep/messages.pyx":404
  * 
  *         if value:
  *             if isinstance(value, bytes):             # <<<<<<<<<<<<<<
  *                 _url = URL(value)
  *             elif isinstance(value, str):
  */
     __pyx_t_1 = PyBytes_Check(__pyx_v_value); 
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (__pyx_t_2) {
 
-      /* "blacksheep/messages.pyx":398
+      /* "blacksheep/messages.pyx":405
  *         if value:
  *             if isinstance(value, bytes):
  *                 _url = URL(value)             # <<<<<<<<<<<<<<
  *             elif isinstance(value, str):
  *                 _url = URL(value.encode('utf8'))
  */
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 398, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 405, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_v__url = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "blacksheep/messages.pyx":397
+      /* "blacksheep/messages.pyx":404
  * 
  *         if value:
  *             if isinstance(value, bytes):             # <<<<<<<<<<<<<<
  *                 _url = URL(value)
  *             elif isinstance(value, str):
  */
       goto __pyx_L4;
     }
 
-    /* "blacksheep/messages.pyx":399
+    /* "blacksheep/messages.pyx":406
  *             if isinstance(value, bytes):
  *                 _url = URL(value)
  *             elif isinstance(value, str):             # <<<<<<<<<<<<<<
  *                 _url = URL(value.encode('utf8'))
  *             elif isinstance(value, URL):
  */
     __pyx_t_2 = PyUnicode_Check(__pyx_v_value); 
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "blacksheep/messages.pyx":400
+      /* "blacksheep/messages.pyx":407
  *                 _url = URL(value)
  *             elif isinstance(value, str):
  *                 _url = URL(value.encode('utf8'))             # <<<<<<<<<<<<<<
  *             elif isinstance(value, URL):
  *                 _url = value
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_5 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_5)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_5);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_n_u_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_n_u_utf8);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 407, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_v__url = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "blacksheep/messages.pyx":399
+      /* "blacksheep/messages.pyx":406
  *             if isinstance(value, bytes):
  *                 _url = URL(value)
  *             elif isinstance(value, str):             # <<<<<<<<<<<<<<
  *                 _url = URL(value.encode('utf8'))
  *             elif isinstance(value, URL):
  */
       goto __pyx_L4;
     }
 
-    /* "blacksheep/messages.pyx":401
+    /* "blacksheep/messages.pyx":408
  *             elif isinstance(value, str):
  *                 _url = URL(value.encode('utf8'))
  *             elif isinstance(value, URL):             # <<<<<<<<<<<<<<
  *                 _url = value
  *             else:
  */
     __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_value, __pyx_ptype_10blacksheep_3url_URL); 
     __pyx_t_2 = (__pyx_t_1 != 0);
     if (likely(__pyx_t_2)) {
 
-      /* "blacksheep/messages.pyx":402
+      /* "blacksheep/messages.pyx":409
  *                 _url = URL(value.encode('utf8'))
  *             elif isinstance(value, URL):
  *                 _url = value             # <<<<<<<<<<<<<<
  *             else:
  *                 raise TypeError('Invalid value type, expected bytes, str, or URL')
  */
-      if (!(likely(((__pyx_v_value) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_value, __pyx_ptype_10blacksheep_3url_URL))))) __PYX_ERR(0, 402, __pyx_L1_error)
+      if (!(likely(((__pyx_v_value) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_value, __pyx_ptype_10blacksheep_3url_URL))))) __PYX_ERR(0, 409, __pyx_L1_error)
       __pyx_t_4 = __pyx_v_value;
       __Pyx_INCREF(__pyx_t_4);
       __pyx_v__url = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "blacksheep/messages.pyx":401
+      /* "blacksheep/messages.pyx":408
  *             elif isinstance(value, str):
  *                 _url = URL(value.encode('utf8'))
  *             elif isinstance(value, URL):             # <<<<<<<<<<<<<<
  *                 _url = value
  *             else:
  */
       goto __pyx_L4;
     }
 
-    /* "blacksheep/messages.pyx":404
+    /* "blacksheep/messages.pyx":411
  *                 _url = value
  *             else:
  *                 raise TypeError('Invalid value type, expected bytes, str, or URL')             # <<<<<<<<<<<<<<
  *         else:
  *             _url = None
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 404, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 404, __pyx_L1_error)
+      __PYX_ERR(0, 411, __pyx_L1_error)
     }
     __pyx_L4:;
 
-    /* "blacksheep/messages.pyx":396
+    /* "blacksheep/messages.pyx":403
  *         cdef URL _url
  * 
  *         if value:             # <<<<<<<<<<<<<<
  *             if isinstance(value, bytes):
  *                 _url = URL(value)
  */
     goto __pyx_L3;
   }
 
-  /* "blacksheep/messages.pyx":406
+  /* "blacksheep/messages.pyx":413
  *                 raise TypeError('Invalid value type, expected bytes, str, or URL')
  *         else:
  *             _url = None             # <<<<<<<<<<<<<<
  * 
  *         if _url:
  */
   /*else*/ {
     __Pyx_INCREF(Py_None);
     __pyx_v__url = ((struct __pyx_obj_10blacksheep_3url_URL *)Py_None);
   }
   __pyx_L3:;
 
-  /* "blacksheep/messages.pyx":408
+  /* "blacksheep/messages.pyx":415
  *             _url = None
  * 
  *         if _url:             # <<<<<<<<<<<<<<
  *             self._path = _url.path
  *             self._raw_query = _url.query
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v__url)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v__url)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 415, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "blacksheep/messages.pyx":409
+    /* "blacksheep/messages.pyx":416
  * 
  *         if _url:
  *             self._path = _url.path             # <<<<<<<<<<<<<<
  *             self._raw_query = _url.query
  *         else:
  */
     __pyx_t_4 = __pyx_v__url->path;
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __Pyx_GOTREF(__pyx_v_self->_path);
     __Pyx_DECREF(__pyx_v_self->_path);
     __pyx_v_self->_path = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "blacksheep/messages.pyx":410
+    /* "blacksheep/messages.pyx":417
  *         if _url:
  *             self._path = _url.path
  *             self._raw_query = _url.query             # <<<<<<<<<<<<<<
  *         else:
  *             self._path = None
  */
     __pyx_t_4 = __pyx_v__url->query;
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __Pyx_GOTREF(__pyx_v_self->_raw_query);
     __Pyx_DECREF(__pyx_v_self->_raw_query);
     __pyx_v_self->_raw_query = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "blacksheep/messages.pyx":408
+    /* "blacksheep/messages.pyx":415
  *             _url = None
  * 
  *         if _url:             # <<<<<<<<<<<<<<
  *             self._path = _url.path
  *             self._raw_query = _url.query
  */
     goto __pyx_L5;
   }
 
-  /* "blacksheep/messages.pyx":412
+  /* "blacksheep/messages.pyx":419
  *             self._raw_query = _url.query
  *         else:
  *             self._path = None             # <<<<<<<<<<<<<<
  *             self._raw_query = None
  *         self._url = _url
  */
   /*else*/ {
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->_path);
     __Pyx_DECREF(__pyx_v_self->_path);
     __pyx_v_self->_path = ((PyObject*)Py_None);
 
-    /* "blacksheep/messages.pyx":413
+    /* "blacksheep/messages.pyx":420
  *         else:
  *             self._path = None
  *             self._raw_query = None             # <<<<<<<<<<<<<<
  *         self._url = _url
  *         # unset the cached host
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->_raw_query);
     __Pyx_DECREF(__pyx_v_self->_raw_query);
     __pyx_v_self->_raw_query = ((PyObject*)Py_None);
   }
   __pyx_L5:;
 
-  /* "blacksheep/messages.pyx":414
+  /* "blacksheep/messages.pyx":421
  *             self._path = None
  *             self._raw_query = None
  *         self._url = _url             # <<<<<<<<<<<<<<
  *         # unset the cached host
  *         self.__dict__["host"] = None
  */
   __Pyx_INCREF(((PyObject *)__pyx_v__url));
   __Pyx_GIVEREF(((PyObject *)__pyx_v__url));
   __Pyx_GOTREF(__pyx_v_self->_url);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->_url));
   __pyx_v_self->_url = __pyx_v__url;
 
-  /* "blacksheep/messages.pyx":416
+  /* "blacksheep/messages.pyx":423
  *         self._url = _url
  *         # unset the cached host
  *         self.__dict__["host"] = None             # <<<<<<<<<<<<<<
  *         self.remove_header(b"host")
  * 
  */
   if (unlikely(__pyx_v_self->__dict__ == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 416, __pyx_L1_error)
+    __PYX_ERR(0, 423, __pyx_L1_error)
   }
-  if (unlikely(PyDict_SetItem(__pyx_v_self->__dict__, __pyx_n_u_host, Py_None) < 0)) __PYX_ERR(0, 416, __pyx_L1_error)
+  if (unlikely(PyDict_SetItem(__pyx_v_self->__dict__, __pyx_n_u_host, Py_None) < 0)) __PYX_ERR(0, 423, __pyx_L1_error)
 
-  /* "blacksheep/messages.pyx":417
+  /* "blacksheep/messages.pyx":424
  *         # unset the cached host
  *         self.__dict__["host"] = None
  *         self.remove_header(b"host")             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.remove_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_n_b_host, 0);
 
-  /* "blacksheep/messages.pyx":393
+  /* "blacksheep/messages.pyx":400
  * 
  *     @url.setter
  *     def url(self, object value):             # <<<<<<<<<<<<<<
  *         cdef URL _url
  * 
  */
 
@@ -12528,15 +12714,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v__url);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":419
+/* "blacksheep/messages.pyx":426
  *         self.remove_header(b"host")
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f'<Request {self.method} {self.url.value.decode()}>'
  * 
  */
 
@@ -12563,84 +12749,84 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "blacksheep/messages.pyx":420
+  /* "blacksheep/messages.pyx":427
  * 
  *     def __repr__(self):
  *         return f'<Request {self.method} {self.url.value.decode()}>'             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_3 = 127;
   __Pyx_INCREF(__pyx_kp_u_Request);
   __pyx_t_2 += 9;
   __Pyx_GIVEREF(__pyx_kp_u_Request);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Request);
-  __pyx_t_4 = __Pyx_PyUnicode_Unicode(__pyx_v_self->method); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_Unicode(__pyx_v_self->method); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u__12);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__12);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__12);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_url); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_url); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_value); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_value); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 420, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_INCREF(__pyx_kp_u__13);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__13);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__13);
-  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":419
+  /* "blacksheep/messages.pyx":426
  *         self.remove_header(b"host")
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f'<Request {self.method} {self.url.value.decode()}>'
  * 
  */
 
@@ -12654,15 +12840,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":423
+/* "blacksheep/messages.pyx":430
  * 
  *     @property
  *     def cookies(self):             # <<<<<<<<<<<<<<
  *         cdef bytes header
  *         cdef list cookies_headers
  */
 
@@ -12707,134 +12893,134 @@
   PyObject *__pyx_t_15 = NULL;
   int __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "blacksheep/messages.pyx":426
+  /* "blacksheep/messages.pyx":433
  *         cdef bytes header
  *         cdef list cookies_headers
  *         cdef dict cookies = {}             # <<<<<<<<<<<<<<
  * 
  *         cookies_headers = self.get_headers(b'cookie')
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_cookies = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":428
+  /* "blacksheep/messages.pyx":435
  *         cdef dict cookies = {}
  * 
  *         cookies_headers = self.get_headers(b'cookie')             # <<<<<<<<<<<<<<
  *         if cookies_headers:
  *             for header in cookies_headers:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_headers(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_n_b_cookie, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_headers(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_n_b_cookie, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_cookies_headers = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":429
+  /* "blacksheep/messages.pyx":436
  * 
  *         cookies_headers = self.get_headers(b'cookie')
  *         if cookies_headers:             # <<<<<<<<<<<<<<
  *             for header in cookies_headers:
  *                 # a single cookie header is expected from the client, but anyway here
  */
   __pyx_t_2 = (__pyx_v_cookies_headers != Py_None)&&(PyList_GET_SIZE(__pyx_v_cookies_headers) != 0);
   if (__pyx_t_2) {
 
-    /* "blacksheep/messages.pyx":430
+    /* "blacksheep/messages.pyx":437
  *         cookies_headers = self.get_headers(b'cookie')
  *         if cookies_headers:
  *             for header in cookies_headers:             # <<<<<<<<<<<<<<
  *                 # a single cookie header is expected from the client, but anyway here
  *                 # multiple headers are handled:
  */
     if (unlikely(__pyx_v_cookies_headers == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 430, __pyx_L1_error)
+      __PYX_ERR(0, 437, __pyx_L1_error)
     }
     __pyx_t_1 = __pyx_v_cookies_headers; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
     for (;;) {
       if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 430, __pyx_L1_error)
+      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 437, __pyx_L1_error)
       #else
-      __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 430, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
-      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 430, __pyx_L1_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 437, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_header, ((PyObject*)__pyx_t_4));
       __pyx_t_4 = 0;
 
-      /* "blacksheep/messages.pyx":433
+      /* "blacksheep/messages.pyx":440
  *                 # a single cookie header is expected from the client, but anyway here
  *                 # multiple headers are handled:
  *                 pairs = header.split(b'; ')             # <<<<<<<<<<<<<<
  * 
  *                 for fragment in pairs:
  */
-      __pyx_t_4 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyBytes_Type_split, __pyx_v_header, __pyx_kp_b__14); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyBytes_Type_split, __pyx_v_header, __pyx_kp_b__14); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 440, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_v_pairs, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "blacksheep/messages.pyx":435
+      /* "blacksheep/messages.pyx":442
  *                 pairs = header.split(b'; ')
  * 
  *                 for fragment in pairs:             # <<<<<<<<<<<<<<
  *                     try:
  *                         name, value = split_value(fragment, b"=")
  */
       if (likely(PyList_CheckExact(__pyx_v_pairs)) || PyTuple_CheckExact(__pyx_v_pairs)) {
         __pyx_t_4 = __pyx_v_pairs; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
         __pyx_t_6 = NULL;
       } else {
-        __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_pairs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 435, __pyx_L1_error)
+        __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_pairs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 442, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
-        __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 435, __pyx_L1_error)
+        __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 442, __pyx_L1_error)
       }
       for (;;) {
         if (likely(!__pyx_t_6)) {
           if (likely(PyList_CheckExact(__pyx_t_4))) {
             if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 435, __pyx_L1_error)
+            __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 442, __pyx_L1_error)
             #else
-            __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 435, __pyx_L1_error)
+            __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 442, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_7);
             #endif
           } else {
             if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 435, __pyx_L1_error)
+            __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 442, __pyx_L1_error)
             #else
-            __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 435, __pyx_L1_error)
+            __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 442, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_7);
             #endif
           }
         } else {
           __pyx_t_7 = __pyx_t_6(__pyx_t_4);
           if (unlikely(!__pyx_t_7)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 435, __pyx_L1_error)
+              else __PYX_ERR(0, 442, __pyx_L1_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_7);
         }
         __Pyx_XDECREF_SET(__pyx_v_fragment, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "blacksheep/messages.pyx":436
+        /* "blacksheep/messages.pyx":443
  * 
  *                 for fragment in pairs:
  *                     try:             # <<<<<<<<<<<<<<
  *                         name, value = split_value(fragment, b"=")
  *                     except ValueError as unpack_error:
  */
         {
@@ -12842,104 +13028,104 @@
           __Pyx_PyThreadState_assign
           __Pyx_ExceptionSave(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10);
           __Pyx_XGOTREF(__pyx_t_8);
           __Pyx_XGOTREF(__pyx_t_9);
           __Pyx_XGOTREF(__pyx_t_10);
           /*try:*/ {
 
-            /* "blacksheep/messages.pyx":437
+            /* "blacksheep/messages.pyx":444
  *                 for fragment in pairs:
  *                     try:
  *                         name, value = split_value(fragment, b"=")             # <<<<<<<<<<<<<<
  *                     except ValueError as unpack_error:
  *                         # discard cookie: in this case it's better to eat the exception
  */
-            if (!(likely(PyBytes_CheckExact(__pyx_v_fragment))||((__pyx_v_fragment) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_fragment)->tp_name), 0))) __PYX_ERR(0, 437, __pyx_L8_error)
-            __pyx_t_7 = __pyx_f_10blacksheep_7cookies_split_value(((PyObject*)__pyx_v_fragment), __pyx_kp_b__15); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 437, __pyx_L8_error)
+            if (!(likely(PyBytes_CheckExact(__pyx_v_fragment))||((__pyx_v_fragment) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_fragment)->tp_name), 0))) __PYX_ERR(0, 444, __pyx_L8_error)
+            __pyx_t_7 = __pyx_f_10blacksheep_7cookies_split_value(((PyObject*)__pyx_v_fragment), __pyx_kp_b__15); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 444, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_7);
             if (likely(__pyx_t_7 != Py_None)) {
               PyObject* sequence = __pyx_t_7;
               Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
               if (unlikely(size != 2)) {
                 if (size > 2) __Pyx_RaiseTooManyValuesError(2);
                 else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-                __PYX_ERR(0, 437, __pyx_L8_error)
+                __PYX_ERR(0, 444, __pyx_L8_error)
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
               __pyx_t_11 = PyTuple_GET_ITEM(sequence, 0); 
               __pyx_t_12 = PyTuple_GET_ITEM(sequence, 1); 
               __Pyx_INCREF(__pyx_t_11);
               __Pyx_INCREF(__pyx_t_12);
               #else
-              __pyx_t_11 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 437, __pyx_L8_error)
+              __pyx_t_11 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 444, __pyx_L8_error)
               __Pyx_GOTREF(__pyx_t_11);
-              __pyx_t_12 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 437, __pyx_L8_error)
+              __pyx_t_12 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 444, __pyx_L8_error)
               __Pyx_GOTREF(__pyx_t_12);
               #endif
               __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
             } else {
-              __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 437, __pyx_L8_error)
+              __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 444, __pyx_L8_error)
             }
             __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_11);
             __pyx_t_11 = 0;
             __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_12);
             __pyx_t_12 = 0;
 
-            /* "blacksheep/messages.pyx":436
+            /* "blacksheep/messages.pyx":443
  * 
  *                 for fragment in pairs:
  *                     try:             # <<<<<<<<<<<<<<
  *                         name, value = split_value(fragment, b"=")
  *                     except ValueError as unpack_error:
  */
           }
 
-          /* "blacksheep/messages.pyx":443
+          /* "blacksheep/messages.pyx":450
  *                         pass
  *                     else:
  *                         cookies[unquote(name.decode())] = unquote(value.rstrip(b'; ').decode())             # <<<<<<<<<<<<<<
  *         return cookies
  * 
  */
           /*else:*/ {
-            __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_unquote); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 443, __pyx_L10_except_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_unquote); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 450, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_12);
-            __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_rstrip); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 443, __pyx_L10_except_error)
+            __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_rstrip); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 450, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_14);
             __pyx_t_15 = NULL;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_14))) {
               __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_14);
               if (likely(__pyx_t_15)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
                 __Pyx_INCREF(__pyx_t_15);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_14, function);
               }
             }
             __pyx_t_13 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_14, __pyx_t_15, __pyx_kp_b__14) : __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_kp_b__14);
             __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-            if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 443, __pyx_L10_except_error)
+            if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 450, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_13);
             __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-            __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_decode); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 443, __pyx_L10_except_error)
+            __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_decode); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 450, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_14);
             __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
             __pyx_t_13 = NULL;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_14))) {
               __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_14);
               if (likely(__pyx_t_13)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
                 __Pyx_INCREF(__pyx_t_13);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_14, function);
               }
             }
             __pyx_t_11 = (__pyx_t_13) ? __Pyx_PyObject_CallOneArg(__pyx_t_14, __pyx_t_13) : __Pyx_PyObject_CallNoArg(__pyx_t_14);
             __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-            if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 443, __pyx_L10_except_error)
+            if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 450, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_11);
             __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
             __pyx_t_14 = NULL;
             if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
               __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_12);
               if (likely(__pyx_t_14)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
@@ -12947,34 +13133,34 @@
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_12, function);
               }
             }
             __pyx_t_7 = (__pyx_t_14) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_14, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_t_11);
             __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-            if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 443, __pyx_L10_except_error)
+            if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 450, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-            __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_unquote); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 443, __pyx_L10_except_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_unquote); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 450, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_11);
-            __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_decode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 443, __pyx_L10_except_error)
+            __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_decode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 450, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_13);
             __pyx_t_15 = NULL;
             if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_13))) {
               __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_13);
               if (likely(__pyx_t_15)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
                 __Pyx_INCREF(__pyx_t_15);
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_13, function);
               }
             }
             __pyx_t_14 = (__pyx_t_15) ? __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_t_15) : __Pyx_PyObject_CallNoArg(__pyx_t_13);
             __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-            if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 443, __pyx_L10_except_error)
+            if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 450, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_14);
             __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
             __pyx_t_13 = NULL;
             if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
               __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_11);
               if (likely(__pyx_t_13)) {
                 PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
@@ -12982,41 +13168,41 @@
                 __Pyx_INCREF(function);
                 __Pyx_DECREF_SET(__pyx_t_11, function);
               }
             }
             __pyx_t_12 = (__pyx_t_13) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_13, __pyx_t_14) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_14);
             __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
             __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-            if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 443, __pyx_L10_except_error)
+            if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 450, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_12);
             __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-            if (unlikely(PyDict_SetItem(__pyx_v_cookies, __pyx_t_12, __pyx_t_7) < 0)) __PYX_ERR(0, 443, __pyx_L10_except_error)
+            if (unlikely(PyDict_SetItem(__pyx_v_cookies, __pyx_t_12, __pyx_t_7) < 0)) __PYX_ERR(0, 450, __pyx_L10_except_error)
             __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
             __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
           }
           __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
           goto __pyx_L15_try_end;
           __pyx_L8_error:;
           __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
           __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
           __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-          /* "blacksheep/messages.pyx":438
+          /* "blacksheep/messages.pyx":445
  *                     try:
  *                         name, value = split_value(fragment, b"=")
  *                     except ValueError as unpack_error:             # <<<<<<<<<<<<<<
  *                         # discard cookie: in this case it's better to eat the exception
  *                         # than blocking a request just because a cookie is malformed
  */
           __pyx_t_16 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
           if (__pyx_t_16) {
             __Pyx_AddTraceback("blacksheep.messages.Request.cookies.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-            if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_12, &__pyx_t_11) < 0) __PYX_ERR(0, 438, __pyx_L10_except_error)
+            if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_12, &__pyx_t_11) < 0) __PYX_ERR(0, 445, __pyx_L10_except_error)
             __Pyx_GOTREF(__pyx_t_7);
             __Pyx_GOTREF(__pyx_t_12);
             __Pyx_GOTREF(__pyx_t_11);
             __Pyx_INCREF(__pyx_t_12);
             __pyx_v_unpack_error = __pyx_t_12;
             /*try:*/ {
             }
@@ -13032,15 +13218,15 @@
             __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
             __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
             goto __pyx_L9_exception_handled;
           }
           goto __pyx_L10_except_error;
           __pyx_L10_except_error:;
 
-          /* "blacksheep/messages.pyx":436
+          /* "blacksheep/messages.pyx":443
  * 
  *                 for fragment in pairs:
  *                     try:             # <<<<<<<<<<<<<<
  *                         name, value = split_value(fragment, b"=")
  *                     except ValueError as unpack_error:
  */
           __Pyx_XGIVEREF(__pyx_t_8);
@@ -13052,56 +13238,56 @@
           __Pyx_XGIVEREF(__pyx_t_8);
           __Pyx_XGIVEREF(__pyx_t_9);
           __Pyx_XGIVEREF(__pyx_t_10);
           __Pyx_ExceptionReset(__pyx_t_8, __pyx_t_9, __pyx_t_10);
           __pyx_L15_try_end:;
         }
 
-        /* "blacksheep/messages.pyx":435
+        /* "blacksheep/messages.pyx":442
  *                 pairs = header.split(b'; ')
  * 
  *                 for fragment in pairs:             # <<<<<<<<<<<<<<
  *                     try:
  *                         name, value = split_value(fragment, b"=")
  */
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "blacksheep/messages.pyx":430
+      /* "blacksheep/messages.pyx":437
  *         cookies_headers = self.get_headers(b'cookie')
  *         if cookies_headers:
  *             for header in cookies_headers:             # <<<<<<<<<<<<<<
  *                 # a single cookie header is expected from the client, but anyway here
  *                 # multiple headers are handled:
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "blacksheep/messages.pyx":429
+    /* "blacksheep/messages.pyx":436
  * 
  *         cookies_headers = self.get_headers(b'cookie')
  *         if cookies_headers:             # <<<<<<<<<<<<<<
  *             for header in cookies_headers:
  *                 # a single cookie header is expected from the client, but anyway here
  */
   }
 
-  /* "blacksheep/messages.pyx":444
+  /* "blacksheep/messages.pyx":451
  *                     else:
  *                         cookies[unquote(name.decode())] = unquote(value.rstrip(b'; ').decode())
  *         return cookies             # <<<<<<<<<<<<<<
  * 
  *     def get_cookie(self, str name):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_cookies);
   __pyx_r = __pyx_v_cookies;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":423
+  /* "blacksheep/messages.pyx":430
  * 
  *     @property
  *     def cookies(self):             # <<<<<<<<<<<<<<
  *         cdef bytes header
  *         cdef list cookies_headers
  */
 
@@ -13127,15 +13313,15 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XDECREF(__pyx_v_unpack_error);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":446
+/* "blacksheep/messages.pyx":453
  *         return cookies
  * 
  *     def get_cookie(self, str name):             # <<<<<<<<<<<<<<
  *         return self.cookies.get(name)
  * 
  */
 
@@ -13144,15 +13330,15 @@
 static PyObject *__pyx_pw_10blacksheep_8messages_7Request_7get_cookie(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_cookie (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 446, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 453, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_7Request_6get_cookie(((struct __pyx_obj_10blacksheep_8messages_Request *)__pyx_v_self), ((PyObject*)__pyx_v_name));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -13167,47 +13353,47 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_cookie", 0);
 
-  /* "blacksheep/messages.pyx":447
+  /* "blacksheep/messages.pyx":454
  * 
  *     def get_cookie(self, str name):
  *         return self.cookies.get(name)             # <<<<<<<<<<<<<<
  * 
  *     def set_cookie(self, str name, str value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cookies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cookies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 454, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_get); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 454, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 447, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 454, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":446
+  /* "blacksheep/messages.pyx":453
  *         return cookies
  * 
  *     def get_cookie(self, str name):             # <<<<<<<<<<<<<<
  *         return self.cookies.get(name)
  * 
  */
 
@@ -13220,15 +13406,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":449
+/* "blacksheep/messages.pyx":456
  *         return self.cookies.get(name)
  * 
  *     def set_cookie(self, str name, str value):             # <<<<<<<<<<<<<<
  *         """
  *         Sets a cookie in the request. This method also ensures that a single
  */
 
@@ -13263,39 +13449,39 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_cookie", 1, 2, 2, 1); __PYX_ERR(0, 449, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_cookie", 1, 2, 2, 1); __PYX_ERR(0, 456, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_cookie") < 0)) __PYX_ERR(0, 449, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_cookie") < 0)) __PYX_ERR(0, 456, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_name = ((PyObject*)values[0]);
     __pyx_v_value = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_cookie", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 449, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_cookie", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 456, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("blacksheep.messages.Request.set_cookie", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 449, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_value), (&PyUnicode_Type), 1, "value", 1))) __PYX_ERR(0, 449, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 456, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_value), (&PyUnicode_Type), 1, "value", 1))) __PYX_ERR(0, 456, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_7Request_8set_cookie(((struct __pyx_obj_10blacksheep_8messages_Request *)__pyx_v_self), __pyx_v_name, __pyx_v_value);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -13316,157 +13502,157 @@
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_cookie", 0);
 
-  /* "blacksheep/messages.pyx":457
+  /* "blacksheep/messages.pyx":464
  *         cdef bytes existing_cookie
  * 
  *         new_value = (quote(name) + "=" + quote(value)).encode()             # <<<<<<<<<<<<<<
  *         existing_cookie = self.get_first_header(b"cookie")
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_quote); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_quote); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_kp_u__15); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_kp_u__15); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_quote); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_quote); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_value);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Add(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Add(__pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 457, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 464, __pyx_L1_error)
   __pyx_v_new_value = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":458
+  /* "blacksheep/messages.pyx":465
  * 
  *         new_value = (quote(name) + "=" + quote(value)).encode()
  *         existing_cookie = self.get_first_header(b"cookie")             # <<<<<<<<<<<<<<
  * 
  *         if existing_cookie:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_n_b_cookie, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_n_b_cookie, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 465, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_existing_cookie = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":460
+  /* "blacksheep/messages.pyx":467
  *         existing_cookie = self.get_first_header(b"cookie")
  * 
  *         if existing_cookie:             # <<<<<<<<<<<<<<
  *             self.set_header(b"cookie", existing_cookie + b";" + new_value)
  *         else:
  */
   __pyx_t_6 = (__pyx_v_existing_cookie != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_existing_cookie) != 0);
   if (__pyx_t_6) {
 
-    /* "blacksheep/messages.pyx":461
+    /* "blacksheep/messages.pyx":468
  * 
  *         if existing_cookie:
  *             self.set_header(b"cookie", existing_cookie + b";" + new_value)             # <<<<<<<<<<<<<<
  *         else:
  *             self.__headers.append((b"cookie", new_value))
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_v_existing_cookie, __pyx_kp_b__16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_v_existing_cookie, __pyx_kp_b__16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_new_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 461, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_new_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.set_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_n_b_cookie, ((PyObject*)__pyx_t_2), 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "blacksheep/messages.pyx":460
+    /* "blacksheep/messages.pyx":467
  *         existing_cookie = self.get_first_header(b"cookie")
  * 
  *         if existing_cookie:             # <<<<<<<<<<<<<<
  *             self.set_header(b"cookie", existing_cookie + b";" + new_value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "blacksheep/messages.pyx":463
+  /* "blacksheep/messages.pyx":470
  *             self.set_header(b"cookie", existing_cookie + b";" + new_value)
  *         else:
  *             self.__headers.append((b"cookie", new_value))             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   /*else*/ {
     if (unlikely(__pyx_v_self->__pyx_base.__pyx___headers == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-      __PYX_ERR(0, 463, __pyx_L1_error)
+      __PYX_ERR(0, 470, __pyx_L1_error)
     }
-    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 463, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_n_b_cookie);
     __Pyx_GIVEREF(__pyx_n_b_cookie);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_n_b_cookie);
     __Pyx_INCREF(__pyx_v_new_value);
     __Pyx_GIVEREF(__pyx_v_new_value);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_new_value);
-    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_self->__pyx_base.__pyx___headers, __pyx_t_2); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 463, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_self->__pyx_base.__pyx___headers, __pyx_t_2); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L3:;
 
-  /* "blacksheep/messages.pyx":449
+  /* "blacksheep/messages.pyx":456
  *         return self.cookies.get(name)
  * 
  *     def set_cookie(self, str name, str value):             # <<<<<<<<<<<<<<
  *         """
  *         Sets a cookie in the request. This method also ensures that a single
  */
 
@@ -13485,15 +13671,15 @@
   __Pyx_XDECREF(__pyx_v_new_value);
   __Pyx_XDECREF(__pyx_v_existing_cookie);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":466
+/* "blacksheep/messages.pyx":473
  * 
  *     @property
  *     def etag(self):             # <<<<<<<<<<<<<<
  *         return self.get_first_header(b"etag")
  * 
  */
 
@@ -13515,29 +13701,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "blacksheep/messages.pyx":467
+  /* "blacksheep/messages.pyx":474
  *     @property
  *     def etag(self):
  *         return self.get_first_header(b"etag")             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_n_b_etag, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_n_b_etag, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":466
+  /* "blacksheep/messages.pyx":473
  * 
  *     @property
  *     def etag(self):             # <<<<<<<<<<<<<<
  *         return self.get_first_header(b"etag")
  * 
  */
 
@@ -13548,15 +13734,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":470
+/* "blacksheep/messages.pyx":477
  * 
  *     @property
  *     def if_none_match(self):             # <<<<<<<<<<<<<<
  *         return self.get_first_header(b"if-none-match")
  * 
  */
 
@@ -13578,29 +13764,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "blacksheep/messages.pyx":471
+  /* "blacksheep/messages.pyx":478
  *     @property
  *     def if_none_match(self):
  *         return self.get_first_header(b"if-none-match")             # <<<<<<<<<<<<<<
  * 
  *     cpdef bint expect_100_continue(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_kp_b_if_none_match, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 471, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_kp_b_if_none_match, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":470
+  /* "blacksheep/messages.pyx":477
  * 
  *     @property
  *     def if_none_match(self):             # <<<<<<<<<<<<<<
  *         return self.get_first_header(b"if-none-match")
  * 
  */
 
@@ -13611,15 +13797,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":473
+/* "blacksheep/messages.pyx":480
  *         return self.get_first_header(b"if-none-match")
  * 
  *     cpdef bint expect_100_continue(self):             # <<<<<<<<<<<<<<
  *         cdef bytes value
  *         value = self.get_first_header(b'expect')
  */
 
@@ -13643,15 +13829,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_expect_100_continue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 473, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_expect_100_continue); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_10blacksheep_8messages_7Request_11expect_100_continue)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -13659,18 +13845,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 473, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 480, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 473, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 480, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -13681,77 +13867,77 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "blacksheep/messages.pyx":475
+  /* "blacksheep/messages.pyx":482
  *     cpdef bint expect_100_continue(self):
  *         cdef bytes value
  *         value = self.get_first_header(b'expect')             # <<<<<<<<<<<<<<
  *         if value and value.lower() == b'100-continue':
  *             return True
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_n_b_expect, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_n_b_expect, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 482, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_value = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":476
+  /* "blacksheep/messages.pyx":483
  *         cdef bytes value
  *         value = self.get_first_header(b'expect')
  *         if value and value.lower() == b'100-continue':             # <<<<<<<<<<<<<<
  *             return True
  *         return False
  */
   __pyx_t_6 = (__pyx_v_value != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_value) != 0);
   if (__pyx_t_6) {
   } else {
     __pyx_t_5 = __pyx_t_6;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_1 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyBytes_Type_lower, __pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyBytes_Type_lower, __pyx_v_value); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 483, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = (__Pyx_PyBytes_Equals(__pyx_t_1, __pyx_kp_b_100_continue, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 476, __pyx_L1_error)
+  __pyx_t_6 = (__Pyx_PyBytes_Equals(__pyx_t_1, __pyx_kp_b_100_continue, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 483, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = __pyx_t_6;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_5) {
 
-    /* "blacksheep/messages.pyx":477
+    /* "blacksheep/messages.pyx":484
  *         value = self.get_first_header(b'expect')
  *         if value and value.lower() == b'100-continue':
  *             return True             # <<<<<<<<<<<<<<
  *         return False
  * 
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "blacksheep/messages.pyx":476
+    /* "blacksheep/messages.pyx":483
  *         cdef bytes value
  *         value = self.get_first_header(b'expect')
  *         if value and value.lower() == b'100-continue':             # <<<<<<<<<<<<<<
  *             return True
  *         return False
  */
   }
 
-  /* "blacksheep/messages.pyx":478
+  /* "blacksheep/messages.pyx":485
  *         if value and value.lower() == b'100-continue':
  *             return True
  *         return False             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":473
+  /* "blacksheep/messages.pyx":480
  *         return self.get_first_header(b"if-none-match")
  * 
  *     cpdef bint expect_100_continue(self):             # <<<<<<<<<<<<<<
  *         cdef bytes value
  *         value = self.get_first_header(b'expect')
  */
 
@@ -13787,15 +13973,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("expect_100_continue", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_10blacksheep_8messages_7Request_expect_100_continue(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 473, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_10blacksheep_8messages_7Request_expect_100_continue(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14793,15 +14979,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":483
+/* "blacksheep/messages.pyx":490
  * cdef class Response(Message):
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         int status,
  */
 
@@ -14817,24 +15003,24 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_status,&__pyx_n_s_headers,&__pyx_n_s_content,0};
     PyObject* values[3] = {0,0,0};
 
-    /* "blacksheep/messages.pyx":486
+    /* "blacksheep/messages.pyx":493
  *         self,
  *         int status,
  *         list headers = None,             # <<<<<<<<<<<<<<
  *         Content content = None
  *     ):
  */
     values[1] = ((PyObject*)Py_None);
 
-    /* "blacksheep/messages.pyx":487
+    /* "blacksheep/messages.pyx":494
  *         int status,
  *         list headers = None,
  *         Content content = None             # <<<<<<<<<<<<<<
  *     ):
  *         self.__headers = headers or []
  */
     values[2] = (PyObject *)((struct __pyx_obj_10blacksheep_8contents_Content *)Py_None);
@@ -14866,44 +15052,44 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_content);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 483, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 490, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_status = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_status == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 485, __pyx_L3_error)
+    __pyx_v_status = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_status == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 492, __pyx_L3_error)
     __pyx_v_headers = ((PyObject*)values[1]);
     __pyx_v_content = ((struct __pyx_obj_10blacksheep_8contents_Content *)values[2]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 483, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 490, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("blacksheep.messages.Response.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_headers), (&PyList_Type), 1, "headers", 1))) __PYX_ERR(0, 486, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_content), __pyx_ptype_10blacksheep_8contents_Content, 1, "content", 0))) __PYX_ERR(0, 487, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_headers), (&PyList_Type), 1, "headers", 1))) __PYX_ERR(0, 493, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_content), __pyx_ptype_10blacksheep_8contents_Content, 1, "content", 0))) __PYX_ERR(0, 494, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_8Response___init__(((struct __pyx_obj_10blacksheep_8messages_Response *)__pyx_v_self), __pyx_v_status, __pyx_v_headers, __pyx_v_content);
 
-  /* "blacksheep/messages.pyx":483
+  /* "blacksheep/messages.pyx":490
  * cdef class Response(Message):
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         int status,
  */
 
@@ -14923,63 +15109,63 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "blacksheep/messages.pyx":489
+  /* "blacksheep/messages.pyx":496
  *         Content content = None
  *     ):
  *         self.__headers = headers or []             # <<<<<<<<<<<<<<
  *         self.status = status
  *         self.content = content
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_headers); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_headers); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 496, __pyx_L1_error)
   if (!__pyx_t_2) {
   } else {
     __Pyx_INCREF(__pyx_v_headers);
     __pyx_t_1 = __pyx_v_headers;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_t_1 = __pyx_t_3;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_L3_bool_binop_done:;
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->__pyx_base.__pyx___headers);
   __Pyx_DECREF(__pyx_v_self->__pyx_base.__pyx___headers);
   __pyx_v_self->__pyx_base.__pyx___headers = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":490
+  /* "blacksheep/messages.pyx":497
  *     ):
  *         self.__headers = headers or []
  *         self.status = status             # <<<<<<<<<<<<<<
  *         self.content = content
  * 
  */
   __pyx_v_self->status = __pyx_v_status;
 
-  /* "blacksheep/messages.pyx":491
+  /* "blacksheep/messages.pyx":498
  *         self.__headers = headers or []
  *         self.status = status
  *         self.content = content             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_content));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_content));
   __Pyx_GOTREF(__pyx_v_self->__pyx_base.content);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->__pyx_base.content));
   __pyx_v_self->__pyx_base.content = __pyx_v_content;
 
-  /* "blacksheep/messages.pyx":483
+  /* "blacksheep/messages.pyx":490
  * cdef class Response(Message):
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         int status,
  */
 
@@ -14992,15 +15178,15 @@
   __Pyx_AddTraceback("blacksheep.messages.Response.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":493
+/* "blacksheep/messages.pyx":500
  *         self.content = content
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f'<Response {self.status}>'
  * 
  */
 
@@ -15025,48 +15211,48 @@
   Py_UCS4 __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "blacksheep/messages.pyx":494
+  /* "blacksheep/messages.pyx":501
  * 
  *     def __repr__(self):
  *         return f'<Response {self.status}>'             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 501, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_3 = 127;
   __Pyx_INCREF(__pyx_kp_u_Response);
   __pyx_t_2 += 10;
   __Pyx_GIVEREF(__pyx_kp_u_Response);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Response);
-  __pyx_t_4 = __Pyx_PyUnicode_From_int(__pyx_v_self->status, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_From_int(__pyx_v_self->status, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 501, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u__13);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__13);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__13);
-  __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 501, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":493
+  /* "blacksheep/messages.pyx":500
  *         self.content = content
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f'<Response {self.status}>'
  * 
  */
 
@@ -15078,15 +15264,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":497
+/* "blacksheep/messages.pyx":504
  * 
  *     @property
  *     def cookies(self):             # <<<<<<<<<<<<<<
  *         return self.get_cookies()
  * 
  */
 
@@ -15110,44 +15296,44 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "blacksheep/messages.pyx":498
+  /* "blacksheep/messages.pyx":505
  *     @property
  *     def cookies(self):
  *         return self.get_cookies()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_cookies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_cookies); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 498, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":497
+  /* "blacksheep/messages.pyx":504
  * 
  *     @property
  *     def cookies(self):             # <<<<<<<<<<<<<<
  *         return self.get_cookies()
  * 
  */
 
@@ -15160,15 +15346,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":501
+/* "blacksheep/messages.pyx":508
  * 
  *     @property
  *     def reason(self) -> str:             # <<<<<<<<<<<<<<
  *         return http.HTTPStatus(self.status).phrase
  * 
  */
 
@@ -15193,53 +15379,53 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "blacksheep/messages.pyx":502
+  /* "blacksheep/messages.pyx":509
  *     @property
  *     def reason(self) -> str:
  *         return http.HTTPStatus(self.status).phrase             # <<<<<<<<<<<<<<
  * 
  *     def get_cookies(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_http); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_http); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_HTTPStatus); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_HTTPStatus); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_phrase); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_phrase); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":501
+  /* "blacksheep/messages.pyx":508
  * 
  *     @property
  *     def reason(self) -> str:             # <<<<<<<<<<<<<<
  *         return http.HTTPStatus(self.status).phrase
  * 
  */
 
@@ -15253,15 +15439,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":504
+/* "blacksheep/messages.pyx":511
  *         return http.HTTPStatus(self.status).phrase
  * 
  *     def get_cookies(self):             # <<<<<<<<<<<<<<
  *         cdef bytes value
  *         cdef Cookie cookie
  */
 
@@ -15290,128 +15476,128 @@
   Py_ssize_t __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_cookies", 0);
 
-  /* "blacksheep/messages.pyx":510
+  /* "blacksheep/messages.pyx":517
  *         cdef list set_cookies_headers
  * 
  *         cookies = {}             # <<<<<<<<<<<<<<
  *         set_cookies_headers = self.get_headers(b'set-cookie')
  *         if set_cookies_headers:
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 510, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 517, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_cookies = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":511
+  /* "blacksheep/messages.pyx":518
  * 
  *         cookies = {}
  *         set_cookies_headers = self.get_headers(b'set-cookie')             # <<<<<<<<<<<<<<
  *         if set_cookies_headers:
  *             for value in set_cookies_headers:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Response *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_headers(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_kp_b_set_cookie, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Response *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_headers(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_kp_b_set_cookie, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_set_cookies_headers = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":512
+  /* "blacksheep/messages.pyx":519
  *         cookies = {}
  *         set_cookies_headers = self.get_headers(b'set-cookie')
  *         if set_cookies_headers:             # <<<<<<<<<<<<<<
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value)
  */
   __pyx_t_2 = (__pyx_v_set_cookies_headers != Py_None)&&(PyList_GET_SIZE(__pyx_v_set_cookies_headers) != 0);
   if (__pyx_t_2) {
 
-    /* "blacksheep/messages.pyx":513
+    /* "blacksheep/messages.pyx":520
  *         set_cookies_headers = self.get_headers(b'set-cookie')
  *         if set_cookies_headers:
  *             for value in set_cookies_headers:             # <<<<<<<<<<<<<<
  *                 cookie = parse_cookie(value)
  *                 cookies[cookie.name] = cookie
  */
     if (unlikely(__pyx_v_set_cookies_headers == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 513, __pyx_L1_error)
+      __PYX_ERR(0, 520, __pyx_L1_error)
     }
     __pyx_t_1 = __pyx_v_set_cookies_headers; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
     for (;;) {
       if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 513, __pyx_L1_error)
+      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 520, __pyx_L1_error)
       #else
-      __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 513, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 520, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
-      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 513, __pyx_L1_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 520, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_value, ((PyObject*)__pyx_t_4));
       __pyx_t_4 = 0;
 
-      /* "blacksheep/messages.pyx":514
+      /* "blacksheep/messages.pyx":521
  *         if set_cookies_headers:
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value)             # <<<<<<<<<<<<<<
  *                 cookies[cookie.name] = cookie
  *         return cookies
  */
-      __pyx_t_4 = ((PyObject *)__pyx_f_10blacksheep_7cookies_parse_cookie(__pyx_v_value, 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 514, __pyx_L1_error)
+      __pyx_t_4 = ((PyObject *)__pyx_f_10blacksheep_7cookies_parse_cookie(__pyx_v_value, 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 521, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_v_cookie, ((struct __pyx_obj_10blacksheep_7cookies_Cookie *)__pyx_t_4));
       __pyx_t_4 = 0;
 
-      /* "blacksheep/messages.pyx":515
+      /* "blacksheep/messages.pyx":522
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value)
  *                 cookies[cookie.name] = cookie             # <<<<<<<<<<<<<<
  *         return cookies
  * 
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cookie), __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 515, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cookie), __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 522, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely(PyDict_SetItem(__pyx_v_cookies, __pyx_t_4, ((PyObject *)__pyx_v_cookie)) < 0)) __PYX_ERR(0, 515, __pyx_L1_error)
+      if (unlikely(PyDict_SetItem(__pyx_v_cookies, __pyx_t_4, ((PyObject *)__pyx_v_cookie)) < 0)) __PYX_ERR(0, 522, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "blacksheep/messages.pyx":513
+      /* "blacksheep/messages.pyx":520
  *         set_cookies_headers = self.get_headers(b'set-cookie')
  *         if set_cookies_headers:
  *             for value in set_cookies_headers:             # <<<<<<<<<<<<<<
  *                 cookie = parse_cookie(value)
  *                 cookies[cookie.name] = cookie
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "blacksheep/messages.pyx":512
+    /* "blacksheep/messages.pyx":519
  *         cookies = {}
  *         set_cookies_headers = self.get_headers(b'set-cookie')
  *         if set_cookies_headers:             # <<<<<<<<<<<<<<
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value)
  */
   }
 
-  /* "blacksheep/messages.pyx":516
+  /* "blacksheep/messages.pyx":523
  *                 cookie = parse_cookie(value)
  *                 cookies[cookie.name] = cookie
  *         return cookies             # <<<<<<<<<<<<<<
  * 
  *     def get_cookie(self, str name):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_cookies);
   __pyx_r = __pyx_v_cookies;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":504
+  /* "blacksheep/messages.pyx":511
  *         return http.HTTPStatus(self.status).phrase
  * 
  *     def get_cookies(self):             # <<<<<<<<<<<<<<
  *         cdef bytes value
  *         cdef Cookie cookie
  */
 
@@ -15427,15 +15613,15 @@
   __Pyx_XDECREF(__pyx_v_cookies);
   __Pyx_XDECREF(__pyx_v_set_cookies_headers);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":518
+/* "blacksheep/messages.pyx":525
  *         return cookies
  * 
  *     def get_cookie(self, str name):             # <<<<<<<<<<<<<<
  *         cdef bytes value
  *         cdef list set_cookies_headers = self.get_headers(b'set-cookie')
  */
 
@@ -15444,15 +15630,15 @@
 static PyObject *__pyx_pw_10blacksheep_8messages_8Response_7get_cookie(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_cookie (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 518, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 525, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_8Response_6get_cookie(((struct __pyx_obj_10blacksheep_8messages_Response *)__pyx_v_self), ((PyObject*)__pyx_v_name));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -15471,138 +15657,138 @@
   Py_ssize_t __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_cookie", 0);
 
-  /* "blacksheep/messages.pyx":520
+  /* "blacksheep/messages.pyx":527
  *     def get_cookie(self, str name):
  *         cdef bytes value
  *         cdef list set_cookies_headers = self.get_headers(b'set-cookie')             # <<<<<<<<<<<<<<
  * 
  *         if set_cookies_headers:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Response *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_headers(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_kp_b_set_cookie, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Response *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_headers(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_kp_b_set_cookie, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 527, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_set_cookies_headers = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":522
+  /* "blacksheep/messages.pyx":529
  *         cdef list set_cookies_headers = self.get_headers(b'set-cookie')
  * 
  *         if set_cookies_headers:             # <<<<<<<<<<<<<<
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value)
  */
   __pyx_t_2 = (__pyx_v_set_cookies_headers != Py_None)&&(PyList_GET_SIZE(__pyx_v_set_cookies_headers) != 0);
   if (__pyx_t_2) {
 
-    /* "blacksheep/messages.pyx":523
+    /* "blacksheep/messages.pyx":530
  * 
  *         if set_cookies_headers:
  *             for value in set_cookies_headers:             # <<<<<<<<<<<<<<
  *                 cookie = parse_cookie(value)
  *                 if cookie.name == name:
  */
     if (unlikely(__pyx_v_set_cookies_headers == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 523, __pyx_L1_error)
+      __PYX_ERR(0, 530, __pyx_L1_error)
     }
     __pyx_t_1 = __pyx_v_set_cookies_headers; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
     for (;;) {
       if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 523, __pyx_L1_error)
+      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 530, __pyx_L1_error)
       #else
-      __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 523, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 530, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
-      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 523, __pyx_L1_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 530, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_value, ((PyObject*)__pyx_t_4));
       __pyx_t_4 = 0;
 
-      /* "blacksheep/messages.pyx":524
+      /* "blacksheep/messages.pyx":531
  *         if set_cookies_headers:
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value)             # <<<<<<<<<<<<<<
  *                 if cookie.name == name:
  *                     return cookie
  */
-      __pyx_t_4 = ((PyObject *)__pyx_f_10blacksheep_7cookies_parse_cookie(__pyx_v_value, 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 524, __pyx_L1_error)
+      __pyx_t_4 = ((PyObject *)__pyx_f_10blacksheep_7cookies_parse_cookie(__pyx_v_value, 0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 531, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_v_cookie, ((struct __pyx_obj_10blacksheep_7cookies_Cookie *)__pyx_t_4));
       __pyx_t_4 = 0;
 
-      /* "blacksheep/messages.pyx":525
+      /* "blacksheep/messages.pyx":532
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value)
  *                 if cookie.name == name:             # <<<<<<<<<<<<<<
  *                     return cookie
  * 
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cookie), __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 525, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cookie), __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 532, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_v_name, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 525, __pyx_L1_error)
+      __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_v_name, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 532, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_2) {
 
-        /* "blacksheep/messages.pyx":526
+        /* "blacksheep/messages.pyx":533
  *                 cookie = parse_cookie(value)
  *                 if cookie.name == name:
  *                     return cookie             # <<<<<<<<<<<<<<
  * 
  *         return None
  */
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(((PyObject *)__pyx_v_cookie));
         __pyx_r = ((PyObject *)__pyx_v_cookie);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
 
-        /* "blacksheep/messages.pyx":525
+        /* "blacksheep/messages.pyx":532
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value)
  *                 if cookie.name == name:             # <<<<<<<<<<<<<<
  *                     return cookie
  * 
  */
       }
 
-      /* "blacksheep/messages.pyx":523
+      /* "blacksheep/messages.pyx":530
  * 
  *         if set_cookies_headers:
  *             for value in set_cookies_headers:             # <<<<<<<<<<<<<<
  *                 cookie = parse_cookie(value)
  *                 if cookie.name == name:
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "blacksheep/messages.pyx":522
+    /* "blacksheep/messages.pyx":529
  *         cdef list set_cookies_headers = self.get_headers(b'set-cookie')
  * 
  *         if set_cookies_headers:             # <<<<<<<<<<<<<<
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value)
  */
   }
 
-  /* "blacksheep/messages.pyx":528
+  /* "blacksheep/messages.pyx":535
  *                     return cookie
  * 
  *         return None             # <<<<<<<<<<<<<<
  * 
  *     def set_cookie(self, Cookie cookie):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":518
+  /* "blacksheep/messages.pyx":525
  *         return cookies
  * 
  *     def get_cookie(self, str name):             # <<<<<<<<<<<<<<
  *         cdef bytes value
  *         cdef list set_cookies_headers = self.get_headers(b'set-cookie')
  */
 
@@ -15617,15 +15803,15 @@
   __Pyx_XDECREF(__pyx_v_set_cookies_headers);
   __Pyx_XDECREF((PyObject *)__pyx_v_cookie);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":530
+/* "blacksheep/messages.pyx":537
  *         return None
  * 
  *     def set_cookie(self, Cookie cookie):             # <<<<<<<<<<<<<<
  *         self.__headers.append((b'set-cookie', write_cookie_for_response(cookie)))
  * 
  */
 
@@ -15634,15 +15820,15 @@
 static PyObject *__pyx_pw_10blacksheep_8messages_8Response_9set_cookie(PyObject *__pyx_v_self, PyObject *__pyx_v_cookie) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_cookie (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cookie), __pyx_ptype_10blacksheep_7cookies_Cookie, 1, "cookie", 0))) __PYX_ERR(0, 530, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cookie), __pyx_ptype_10blacksheep_7cookies_Cookie, 1, "cookie", 0))) __PYX_ERR(0, 537, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_8Response_8set_cookie(((struct __pyx_obj_10blacksheep_8messages_Response *)__pyx_v_self), ((struct __pyx_obj_10blacksheep_7cookies_Cookie *)__pyx_v_cookie));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -15657,39 +15843,39 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_cookie", 0);
 
-  /* "blacksheep/messages.pyx":531
+  /* "blacksheep/messages.pyx":538
  * 
  *     def set_cookie(self, Cookie cookie):
  *         self.__headers.append((b'set-cookie', write_cookie_for_response(cookie)))             # <<<<<<<<<<<<<<
  * 
  *     def set_cookies(self, list cookies):
  */
   if (unlikely(__pyx_v_self->__pyx_base.__pyx___headers == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-    __PYX_ERR(0, 531, __pyx_L1_error)
+    __PYX_ERR(0, 538, __pyx_L1_error)
   }
-  __pyx_t_1 = __pyx_f_10blacksheep_7cookies_write_cookie_for_response(__pyx_v_cookie); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 531, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_10blacksheep_7cookies_write_cookie_for_response(__pyx_v_cookie); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 531, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_kp_b_set_cookie);
   __Pyx_GIVEREF(__pyx_kp_b_set_cookie);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_b_set_cookie);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_self->__pyx_base.__pyx___headers, __pyx_t_2); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 531, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_self->__pyx_base.__pyx___headers, __pyx_t_2); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "blacksheep/messages.pyx":530
+  /* "blacksheep/messages.pyx":537
  *         return None
  * 
  *     def set_cookie(self, Cookie cookie):             # <<<<<<<<<<<<<<
  *         self.__headers.append((b'set-cookie', write_cookie_for_response(cookie)))
  * 
  */
 
@@ -15703,15 +15889,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":533
+/* "blacksheep/messages.pyx":540
  *         self.__headers.append((b'set-cookie', write_cookie_for_response(cookie)))
  * 
  *     def set_cookies(self, list cookies):             # <<<<<<<<<<<<<<
  *         cdef Cookie cookie
  *         for cookie in cookies:
  */
 
@@ -15720,15 +15906,15 @@
 static PyObject *__pyx_pw_10blacksheep_8messages_8Response_11set_cookies(PyObject *__pyx_v_self, PyObject *__pyx_v_cookies) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_cookies (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cookies), (&PyList_Type), 1, "cookies", 1))) __PYX_ERR(0, 533, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cookies), (&PyList_Type), 1, "cookies", 1))) __PYX_ERR(0, 540, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_8Response_10set_cookies(((struct __pyx_obj_10blacksheep_8messages_Response *)__pyx_v_self), ((PyObject*)__pyx_v_cookies));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -15746,75 +15932,75 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_cookies", 0);
 
-  /* "blacksheep/messages.pyx":535
+  /* "blacksheep/messages.pyx":542
  *     def set_cookies(self, list cookies):
  *         cdef Cookie cookie
  *         for cookie in cookies:             # <<<<<<<<<<<<<<
  *             self.set_cookie(cookie)
  * 
  */
   if (unlikely(__pyx_v_cookies == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 535, __pyx_L1_error)
+    __PYX_ERR(0, 542, __pyx_L1_error)
   }
   __pyx_t_1 = __pyx_v_cookies; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
   for (;;) {
     if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 535, __pyx_L1_error)
+    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 542, __pyx_L1_error)
     #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_10blacksheep_7cookies_Cookie))))) __PYX_ERR(0, 535, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_10blacksheep_7cookies_Cookie))))) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_cookie, ((struct __pyx_obj_10blacksheep_7cookies_Cookie *)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "blacksheep/messages.pyx":536
+    /* "blacksheep/messages.pyx":543
  *         cdef Cookie cookie
  *         for cookie in cookies:
  *             self.set_cookie(cookie)             # <<<<<<<<<<<<<<
  * 
  *     def unset_cookie(self, str name):
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_cookie_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 536, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_cookie_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, ((PyObject *)__pyx_v_cookie)) : __Pyx_PyObject_CallOneArg(__pyx_t_4, ((PyObject *)__pyx_v_cookie));
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 536, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 543, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "blacksheep/messages.pyx":535
+    /* "blacksheep/messages.pyx":542
  *     def set_cookies(self, list cookies):
  *         cdef Cookie cookie
  *         for cookie in cookies:             # <<<<<<<<<<<<<<
  *             self.set_cookie(cookie)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":533
+  /* "blacksheep/messages.pyx":540
  *         self.__headers.append((b'set-cookie', write_cookie_for_response(cookie)))
  * 
  *     def set_cookies(self, list cookies):             # <<<<<<<<<<<<<<
  *         cdef Cookie cookie
  *         for cookie in cookies:
  */
 
@@ -15831,15 +16017,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_cookie);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":538
+/* "blacksheep/messages.pyx":545
  *             self.set_cookie(cookie)
  * 
  *     def unset_cookie(self, str name):             # <<<<<<<<<<<<<<
  *         self.set_cookie(
  *             Cookie(
  */
 
@@ -15848,15 +16034,15 @@
 static PyObject *__pyx_pw_10blacksheep_8messages_8Response_13unset_cookie(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("unset_cookie (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 538, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 545, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_8Response_12unset_cookie(((struct __pyx_obj_10blacksheep_8messages_Response *)__pyx_v_self), ((PyObject*)__pyx_v_name));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -15874,84 +16060,84 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("unset_cookie", 0);
 
-  /* "blacksheep/messages.pyx":539
+  /* "blacksheep/messages.pyx":546
  * 
  *     def unset_cookie(self, str name):
  *         self.set_cookie(             # <<<<<<<<<<<<<<
  *             Cookie(
  *                 name,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_cookie_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 539, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_cookie_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "blacksheep/messages.pyx":543
+  /* "blacksheep/messages.pyx":550
  *                 name,
  *                 '',
  *                 datetime.utcnow() - timedelta(days=365)             # <<<<<<<<<<<<<<
  *             )
  *         )
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_datetime); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_datetime); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_utcnow); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_utcnow); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 543, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_timedelta); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_timedelta); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_days, __pyx_int_365) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 543, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_days, __pyx_int_365) < 0) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 550, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "blacksheep/messages.pyx":540
+  /* "blacksheep/messages.pyx":547
  *     def unset_cookie(self, str name):
  *         self.set_cookie(
  *             Cookie(             # <<<<<<<<<<<<<<
  *                 name,
  *                 '',
  */
-  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 547, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_name);
   __Pyx_GIVEREF(__pyx_v_name);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_name);
   __Pyx_INCREF(__pyx_kp_u__3);
   __Pyx_GIVEREF(__pyx_kp_u__3);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_kp_u__3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_7cookies_Cookie), __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 540, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10blacksheep_7cookies_Cookie), __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 547, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -15959,20 +16145,20 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 539, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":538
+  /* "blacksheep/messages.pyx":545
  *             self.set_cookie(cookie)
  * 
  *     def unset_cookie(self, str name):             # <<<<<<<<<<<<<<
  *         self.set_cookie(
  *             Cookie(
  */
 
@@ -15990,15 +16176,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":547
+/* "blacksheep/messages.pyx":554
  *         )
  * 
  *     def remove_cookie(self, str name):             # <<<<<<<<<<<<<<
  *         cdef list to_remove = []
  *         cdef tuple value
  */
 
@@ -16007,15 +16193,15 @@
 static PyObject *__pyx_pw_10blacksheep_8messages_8Response_15remove_cookie(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("remove_cookie (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 547, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(0, 554, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_8Response_14remove_cookie(((struct __pyx_obj_10blacksheep_8messages_Response *)__pyx_v_self), ((PyObject*)__pyx_v_name));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -16037,152 +16223,152 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("remove_cookie", 0);
 
-  /* "blacksheep/messages.pyx":548
+  /* "blacksheep/messages.pyx":555
  * 
  *     def remove_cookie(self, str name):
  *         cdef list to_remove = []             # <<<<<<<<<<<<<<
  *         cdef tuple value
  *         cdef list set_cookies_headers = self.get_headers_tuples(b'set-cookie')
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 548, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 555, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_to_remove = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":550
+  /* "blacksheep/messages.pyx":557
  *         cdef list to_remove = []
  *         cdef tuple value
  *         cdef list set_cookies_headers = self.get_headers_tuples(b'set-cookie')             # <<<<<<<<<<<<<<
  * 
  *         if set_cookies_headers:
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Response *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_headers_tuples(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_kp_b_set_cookie); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Response *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.get_headers_tuples(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_kp_b_set_cookie); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_set_cookies_headers = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":552
+  /* "blacksheep/messages.pyx":559
  *         cdef list set_cookies_headers = self.get_headers_tuples(b'set-cookie')
  * 
  *         if set_cookies_headers:             # <<<<<<<<<<<<<<
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value[1])
  */
   __pyx_t_2 = (__pyx_v_set_cookies_headers != Py_None)&&(PyList_GET_SIZE(__pyx_v_set_cookies_headers) != 0);
   if (__pyx_t_2) {
 
-    /* "blacksheep/messages.pyx":553
+    /* "blacksheep/messages.pyx":560
  * 
  *         if set_cookies_headers:
  *             for value in set_cookies_headers:             # <<<<<<<<<<<<<<
  *                 cookie = parse_cookie(value[1])
  *                 if cookie.name == name:
  */
     if (unlikely(__pyx_v_set_cookies_headers == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 553, __pyx_L1_error)
+      __PYX_ERR(0, 560, __pyx_L1_error)
     }
     __pyx_t_1 = __pyx_v_set_cookies_headers; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
     for (;;) {
       if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 553, __pyx_L1_error)
+      __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_4); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 560, __pyx_L1_error)
       #else
-      __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 553, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 560, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       #endif
-      if (!(likely(PyTuple_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 553, __pyx_L1_error)
+      if (!(likely(PyTuple_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 560, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_value, ((PyObject*)__pyx_t_4));
       __pyx_t_4 = 0;
 
-      /* "blacksheep/messages.pyx":554
+      /* "blacksheep/messages.pyx":561
  *         if set_cookies_headers:
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value[1])             # <<<<<<<<<<<<<<
  *                 if cookie.name == name:
  *                     to_remove.append(value)
  */
       if (unlikely(__pyx_v_value == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 554, __pyx_L1_error)
+        __PYX_ERR(0, 561, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_GetItemInt_Tuple(__pyx_v_value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 554, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_GetItemInt_Tuple(__pyx_v_value, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 561, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 554, __pyx_L1_error)
-      __pyx_t_5 = ((PyObject *)__pyx_f_10blacksheep_7cookies_parse_cookie(((PyObject*)__pyx_t_4), 0)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 554, __pyx_L1_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 561, __pyx_L1_error)
+      __pyx_t_5 = ((PyObject *)__pyx_f_10blacksheep_7cookies_parse_cookie(((PyObject*)__pyx_t_4), 0)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 561, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_XDECREF_SET(__pyx_v_cookie, ((struct __pyx_obj_10blacksheep_7cookies_Cookie *)__pyx_t_5));
       __pyx_t_5 = 0;
 
-      /* "blacksheep/messages.pyx":555
+      /* "blacksheep/messages.pyx":562
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value[1])
  *                 if cookie.name == name:             # <<<<<<<<<<<<<<
  *                     to_remove.append(value)
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cookie), __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 555, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_cookie), __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 562, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_5, __pyx_v_name, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 555, __pyx_L1_error)
+      __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_5, __pyx_v_name, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 562, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       if (__pyx_t_2) {
 
-        /* "blacksheep/messages.pyx":556
+        /* "blacksheep/messages.pyx":563
  *                 cookie = parse_cookie(value[1])
  *                 if cookie.name == name:
  *                     to_remove.append(value)             # <<<<<<<<<<<<<<
  * 
  *         self.remove_headers(to_remove)
  */
-        __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_to_remove, __pyx_v_value); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 556, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyList_Append(__pyx_v_to_remove, __pyx_v_value); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 563, __pyx_L1_error)
 
-        /* "blacksheep/messages.pyx":555
+        /* "blacksheep/messages.pyx":562
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value[1])
  *                 if cookie.name == name:             # <<<<<<<<<<<<<<
  *                     to_remove.append(value)
  * 
  */
       }
 
-      /* "blacksheep/messages.pyx":553
+      /* "blacksheep/messages.pyx":560
  * 
  *         if set_cookies_headers:
  *             for value in set_cookies_headers:             # <<<<<<<<<<<<<<
  *                 cookie = parse_cookie(value[1])
  *                 if cookie.name == name:
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "blacksheep/messages.pyx":552
+    /* "blacksheep/messages.pyx":559
  *         cdef list set_cookies_headers = self.get_headers_tuples(b'set-cookie')
  * 
  *         if set_cookies_headers:             # <<<<<<<<<<<<<<
  *             for value in set_cookies_headers:
  *                 cookie = parse_cookie(value[1])
  */
   }
 
-  /* "blacksheep/messages.pyx":558
+  /* "blacksheep/messages.pyx":565
  *                     to_remove.append(value)
  * 
  *         self.remove_headers(to_remove)             # <<<<<<<<<<<<<<
  * 
  *     cpdef bint is_redirect(self):
  */
   ((struct __pyx_vtabstruct_10blacksheep_8messages_Response *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.remove_headers(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_self), __pyx_v_to_remove);
 
-  /* "blacksheep/messages.pyx":547
+  /* "blacksheep/messages.pyx":554
  *         )
  * 
  *     def remove_cookie(self, str name):             # <<<<<<<<<<<<<<
  *         cdef list to_remove = []
  *         cdef tuple value
  */
 
@@ -16201,15 +16387,15 @@
   __Pyx_XDECREF(__pyx_v_set_cookies_headers);
   __Pyx_XDECREF((PyObject *)__pyx_v_cookie);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":560
+/* "blacksheep/messages.pyx":567
  *         self.remove_headers(to_remove)
  * 
  *     cpdef bint is_redirect(self):             # <<<<<<<<<<<<<<
  *         return self.status in {301, 302, 303, 307, 308}
  * 
  */
 
@@ -16231,15 +16417,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_redirect); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 560, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_is_redirect); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 567, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_10blacksheep_8messages_8Response_17is_redirect)) {
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
@@ -16247,18 +16433,18 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 560, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 567, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 560, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 567, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_5;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -16269,15 +16455,15 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "blacksheep/messages.pyx":561
+  /* "blacksheep/messages.pyx":568
  * 
  *     cpdef bint is_redirect(self):
  *         return self.status in {301, 302, 303, 307, 308}             # <<<<<<<<<<<<<<
  * 
  * 
  */
   switch (__pyx_v_self->status) {
@@ -16291,15 +16477,15 @@
     default:
     __pyx_t_5 = 0;
     break;
   }
   __pyx_r = __pyx_t_5;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":560
+  /* "blacksheep/messages.pyx":567
  *         self.remove_headers(to_remove)
  * 
  *     cpdef bint is_redirect(self):             # <<<<<<<<<<<<<<
  *         return self.status in {301, 302, 303, 307, 308}
  * 
  */
 
@@ -16334,15 +16520,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_redirect", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_10blacksheep_8messages_8Response_is_redirect(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 560, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_10blacksheep_8messages_8Response_is_redirect(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -16832,15 +17018,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":564
+/* "blacksheep/messages.pyx":571
  * 
  * 
  * cpdef bint is_cors_request(Request request):             # <<<<<<<<<<<<<<
  *     return bool(request.get_first_header(b"Origin"))
  * 
  */
 
@@ -16851,29 +17037,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_cors_request", 0);
 
-  /* "blacksheep/messages.pyx":565
+  /* "blacksheep/messages.pyx":572
  * 
  * cpdef bint is_cors_request(Request request):
  *     return bool(request.get_first_header(b"Origin"))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_request->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_request), __pyx_n_b_Origin, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 565, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_request->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_request), __pyx_n_b_Origin, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = (__pyx_t_1 != Py_None)&&(PyBytes_GET_SIZE(__pyx_t_1) != 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = (!(!__pyx_t_2));
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":564
+  /* "blacksheep/messages.pyx":571
  * 
  * 
  * cpdef bint is_cors_request(Request request):             # <<<<<<<<<<<<<<
  *     return bool(request.get_first_header(b"Origin"))
  * 
  */
 
@@ -16892,15 +17078,15 @@
 static PyObject *__pyx_pw_10blacksheep_8messages_5is_cors_request(PyObject *__pyx_self, PyObject *__pyx_v_request) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_cors_request (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 564, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 571, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_4is_cors_request(__pyx_self, ((struct __pyx_obj_10blacksheep_8messages_Request *)__pyx_v_request));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -16913,15 +17099,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_cors_request", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_10blacksheep_8messages_is_cors_request(__pyx_v_request, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_10blacksheep_8messages_is_cors_request(__pyx_v_request, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 571, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -16930,15 +17116,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":568
+/* "blacksheep/messages.pyx":575
  * 
  * 
  * cpdef bint is_cors_preflight_request(Request request):             # <<<<<<<<<<<<<<
  *     if request.method != "OPTIONS" or not is_cors_request(request):
  *         return False
  */
 
@@ -16952,76 +17138,76 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_cors_preflight_request", 0);
 
-  /* "blacksheep/messages.pyx":569
+  /* "blacksheep/messages.pyx":576
  * 
  * cpdef bint is_cors_preflight_request(Request request):
  *     if request.method != "OPTIONS" or not is_cors_request(request):             # <<<<<<<<<<<<<<
  *         return False
  * 
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_request->method, __pyx_n_u_OPTIONS, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 569, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_request->method, __pyx_n_u_OPTIONS, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 576, __pyx_L1_error)
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (!__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_3 = ((!(__pyx_f_10blacksheep_8messages_is_cors_request(__pyx_v_request, 0) != 0)) != 0);
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "blacksheep/messages.pyx":570
+    /* "blacksheep/messages.pyx":577
  * cpdef bint is_cors_preflight_request(Request request):
  *     if request.method != "OPTIONS" or not is_cors_request(request):
  *         return False             # <<<<<<<<<<<<<<
  * 
  *     next_request_method = request.get_first_header(
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "blacksheep/messages.pyx":569
+    /* "blacksheep/messages.pyx":576
  * 
  * cpdef bint is_cors_preflight_request(Request request):
  *     if request.method != "OPTIONS" or not is_cors_request(request):             # <<<<<<<<<<<<<<
  *         return False
  * 
  */
   }
 
-  /* "blacksheep/messages.pyx":572
+  /* "blacksheep/messages.pyx":579
  *         return False
  * 
  *     next_request_method = request.get_first_header(             # <<<<<<<<<<<<<<
  *         b"Access-Control-Request-Method"
  *     )
  */
-  __pyx_t_4 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_request->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_request), __pyx_kp_b_Access_Control_Request_Method, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 572, __pyx_L1_error)
+  __pyx_t_4 = ((struct __pyx_vtabstruct_10blacksheep_8messages_Request *)__pyx_v_request->__pyx_base.__pyx_vtab)->__pyx_base.get_first_header(((struct __pyx_obj_10blacksheep_8messages_Message *)__pyx_v_request), __pyx_kp_b_Access_Control_Request_Method, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_v_next_request_method = ((PyObject*)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "blacksheep/messages.pyx":576
+  /* "blacksheep/messages.pyx":583
  *     )
  * 
  *     return bool(next_request_method)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_1 = (__pyx_v_next_request_method != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_next_request_method) != 0);
   __pyx_r = (!(!__pyx_t_1));
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":568
+  /* "blacksheep/messages.pyx":575
  * 
  * 
  * cpdef bint is_cors_preflight_request(Request request):             # <<<<<<<<<<<<<<
  *     if request.method != "OPTIONS" or not is_cors_request(request):
  *         return False
  */
 
@@ -17041,15 +17227,15 @@
 static PyObject *__pyx_pw_10blacksheep_8messages_7is_cors_preflight_request(PyObject *__pyx_self, PyObject *__pyx_v_request) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_cors_preflight_request (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 568, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 575, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_6is_cors_preflight_request(__pyx_self, ((struct __pyx_obj_10blacksheep_8messages_Request *)__pyx_v_request));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -17062,15 +17248,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_cors_preflight_request", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_10blacksheep_8messages_is_cors_preflight_request(__pyx_v_request, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_10blacksheep_8messages_is_cors_preflight_request(__pyx_v_request, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 575, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -17079,15 +17265,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":579
+/* "blacksheep/messages.pyx":586
  * 
  * 
  * cdef bytes ensure_bytes(value):             # <<<<<<<<<<<<<<
  *     if isinstance(value, str):
  *         return value.encode()
  */
 
@@ -17100,111 +17286,111 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("ensure_bytes", 0);
 
-  /* "blacksheep/messages.pyx":580
+  /* "blacksheep/messages.pyx":587
  * 
  * cdef bytes ensure_bytes(value):
  *     if isinstance(value, str):             # <<<<<<<<<<<<<<
  *         return value.encode()
  *     if isinstance(value, bytes):
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_value); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "blacksheep/messages.pyx":581
+    /* "blacksheep/messages.pyx":588
  * cdef bytes ensure_bytes(value):
  *     if isinstance(value, str):
  *         return value.encode()             # <<<<<<<<<<<<<<
  *     if isinstance(value, bytes):
  *         return value
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 581, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 588, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 581, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 588, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 581, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 588, __pyx_L1_error)
     __pyx_r = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "blacksheep/messages.pyx":580
+    /* "blacksheep/messages.pyx":587
  * 
  * cdef bytes ensure_bytes(value):
  *     if isinstance(value, str):             # <<<<<<<<<<<<<<
  *         return value.encode()
  *     if isinstance(value, bytes):
  */
   }
 
-  /* "blacksheep/messages.pyx":582
+  /* "blacksheep/messages.pyx":589
  *     if isinstance(value, str):
  *         return value.encode()
  *     if isinstance(value, bytes):             # <<<<<<<<<<<<<<
  *         return value
  *     raise ValueError("Input value must be bytes or str")
  */
   __pyx_t_2 = PyBytes_Check(__pyx_v_value); 
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "blacksheep/messages.pyx":583
+    /* "blacksheep/messages.pyx":590
  *         return value.encode()
  *     if isinstance(value, bytes):
  *         return value             # <<<<<<<<<<<<<<
  *     raise ValueError("Input value must be bytes or str")
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    if (!(likely(PyBytes_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 583, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 590, __pyx_L1_error)
     __Pyx_INCREF(__pyx_v_value);
     __pyx_r = ((PyObject*)__pyx_v_value);
     goto __pyx_L0;
 
-    /* "blacksheep/messages.pyx":582
+    /* "blacksheep/messages.pyx":589
  *     if isinstance(value, str):
  *         return value.encode()
  *     if isinstance(value, bytes):             # <<<<<<<<<<<<<<
  *         return value
  *     raise ValueError("Input value must be bytes or str")
  */
   }
 
-  /* "blacksheep/messages.pyx":584
+  /* "blacksheep/messages.pyx":591
  *     if isinstance(value, bytes):
  *         return value
  *     raise ValueError("Input value must be bytes or str")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 584, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_3, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 584, __pyx_L1_error)
+  __PYX_ERR(0, 591, __pyx_L1_error)
 
-  /* "blacksheep/messages.pyx":579
+  /* "blacksheep/messages.pyx":586
  * 
  * 
  * cdef bytes ensure_bytes(value):             # <<<<<<<<<<<<<<
  *     if isinstance(value, str):
  *         return value.encode()
  */
 
@@ -17217,15 +17403,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":587
+/* "blacksheep/messages.pyx":594
  * 
  * 
  * cpdef URL get_request_absolute_url(Request request):             # <<<<<<<<<<<<<<
  *     if request.url.is_absolute:
  *         # outgoing request
  */
 
@@ -17240,130 +17426,130 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_request_absolute_url", 0);
 
-  /* "blacksheep/messages.pyx":588
+  /* "blacksheep/messages.pyx":595
  * 
  * cpdef URL get_request_absolute_url(Request request):
  *     if request.url.is_absolute:             # <<<<<<<<<<<<<<
  *         # outgoing request
  *         return request.url
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_url); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_url); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 595, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_is_absolute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_is_absolute); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 595, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 595, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_3) {
 
-    /* "blacksheep/messages.pyx":590
+    /* "blacksheep/messages.pyx":597
  *     if request.url.is_absolute:
  *         # outgoing request
  *         return request.url             # <<<<<<<<<<<<<<
  * 
  *     # incoming request
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_url); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 590, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_url); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 597, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_10blacksheep_3url_URL))))) __PYX_ERR(0, 590, __pyx_L1_error)
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_10blacksheep_3url_URL))))) __PYX_ERR(0, 597, __pyx_L1_error)
     __pyx_r = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_2);
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "blacksheep/messages.pyx":588
+    /* "blacksheep/messages.pyx":595
  * 
  * cpdef URL get_request_absolute_url(Request request):
  *     if request.url.is_absolute:             # <<<<<<<<<<<<<<
  *         # outgoing request
  *         return request.url
  */
   }
 
-  /* "blacksheep/messages.pyx":593
+  /* "blacksheep/messages.pyx":600
  * 
  *     # incoming request
  *     return build_absolute_url(             # <<<<<<<<<<<<<<
  *         ensure_bytes(request.scheme),
  *         ensure_bytes(request.host),
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-  /* "blacksheep/messages.pyx":594
+  /* "blacksheep/messages.pyx":601
  *     # incoming request
  *     return build_absolute_url(
  *         ensure_bytes(request.scheme),             # <<<<<<<<<<<<<<
  *         ensure_bytes(request.host),
  *         ensure_bytes(request.base_path),
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_scheme); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 594, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_scheme); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 594, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "blacksheep/messages.pyx":595
+  /* "blacksheep/messages.pyx":602
  *     return build_absolute_url(
  *         ensure_bytes(request.scheme),
  *         ensure_bytes(request.host),             # <<<<<<<<<<<<<<
  *         ensure_bytes(request.base_path),
  *         request._path
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_host); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 595, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_host); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 595, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "blacksheep/messages.pyx":596
+  /* "blacksheep/messages.pyx":603
  *         ensure_bytes(request.scheme),
  *         ensure_bytes(request.host),
  *         ensure_bytes(request.base_path),             # <<<<<<<<<<<<<<
  *         request._path
  *     )
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_base_path); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_base_path); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __pyx_t_5 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "blacksheep/messages.pyx":597
+  /* "blacksheep/messages.pyx":604
  *         ensure_bytes(request.host),
  *         ensure_bytes(request.base_path),
  *         request._path             # <<<<<<<<<<<<<<
  *     )
  * 
  */
   __pyx_t_2 = __pyx_v_request->_path;
   __Pyx_INCREF(__pyx_t_2);
 
-  /* "blacksheep/messages.pyx":593
+  /* "blacksheep/messages.pyx":600
  * 
  *     # incoming request
  *     return build_absolute_url(             # <<<<<<<<<<<<<<
  *         ensure_bytes(request.scheme),
  *         ensure_bytes(request.host),
  */
-  __pyx_t_6 = ((PyObject *)__pyx_f_10blacksheep_3url_build_absolute_url(((PyObject*)__pyx_t_1), ((PyObject*)__pyx_t_4), ((PyObject*)__pyx_t_5), ((PyObject*)__pyx_t_2), 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 593, __pyx_L1_error)
+  __pyx_t_6 = ((PyObject *)__pyx_f_10blacksheep_3url_build_absolute_url(((PyObject*)__pyx_t_1), ((PyObject*)__pyx_t_4), ((PyObject*)__pyx_t_5), ((PyObject*)__pyx_t_2), 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_6);
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":587
+  /* "blacksheep/messages.pyx":594
  * 
  * 
  * cpdef URL get_request_absolute_url(Request request):             # <<<<<<<<<<<<<<
  *     if request.url.is_absolute:
  *         # outgoing request
  */
 
@@ -17387,15 +17573,15 @@
 static PyObject *__pyx_pw_10blacksheep_8messages_9get_request_absolute_url(PyObject *__pyx_self, PyObject *__pyx_v_request) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_request_absolute_url (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 587, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 594, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_8get_request_absolute_url(__pyx_self, ((struct __pyx_obj_10blacksheep_8messages_Request *)__pyx_v_request));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -17408,15 +17594,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_request_absolute_url", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_10blacksheep_8messages_get_request_absolute_url(__pyx_v_request, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 587, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_10blacksheep_8messages_get_request_absolute_url(__pyx_v_request, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -17425,15 +17611,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/messages.pyx":601
+/* "blacksheep/messages.pyx":608
  * 
  * 
  * cpdef URL get_absolute_url_to_path(Request request, str path):             # <<<<<<<<<<<<<<
  *     return build_absolute_url(
  *         ensure_bytes(request.scheme),
  */
 
@@ -17447,89 +17633,89 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_absolute_url_to_path", 0);
 
-  /* "blacksheep/messages.pyx":602
+  /* "blacksheep/messages.pyx":609
  * 
  * cpdef URL get_absolute_url_to_path(Request request, str path):
  *     return build_absolute_url(             # <<<<<<<<<<<<<<
  *         ensure_bytes(request.scheme),
  *         ensure_bytes(request.host),
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-  /* "blacksheep/messages.pyx":603
+  /* "blacksheep/messages.pyx":610
  * cpdef URL get_absolute_url_to_path(Request request, str path):
  *     return build_absolute_url(
  *         ensure_bytes(request.scheme),             # <<<<<<<<<<<<<<
  *         ensure_bytes(request.host),
  *         ensure_bytes(request.base_path),
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_scheme); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 603, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_scheme); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 603, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":604
+  /* "blacksheep/messages.pyx":611
  *     return build_absolute_url(
  *         ensure_bytes(request.scheme),
  *         ensure_bytes(request.host),             # <<<<<<<<<<<<<<
  *         ensure_bytes(request.base_path),
  *         ensure_bytes(path)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_host); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 604, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_host); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 604, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":605
+  /* "blacksheep/messages.pyx":612
  *         ensure_bytes(request.scheme),
  *         ensure_bytes(request.host),
  *         ensure_bytes(request.base_path),             # <<<<<<<<<<<<<<
  *         ensure_bytes(path)
  *     )
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_base_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_request), __pyx_n_s_base_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 605, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "blacksheep/messages.pyx":606
+  /* "blacksheep/messages.pyx":613
  *         ensure_bytes(request.host),
  *         ensure_bytes(request.base_path),
  *         ensure_bytes(path)             # <<<<<<<<<<<<<<
  *     )
  */
-  __pyx_t_1 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_10blacksheep_8messages_ensure_bytes(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "blacksheep/messages.pyx":602
+  /* "blacksheep/messages.pyx":609
  * 
  * cpdef URL get_absolute_url_to_path(Request request, str path):
  *     return build_absolute_url(             # <<<<<<<<<<<<<<
  *         ensure_bytes(request.scheme),
  *         ensure_bytes(request.host),
  */
-  __pyx_t_5 = ((PyObject *)__pyx_f_10blacksheep_3url_build_absolute_url(((PyObject*)__pyx_t_2), ((PyObject*)__pyx_t_3), ((PyObject*)__pyx_t_4), ((PyObject*)__pyx_t_1), 0)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 602, __pyx_L1_error)
+  __pyx_t_5 = ((PyObject *)__pyx_f_10blacksheep_3url_build_absolute_url(((PyObject*)__pyx_t_2), ((PyObject*)__pyx_t_3), ((PyObject*)__pyx_t_4), ((PyObject*)__pyx_t_1), 0)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_5);
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/messages.pyx":601
+  /* "blacksheep/messages.pyx":608
  * 
  * 
  * cpdef URL get_absolute_url_to_path(Request request, str path):             # <<<<<<<<<<<<<<
  *     return build_absolute_url(
  *         ensure_bytes(request.scheme),
  */
 
@@ -17578,39 +17764,39 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_request)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_path)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_absolute_url_to_path", 1, 2, 2, 1); __PYX_ERR(0, 601, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_absolute_url_to_path", 1, 2, 2, 1); __PYX_ERR(0, 608, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_absolute_url_to_path") < 0)) __PYX_ERR(0, 601, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_absolute_url_to_path") < 0)) __PYX_ERR(0, 608, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_request = ((struct __pyx_obj_10blacksheep_8messages_Request *)values[0]);
     __pyx_v_path = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_absolute_url_to_path", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 601, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_absolute_url_to_path", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 608, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("blacksheep.messages.get_absolute_url_to_path", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 601, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 601, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_request), __pyx_ptype_10blacksheep_8messages_Request, 1, "request", 0))) __PYX_ERR(0, 608, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyUnicode_Type), 1, "path", 1))) __PYX_ERR(0, 608, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_8messages_10get_absolute_url_to_path(__pyx_self, __pyx_v_request, __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -17623,15 +17809,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_absolute_url_to_path", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_10blacksheep_8messages_get_absolute_url_to_path(__pyx_v_request, __pyx_v_path, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_10blacksheep_8messages_get_absolute_url_to_path(__pyx_v_request, __pyx_v_path, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -20346,14 +20532,24 @@
   }
 }
 
 static PyObject *__pyx_getprop_10blacksheep_8messages_7Request_query(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_10blacksheep_8messages_7Request_5query_1__get__(o);
 }
 
+static int __pyx_setprop_10blacksheep_8messages_7Request_query(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_10blacksheep_8messages_7Request_5query_3__set__(o, v);
+  }
+  else {
+    PyErr_SetString(PyExc_NotImplementedError, "__del__");
+    return -1;
+  }
+}
+
 static PyObject *__pyx_getprop_10blacksheep_8messages_7Request_url(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_10blacksheep_8messages_7Request_3url_1__get__(o);
 }
 
 static int __pyx_setprop_10blacksheep_8messages_7Request_url(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
   if (v) {
     return __pyx_pw_10blacksheep_8messages_7Request_3url_3__set__(o, v);
@@ -20471,15 +20667,15 @@
   {(char *)"scheme", __pyx_getprop_10blacksheep_8messages_7Request_scheme, __pyx_setprop_10blacksheep_8messages_7Request_scheme, (char *)0, 0},
   {(char *)"host", __pyx_getprop_10blacksheep_8messages_7Request_host, __pyx_setprop_10blacksheep_8messages_7Request_host, (char *)0, 0},
   {(char *)"path", __pyx_getprop_10blacksheep_8messages_7Request_path, 0, (char *)0, 0},
   {(char *)"base_path", __pyx_getprop_10blacksheep_8messages_7Request_base_path, __pyx_setprop_10blacksheep_8messages_7Request_base_path, (char *)0, 0},
   {(char *)"client_ip", __pyx_getprop_10blacksheep_8messages_7Request_client_ip, 0, (char *)0, 0},
   {(char *)"original_client_ip", __pyx_getprop_10blacksheep_8messages_7Request_original_client_ip, __pyx_setprop_10blacksheep_8messages_7Request_original_client_ip, (char *)0, 0},
   {(char *)"session", __pyx_getprop_10blacksheep_8messages_7Request_session, __pyx_setprop_10blacksheep_8messages_7Request_session, (char *)0, 0},
-  {(char *)"query", __pyx_getprop_10blacksheep_8messages_7Request_query, 0, (char *)0, 0},
+  {(char *)"query", __pyx_getprop_10blacksheep_8messages_7Request_query, __pyx_setprop_10blacksheep_8messages_7Request_query, (char *)0, 0},
   {(char *)"url", __pyx_getprop_10blacksheep_8messages_7Request_url, __pyx_setprop_10blacksheep_8messages_7Request_url, (char *)0, 0},
   {(char *)"cookies", __pyx_getprop_10blacksheep_8messages_7Request_cookies, 0, (char *)0, 0},
   {(char *)"etag", __pyx_getprop_10blacksheep_8messages_7Request_etag, 0, (char *)0, 0},
   {(char *)"if_none_match", __pyx_getprop_10blacksheep_8messages_7Request_if_none_match, 0, (char *)0, 0},
   {(char *)"method", __pyx_getprop_10blacksheep_8messages_7Request_method, __pyx_setprop_10blacksheep_8messages_7Request_method, (char *)0, 0},
   {(char *)"_url", __pyx_getprop_10blacksheep_8messages_7Request__url, __pyx_setprop_10blacksheep_8messages_7Request__url, (char *)0, 0},
   {(char *)"_path", __pyx_getprop_10blacksheep_8messages_7Request__path, __pyx_setprop_10blacksheep_8messages_7Request__path, (char *)0, 0},
@@ -21783,20 +21979,22 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_text, __pyx_k_text, sizeof(__pyx_k_text), 0, 0, 1, 1},
   {&__pyx_n_s_throw, __pyx_k_throw, sizeof(__pyx_k_throw), 0, 0, 1, 1},
   {&__pyx_n_s_timedelta, __pyx_k_timedelta, sizeof(__pyx_k_timedelta), 0, 0, 1, 1},
   {&__pyx_n_s_unquote, __pyx_k_unquote, sizeof(__pyx_k_unquote), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_url, __pyx_k_url, sizeof(__pyx_k_url), 0, 0, 1, 1},
+  {&__pyx_n_s_urlencode, __pyx_k_urlencode, sizeof(__pyx_k_urlencode), 0, 0, 1, 1},
   {&__pyx_n_s_urllib_parse, __pyx_k_urllib_parse, sizeof(__pyx_k_urllib_parse), 0, 0, 1, 1},
   {&__pyx_n_u_user, __pyx_k_user, sizeof(__pyx_k_user), 0, 1, 0, 1},
   {&__pyx_n_s_utcnow, __pyx_k_utcnow, sizeof(__pyx_k_utcnow), 0, 0, 1, 1},
   {&__pyx_n_u_utf8, __pyx_k_utf8, sizeof(__pyx_k_utf8), 0, 1, 0, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_with_content, __pyx_k_with_content, sizeof(__pyx_k_with_content), 0, 0, 1, 1},
+  {&__pyx_n_s_with_query, __pyx_k_with_query, sizeof(__pyx_k_with_query), 0, 0, 1, 1},
   {&__pyx_n_b_xml, __pyx_k_xml, sizeof(__pyx_k_xml), 0, 0, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(0, 9, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 77, __pyx_L1_error)
   __pyx_builtin_UnicodeDecodeError = __Pyx_GetBuiltinName(__pyx_n_s_UnicodeDecodeError); if (!__pyx_builtin_UnicodeDecodeError) __PYX_ERR(0, 148, __pyx_L1_error)
@@ -21875,33 +22073,33 @@
  *                 "A session is not configured for this request, activate "
  *                 "sessions using `app.use_sessions` method."
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_A_session_is_not_configured_for); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "blacksheep/messages.pyx":404
+  /* "blacksheep/messages.pyx":411
  *                 _url = value
  *             else:
  *                 raise TypeError('Invalid value type, expected bytes, str, or URL')             # <<<<<<<<<<<<<<
  *         else:
  *             _url = None
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_Invalid_value_type_expected_byte); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_Invalid_value_type_expected_byte); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "blacksheep/messages.pyx":584
+  /* "blacksheep/messages.pyx":591
  *     if isinstance(value, bytes):
  *         return value
  *     raise ValueError("Input value must be bytes or str")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_Input_value_must_be_bytes_or_str); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 584, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_u_Input_value_must_be_bytes_or_str); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x976f334, 0x6a36ccd, 0x4337ce2):             # <<<<<<<<<<<<<<
@@ -22059,22 +22257,22 @@
   if (__pyx_type_10blacksheep_8messages_Request.tp_weaklistoffset == 0) __pyx_type_10blacksheep_8messages_Request.tp_weaklistoffset = offsetof(struct __pyx_obj_10blacksheep_8messages_Request, __pyx_base.__weakref__);
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10blacksheep_8messages_Request) < 0) __PYX_ERR(0, 264, __pyx_L1_error)
   __pyx_ptype_10blacksheep_8messages_Request = &__pyx_type_10blacksheep_8messages_Request;
   __pyx_vtabptr_10blacksheep_8messages_Response = &__pyx_vtable_10blacksheep_8messages_Response;
   __pyx_vtable_10blacksheep_8messages_Response.__pyx_base = *__pyx_vtabptr_10blacksheep_8messages_Message;
   __pyx_vtable_10blacksheep_8messages_Response.is_redirect = (int (*)(struct __pyx_obj_10blacksheep_8messages_Response *, int __pyx_skip_dispatch))__pyx_f_10blacksheep_8messages_8Response_is_redirect;
   __pyx_type_10blacksheep_8messages_Response.tp_base = __pyx_ptype_10blacksheep_8messages_Message;
-  if (PyType_Ready(&__pyx_type_10blacksheep_8messages_Response) < 0) __PYX_ERR(0, 481, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10blacksheep_8messages_Response) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10blacksheep_8messages_Response.tp_print = 0;
   #endif
-  if (__Pyx_SetVtable(__pyx_type_10blacksheep_8messages_Response.tp_dict, __pyx_vtabptr_10blacksheep_8messages_Response) < 0) __PYX_ERR(0, 481, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Response_2, (PyObject *)&__pyx_type_10blacksheep_8messages_Response) < 0) __PYX_ERR(0, 481, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_10blacksheep_8messages_Response.tp_dict, __pyx_vtabptr_10blacksheep_8messages_Response) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Response_2, (PyObject *)&__pyx_type_10blacksheep_8messages_Response) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
   if (__pyx_type_10blacksheep_8messages_Response.tp_weaklistoffset == 0) __pyx_type_10blacksheep_8messages_Response.tp_weaklistoffset = offsetof(struct __pyx_obj_10blacksheep_8messages_Response, __pyx_base.__weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10blacksheep_8messages_Response) < 0) __PYX_ERR(0, 481, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10blacksheep_8messages_Response) < 0) __PYX_ERR(0, 488, __pyx_L1_error)
   __pyx_ptype_10blacksheep_8messages_Response = &__pyx_type_10blacksheep_8messages_Response;
   if (PyType_Ready(&__pyx_type_10blacksheep_8messages___pyx_scope_struct__read) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10blacksheep_8messages___pyx_scope_struct__read.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10blacksheep_8messages___pyx_scope_struct__read.tp_dictoffset && __pyx_type_10blacksheep_8messages___pyx_scope_struct__read.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10blacksheep_8messages___pyx_scope_struct__read.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -22503,15 +22701,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "blacksheep/messages.pyx":3
  * import http
  * import re
  * from datetime import datetime, timedelta             # <<<<<<<<<<<<<<
  * from json.decoder import JSONDecodeError
- * from urllib.parse import parse_qs, quote, unquote
+ * from urllib.parse import parse_qs, quote, unquote, urlencode
  */
   __pyx_t_1 = PyList_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_datetime);
   __Pyx_GIVEREF(__pyx_n_s_datetime);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_datetime);
   __Pyx_INCREF(__pyx_n_s_timedelta);
@@ -22530,15 +22728,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "blacksheep/messages.pyx":4
  * import re
  * from datetime import datetime, timedelta
  * from json.decoder import JSONDecodeError             # <<<<<<<<<<<<<<
- * from urllib.parse import parse_qs, quote, unquote
+ * from urllib.parse import parse_qs, quote, unquote, urlencode
  * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_JSONDecodeError);
   __Pyx_GIVEREF(__pyx_n_s_JSONDecodeError);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_JSONDecodeError);
@@ -22550,29 +22748,32 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_JSONDecodeError, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "blacksheep/messages.pyx":5
  * from datetime import datetime, timedelta
  * from json.decoder import JSONDecodeError
- * from urllib.parse import parse_qs, quote, unquote             # <<<<<<<<<<<<<<
+ * from urllib.parse import parse_qs, quote, unquote, urlencode             # <<<<<<<<<<<<<<
  * 
  * try:
  */
-  __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_parse_qs);
   __Pyx_GIVEREF(__pyx_n_s_parse_qs);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_parse_qs);
   __Pyx_INCREF(__pyx_n_s_quote);
   __Pyx_GIVEREF(__pyx_n_s_quote);
   PyList_SET_ITEM(__pyx_t_1, 1, __pyx_n_s_quote);
   __Pyx_INCREF(__pyx_n_s_unquote);
   __Pyx_GIVEREF(__pyx_n_s_unquote);
   PyList_SET_ITEM(__pyx_t_1, 2, __pyx_n_s_unquote);
+  __Pyx_INCREF(__pyx_n_s_urlencode);
+  __Pyx_GIVEREF(__pyx_n_s_urlencode);
+  PyList_SET_ITEM(__pyx_t_1, 3, __pyx_n_s_urlencode);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_urllib_parse, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_parse_qs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_parse_qs, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -22580,18 +22781,22 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_quote, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_unquote); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_unquote, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_urlencode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_urlencode, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "blacksheep/messages.pyx":7
- * from urllib.parse import parse_qs, quote, unquote
+ * from urllib.parse import parse_qs, quote, unquote, urlencode
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import cchardet as chardet
  * except ImportError:
  */
   {
     __Pyx_PyThreadState_declare
@@ -22611,15 +22816,15 @@
  */
       __pyx_t_2 = __Pyx_Import(__pyx_n_s_cchardet, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L2_error)
       __Pyx_GOTREF(__pyx_t_2);
       if (PyDict_SetItem(__pyx_d, __pyx_n_s_chardet, __pyx_t_2) < 0) __PYX_ERR(0, 8, __pyx_L2_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
       /* "blacksheep/messages.pyx":7
- * from urllib.parse import parse_qs, quote, unquote
+ * from urllib.parse import parse_qs, quote, unquote, urlencode
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import cchardet as chardet
  * except ImportError:
  */
     }
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -22661,15 +22866,15 @@
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L3_exception_handled;
     }
     goto __pyx_L4_except_error;
     __pyx_L4_except_error:;
 
     /* "blacksheep/messages.pyx":7
- * from urllib.parse import parse_qs, quote, unquote
+ * from urllib.parse import parse_qs, quote, unquote, urlencode
  * 
  * try:             # <<<<<<<<<<<<<<
  *     import cchardet as chardet
  * except ImportError:
  */
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
```

### Comparing `blacksheep-2.0a4/blacksheep/messages.pxd` & `blacksheep-2.0a5/blacksheep/messages.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/messages.pyi` & `blacksheep-2.0a5/blacksheep/messages.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, Generator, List, Optional, Union
+from typing import Any, Callable, Dict, Generator, List, Optional, Sequence, Union
 
 from guardpost import Identity
 
 from .asgi import ASGIScopeInterface
 from .contents import Content, FormPart
 from .cookies import Cookie
 from .headers import Headers, HeaderType
@@ -70,14 +70,16 @@
         self._session: Optional[Session]
     @classmethod
     def incoming(
         cls, method: str, path: bytes, query: bytes, headers: List[HeaderType]
     ) -> "Request": ...
     @property
     def query(self) -> Dict[str, List[str]]: ...
+    @query.setter
+    def query(self, value: Dict[str, Union[str, Sequence[str]]]): ...
     @property
     def url(self) -> URL: ...
     @url.setter
     def url(self, value: Union[URL, bytes, str]) -> None: ...
     def __repr__(self) -> str: ...
     @property
     def session(self) -> Session: ...
```

### Comparing `blacksheep-2.0a4/blacksheep/messages.pyx` & `blacksheep-2.0a5/blacksheep/messages.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import http
 import re
 from datetime import datetime, timedelta
 from json.decoder import JSONDecodeError
-from urllib.parse import parse_qs, quote, unquote
+from urllib.parse import parse_qs, quote, unquote, urlencode
 
 try:
     import cchardet as chardet
 except ImportError:
     import chardet
 
 from blacksheep.multipart import parse_multipart
@@ -371,17 +371,24 @@
         request._path = path
         request._raw_query = query
         return request
 
     @property
     def query(self):
         if self._raw_query:
-            return parse_qs(self._raw_query.decode('utf8'))
+            return parse_qs(self._raw_query.decode("utf8"))
         return {}
 
+    @query.setter
+    def query(self, value):
+        cdef bytes raw_query
+        raw_query = urlencode(value, True).encode("utf8")
+        self._raw_query = raw_query
+        self.url = self.url.with_query(raw_query)
+
     @property
     def url(self):
         if self._url:
             return self._url
 
         if self._raw_query:
             self._url = URL(self._path + b'?' + self._raw_query)
```

### Comparing `blacksheep-2.0a4/blacksheep/middlewares.py` & `blacksheep-2.0a5/blacksheep/middlewares.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/multipart.py` & `blacksheep-2.0a5/blacksheep/multipart.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/ranges.py` & `blacksheep-2.0a5/blacksheep/ranges.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/scribe.c` & `blacksheep-2.0a5/blacksheep/scribe.c`

 * *Files 0% similar despite different names*

```diff
@@ -1471,14 +1471,15 @@
  */
 
 struct __pyx_vtabstruct_10blacksheep_3url_URL {
   struct __pyx_obj_10blacksheep_3url_URL *(*join)(struct __pyx_obj_10blacksheep_3url_URL *, struct __pyx_obj_10blacksheep_3url_URL *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*base_url)(struct __pyx_obj_10blacksheep_3url_URL *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*with_host)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*with_scheme)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
+  struct __pyx_obj_10blacksheep_3url_URL *(*with_query)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_10blacksheep_3url_URL *__pyx_vtabptr_10blacksheep_3url_URL;
 
 
 /* "messages.pxd":18
  * 
  *
```

### Comparing `blacksheep-2.0a4/blacksheep/scribe.pxd` & `blacksheep-2.0a5/blacksheep/scribe.pxd`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/scribe.pyi` & `blacksheep-2.0a5/blacksheep/scribe.pyi`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/scribe.pyx` & `blacksheep-2.0a5/blacksheep/scribe.pyx`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/application.py` & `blacksheep-2.0a5/blacksheep/server/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 from contextlib import asynccontextmanager
+from functools import wraps
+from inspect import signature, unwrap
 from pathlib import Path
 from typing import (
     Any,
     Awaitable,
     Callable,
     Iterable,
     List,
@@ -22,14 +24,15 @@
     UnauthorizedError,
 )
 from guardpost.common import AuthenticatedRequirement
 from itsdangerous import Serializer
 from rodi import ContainerProtocol
 
 from blacksheep.baseapp import BaseApplication, handle_not_found
+from blacksheep.common import extend
 from blacksheep.common.files.asyncfs import FilesHandler
 from blacksheep.contents import ASGIContent
 from blacksheep.exceptions import HTTPException
 from blacksheep.messages import Request, Response
 from blacksheep.middlewares import get_middlewares_chain
 from blacksheep.scribe import send_asgi_response
 from blacksheep.server.asgi import get_request_url_from_scope
@@ -82,19 +85,25 @@
 
 class ApplicationEvent:
     def __init__(self, context: Any) -> None:
         self._handlers: List[Callable[..., Any]] = []
         self.context = context
 
     def __iadd__(self, handler: Callable[..., Any]) -> "ApplicationEvent":
-        self._handlers.append(handler)
+        self._handlers.append(self._wrap_discard(handler))
         return self
 
     def __isub__(self, handler: Callable[..., Any]) -> "ApplicationEvent":
-        self._handlers.remove(handler)
+        to_remove = [
+            callback
+            for callback in self._handlers
+            if callback is handler or unwrap(callback) is handler
+        ]
+        for callback in to_remove:
+            self._handlers.remove(callback)
         return self
 
     def __len__(self) -> int:
         return len(self._handlers)
 
     def __call__(self, *args) -> Any:
         if args:
@@ -107,14 +116,29 @@
 
         return decorator
 
     async def fire(self, *args: Any, **kwargs: Any) -> None:
         for handler in self._handlers:
             await handler(self.context, *args, **kwargs)
 
+    def _wrap_discard(self, function):
+        """
+        If the given function does not accept any parameter, returns a wrapper with a
+        discard parameter; otherwise returns the same function.
+        """
+        if len(signature(function).parameters) == 0:
+
+            @wraps(function)
+            async def wrap_handler(_):
+                await function()
+
+            return wrap_handler
+        else:
+            return function
+
 
 class ApplicationSyncEvent(ApplicationEvent):
     """
     ApplicationEvent whose subscribers must be synchronous functions.
     """
 
     def fire_sync(self, *args: Any, **keywargs: Any) -> None:
@@ -135,21 +159,14 @@
     def __init__(self) -> None:
         super().__init__(
             "The application is already running, configure CORS rules "
             "before starting the application"
         )
 
 
-def _extend(obj, cls):
-    """Applies a mixin to an instance of a class."""
-    base_cls = obj.__class__
-    base_cls_name = obj.__class__.__name__
-    obj.__class__ = type(base_cls_name, (cls, base_cls), {})
-
-
 class Application(BaseApplication):
     """
     Server application class.
     """
 
     def __init__(
         self,
@@ -580,14 +597,15 @@
             controller_type = getattr(handler, "controller_type")
             controller_types.append(controller_type)
             handler.__annotations__["self"] = ControllerParameter[controller_type]
             self.router.add(
                 route.method,
                 self.get_controller_handler_pattern(controller_type, route),
                 handler,
+                controller_type._filters_,
             )
         return controller_types
 
     def register_controllers(self, controller_types: List[Type]):
         """
         Registers controller types as transient services
         in the application service container.
@@ -663,16 +681,19 @@
 
         if self.middlewares:
             self._apply_middlewares_in_routes()
 
     def extend(self, mixin) -> None:
         """
         Extends the class with additional features, applying the given mixin class.
+
+        This method should be used for those scenarios where opting-in for a feature
+        incurs a performance fee, so that said fee is paid only when necessary.
         """
-        _extend(self, mixin)
+        extend(self, mixin)
 
     async def start(self):
         if self.started:
             return
 
         self.started = True
         if self.on_start:
@@ -788,15 +809,15 @@
         await send_asgi_response(response, send)
 
     async def __call__(self, scope, receive, send):
         if scope["type"] == "lifespan":
             return await super()._handle_lifespan(receive, send)  # type: ignore
 
         for route in self.mount_registry.mounted_apps:  # type: ignore
-            route_match = route.match(scope["raw_path"])
+            route_match = route.match_by_path(scope["raw_path"])
             if route_match:
                 raw_path = scope["raw_path"]
                 if raw_path == route.pattern.rstrip(b"/*") and scope["type"] == "http":
                     return await self._handle_redirect_to_mount_root(scope, send)
                 self.handle_mount_path(scope, route_match)
                 return await route.handler(scope, receive, send)
```

### Comparing `blacksheep-2.0a4/blacksheep/server/asgi.py` & `blacksheep-2.0a5/blacksheep/server/asgi.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/authentication/__init__.py` & `blacksheep-2.0a5/blacksheep/server/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/authentication/cookie.py` & `blacksheep-2.0a5/blacksheep/server/authentication/cookie.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/authentication/jwt.py` & `blacksheep-2.0a5/blacksheep/server/authentication/jwt.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/authentication/oidc.py` & `blacksheep-2.0a5/blacksheep/server/authentication/oidc.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from blacksheep.exceptions import BadRequest, Unauthorized
 from blacksheep.messages import Request, Response, get_absolute_url_to_path
 from blacksheep.server.application import Application, ApplicationEvent
 from blacksheep.server.authentication.cookie import CookieAuthentication
 from blacksheep.server.authentication.jwt import JWTBearerAuthentication
 from blacksheep.server.authorization import allow_anonymous
 from blacksheep.server.dataprotection import generate_secret, get_serializer
+from blacksheep.server.headers.cache import cache_control
 from blacksheep.server.responses import accepted, bad_request, html, json, ok, redirect
 from blacksheep.utils import ensure_str
 from blacksheep.utils.aio import FailedRequestError, HTTPHandler
 
 
 def get_logger() -> logging.Logger:
     logger = logging.getLogger("blacksheep.oidc")
@@ -1067,27 +1068,31 @@
         settings,
         parameters_builder=parameters_builder,
         auth_handler=auth_handler,
     )
 
     @allow_anonymous()
     @app.router.get(settings.entry_path)
+    @cache_control(no_cache=True, no_store=True)
     async def redirect_to_sign_in(request: Request):
         return await handler.redirect_to_sign_in(request)
 
     @allow_anonymous()
     @app.router.post(settings.callback_path)
+    @cache_control(no_cache=True, no_store=True)
     async def handle_auth_redirect(request: Request):
         return await handler.handle_auth_redirect(request)
 
     @app.router.get(settings.logout_path)
+    @cache_control(no_cache=True, no_store=True)
     async def redirect_to_logout(request: Request):
         return await handler.handle_logout_redirect(request)
 
     @app.router.post(settings.refresh_token_path)
+    @cache_control(no_cache=True, no_store=True)
     async def refresh_token(request: Request):
         return await handler.handle_refresh_token_request(request)
 
     if is_default:
 
         @app.on_middlewares_configuration
         def insert_challenge_middleware(app):
```

### Comparing `blacksheep-2.0a4/blacksheep/server/authorization/__init__.py` & `blacksheep-2.0a5/blacksheep/server/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/bindings.py` & `blacksheep-2.0a5/blacksheep/server/bindings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/controllers.py` & `blacksheep-2.0a5/blacksheep/server/controllers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 import sys
 from io import BytesIO
-from typing import Any, AsyncIterable, Callable, Optional, Union
+from typing import (
+    Any,
+    AsyncIterable,
+    Callable,
+    ClassVar,
+    Optional,
+    Sequence,
+    Type,
+    Union,
+)
 
 from blacksheep import Request, Response
+from blacksheep.common.types import HeadersType, ParamsType
 from blacksheep.server.responses import (
     ContentDispositionType,
     MessageType,
     accepted,
     bad_request,
     created,
     file,
@@ -24,15 +34,15 @@
     status_code,
     temporary_redirect,
     text,
     unauthorized,
     view,
     view_async,
 )
-from blacksheep.server.routing import RoutesRegistry
+from blacksheep.server.routing import RouteFilter, RoutesRegistry, normalize_filters
 from blacksheep.utils import AnyStr, join_fragments
 
 # singleton router used to store initial configuration,
 # before the application starts
 # this is used as *default* router for controllers, but it can be overridden
 # - see for example tests in test_controllers
 router = RoutesRegistry()
@@ -46,14 +56,43 @@
 delete = router.delete
 trace = router.trace
 options = router.options
 connect = router.connect
 ws = router.ws
 
 
+def filters(
+    *filters: RouteFilter,
+    host: Optional[str] = None,
+    headers: Optional[HeadersType] = None,
+    params: Optional[ParamsType] = None,
+):
+    """
+    Configures a set of filters for a decorated controller type.
+    Filters are applied to all routes defined in the controller.
+
+    ---
+    Example: match a "/" route only if the request includes an header "X-Area: Special"
+
+    ```py
+    @filters(headers={"X-Area": "Special"})
+    class Special(Controller):
+        @get("/")
+        def special(self):
+            ...
+    ```
+    """
+
+    def class_deco(cls: Type["Controller"]):
+        cls._filters_ = normalize_filters(host, headers, params, list(*filters))
+        return cls
+
+    return class_deco
+
+
 class CannotDetermineDefaultViewNameError(RuntimeError):
     def __init__(self):
         super().__init__(
             "Cannot determine the default view name to be used "
             "for the calling function. "
             "Modify your Controller `view()` function call to specify the name"
             " of the view to be used."
@@ -68,14 +107,16 @@
             if hasattr(value, "route_handler"):
                 setattr(value, "controller_type", cls)
 
 
 class Controller(metaclass=ControllerMeta):
     """Base class for all controllers."""
 
+    _filters_: ClassVar[Sequence[RouteFilter]] = []
+
     @classmethod
     def route(cls) -> Optional[str]:
         """
         The base route to be used by all request handlers defined on a
         controller type.
         Override this class method in subclasses, to implement base routes.
         """
@@ -240,15 +281,15 @@
     def file(
         self,
         value: Union[
             Callable[[], AsyncIterable[bytes]], str, bytes, bytearray, BytesIO
         ],
         content_type: str,
         *,
-        file_name: str = None,
+        file_name: Optional[str] = None,
         content_disposition: ContentDispositionType = ContentDispositionType.ATTACHMENT,
     ) -> Response:
         """
         Returns a binary file response with given content type and optional
         file name, for download (attachment)
         (default HTTP 200 OK). This method supports both call with bytes,
         or a generator yielding chunks.
@@ -379,11 +420,7 @@
     @classmethod
     def route(cls) -> Optional[str]:
         cls_name = cls.class_name()
         cls_version = cls.version() or ""
         if cls_version and cls_name.endswith(cls_version.lower()):
             cls_name = cls_name[: -len(cls_version)]
         return join_fragments("api", cls_version, cls_name)
-
-
-# For backward compatibility
-ApiController = APIController
```

### Comparing `blacksheep-2.0a4/blacksheep/server/cors.py` & `blacksheep-2.0a5/blacksheep/server/cors.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/csrf.py` & `blacksheep-2.0a5/blacksheep/server/csrf.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/dataprotection.py` & `blacksheep-2.0a5/blacksheep/server/dataprotection.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/di.py` & `blacksheep-2.0a5/blacksheep/server/di.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/errors.py` & `blacksheep-2.0a5/blacksheep/server/errors.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/files/__init__.py` & `blacksheep-2.0a5/blacksheep/server/files/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/files/dynamic.py` & `blacksheep-2.0a5/blacksheep/server/files/dynamic.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/files/static.py` & `blacksheep-2.0a5/blacksheep/server/files/static.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/headers/cache.py` & `blacksheep-2.0a5/blacksheep/server/headers/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 import inspect
 from functools import wraps
 from typing import Optional
 
 from blacksheep import Request, Response
-from blacksheep.normalization import copy_special_attributes
 from blacksheep.server.normalization import ensure_response
 
 
 def write_cache_control_response_header(
     *,
     max_age: Optional[int] = None,
     shared_max_age: Optional[int] = None,
@@ -69,14 +68,20 @@
         raise ValueError("A cache cannot be private and public at the same time.")
 
     def extend(part: bytes):
         if len(value):
             value.extend(b", ")
         value.extend(part)
 
+    if private:
+        extend(b"private")
+
+    if public:
+        extend(b"public")
+
     if max_age is not None:
         extend(f"max-age={max_age}".encode("ascii"))
 
     if shared_max_age is not None:
         extend(f"s-maxage={shared_max_age}".encode("ascii"))
 
     if no_cache:
@@ -87,20 +92,14 @@
 
     if proxy_revalidate:
         extend(b"proxy-revalidate")
 
     if no_store:
         extend(b"no-store")
 
-    if private:
-        extend(b"private")
-
-    if public:
-        extend(b"public")
-
     if must_understand:
         extend(b"must-understand")
 
     if no_transform:
         extend(b"no-transform")
 
     if immutable:
@@ -267,15 +266,14 @@
 
             @wraps(next_handler)
             def wrapped(*args, **kwargs):
                 response = ensure_response(next_handler(*args, **kwargs))
                 response.add_header(b"cache-control", header_value)
                 return response
 
-            copy_special_attributes(next_handler, wrapped)
             return wrapped
 
     return decorator
 
 
 class CacheControlMiddleware:
     """
```

### Comparing `blacksheep-2.0a4/blacksheep/server/normalization.py` & `blacksheep-2.0a5/blacksheep/server/normalization.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/openapi/common.py` & `blacksheep-2.0a5/blacksheep/server/openapi/common.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/openapi/docstrings.py` & `blacksheep-2.0a5/blacksheep/server/openapi/docstrings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/openapi/exceptions.py` & `blacksheep-2.0a5/blacksheep/server/openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/openapi/ui.py` & `blacksheep-2.0a5/blacksheep/server/openapi/ui.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/openapi/v3.py` & `blacksheep-2.0a5/blacksheep/server/openapi/v3.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/remotes/forwarding.py` & `blacksheep-2.0a5/blacksheep/server/remotes/forwarding.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/remotes/hosts.py` & `blacksheep-2.0a5/blacksheep/server/remotes/hosts.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/rendering/abc.py` & `blacksheep-2.0a5/blacksheep/server/rendering/abc.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/rendering/jinja2.py` & `blacksheep-2.0a5/blacksheep/server/rendering/jinja2.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/res/error.css` & `blacksheep-2.0a5/blacksheep/server/res/error.css`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/res/error.html` & `blacksheep-2.0a5/blacksheep/server/res/error.html`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/res/redoc-ui.html` & `blacksheep-2.0a5/blacksheep/server/res/redoc-ui.html`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/res/swagger-ui.html` & `blacksheep-2.0a5/blacksheep/server/res/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/responses.py` & `blacksheep-2.0a5/blacksheep/server/responses.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/security/hsts.py` & `blacksheep-2.0a5/blacksheep/server/security/hsts.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/server/websocket.py` & `blacksheep-2.0a5/blacksheep/server/websocket.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/sessions/__init__.py` & `blacksheep-2.0a5/blacksheep/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/settings/di.py` & `blacksheep-2.0a5/blacksheep/settings/di.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/settings/html.py` & `blacksheep-2.0a5/blacksheep/settings/html.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/settings/json.py` & `blacksheep-2.0a5/blacksheep/settings/json.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/testing/client.py` & `blacksheep-2.0a5/blacksheep/testing/client.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/testing/helpers.py` & `blacksheep-2.0a5/blacksheep/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/testing/messages.py` & `blacksheep-2.0a5/blacksheep/testing/messages.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/testing/simulator.py` & `blacksheep-2.0a5/blacksheep/testing/simulator.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/url.c` & `blacksheep-2.0a5/blacksheep/url.c`

 * *Files 2% similar despite different names*

```diff
@@ -1002,14 +1002,15 @@
  */
 
 struct __pyx_vtabstruct_10blacksheep_3url_URL {
   struct __pyx_obj_10blacksheep_3url_URL *(*join)(struct __pyx_obj_10blacksheep_3url_URL *, struct __pyx_obj_10blacksheep_3url_URL *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*base_url)(struct __pyx_obj_10blacksheep_3url_URL *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*with_host)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
   struct __pyx_obj_10blacksheep_3url_URL *(*with_scheme)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
+  struct __pyx_obj_10blacksheep_3url_URL *(*with_query)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_10blacksheep_3url_URL *__pyx_vtabptr_10blacksheep_3url_URL;
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
@@ -1497,14 +1498,15 @@
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static struct __pyx_obj_10blacksheep_3url_URL *__pyx_f_10blacksheep_3url_3URL_join(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_other, int __pyx_skip_dispatch); /* proto*/
 static struct __pyx_obj_10blacksheep_3url_URL *__pyx_f_10blacksheep_3url_3URL_base_url(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, int __pyx_skip_dispatch); /* proto*/
 static struct __pyx_obj_10blacksheep_3url_URL *__pyx_f_10blacksheep_3url_3URL_with_host(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_host, int __pyx_skip_dispatch); /* proto*/
+static struct __pyx_obj_10blacksheep_3url_URL *__pyx_f_10blacksheep_3url_3URL_with_query(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_query, int __pyx_skip_dispatch); /* proto*/
 static struct __pyx_obj_10blacksheep_3url_URL *__pyx_f_10blacksheep_3url_3URL_with_scheme(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_schema, int __pyx_skip_dispatch); /* proto*/
 
 /* Module declarations from 'blacksheep.url' */
 static PyTypeObject *__pyx_ptype_10blacksheep_3url_URL = 0;
 static PyTypeObject *__pyx_ptype_10blacksheep_3url_InvalidURL = 0;
 static struct __pyx_obj_10blacksheep_3url_URL *__pyx_f_10blacksheep_3url_build_absolute_url(PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_10blacksheep_3url___pyx_unpickle_InvalidURL__set_state(struct __pyx_obj_10blacksheep_3url_InvalidURL *, PyObject *); /*proto*/
@@ -1567,14 +1569,15 @@
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_with_host[] = "with_host";
 static const char __pyx_k_InvalidURL[] = "InvalidURL";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
+static const char __pyx_k_with_query[] = "with_query";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_with_scheme[] = "with_scheme";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_valid_schema[] = "valid_schema";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_NotImplemented[] = "NotImplemented";
@@ -1667,38 +1670,40 @@
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_super;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_valid_schema;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_s_with_host;
+static PyObject *__pyx_n_s_with_query;
 static PyObject *__pyx_n_s_with_scheme;
 static int __pyx_pf_10blacksheep_3url_10InvalidURL___init__(struct __pyx_obj_10blacksheep_3url_InvalidURL *__pyx_v_self, PyObject *__pyx_v_message); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_10InvalidURL_2__reduce_cython__(struct __pyx_obj_10blacksheep_3url_InvalidURL *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_10InvalidURL_4__setstate_cython__(struct __pyx_obj_10blacksheep_3url_InvalidURL *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_valid_schema(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_schema); /* proto */
 static int __pyx_pf_10blacksheep_3url_3URL___init__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_2__repr__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_4__str__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_6join(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_8base_url(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_10with_host(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_host); /* proto */
-static PyObject *__pyx_pf_10blacksheep_3url_3URL_12with_scheme(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_schema); /* proto */
-static PyObject *__pyx_pf_10blacksheep_3url_3URL_14__add__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_10blacksheep_3url_3URL_16__eq__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_12with_query(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_query); /* proto */
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_14with_scheme(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_schema); /* proto */
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_16__add__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_18__eq__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_5value___get__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_6schema___get__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_4host___get__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_4port___get__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_4path___get__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_5query___get__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_8fragment___get__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_3URL_11is_absolute___get__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10blacksheep_3url_3URL_18__reduce_cython__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10blacksheep_3url_3URL_20__setstate_cython__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_20__reduce_cython__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_22__setstate_cython__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_2build_absolute_url(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_scheme, PyObject *__pyx_v_host, PyObject *__pyx_v_base_path, PyObject *__pyx_v_path); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_4__pyx_unpickle_InvalidURL(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_10blacksheep_3url_6__pyx_unpickle_URL(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_10blacksheep_3url_URL(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_10blacksheep_3url_InvalidURL(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyBytes_Type_lstrip = {0, &__pyx_n_s_lstrip, 0, 0, 0};
 static PyObject *__pyx_int_46;
@@ -3557,22 +3562,22 @@
   return __pyx_r;
 }
 
 /* "blacksheep/url.pyx":72
  *         return URL(base_url)
  * 
  *     cpdef URL with_host(self, bytes host):             # <<<<<<<<<<<<<<
+ *         cdef bytes query, fragment
  *         if not self.is_absolute:
- *             raise TypeError("Cannot generate a URL from a partial URL")
  */
 
 static PyObject *__pyx_pw_10blacksheep_3url_3URL_11with_host(PyObject *__pyx_v_self, PyObject *__pyx_v_host); /*proto*/
 static struct __pyx_obj_10blacksheep_3url_URL *__pyx_f_10blacksheep_3url_3URL_with_host(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_host, int __pyx_skip_dispatch) {
-  PyObject *__pyx_v_query = NULL;
-  PyObject *__pyx_v_fragment = NULL;
+  PyObject *__pyx_v_query = 0;
+  PyObject *__pyx_v_fragment = 0;
   struct __pyx_obj_10blacksheep_3url_URL *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -3624,121 +3629,121 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "blacksheep/url.pyx":73
- * 
+  /* "blacksheep/url.pyx":74
  *     cpdef URL with_host(self, bytes host):
+ *         cdef bytes query, fragment
  *         if not self.is_absolute:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot generate a URL from a partial URL")
  *         query = b"?" + self.query if self.query else b""
  */
   __pyx_t_5 = ((!(__pyx_v_self->is_absolute != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "blacksheep/url.pyx":74
- *     cpdef URL with_host(self, bytes host):
+    /* "blacksheep/url.pyx":75
+ *         cdef bytes query, fragment
  *         if not self.is_absolute:
  *             raise TypeError("Cannot generate a URL from a partial URL")             # <<<<<<<<<<<<<<
  *         query = b"?" + self.query if self.query else b""
  *         fragment = b"#" + self.fragment if self.fragment else b""
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 74, __pyx_L1_error)
+    __PYX_ERR(0, 75, __pyx_L1_error)
 
-    /* "blacksheep/url.pyx":73
- * 
+    /* "blacksheep/url.pyx":74
  *     cpdef URL with_host(self, bytes host):
+ *         cdef bytes query, fragment
  *         if not self.is_absolute:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot generate a URL from a partial URL")
  *         query = b"?" + self.query if self.query else b""
  */
   }
 
-  /* "blacksheep/url.pyx":75
+  /* "blacksheep/url.pyx":76
  *         if not self.is_absolute:
  *             raise TypeError("Cannot generate a URL from a partial URL")
  *         query = b"?" + self.query if self.query else b""             # <<<<<<<<<<<<<<
  *         fragment = b"#" + self.fragment if self.fragment else b""
  *         return URL(self.schema + b"://" + host + self.path + query + fragment)
  */
   __pyx_t_5 = (__pyx_v_self->query != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_self->query) != 0);
   if (__pyx_t_5) {
-    __pyx_t_2 = PyNumber_Add(__pyx_kp_b__11, __pyx_v_self->query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_kp_b__11, __pyx_v_self->query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_b__3);
     __pyx_t_1 = __pyx_kp_b__3;
   }
   __pyx_v_query = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/url.pyx":76
+  /* "blacksheep/url.pyx":77
  *             raise TypeError("Cannot generate a URL from a partial URL")
  *         query = b"?" + self.query if self.query else b""
  *         fragment = b"#" + self.fragment if self.fragment else b""             # <<<<<<<<<<<<<<
  *         return URL(self.schema + b"://" + host + self.path + query + fragment)
  * 
  */
   __pyx_t_5 = (__pyx_v_self->fragment != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_self->fragment) != 0);
   if (__pyx_t_5) {
-    __pyx_t_2 = PyNumber_Add(__pyx_kp_b__12, __pyx_v_self->fragment); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Add(__pyx_kp_b__12, __pyx_v_self->fragment); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   } else {
     __Pyx_INCREF(__pyx_kp_b__3);
     __pyx_t_1 = __pyx_kp_b__3;
   }
   __pyx_v_fragment = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "blacksheep/url.pyx":77
+  /* "blacksheep/url.pyx":78
  *         query = b"?" + self.query if self.query else b""
  *         fragment = b"#" + self.fragment if self.fragment else b""
  *         return URL(self.schema + b"://" + host + self.path + query + fragment)             # <<<<<<<<<<<<<<
  * 
- *     cpdef URL with_scheme(self, bytes schema):
+ *     cpdef URL with_query(self, bytes query):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __pyx_t_1 = PyNumber_Add(__pyx_v_self->schema, __pyx_kp_b__8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_v_self->schema, __pyx_kp_b__8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_host); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_host); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_v_self->path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_v_self->path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_v_fragment); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_v_fragment); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* "blacksheep/url.pyx":72
  *         return URL(base_url)
  * 
  *     cpdef URL with_host(self, bytes host):             # <<<<<<<<<<<<<<
+ *         cdef bytes query, fragment
  *         if not self.is_absolute:
- *             raise TypeError("Cannot generate a URL from a partial URL")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -3796,23 +3801,273 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/url.pyx":79
+/* "blacksheep/url.pyx":80
+ *         return URL(self.schema + b"://" + host + self.path + query + fragment)
+ * 
+ *     cpdef URL with_query(self, bytes query):             # <<<<<<<<<<<<<<
+ *         cdef bytes fragment
+ *         query = b"?" + query if query else b""
+ */
+
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_13with_query(PyObject *__pyx_v_self, PyObject *__pyx_v_query); /*proto*/
+static struct __pyx_obj_10blacksheep_3url_URL *__pyx_f_10blacksheep_3url_3URL_with_query(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_query, int __pyx_skip_dispatch) {
+  PyObject *__pyx_v_fragment = 0;
+  struct __pyx_obj_10blacksheep_3url_URL *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("with_query", 0);
+  __Pyx_INCREF(__pyx_v_query);
+  /* Check if called by wrapper */
+  if (unlikely(__pyx_skip_dispatch)) ;
+  /* Check if overridden in Python */
+  else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
+    #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+    static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
+    if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
+      PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
+      #endif
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_with_query); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_10blacksheep_3url_3URL_13with_query)) {
+        __Pyx_XDECREF(((PyObject *)__pyx_r));
+        __Pyx_INCREF(__pyx_t_1);
+        __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+          if (likely(__pyx_t_4)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+            __Pyx_INCREF(__pyx_t_4);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_3, function);
+          }
+        }
+        __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_query) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_query);
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_2);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_10blacksheep_3url_URL))))) __PYX_ERR(0, 80, __pyx_L1_error)
+        __pyx_r = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_2);
+        __pyx_t_2 = 0;
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+        goto __pyx_L0;
+      }
+      #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+      __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
+      __pyx_obj_dict_version = __Pyx_get_object_dict_version(((PyObject *)__pyx_v_self));
+      if (unlikely(__pyx_type_dict_guard != __pyx_tp_dict_version)) {
+        __pyx_tp_dict_version = __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
+      }
+      #endif
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+    }
+    #endif
+  }
+
+  /* "blacksheep/url.pyx":82
+ *     cpdef URL with_query(self, bytes query):
+ *         cdef bytes fragment
+ *         query = b"?" + query if query else b""             # <<<<<<<<<<<<<<
+ *         fragment = b"#" + self.fragment if self.fragment else b""
+ *         if self.is_absolute:
+ */
+  __pyx_t_5 = (__pyx_v_query != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_query) != 0);
+  if (__pyx_t_5) {
+    __pyx_t_2 = PyNumber_Add(__pyx_kp_b__11, __pyx_v_query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __pyx_t_2;
+    __pyx_t_2 = 0;
+  } else {
+    __Pyx_INCREF(__pyx_kp_b__3);
+    __pyx_t_1 = __pyx_kp_b__3;
+  }
+  __Pyx_DECREF_SET(__pyx_v_query, ((PyObject*)__pyx_t_1));
+  __pyx_t_1 = 0;
+
+  /* "blacksheep/url.pyx":83
+ *         cdef bytes fragment
+ *         query = b"?" + query if query else b""
+ *         fragment = b"#" + self.fragment if self.fragment else b""             # <<<<<<<<<<<<<<
+ *         if self.is_absolute:
+ *             return URL(self.schema + b"://" + self.host + self.path + query + fragment)
+ */
+  __pyx_t_5 = (__pyx_v_self->fragment != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_self->fragment) != 0);
+  if (__pyx_t_5) {
+    __pyx_t_2 = PyNumber_Add(__pyx_kp_b__12, __pyx_v_self->fragment); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __pyx_t_2;
+    __pyx_t_2 = 0;
+  } else {
+    __Pyx_INCREF(__pyx_kp_b__3);
+    __pyx_t_1 = __pyx_kp_b__3;
+  }
+  __pyx_v_fragment = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "blacksheep/url.pyx":84
+ *         query = b"?" + query if query else b""
+ *         fragment = b"#" + self.fragment if self.fragment else b""
+ *         if self.is_absolute:             # <<<<<<<<<<<<<<
+ *             return URL(self.schema + b"://" + self.host + self.path + query + fragment)
+ *         return URL(self.path + query + fragment)
+ */
+  __pyx_t_5 = (__pyx_v_self->is_absolute != 0);
+  if (__pyx_t_5) {
+
+    /* "blacksheep/url.pyx":85
+ *         fragment = b"#" + self.fragment if self.fragment else b""
+ *         if self.is_absolute:
+ *             return URL(self.schema + b"://" + self.host + self.path + query + fragment)             # <<<<<<<<<<<<<<
+ *         return URL(self.path + query + fragment)
+ * 
+ */
+    __Pyx_XDECREF(((PyObject *)__pyx_r));
+    __pyx_t_1 = PyNumber_Add(__pyx_v_self->schema, __pyx_kp_b__8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_self->host); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_v_self->path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_v_fragment); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_r = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_2);
+    __pyx_t_2 = 0;
+    goto __pyx_L0;
+
+    /* "blacksheep/url.pyx":84
+ *         query = b"?" + query if query else b""
+ *         fragment = b"#" + self.fragment if self.fragment else b""
+ *         if self.is_absolute:             # <<<<<<<<<<<<<<
+ *             return URL(self.schema + b"://" + self.host + self.path + query + fragment)
+ *         return URL(self.path + query + fragment)
+ */
+  }
+
+  /* "blacksheep/url.pyx":86
+ *         if self.is_absolute:
+ *             return URL(self.schema + b"://" + self.host + self.path + query + fragment)
+ *         return URL(self.path + query + fragment)             # <<<<<<<<<<<<<<
+ * 
+ *     cpdef URL with_scheme(self, bytes schema):
+ */
+  __Pyx_XDECREF(((PyObject *)__pyx_r));
+  __pyx_t_2 = PyNumber_Add(__pyx_v_self->path, __pyx_v_query); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyNumber_Add(__pyx_t_2, __pyx_v_fragment); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_2);
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "blacksheep/url.pyx":80
  *         return URL(self.schema + b"://" + host + self.path + query + fragment)
  * 
+ *     cpdef URL with_query(self, bytes query):             # <<<<<<<<<<<<<<
+ *         cdef bytes fragment
+ *         query = b"?" + query if query else b""
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("blacksheep.url.URL.with_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_fragment);
+  __Pyx_XDECREF(__pyx_v_query);
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_13with_query(PyObject *__pyx_v_self, PyObject *__pyx_v_query); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_13with_query(PyObject *__pyx_v_self, PyObject *__pyx_v_query) {
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("with_query (wrapper)", 0);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_query), (&PyBytes_Type), 1, "query", 1))) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10blacksheep_3url_3URL_12with_query(((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_v_self), ((PyObject*)__pyx_v_query));
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_12with_query(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_query) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("with_query", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = ((PyObject *)__pyx_f_10blacksheep_3url_3URL_with_query(__pyx_v_self, __pyx_v_query, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("blacksheep.url.URL.with_query", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "blacksheep/url.pyx":88
+ *         return URL(self.path + query + fragment)
+ * 
  *     cpdef URL with_scheme(self, bytes schema):             # <<<<<<<<<<<<<<
  *         valid_schema(schema)
  * 
  */
 
-static PyObject *__pyx_pw_10blacksheep_3url_3URL_13with_scheme(PyObject *__pyx_v_self, PyObject *__pyx_v_schema); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_15with_scheme(PyObject *__pyx_v_self, PyObject *__pyx_v_schema); /*proto*/
 static struct __pyx_obj_10blacksheep_3url_URL *__pyx_f_10blacksheep_3url_3URL_with_scheme(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_schema, int __pyx_skip_dispatch) {
   struct __pyx_obj_10blacksheep_3url_URL *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -3827,35 +4082,35 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_with_scheme); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_with_scheme); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_10blacksheep_3url_3URL_13with_scheme)) {
+      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_10blacksheep_3url_3URL_15with_scheme)) {
         __Pyx_XDECREF(((PyObject *)__pyx_r));
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_schema);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_10blacksheep_3url_URL))))) __PYX_ERR(0, 79, __pyx_L1_error)
+        if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_10blacksheep_3url_URL))))) __PYX_ERR(0, 88, __pyx_L1_error)
         __pyx_r = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_2);
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -3866,106 +4121,106 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "blacksheep/url.pyx":80
+  /* "blacksheep/url.pyx":89
  * 
  *     cpdef URL with_scheme(self, bytes schema):
  *         valid_schema(schema)             # <<<<<<<<<<<<<<
  * 
  *         if not self.is_absolute:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_valid_schema); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_valid_schema); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_schema) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_schema);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "blacksheep/url.pyx":82
+  /* "blacksheep/url.pyx":91
  *         valid_schema(schema)
  * 
  *         if not self.is_absolute:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot generate a URL from a partial URL")
  * 
  */
   __pyx_t_5 = ((!(__pyx_v_self->is_absolute != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "blacksheep/url.pyx":83
+    /* "blacksheep/url.pyx":92
  * 
  *         if not self.is_absolute:
  *             raise TypeError("Cannot generate a URL from a partial URL")             # <<<<<<<<<<<<<<
  * 
  *         return URL(schema + self.value[len(self.schema):])
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 83, __pyx_L1_error)
+    __PYX_ERR(0, 92, __pyx_L1_error)
 
-    /* "blacksheep/url.pyx":82
+    /* "blacksheep/url.pyx":91
  *         valid_schema(schema)
  * 
  *         if not self.is_absolute:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot generate a URL from a partial URL")
  * 
  */
   }
 
-  /* "blacksheep/url.pyx":85
+  /* "blacksheep/url.pyx":94
  *             raise TypeError("Cannot generate a URL from a partial URL")
  * 
  *         return URL(schema + self.value[len(self.schema):])             # <<<<<<<<<<<<<<
  * 
  *     def __add__(self, other):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   if (unlikely(__pyx_v_self->value == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 85, __pyx_L1_error)
+    __PYX_ERR(0, 94, __pyx_L1_error)
   }
   __pyx_t_1 = __pyx_v_self->schema;
   __Pyx_INCREF(__pyx_t_1);
   if (unlikely(__pyx_t_1 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 85, __pyx_L1_error)
+    __PYX_ERR(0, 94, __pyx_L1_error)
   }
-  __pyx_t_6 = PyBytes_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_6 = PyBytes_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PySequence_GetSlice(__pyx_v_self->value, __pyx_t_6, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_1 = PySequence_GetSlice(__pyx_v_self->value, __pyx_t_6, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Add(__pyx_v_schema, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_v_schema, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/url.pyx":79
- *         return URL(self.schema + b"://" + host + self.path + query + fragment)
+  /* "blacksheep/url.pyx":88
+ *         return URL(self.path + query + fragment)
  * 
  *     cpdef URL with_scheme(self, bytes schema):             # <<<<<<<<<<<<<<
  *         valid_schema(schema)
  * 
  */
 
   /* function exit code */
@@ -3979,44 +4234,44 @@
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_3url_3URL_13with_scheme(PyObject *__pyx_v_self, PyObject *__pyx_v_schema); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_3url_3URL_13with_scheme(PyObject *__pyx_v_self, PyObject *__pyx_v_schema) {
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_15with_scheme(PyObject *__pyx_v_self, PyObject *__pyx_v_schema); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_15with_scheme(PyObject *__pyx_v_self, PyObject *__pyx_v_schema) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("with_scheme (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_schema), (&PyBytes_Type), 1, "schema", 1))) __PYX_ERR(0, 79, __pyx_L1_error)
-  __pyx_r = __pyx_pf_10blacksheep_3url_3URL_12with_scheme(((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_v_self), ((PyObject*)__pyx_v_schema));
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_schema), (&PyBytes_Type), 1, "schema", 1))) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10blacksheep_3url_3URL_14with_scheme(((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_v_self), ((PyObject*)__pyx_v_schema));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_3url_3URL_12with_scheme(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_schema) {
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_14with_scheme(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_schema) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("with_scheme", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_10blacksheep_3url_3URL_with_scheme(__pyx_v_self, __pyx_v_schema, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_10blacksheep_3url_3URL_with_scheme(__pyx_v_self, __pyx_v_schema, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4025,163 +4280,163 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/url.pyx":87
+/* "blacksheep/url.pyx":96
  *         return URL(schema + self.value[len(self.schema):])
  * 
  *     def __add__(self, other):             # <<<<<<<<<<<<<<
  *         if isinstance(other, bytes):
  *             return self.join(URL(other))
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_3url_3URL_15__add__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_3url_3URL_15__add__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_17__add__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_17__add__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__add__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10blacksheep_3url_3URL_14__add__(((PyObject *)__pyx_v_self), ((PyObject *)__pyx_v_other));
+  __pyx_r = __pyx_pf_10blacksheep_3url_3URL_16__add__(((PyObject *)__pyx_v_self), ((PyObject *)__pyx_v_other));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_3url_3URL_14__add__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_16__add__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__add__", 0);
 
-  /* "blacksheep/url.pyx":88
+  /* "blacksheep/url.pyx":97
  * 
  *     def __add__(self, other):
  *         if isinstance(other, bytes):             # <<<<<<<<<<<<<<
  *             return self.join(URL(other))
  * 
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_other); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "blacksheep/url.pyx":89
+    /* "blacksheep/url.pyx":98
  *     def __add__(self, other):
  *         if isinstance(other, bytes):
  *             return self.join(URL(other))             # <<<<<<<<<<<<<<
  * 
  *         if isinstance(other, URL):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_join); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_join); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 98, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_v_other); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_v_other); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "blacksheep/url.pyx":88
+    /* "blacksheep/url.pyx":97
  * 
  *     def __add__(self, other):
  *         if isinstance(other, bytes):             # <<<<<<<<<<<<<<
  *             return self.join(URL(other))
  * 
  */
   }
 
-  /* "blacksheep/url.pyx":91
+  /* "blacksheep/url.pyx":100
  *             return self.join(URL(other))
  * 
  *         if isinstance(other, URL):             # <<<<<<<<<<<<<<
  *             return self.join(other)
  *         return NotImplemented
  */
   __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_other, __pyx_ptype_10blacksheep_3url_URL); 
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "blacksheep/url.pyx":92
+    /* "blacksheep/url.pyx":101
  * 
  *         if isinstance(other, URL):
  *             return self.join(other)             # <<<<<<<<<<<<<<
  *         return NotImplemented
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_join); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_join); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_other) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_other);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "blacksheep/url.pyx":91
+    /* "blacksheep/url.pyx":100
  *             return self.join(URL(other))
  * 
  *         if isinstance(other, URL):             # <<<<<<<<<<<<<<
  *             return self.join(other)
  *         return NotImplemented
  */
   }
 
-  /* "blacksheep/url.pyx":93
+  /* "blacksheep/url.pyx":102
  *         if isinstance(other, URL):
  *             return self.join(other)
  *         return NotImplemented             # <<<<<<<<<<<<<<
  * 
  *     def __eq__(self, other):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_builtin_NotImplemented);
   __pyx_r = __pyx_builtin_NotImplemented;
   goto __pyx_L0;
 
-  /* "blacksheep/url.pyx":87
+  /* "blacksheep/url.pyx":96
  *         return URL(schema + self.value[len(self.schema):])
  * 
  *     def __add__(self, other):             # <<<<<<<<<<<<<<
  *         if isinstance(other, bytes):
  *             return self.join(URL(other))
  */
 
@@ -4195,96 +4450,96 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/url.pyx":95
+/* "blacksheep/url.pyx":104
  *         return NotImplemented
  * 
  *     def __eq__(self, other):             # <<<<<<<<<<<<<<
  *         if isinstance(other, URL):
  *             return self.value == other.value
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_3url_3URL_17__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_3url_3URL_17__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_19__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_other); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_19__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__eq__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10blacksheep_3url_3URL_16__eq__(((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_v_self), ((PyObject *)__pyx_v_other));
+  __pyx_r = __pyx_pf_10blacksheep_3url_3URL_18__eq__(((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_v_self), ((PyObject *)__pyx_v_other));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_3url_3URL_16__eq__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_18__eq__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__eq__", 0);
 
-  /* "blacksheep/url.pyx":96
+  /* "blacksheep/url.pyx":105
  * 
  *     def __eq__(self, other):
  *         if isinstance(other, URL):             # <<<<<<<<<<<<<<
  *             return self.value == other.value
  *         return NotImplemented
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_other, __pyx_ptype_10blacksheep_3url_URL); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "blacksheep/url.pyx":97
+    /* "blacksheep/url.pyx":106
  *     def __eq__(self, other):
  *         if isinstance(other, URL):
  *             return self.value == other.value             # <<<<<<<<<<<<<<
  *         return NotImplemented
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_other, __pyx_n_s_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyObject_RichCompare(__pyx_v_self->value, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_v_self->value, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "blacksheep/url.pyx":96
+    /* "blacksheep/url.pyx":105
  * 
  *     def __eq__(self, other):
  *         if isinstance(other, URL):             # <<<<<<<<<<<<<<
  *             return self.value == other.value
  *         return NotImplemented
  */
   }
 
-  /* "blacksheep/url.pyx":98
+  /* "blacksheep/url.pyx":107
  *         if isinstance(other, URL):
  *             return self.value == other.value
  *         return NotImplemented             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_builtin_NotImplemented);
   __pyx_r = __pyx_builtin_NotImplemented;
   goto __pyx_L0;
 
-  /* "blacksheep/url.pyx":95
+  /* "blacksheep/url.pyx":104
  *         return NotImplemented
  * 
  *     def __eq__(self, other):             # <<<<<<<<<<<<<<
  *         if isinstance(other, URL):
  *             return self.value == other.value
  */
 
@@ -4619,27 +4874,27 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_3url_3URL_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_3url_3URL_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_21__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_21__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10blacksheep_3url_3URL_18__reduce_cython__(((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10blacksheep_3url_3URL_20__reduce_cython__(((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_3url_3URL_18__reduce_cython__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self) {
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_20__reduce_cython__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -4918,27 +5173,27 @@
  *     else:
  *         return __pyx_unpickle_URL, (type(self), 0x34a39a6, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_URL__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10blacksheep_3url_3URL_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_10blacksheep_3url_3URL_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_23__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_10blacksheep_3url_3URL_23__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10blacksheep_3url_3URL_20__setstate_cython__(((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_10blacksheep_3url_3URL_22__setstate_cython__(((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10blacksheep_3url_3URL_20__setstate_cython__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_10blacksheep_3url_3URL_22__setstate_cython__(struct __pyx_obj_10blacksheep_3url_URL *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -4969,15 +5224,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "blacksheep/url.pyx":101
+/* "blacksheep/url.pyx":110
  * 
  * 
  * cpdef URL build_absolute_url(             # <<<<<<<<<<<<<<
  *     bytes scheme,
  *     bytes host,
  */
 
@@ -4991,154 +5246,154 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("build_absolute_url", 0);
 
-  /* "blacksheep/url.pyx":107
+  /* "blacksheep/url.pyx":116
  *     bytes path
  * ):
  *     valid_schema(scheme)             # <<<<<<<<<<<<<<
  *     return URL(
  *         scheme
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_valid_schema); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_valid_schema); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_scheme) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_scheme);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "blacksheep/url.pyx":108
+  /* "blacksheep/url.pyx":117
  * ):
  *     valid_schema(scheme)
  *     return URL(             # <<<<<<<<<<<<<<
  *         scheme
  *         + b"://"
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-  /* "blacksheep/url.pyx":110
+  /* "blacksheep/url.pyx":119
  *     return URL(
  *         scheme
  *         + b"://"             # <<<<<<<<<<<<<<
  *         + host
  *         + (b"/" if base_path else b"") + base_path.lstrip(b"/").rstrip(b"/")
  */
-  __pyx_t_1 = PyNumber_Add(__pyx_v_scheme, __pyx_kp_b__8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_v_scheme, __pyx_kp_b__8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "blacksheep/url.pyx":111
+  /* "blacksheep/url.pyx":120
  *         scheme
  *         + b"://"
  *         + host             # <<<<<<<<<<<<<<
  *         + (b"/" if base_path else b"") + base_path.lstrip(b"/").rstrip(b"/")
  *         + (b"/" if path else b"") + path.lstrip(b"/")
  */
-  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_host); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_v_host); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "blacksheep/url.pyx":112
+  /* "blacksheep/url.pyx":121
  *         + b"://"
  *         + host
  *         + (b"/" if base_path else b"") + base_path.lstrip(b"/").rstrip(b"/")             # <<<<<<<<<<<<<<
  *         + (b"/" if path else b"") + path.lstrip(b"/")
  *     )
  */
   __pyx_t_4 = (__pyx_v_base_path != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_base_path) != 0);
   if (__pyx_t_4) {
     __Pyx_INCREF(__pyx_kp_b_);
     __pyx_t_1 = __pyx_kp_b_;
   } else {
     __Pyx_INCREF(__pyx_kp_b__3);
     __pyx_t_1 = __pyx_kp_b__3;
   }
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_2 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyBytes_Type_lstrip, __pyx_v_base_path, __pyx_kp_b_); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyBytes_Type_lstrip, __pyx_v_base_path, __pyx_kp_b_); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_rstrip); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_rstrip); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_2, __pyx_kp_b_) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_b_);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyNumber_Add(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Add(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "blacksheep/url.pyx":113
+  /* "blacksheep/url.pyx":122
  *         + host
  *         + (b"/" if base_path else b"") + base_path.lstrip(b"/").rstrip(b"/")
  *         + (b"/" if path else b"") + path.lstrip(b"/")             # <<<<<<<<<<<<<<
  *     )
  */
   __pyx_t_4 = (__pyx_v_path != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_path) != 0);
   if (__pyx_t_4) {
     __Pyx_INCREF(__pyx_kp_b_);
     __pyx_t_1 = __pyx_kp_b_;
   } else {
     __Pyx_INCREF(__pyx_kp_b__3);
     __pyx_t_1 = __pyx_kp_b__3;
   }
-  __pyx_t_3 = PyNumber_Add(__pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyBytes_Type_lstrip, __pyx_v_path, __pyx_kp_b_); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyBytes_Type_lstrip, __pyx_v_path, __pyx_kp_b_); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = PyNumber_Add(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Add(__pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "blacksheep/url.pyx":108
+  /* "blacksheep/url.pyx":117
  * ):
  *     valid_schema(scheme)
  *     return URL(             # <<<<<<<<<<<<<<
  *         scheme
  *         + b"://"
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10blacksheep_3url_URL), __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_r = ((struct __pyx_obj_10blacksheep_3url_URL *)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "blacksheep/url.pyx":101
+  /* "blacksheep/url.pyx":110
  * 
  * 
  * cpdef URL build_absolute_url(             # <<<<<<<<<<<<<<
  *     bytes scheme,
  *     bytes host,
  */
 
@@ -5192,31 +5447,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_scheme)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_host)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("build_absolute_url", 1, 4, 4, 1); __PYX_ERR(0, 101, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("build_absolute_url", 1, 4, 4, 1); __PYX_ERR(0, 110, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_base_path)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("build_absolute_url", 1, 4, 4, 2); __PYX_ERR(0, 101, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("build_absolute_url", 1, 4, 4, 2); __PYX_ERR(0, 110, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_path)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("build_absolute_url", 1, 4, 4, 3); __PYX_ERR(0, 101, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("build_absolute_url", 1, 4, 4, 3); __PYX_ERR(0, 110, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "build_absolute_url") < 0)) __PYX_ERR(0, 101, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "build_absolute_url") < 0)) __PYX_ERR(0, 110, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -5225,24 +5480,24 @@
     __pyx_v_scheme = ((PyObject*)values[0]);
     __pyx_v_host = ((PyObject*)values[1]);
     __pyx_v_base_path = ((PyObject*)values[2]);
     __pyx_v_path = ((PyObject*)values[3]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("build_absolute_url", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 101, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("build_absolute_url", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 110, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("blacksheep.url.build_absolute_url", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_scheme), (&PyBytes_Type), 1, "scheme", 1))) __PYX_ERR(0, 102, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_host), (&PyBytes_Type), 1, "host", 1))) __PYX_ERR(0, 103, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_base_path), (&PyBytes_Type), 1, "base_path", 1))) __PYX_ERR(0, 104, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyBytes_Type), 1, "path", 1))) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_scheme), (&PyBytes_Type), 1, "scheme", 1))) __PYX_ERR(0, 111, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_host), (&PyBytes_Type), 1, "host", 1))) __PYX_ERR(0, 112, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_base_path), (&PyBytes_Type), 1, "base_path", 1))) __PYX_ERR(0, 113, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_path), (&PyBytes_Type), 1, "path", 1))) __PYX_ERR(0, 114, __pyx_L1_error)
   __pyx_r = __pyx_pf_10blacksheep_3url_2build_absolute_url(__pyx_self, __pyx_v_scheme, __pyx_v_host, __pyx_v_base_path, __pyx_v_path);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5255,15 +5510,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("build_absolute_url", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_10blacksheep_3url_build_absolute_url(__pyx_v_scheme, __pyx_v_host, __pyx_v_base_path, __pyx_v_path, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_10blacksheep_3url_build_absolute_url(__pyx_v_scheme, __pyx_v_host, __pyx_v_base_path, __pyx_v_path, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6175,19 +6430,19 @@
   Py_CLEAR(p->fragment);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyObject *__pyx_tp_richcompare_10blacksheep_3url_URL(PyObject *o1, PyObject *o2, int op) {
   switch (op) {
     case Py_EQ: {
-      return __pyx_pw_10blacksheep_3url_3URL_17__eq__(o1, o2);
+      return __pyx_pw_10blacksheep_3url_3URL_19__eq__(o1, o2);
     }
     case Py_NE: {
       PyObject *ret;
-      ret = __pyx_pw_10blacksheep_3url_3URL_17__eq__(o1, o2);
+      ret = __pyx_pw_10blacksheep_3url_3URL_19__eq__(o1, o2);
       if (likely(ret && ret != Py_NotImplemented)) {
         int b = __Pyx_PyObject_IsTrue(ret); Py_DECREF(ret);
         if (unlikely(b < 0)) return NULL;
         ret = (b) ? Py_False : Py_True;
         Py_INCREF(ret);
       }
       return ret;
@@ -6230,17 +6485,18 @@
   return __pyx_pw_10blacksheep_3url_3URL_11is_absolute_1__get__(o);
 }
 
 static PyMethodDef __pyx_methods_10blacksheep_3url_URL[] = {
   {"join", (PyCFunction)__pyx_pw_10blacksheep_3url_3URL_7join, METH_O, 0},
   {"base_url", (PyCFunction)__pyx_pw_10blacksheep_3url_3URL_9base_url, METH_NOARGS, 0},
   {"with_host", (PyCFunction)__pyx_pw_10blacksheep_3url_3URL_11with_host, METH_O, 0},
-  {"with_scheme", (PyCFunction)__pyx_pw_10blacksheep_3url_3URL_13with_scheme, METH_O, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_10blacksheep_3url_3URL_19__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_10blacksheep_3url_3URL_21__setstate_cython__, METH_O, 0},
+  {"with_query", (PyCFunction)__pyx_pw_10blacksheep_3url_3URL_13with_query, METH_O, 0},
+  {"with_scheme", (PyCFunction)__pyx_pw_10blacksheep_3url_3URL_15with_scheme, METH_O, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_10blacksheep_3url_3URL_21__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_10blacksheep_3url_3URL_23__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_10blacksheep_3url_URL[] = {
   {(char *)"value", __pyx_getprop_10blacksheep_3url_3URL_value, 0, (char *)0, 0},
   {(char *)"schema", __pyx_getprop_10blacksheep_3url_3URL_schema, 0, (char *)0, 0},
   {(char *)"host", __pyx_getprop_10blacksheep_3url_3URL_host, 0, (char *)0, 0},
@@ -6249,15 +6505,15 @@
   {(char *)"query", __pyx_getprop_10blacksheep_3url_3URL_query, 0, (char *)0, 0},
   {(char *)"fragment", __pyx_getprop_10blacksheep_3url_3URL_fragment, 0, (char *)0, 0},
   {(char *)"is_absolute", __pyx_getprop_10blacksheep_3url_3URL_is_absolute, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PyNumberMethods __pyx_tp_as_number_URL = {
-  __pyx_pw_10blacksheep_3url_3URL_15__add__, /*nb_add*/
+  __pyx_pw_10blacksheep_3url_3URL_17__add__, /*nb_add*/
   0, /*nb_subtract*/
   0, /*nb_multiply*/
   #if PY_MAJOR_VERSION < 3 || (CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x03050000)
   0, /*nb_divide*/
   #endif
   0, /*nb_remainder*/
   0, /*nb_divmod*/
@@ -6611,22 +6867,23 @@
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_valid_schema, __pyx_k_valid_schema, sizeof(__pyx_k_valid_schema), 0, 0, 1, 1},
   {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
   {&__pyx_n_s_with_host, __pyx_k_with_host, sizeof(__pyx_k_with_host), 0, 0, 1, 1},
+  {&__pyx_n_s_with_query, __pyx_k_with_query, sizeof(__pyx_k_with_query), 0, 0, 1, 1},
   {&__pyx_n_s_with_scheme, __pyx_k_with_scheme, sizeof(__pyx_k_with_scheme), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 7, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 50, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 74, __pyx_L1_error)
-  __pyx_builtin_NotImplemented = __Pyx_GetBuiltinName(__pyx_n_s_NotImplemented); if (!__pyx_builtin_NotImplemented) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_builtin_NotImplemented = __Pyx_GetBuiltinName(__pyx_n_s_NotImplemented); if (!__pyx_builtin_NotImplemented) __PYX_ERR(0, 102, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -6650,22 +6907,22 @@
  *         cdef bytes base_url
  * 
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_This_URL_is_relative_Cannot_extr); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 61, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "blacksheep/url.pyx":74
- *     cpdef URL with_host(self, bytes host):
+  /* "blacksheep/url.pyx":75
+ *         cdef bytes query, fragment
  *         if not self.is_absolute:
  *             raise TypeError("Cannot generate a URL from a partial URL")             # <<<<<<<<<<<<<<
  *         query = b"?" + self.query if self.query else b""
  *         fragment = b"#" + self.fragment if self.fragment else b""
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Cannot_generate_a_URL_from_a_par); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Cannot_generate_a_URL_from_a_par); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd41d8cd, 0xe3b0c44, 0xda39a3e):             # <<<<<<<<<<<<<<
@@ -6774,14 +7031,15 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_10blacksheep_3url_URL = &__pyx_vtable_10blacksheep_3url_URL;
   __pyx_vtable_10blacksheep_3url_URL.join = (struct __pyx_obj_10blacksheep_3url_URL *(*)(struct __pyx_obj_10blacksheep_3url_URL *, struct __pyx_obj_10blacksheep_3url_URL *, int __pyx_skip_dispatch))__pyx_f_10blacksheep_3url_3URL_join;
   __pyx_vtable_10blacksheep_3url_URL.base_url = (struct __pyx_obj_10blacksheep_3url_URL *(*)(struct __pyx_obj_10blacksheep_3url_URL *, int __pyx_skip_dispatch))__pyx_f_10blacksheep_3url_3URL_base_url;
   __pyx_vtable_10blacksheep_3url_URL.with_host = (struct __pyx_obj_10blacksheep_3url_URL *(*)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch))__pyx_f_10blacksheep_3url_3URL_with_host;
   __pyx_vtable_10blacksheep_3url_URL.with_scheme = (struct __pyx_obj_10blacksheep_3url_URL *(*)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch))__pyx_f_10blacksheep_3url_3URL_with_scheme;
+  __pyx_vtable_10blacksheep_3url_URL.with_query = (struct __pyx_obj_10blacksheep_3url_URL *(*)(struct __pyx_obj_10blacksheep_3url_URL *, PyObject *, int __pyx_skip_dispatch))__pyx_f_10blacksheep_3url_3URL_with_query;
   if (PyType_Ready(&__pyx_type_10blacksheep_3url_URL) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10blacksheep_3url_URL.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10blacksheep_3url_URL.tp_dictoffset && __pyx_type_10blacksheep_3url_URL.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10blacksheep_3url_URL.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
```

### Comparing `blacksheep-2.0a4/blacksheep/url.pxd` & `blacksheep-2.0a5/blacksheep/url.pxd`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     cdef readonly bytes fragment
     cdef readonly bint is_absolute
 
     cpdef URL join(self, URL other)
     cpdef URL base_url(self)
     cpdef URL with_host(self, bytes host)
     cpdef URL with_scheme(self, bytes schema)
+    cpdef URL with_query(self, bytes query)
 
 
 cpdef URL build_absolute_url(
     bytes scheme,
     bytes host,
     bytes base_path,
     bytes path
```

### Comparing `blacksheep-2.0a4/blacksheep/url.pyi` & `blacksheep-2.0a5/blacksheep/url.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -11,11 +11,12 @@
     path: bytes
     query: bytes
     fragment: Optional[bytes]
     is_absolute: Any
     def __init__(self, value: bytes) -> None: ...
     def join(self, other: "URL") -> "URL": ...
     def base_url(self) -> "URL": ...
-    def with_host(self, value: bytes) -> "URL": ...
-    def with_scheme(self, value: bytes) -> "URL": ...
+    def with_host(self, host: bytes) -> "URL": ...
+    def with_scheme(self, scheme: bytes) -> "URL": ...
+    def with_query(self, query: bytes) -> "URL": ...
     def __add__(self, other: Union[bytes, "URL"]) -> "URL": ...
     def __eq__(self, other: object) -> bool: ...
```

### Comparing `blacksheep-2.0a4/blacksheep/url.pyx` & `blacksheep-2.0a5/blacksheep/url.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -66,20 +66,29 @@
         if self.port != 0:
             if (self.schema == b'http' and self.port != 80) or (self.schema == b'https' and self.port != 443):
                 base_url = base_url + b':' + str(self.port).encode()
 
         return URL(base_url)
 
     cpdef URL with_host(self, bytes host):
+        cdef bytes query, fragment
         if not self.is_absolute:
             raise TypeError("Cannot generate a URL from a partial URL")
         query = b"?" + self.query if self.query else b""
         fragment = b"#" + self.fragment if self.fragment else b""
         return URL(self.schema + b"://" + host + self.path + query + fragment)
 
+    cpdef URL with_query(self, bytes query):
+        cdef bytes fragment
+        query = b"?" + query if query else b""
+        fragment = b"#" + self.fragment if self.fragment else b""
+        if self.is_absolute:
+            return URL(self.schema + b"://" + self.host + self.path + query + fragment)
+        return URL(self.path + query + fragment)
+
     cpdef URL with_scheme(self, bytes schema):
         valid_schema(schema)
 
         if not self.is_absolute:
             raise TypeError("Cannot generate a URL from a partial URL")
 
         return URL(schema + self.value[len(self.schema):])
```

### Comparing `blacksheep-2.0a4/blacksheep/utils/__init__.py` & `blacksheep-2.0a5/blacksheep/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep/utils/aio.py` & `blacksheep-2.0a5/blacksheep/utils/aio.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/blacksheep.egg-info/PKG-INFO` & `blacksheep-2.0a5/blacksheep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacksheep
-Version: 2.0a4
+Version: 2.0a5
 Summary: Fast web framework for Python asyncio
 Home-page: https://github.com/Neoteroi/BlackSheep
 Author: Roberto Prevato
 Author-email: roberto.prevato@gmail.com
 License: MIT
 Keywords: BlackSheep web framework
 Platform: *nix
```

### Comparing `blacksheep-2.0a4/blacksheep.egg-info/SOURCES.txt` & `blacksheep-2.0a5/blacksheep.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 blacksheep/client/__init__.py
 blacksheep/client/connection.py
 blacksheep/client/cookies.py
 blacksheep/client/exceptions.py
 blacksheep/client/pool.py
 blacksheep/client/session.py
 blacksheep/common/__init__.py
+blacksheep/common/types.py
 blacksheep/common/files/__init__.py
 blacksheep/common/files/asyncfs.py
 blacksheep/common/files/info.py
 blacksheep/common/files/pathsutils.py
 blacksheep/includes/consts.pxi
 blacksheep/server/__init__.py
 blacksheep/server/application.py
@@ -118,14 +119,15 @@
 blacksheep/testing/simulator.py
 blacksheep/utils/__init__.py
 blacksheep/utils/aio.py
 tests/test_application.py
 tests/test_auth.py
 tests/test_auth_cookie.py
 tests/test_bindings.py
+tests/test_caching.py
 tests/test_contents.py
 tests/test_controllers.py
 tests/test_cookies.py
 tests/test_cors.py
 tests/test_csrf.py
 tests/test_dataprotection.py
 tests/test_env.py
```

### Comparing `blacksheep-2.0a4/setup.py` & `blacksheep-2.0a5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 COMPILE_ARGS = ["-O2"]
 
 
 setup(
     name="blacksheep",
-    version="2.0a4",
+    version="2.0a5",
     description="Fast web framework for Python asyncio",
     long_description=readme(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
@@ -96,17 +96,17 @@
     ],
     install_requires=[
         "httptools>=0.5",
         "certifi>=2022.9.24",
         "cchardet~=2.1.7; python_version < '3.11'",
         "chardet==5.0.0; python_version > '3.10'",
         "guardpost~=1.0.0",
-        "rodi~=2.0.0",
+        "rodi~=2.0.2",
         "essentials>=1.1.4,<2.0",
-        "essentials-openapi>=0.1.4,<1.1",
+        "essentials-openapi>=1.0.6,<1.1",
         "typing_extensions; python_version < '3.8'",
         "python-dateutil~=2.8.2",
         "itsdangerous~=2.1.2",
     ],
     extras_require={
         "full": [
             "cryptography~=38.0.1",
```

### Comparing `blacksheep-2.0a4/tests/test_application.py` & `blacksheep-2.0a5/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_auth.py` & `blacksheep-2.0a5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_auth_cookie.py` & `blacksheep-2.0a5/tests/test_auth_cookie.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_bindings.py` & `blacksheep-2.0a5/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_contents.py` & `blacksheep-2.0a5/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_controllers.py` & `blacksheep-2.0a5/tests/test_controllers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 
 import pytest
 from guardpost import User
 from rodi import inject
 
 from blacksheep import Request, Response
 from blacksheep.server.application import Application
-from blacksheep.server.controllers import APIController, Controller, RoutesRegistry
+from blacksheep.server.controllers import (
+    APIController,
+    Controller,
+    RoutesRegistry,
+    filters,
+)
 from blacksheep.server.responses import text
 from blacksheep.server.routing import RouteDuplicate
 from blacksheep.server.websocket import WebSocket
 from blacksheep.testing.helpers import get_example_scope
 from blacksheep.testing.messages import MockReceive, MockSend
 from blacksheep.utils import ensure_str
 from tests.test_files_serving import get_file_path
@@ -904,7 +909,34 @@
 
     app.setup_controllers()
     await app(get_example_scope("GET", "/"), MockReceive(), MockSend())
 
     assert app.response.status == 200
     data = await app.response.text()
     assert data == "Hello World"
+
+
+@pytest.mark.asyncio
+async def test_controller_filters(app):
+    app.controllers_router = RoutesRegistry()
+    get = app.controllers_router.get
+
+    @filters(headers={"X-Area": "51"})
+    class Home(Controller):
+        @get("/")
+        async def index(self) -> str:
+            return "Hello World"
+
+    app.setup_controllers()
+    await app(get_example_scope("GET", "/"), MockReceive(), MockSend())
+
+    assert app.response.status == 404
+
+    await app(
+        get_example_scope("GET", "/", extra_headers={"X-Area": "51"}),
+        MockReceive(),
+        MockSend(),
+    )
+
+    assert app.response.status == 200
+    data = await app.response.text()
+    assert data == "Hello World"
```

### Comparing `blacksheep-2.0a4/tests/test_cookies.py` & `blacksheep-2.0a5/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_cors.py` & `blacksheep-2.0a5/tests/test_cors.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_csrf.py` & `blacksheep-2.0a5/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_dataprotection.py` & `blacksheep-2.0a5/tests/test_dataprotection.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_files_handler.py` & `blacksheep-2.0a5/tests/test_files_handler.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_files_serving.py` & `blacksheep-2.0a5/tests/test_files_serving.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_forwarding.py` & `blacksheep-2.0a5/tests/test_forwarding.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_headers.py` & `blacksheep-2.0a5/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_multipart.py` & `blacksheep-2.0a5/tests/test_multipart.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_normalization.py` & `blacksheep-2.0a5/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_openapi_docstrings.py` & `blacksheep-2.0a5/tests/test_openapi_docstrings.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_openapi_v3.py` & `blacksheep-2.0a5/tests/test_openapi_v3.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_pathutils.py` & `blacksheep-2.0a5/tests/test_pathutils.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_ranges.py` & `blacksheep-2.0a5/tests/test_ranges.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_requests.py` & `blacksheep-2.0a5/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_responses.py` & `blacksheep-2.0a5/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_sessions.py` & `blacksheep-2.0a5/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_templating.py` & `blacksheep-2.0a5/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_testing.py` & `blacksheep-2.0a5/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_url.py` & `blacksheep-2.0a5/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_utils.py` & `blacksheep-2.0a5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `blacksheep-2.0a4/tests/test_websocket.py` & `blacksheep-2.0a5/tests/test_websocket.py`

 * *Files identical despite different names*

