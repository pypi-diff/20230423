# Comparing `tmp/fastapi_all_out-0.2.3.tar.gz` & `tmp/fastapi_all_out-0.2.4.tar.gz`

## Comparing `fastapi_all_out-0.2.3.tar` & `fastapi_all_out-0.2.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/__init__.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/app.py
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/code_responses.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/enums.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/lazy.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/mailing.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/models.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/responses.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/schemas.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/__init__.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/base.py
--rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/router.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/schemas.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/user_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/jwt/__init__.py
--rw-r--r--   0        0        0     6654 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/jwt/backend.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/jwt/schemas.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/jwt/strategy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/roles/__init__.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/roles/router.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/auth/roles/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/__init__.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/conntection.py
--rw-r--r--   0        0        0    33336 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/repository.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/repository_meta.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/user_repository.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/user_service.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/fields/__init__.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/filters/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/filters/fk.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/filters/int.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/filters/simple.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/filters/str.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/models/__init__.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/models/base.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/models/base_user.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/models/content_type.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/models/permissions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/management/__init__.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/management/command.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/pydantic/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/pydantic/camel_model.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/pydantic/comma_separated.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/pydantic/fields/__init__.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/pydantic/fields/field_in_related_model.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/pydantic/fields/password.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/pydantic/fields/phonenumber.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/pydantic/fields/related_list.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/pydantic/fields/username.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/__init__.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/base_repository.py
--rw-r--r--   0        0        0    20297 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/crud_router.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/exceptions.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/utils.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/base.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/bool.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/fk.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/int.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/int_btw.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/str.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/templates/activation.html
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/fastapi_all_out/templates/password_reset.html
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/LICENSE.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/README.md
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/__init__.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/app.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/code_responses.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/enums.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/lazy.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/mailing.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/models.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/responses.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/schemas.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/__init__.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/base.py
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/router.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/schemas.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/user_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/jwt/__init__.py
+-rw-r--r--   0        0        0     6654 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/jwt/backend.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/jwt/schemas.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/jwt/strategy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/roles/__init__.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/roles/router.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/auth/roles/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/__init__.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/conntection.py
+-rw-r--r--   0        0        0    33337 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/repository.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/repository_meta.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/user_repository.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/user_service.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/fields/__init__.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/filters/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/filters/fk.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/filters/int.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/filters/simple.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/filters/str.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/models/__init__.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/models/base.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/models/base_user.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/models/content_type.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/models/permissions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/management/__init__.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/management/command.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/pydantic/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/pydantic/camel_model.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/pydantic/comma_separated.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/pydantic/fields/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/pydantic/fields/field_in_related_model.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/pydantic/fields/password.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/pydantic/fields/phonenumber.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/pydantic/fields/related_list.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/pydantic/fields/username.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/__init__.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/base_repository.py
+-rw-r--r--   0        0        0    20298 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/crud_router.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/exceptions.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/utils.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/base.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/bool.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/fk.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/int.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/int_btw.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/str.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/templates/activation.html
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/fastapi_all_out/templates/password_reset.html
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/README.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.4/PKG-INFO
```

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/app.py` & `fastapi_all_out-0.2.4/fastapi_all_out/app.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/code_responses.py` & `fastapi_all_out-0.2.4/fastapi_all_out/code_responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/lazy.py` & `fastapi_all_out-0.2.4/fastapi_all_out/lazy.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/mailing.py` & `fastapi_all_out-0.2.4/fastapi_all_out/mailing.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/models.py` & `fastapi_all_out-0.2.4/fastapi_all_out/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/responses.py` & `fastapi_all_out-0.2.4/fastapi_all_out/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/settings.py` & `fastapi_all_out-0.2.4/fastapi_all_out/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/auth/base.py` & `fastapi_all_out-0.2.4/fastapi_all_out/auth/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/auth/router.py` & `fastapi_all_out-0.2.4/fastapi_all_out/auth/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/auth/schemas.py` & `fastapi_all_out-0.2.4/fastapi_all_out/auth/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/auth/user_service.py` & `fastapi_all_out-0.2.4/fastapi_all_out/auth/user_service.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/auth/jwt/backend.py` & `fastapi_all_out-0.2.4/fastapi_all_out/auth/jwt/backend.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/auth/jwt/schemas.py` & `fastapi_all_out-0.2.4/fastapi_all_out/auth/jwt/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/auth/jwt/strategy.py` & `fastapi_all_out-0.2.4/fastapi_all_out/auth/jwt/strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/auth/roles/router.py` & `fastapi_all_out-0.2.4/fastapi_all_out/auth/roles/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/auth/roles/schemas.py` & `fastapi_all_out-0.2.4/fastapi_all_out/auth/roles/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/conntection.py` & `fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/conntection.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/repository.py` & `fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def qs_prefetch_related(self) -> set[str]:
         return set()
 
     async def get_all(
             self,
             skip: Optional[int],
             limit: Optional[int],
-            sort: set[str],
+            sort: list[str],
             filters: list["BaseFilter"],
     ) -> tuple[list[DB_MODEL], int]:
         query = self.get_queryset()
         for f in filters:
             query = f.filter(query)
         base_query = query
         if sort:
```

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/user_repository.py` & `fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/user_repository.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/user_service.py` & `fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/user_service.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py` & `fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/filters/simple.py` & `fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/filters/simple.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/filters/str.py` & `fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/models/base.py` & `fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/models/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/models/base_user.py` & `fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/models/base_user.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/models/content_type.py` & `fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/models/content_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/contrib/tortoise/models/permissions.py` & `fastapi_all_out-0.2.4/fastapi_all_out/contrib/tortoise/models/permissions.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/management/command.py` & `fastapi_all_out-0.2.4/fastapi_all_out/management/command.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/pydantic/camel_model.py` & `fastapi_all_out-0.2.4/fastapi_all_out/pydantic/camel_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/pydantic/comma_separated.py` & `fastapi_all_out-0.2.4/fastapi_all_out/pydantic/comma_separated.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/pydantic/fields/field_in_related_model.py` & `fastapi_all_out-0.2.4/fastapi_all_out/pydantic/fields/field_in_related_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/pydantic/fields/password.py` & `fastapi_all_out-0.2.4/fastapi_all_out/pydantic/fields/password.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/pydantic/fields/phonenumber.py` & `fastapi_all_out-0.2.4/fastapi_all_out/pydantic/fields/phonenumber.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/pydantic/fields/related_list.py` & `fastapi_all_out-0.2.4/fastapi_all_out/pydantic/fields/related_list.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/pydantic/fields/username.py` & `fastapi_all_out-0.2.4/fastapi_all_out/pydantic/fields/username.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/routers/base_repository.py` & `fastapi_all_out-0.2.4/fastapi_all_out/routers/base_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     def get_queryset(self): ...
 
     @abstractmethod
     async def get_all(
             self,
             skip: Optional[int],
             limit: Optional[int],
-            sort: set[str],
+            sort: list[str],
             filters: list[BaseFilter],
     ) -> tuple[list[DB_MODEL], int]: ...
 
     @abstractmethod
     async def get_many(self, item_ids: list[PK]) -> list[DB_MODEL]: ...
 
     @abstractmethod
```

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/routers/crud_router.py` & `fastapi_all_out-0.2.4/fastapi_all_out/routers/crud_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         list_item_schema = self.get_read_list_item_schema()
 
         async def route(
                 background_tasks: BackgroundTasks,
                 request: Request,
                 response: Response,
                 pagination: PAGINATION = pagination_factory(self.max_page_size),
-                sort: set[str] = Depends(sort_factory(self.available_sort)),
+                sort: list[str] = Depends(sort_factory(self.available_sort)),
                 applied_filters: list[BaseFilter] = Depends(get_filters(self.filters))
         ):
             raise_if_error_in_filters(applied_filters)
             skip, limit = pagination
             repository = self.repo(request=request, background_tasks=background_tasks, response=response)
             result, total = await repository.get_all(
                 skip=skip,
```

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/routers/exceptions.py` & `fastapi_all_out-0.2.4/fastapi_all_out/routers/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/routers/utils.py` & `fastapi_all_out-0.2.4/fastapi_all_out/routers/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,21 +33,26 @@
 def get_filters(filters: list[Type["BaseFilter"]]):
     def wrapper(request: Request) -> list["BaseFilter"]:
         qp = request.query_params
         return [final_f for f in filters if (final_f := f.from_qs(qp))]
     return wrapper
 
 
-def sort_factory(available: set[str]) -> Callable[[...], set[str]]:
+def sort_factory(available: set[str]) -> Callable[[...], list[str]]:
+    available_bidirectional: set[str] = set()
+    for x in available:
+        available_bidirectional.add(x)
+        available_bidirectional.add('-' + x)
+
     def sort(fields: CommaSeparatedOf(str, wrapper=snake_case, in_query=True) = Query(
         None,
         alias='sort',
-        description=f'Пиши,поля,через,запятую. Доступно: {", ".join(available)}'
-    )) -> set[str]:
-        result: set[str] = set()
+        description=f'Пиши,поля,через,запятую. Доступно (+ эти же с минусами): {", ".join(available)}'
+    )) -> list[str]:
+        result: list[str] = []
         if fields:
             for field in fields:
-                if field in available:
-                    result.add(field)
+                if field in available_bidirectional:
+                    result.append(field)
         return result
 
     return sort
```

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/base.py` & `fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/bool.py` & `fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/bool.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/int.py` & `fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/int.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/int_btw.py` & `fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/int_btw.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/routers/filters/str.py` & `fastapi_all_out-0.2.4/fastapi_all_out/routers/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/templates/activation.html` & `fastapi_all_out-0.2.4/fastapi_all_out/templates/activation.html`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/fastapi_all_out/templates/password_reset.html` & `fastapi_all_out-0.2.4/fastapi_all_out/templates/password_reset.html`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/LICENSE.md` & `fastapi_all_out-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.3/pyproject.toml` & `fastapi_all_out-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build]
 ignore-vcs = true
 include = ["fastapi_all_out"]
 
 [project]
 name = "fastapi-all-out"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 maintainers = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 keywords = ["DDD", "Domain-driven design", "Database", "WEB", "Architecture", "Backend"]
```

### Comparing `fastapi_all_out-0.2.3/PKG-INFO` & `fastapi_all_out-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-all-out
-Version: 0.2.3
+Version: 0.2.4
 Summary: Makes fastapi much easier and stronger, then Django
 Project-URL: Github, https://github.com/alta7700/fastapi_all_out/
 Author-email: Alexandr Tamrazov <alta77@mail.ru>
 Maintainer-email: Alexandr Tamrazov <alta77@mail.ru>
 License: Copyright © 2023 Alexandr Tamrazov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

