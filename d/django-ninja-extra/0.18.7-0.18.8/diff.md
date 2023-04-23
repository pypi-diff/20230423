# Comparing `tmp/django-ninja-extra-0.18.7.tar.gz` & `tmp/django-ninja-extra-0.18.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ninja-extra-0.18.7.tar", last modified: Sat Mar 11 08:10:06 2023, max compression
+gzip compressed data, was "django-ninja-extra-0.18.8.tar", last modified: Sun Apr 23 05:58:08 2023, max compression
```

## Comparing `django-ninja-extra-0.18.7.tar` & `django-ninja-extra-0.18.8.tar`

### file list

```diff
@@ -1,121 +1,127 @@
--rw-r--r--   0        0        0      269 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/.coveragerc
--rw-r--r--   0        0        0       64 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/.dockerignore
--rw-r--r--   0        0        0      126 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/.flake8
--rw-r--r--   0        0        0      528 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/.github/dependabot.yml
--rw-r--r--   0        0        0      661 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/.github/workflows/publish.yml
--rw-r--r--   0        0        0      571 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/.github/workflows/test.yml
--rw-r--r--   0        0        0     1323 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/.github/workflows/test_full.yml
--rw-r--r--   0        0        0      114 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/.gitignore
--rw-r--r--   0        0        0       52 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/.isort.cfg
--rw-r--r--   0        0        0     1073 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1082 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/LICENSE
--rw-r--r--   0        0        0      968 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/Makefile
--rw-r--r--   0        0        0     4088 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/README.md
--rw-r--r--   0        0        0     3315 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/docs/api_controller/api_controller_permission.md
--rw-r--r--   0        0        0     3476 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/docs/api_controller/api_controller_route.md
--rw-r--r--   0        0        0     1546 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/docs/api_controller/api_controller_router.md
--rw-r--r--   0        0        0     8947 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/docs/api_controller/index.md
--rw-r--r--   0        0        0    51900 2023-03-11 08:09:43.353874 django-ninja-extra-0.18.7/docs/images/benchmark.png
--rw-r--r--   0        0        0  1100522 2023-03-11 08:09:43.357874 django-ninja-extra-0.18.7/docs/images/custom_exception.gif
--rwxr-xr-x   0        0        0  5136836 2023-03-11 08:09:43.389875 django-ninja-extra-0.18.7/docs/images/pagination_example.gif
--rw-r--r--   0        0        0  1478750 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/images/ui_swagger_preview_readme.gif
--rw-r--r--   0        0        0     4133 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/index.md
--rw-r--r--   0        0        0     5705 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/route_context.md
--rw-r--r--   0        0        0    12801 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/service_module_injector.md
--rw-r--r--   0        0        0     1662 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/settings.md
--rw-r--r--   0        0        0     1507 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/tutorial/authentication.md
--rw-r--r--   0        0        0     1497 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/tutorial/body_request.md
--rw-r--r--   0        0        0      975 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/tutorial/custom_exception.md
--rw-r--r--   0        0        0     1025 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/tutorial/form.md
--rw-r--r--   0        0        0     2958 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/tutorial/index.md
--rw-r--r--   0        0        0     2324 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/tutorial/pagination.md
--rw-r--r--   0        0        0      595 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/tutorial/path.md
--rw-r--r--   0        0        0      756 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/tutorial/query.md
--rw-r--r--   0        0        0     1276 2023-03-11 08:09:43.393875 django-ninja-extra-0.18.7/docs/tutorial/schema.md
--rw-r--r--   0        0        0     1847 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/docs/tutorial/testing.md
--rw-r--r--   0        0        0     7330 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/docs/tutorial/throttling.md
--rw-r--r--   0        0        0     2064 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/docs/tutorial/versioning.md
--rw-r--r--   0        0        0     1673 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/mkdocs.yml
--rw-r--r--   0        0        0      414 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/mypy.ini
--rw-r--r--   0        0        0     1087 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/__init__.py
--rw-r--r--   0        0        0     1291 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/apps.py
--rw-r--r--   0        0        0      440 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/compatible.py
--rw-r--r--   0        0        0       55 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/conf/__init__.py
--rw-r--r--   0        0        0     2858 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/conf/settings.py
--rw-r--r--   0        0        0      238 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/constants.py
--rw-r--r--   0        0        0      700 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/controllers/__init__.py
--rw-r--r--   0        0        0    17751 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/controllers/base.py
--rw-r--r--   0        0        0     1313 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/controllers/registry.py
--rw-r--r--   0        0        0     6265 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/controllers/response.py
--rw-r--r--   0        0        0    25918 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/controllers/route/__init__.py
--rw-r--r--   0        0        0     1125 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/controllers/route/context.py
--rw-r--r--   0        0        0     7724 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/controllers/route/route_functions.py
--rw-r--r--   0        0        0     1434 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/dependency_resolver.py
--rw-r--r--   0        0        0     1876 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/details.py
--rw-r--r--   0        0        0     8814 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/exceptions.py
--rw-r--r--   0        0        0     1775 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/generic.py
--rw-r--r--   0        0        0      243 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/helper.py
--rw-r--r--   0        0        0      670 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/lazy.py
--rw-r--r--   0        0        0       61 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/logger.py
--rw-r--r--   0        0        0     4322 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/main.py
--rw-r--r--   0        0        0     1305 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/modules.py
--rw-r--r--   0        0        0    19913 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/operation.py
--rw-r--r--   0        0        0     7993 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/pagination.py
--rw-r--r--   0        0        0      281 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/permissions/__init__.py
--rw-r--r--   0        0        0     5311 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/permissions/base.py
--rw-r--r--   0        0        0     1622 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/permissions/common.py
--rw-r--r--   0        0        0        0 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/py.typed
--rw-r--r--   0        0        0     2194 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/router.py
--rw-r--r--   0        0        0      313 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/schemas/__init__.py
--rw-r--r--   0        0        0     3573 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/schemas/response.py
--rw-r--r--   0        0        0      748 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/security/__init__.py
--rw-r--r--   0        0        0      880 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/security/api_key.py
--rw-r--r--   0        0        0     1705 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/security/http.py
--rw-r--r--   0        0        0      542 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/security/session.py
--rw-r--r--   0        0        0     2516 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/shortcuts.py
--rw-r--r--   0        0        0      103 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/signals.py
--rw-r--r--   0        0        0     2515 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/status.py
--rw-r--r--   0        0        0      112 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/testing/__init__.py
--rw-r--r--   0        0        0     2059 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/testing/client.py
--rw-r--r--   0        0        0      318 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/throttling/__init__.py
--rw-r--r--   0        0        0     3921 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/throttling/decorator.py
--rw-r--r--   0        0        0     8211 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/throttling/model.py
--rw-r--r--   0        0        0      267 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/types.py
--rw-r--r--   0        0        0     1116 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/ninja_extra/urls.py
--rw-r--r--   0        0        0     2392 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/pyproject.toml
--rwxr-xr-x   0        0        0       61 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/pytest.ini
--rw-r--r--   0        0        0        0 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/__init__.py
--rw-r--r--   0        0        0     2180 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/conftest.py
--rw-r--r--   0        0        0     1332 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/controllers.py
--rw-r--r--   0        0        0      495 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/models.py
--rw-r--r--   0        0        0       89 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/schemas.py
--rw-r--r--   0        0        0     2121 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_api_instance.py
--rw-r--r--   0        0        0     7322 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_async_auth.py
--rw-r--r--   0        0        0    12405 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_controller.py
--rw-r--r--   0        0        0     1571 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_controller_registry.py
--rw-r--r--   0        0        0     2725 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_controller_response.py
--rw-r--r--   0        0        0     1871 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_dependency_resolver.py
--rw-r--r--   0        0        0     1059 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_django_model.py
--rw-r--r--   0        0        0     3533 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_django_ninja_router.py
--rw-r--r--   0        0        0     2157 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_event_controller.py
--rw-r--r--   0        0        0     6706 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_exceptions.py
--rw-r--r--   0        0        0     2048 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_generic_patch.py
--rw-r--r--   0        0        0      460 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_lazy_import.py
--rw-r--r--   0        0        0     4044 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_operation.py
--rw-r--r--   0        0        0    12132 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_pagination.py
--rw-r--r--   0        0        0     9919 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_permissions.py
--rw-r--r--   0        0        0    13878 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_route.py
--rw-r--r--   0        0        0     1509 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_settings.py
--rw-r--r--   0        0        0     2466 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_shortcuts.py
--rw-r--r--   0        0        0     1051 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_status.py
--rw-r--r--   0        0        0     1274 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_testclient.py
--rw-r--r--   0        0        0        0 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_throthling/__init__.py
--rw-r--r--   0        0        0      461 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_throthling/sample_models.py
--rw-r--r--   0        0        0    10309 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_throthling/test_decorator.py
--rw-r--r--   0        0        0     7286 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_throthling/test_models.py
--rw-r--r--   0        0        0     2797 2023-03-11 08:09:43.397875 django-ninja-extra-0.18.7/tests/test_throthling/test_throttle_controller.py
--rw-r--r--   0        0        0     3536 2023-03-11 08:09:43.401875 django-ninja-extra-0.18.7/tests/test_throthling/test_throttle_decorator_on_controllers.py
--rw-r--r--   0        0        0     3345 2023-03-11 08:09:43.401875 django-ninja-extra-0.18.7/tests/test_throthling/test_throttling_xxf.py
--rw-r--r--   0        0        0      293 2023-03-11 08:09:43.401875 django-ninja-extra-0.18.7/tests/urls.py
--rw-r--r--   0        0        0     1769 2023-03-11 08:09:43.401875 django-ninja-extra-0.18.7/tests/utils.py
--rw-r--r--   0        0        0     7057 1970-01-01 00:00:00.000000 django-ninja-extra-0.18.7/PKG-INFO
+-rw-r--r--   0        0        0      269 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/.coveragerc
+-rw-r--r--   0        0        0       64 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/.dockerignore
+-rw-r--r--   0        0        0      126 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/.flake8
+-rw-r--r--   0        0        0      528 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/.github/dependabot.yml
+-rw-r--r--   0        0        0      661 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      571 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1323 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0      114 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/.gitignore
+-rw-r--r--   0        0        0       52 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/.isort.cfg
+-rw-r--r--   0        0        0     1069 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1082 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/LICENSE
+-rw-r--r--   0        0        0      968 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/Makefile
+-rw-r--r--   0        0        0     4089 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/README.md
+-rw-r--r--   0        0        0     3371 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/docs/api_controller/api_controller_permission.md
+-rw-r--r--   0        0        0     3476 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/docs/api_controller/api_controller_route.md
+-rw-r--r--   0        0        0     1546 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/docs/api_controller/api_controller_router.md
+-rw-r--r--   0        0        0     7774 2023-04-23 05:57:47.673720 django-ninja-extra-0.18.8/docs/api_controller/index.md
+-rw-r--r--   0        0        0    51900 2023-04-23 05:57:47.677721 django-ninja-extra-0.18.8/docs/images/benchmark.png
+-rw-r--r--   0        0        0  1100522 2023-04-23 05:57:47.681721 django-ninja-extra-0.18.8/docs/images/custom_exception.gif
+-rwxr-xr-x   0        0        0  5136836 2023-04-23 05:57:47.709721 django-ninja-extra-0.18.8/docs/images/pagination_example.gif
+-rw-r--r--   0        0        0  1478750 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/images/ui_swagger_preview_readme.gif
+-rw-r--r--   0        0        0     4133 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/index.md
+-rw-r--r--   0        0        0     5705 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/route_context.md
+-rw-r--r--   0        0        0    12801 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/service_module_injector.md
+-rw-r--r--   0        0        0     2028 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/settings.md
+-rw-r--r--   0        0        0     2694 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/authentication.md
+-rw-r--r--   0        0        0     1497 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/body_request.md
+-rw-r--r--   0        0        0      975 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/custom_exception.md
+-rw-r--r--   0        0        0     1025 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/form.md
+-rw-r--r--   0        0        0     2958 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/index.md
+-rw-r--r--   0        0        0     2782 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/ordering.md
+-rw-r--r--   0        0        0     2324 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/pagination.md
+-rw-r--r--   0        0        0      595 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/path.md
+-rw-r--r--   0        0        0      756 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/query.md
+-rw-r--r--   0        0        0     1276 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/schema.md
+-rw-r--r--   0        0        0     3621 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/searching.md
+-rw-r--r--   0        0        0     1847 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/testing.md
+-rw-r--r--   0        0        0     7330 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/throttling.md
+-rw-r--r--   0        0        0     2064 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/docs/tutorial/versioning.md
+-rw-r--r--   0        0        0     1778 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/mkdocs.yml
+-rw-r--r--   0        0        0      414 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/mypy.ini
+-rw-r--r--   0        0        0     1087 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/__init__.py
+-rw-r--r--   0        0        0     1291 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/apps.py
+-rw-r--r--   0        0        0      440 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/compatible.py
+-rw-r--r--   0        0        0       55 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/conf/__init__.py
+-rw-r--r--   0        0        0     3554 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/conf/settings.py
+-rw-r--r--   0        0        0      276 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/constants.py
+-rw-r--r--   0        0        0      700 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/controllers/__init__.py
+-rw-r--r--   0        0        0    17997 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/controllers/base.py
+-rw-r--r--   0        0        0     1313 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/controllers/registry.py
+-rw-r--r--   0        0        0     6265 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/controllers/response.py
+-rw-r--r--   0        0        0    25969 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/controllers/route/__init__.py
+-rw-r--r--   0        0        0     1125 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/controllers/route/context.py
+-rw-r--r--   0        0        0     7744 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/controllers/route/route_functions.py
+-rw-r--r--   0        0        0     1434 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/dependency_resolver.py
+-rw-r--r--   0        0        0     1876 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/details.py
+-rw-r--r--   0        0        0     8814 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/exceptions.py
+-rw-r--r--   0        0        0     1775 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/generic.py
+-rw-r--r--   0        0        0      597 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/helper.py
+-rw-r--r--   0        0        0      670 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/lazy.py
+-rw-r--r--   0        0        0       61 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/logger.py
+-rw-r--r--   0        0        0     4322 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/main.py
+-rw-r--r--   0        0        0     1305 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/modules.py
+-rw-r--r--   0        0        0    19913 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/operation.py
+-rw-r--r--   0        0        0     8324 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/ordering.py
+-rw-r--r--   0        0        0     8275 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/pagination.py
+-rw-r--r--   0        0        0      281 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/permissions/__init__.py
+-rw-r--r--   0        0        0     5311 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/permissions/base.py
+-rw-r--r--   0        0        0     1622 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/permissions/common.py
+-rw-r--r--   0        0        0        0 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/py.typed
+-rw-r--r--   0        0        0     2194 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/router.py
+-rw-r--r--   0        0        0      313 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/schemas/__init__.py
+-rw-r--r--   0        0        0     3573 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/schemas/response.py
+-rw-r--r--   0        0        0     9412 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/searching.py
+-rw-r--r--   0        0        0      748 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/security/__init__.py
+-rw-r--r--   0        0        0      880 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/security/api_key.py
+-rw-r--r--   0        0        0     1705 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/security/http.py
+-rw-r--r--   0        0        0      542 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/security/session.py
+-rw-r--r--   0        0        0     2516 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/shortcuts.py
+-rw-r--r--   0        0        0      103 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/signals.py
+-rw-r--r--   0        0        0     2515 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/status.py
+-rw-r--r--   0        0        0      112 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/testing/__init__.py
+-rw-r--r--   0        0        0     2059 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/testing/client.py
+-rw-r--r--   0        0        0      318 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/throttling/__init__.py
+-rw-r--r--   0        0        0     3921 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/throttling/decorator.py
+-rw-r--r--   0        0        0     8211 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/throttling/model.py
+-rw-r--r--   0        0        0      267 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/types.py
+-rw-r--r--   0        0        0     1116 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/ninja_extra/urls.py
+-rw-r--r--   0        0        0     2392 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/pyproject.toml
+-rwxr-xr-x   0        0        0       61 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/pytest.ini
+-rw-r--r--   0        0        0        0 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/__init__.py
+-rw-r--r--   0        0        0     2181 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/conftest.py
+-rw-r--r--   0        0        0     1332 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/controllers.py
+-rw-r--r--   0        0        0      495 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/models.py
+-rw-r--r--   0        0        0       89 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/schemas.py
+-rw-r--r--   0        0        0     2121 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_api_instance.py
+-rw-r--r--   0        0        0     7322 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_async_auth.py
+-rw-r--r--   0        0        0    13342 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_controller.py
+-rw-r--r--   0        0        0     1571 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_controller_registry.py
+-rw-r--r--   0        0        0     2725 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_controller_response.py
+-rw-r--r--   0        0        0     1871 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_dependency_resolver.py
+-rw-r--r--   0        0        0     1059 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_django_model.py
+-rw-r--r--   0        0        0     3533 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_django_ninja_router.py
+-rw-r--r--   0        0        0     2157 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_event_controller.py
+-rw-r--r--   0        0        0     6706 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_exceptions.py
+-rw-r--r--   0        0        0     2048 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_generic_patch.py
+-rw-r--r--   0        0        0      460 2023-04-23 05:57:47.717722 django-ninja-extra-0.18.8/tests/test_lazy_import.py
+-rw-r--r--   0        0        0     4227 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_operation.py
+-rw-r--r--   0        0        0    14220 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_ordering.py
+-rw-r--r--   0        0        0    12132 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_pagination.py
+-rw-r--r--   0        0        0    10048 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_permissions.py
+-rw-r--r--   0        0        0    15512 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_route.py
+-rw-r--r--   0        0        0    13597 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_searching.py
+-rw-r--r--   0        0        0     2316 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_settings.py
+-rw-r--r--   0        0        0     2466 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_shortcuts.py
+-rw-r--r--   0        0        0     1051 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_status.py
+-rw-r--r--   0        0        0     1274 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_testclient.py
+-rw-r--r--   0        0        0        0 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_throthling/__init__.py
+-rw-r--r--   0        0        0      461 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_throthling/sample_models.py
+-rw-r--r--   0        0        0    10309 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_throthling/test_decorator.py
+-rw-r--r--   0        0        0     7286 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_throthling/test_models.py
+-rw-r--r--   0        0        0     2797 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_throthling/test_throttle_controller.py
+-rw-r--r--   0        0        0     3536 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_throthling/test_throttle_decorator_on_controllers.py
+-rw-r--r--   0        0        0     3345 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/test_throthling/test_throttling_xxf.py
+-rw-r--r--   0        0        0      293 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/urls.py
+-rw-r--r--   0        0        0     1769 2023-04-23 05:57:47.721722 django-ninja-extra-0.18.8/tests/utils.py
+-rw-r--r--   0        0        0     7058 1970-01-01 00:00:00.000000 django-ninja-extra-0.18.8/PKG-INFO
```

### Comparing `django-ninja-extra-0.18.7/.github/dependabot.yml` & `django-ninja-extra-0.18.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/.github/workflows/publish.yml` & `django-ninja-extra-0.18.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/.github/workflows/test.yml` & `django-ninja-extra-0.18.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/.github/workflows/test_full.yml` & `django-ninja-extra-0.18.8/.github/workflows/test_full.yml`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/.pre-commit-config.yaml` & `django-ninja-extra-0.18.8/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 - repo: local
   hooks:
     - id: code_formatting
       args: []
       name: Code Formatting
       entry: "make fmt"
       types: [python]
-      language_version: python3.8
+      language_version: python3
       language: python
     - id: code_linting
       args: [ ]
       name: Code Linting
       entry: "make lint"
       types: [ python ]
-      language_version: python3.8
+      language_version: python3
       language: python
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v2.3.0
   hooks:
   - id: end-of-file-fixer
     exclude: >-
       ^examples/[^/]*\.svg$
```

### Comparing `django-ninja-extra-0.18.7/LICENSE` & `django-ninja-extra-0.18.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/Makefile` & `django-ninja-extra-0.18.8/Makefile`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/README.md` & `django-ninja-extra-0.18.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![Test](https://github.com/eadwinCode/django-ninja-extra/workflows/Test/badge.svg)
 [![PyPI version](https://badge.fury.io/py/django-ninja-extra.svg)](https://badge.fury.io/py/django-ninja-extra)
 [![PyPI version](https://img.shields.io/pypi/v/django-ninja-extra.svg)](https://pypi.python.org/pypi/django-ninja-extra)
 [![PyPI version](https://img.shields.io/pypi/pyversions/django-ninja-extra.svg)](https://pypi.python.org/pypi/django-ninja-extra)
 [![PyPI version](https://img.shields.io/pypi/djversions/django-ninja-extra.svg)](https://pypi.python.org/pypi/django-ninja-extra)
 [![Codecov](https://img.shields.io/codecov/c/gh/eadwinCode/django-ninja-extra)](https://codecov.io/gh/eadwinCode/django-ninja-extra)
-[![Downloads](https://pepy.tech/badge/django-ninja-extra/month)](https://pepy.tech/project/django-ninja-extra)
+[![Downloads](https://static.pepy.tech/badge/django-ninja-extra)](https://pepy.tech/project/django-ninja-extra)
 
 # Django Ninja Extra
 
 The **Django Ninja Extra** package offers a convenient, **class-based** approach to quickly building and configuring high-performance APIs. 
 Utilizing the core features of [**Django Ninja**](https://django-ninja.rest-framework.com), it allows for speedy development without sacrificing performance."
 
 **Key features:**
```

### Comparing `django-ninja-extra-0.18.7/docs/api_controller/api_controller_permission.md` & `django-ninja-extra-0.18.8/docs/api_controller/api_controller_permission.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,26 +49,26 @@
     class ReadOnly(permissions.BasePermission):
         def has_permission(self, request, view):
             return request.method in permissions.SAFE_METHODS
     
     @api_controller(permissions=[permissions.IsAuthenticated | ReadOnly()])
     ...
     ```
-For example:
-```python
-from ninja_extra import permissions
-
-class UserWithPermission(permissions.BasePermission):
-    def __init__(self, permission: str) -> None:
-        self._permission = permission
-    
-    def has_permission(self, request, view):
-        return request.user.has_perm(self._permission)
+    For example:
+    ```python
+    from ninja_extra import permissions
     
-# in controller or route function
-permissions=[UserWithPermission('blog.add')]
-```
+    class UserWithPermission(permissions.BasePermission):
+        def __init__(self, permission: str) -> None:
+            self._permission = permission
+        
+        def has_permission(self, request, view):
+            return request.user.has_perm(self._permission)
+        
+    # in controller or route function
+    permissions=[UserWithPermission('blog.add')]
+    ```
 
 ## **Permissions Supported Operands**
 - & (and) eg: `permissions.IsAuthenticated & ReadOnly`
 - | (or) eg: `permissions.IsAuthenticated | ReadOnly`
-- ~ (not) eg: `!(permissions.IsAuthenticated & ReadOnly)`
+- ~ (not) eg: `~(permissions.IsAuthenticated & ReadOnly)`
```

### Comparing `django-ninja-extra-0.18.7/docs/api_controller/api_controller_route.md` & `django-ninja-extra-0.18.8/docs/api_controller/api_controller_route.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/api_controller/api_controller_router.md` & `django-ninja-extra-0.18.8/docs/api_controller/api_controller_router.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/api_controller/index.md` & `django-ninja-extra-0.18.8/docs/api_controller/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # **Controller**
-The term 'APIController' is borrowed from the C# ASP.NET environment, which uses the MVC framework. Although Django is not an MVC framework, it is still possible to mimic the concept by using similar patterns and principles.
-Django-Ninja-Extra's APIController is modeled after the C# ASP.NET ApiController, providing an object-oriented approach to creating controller models and implementing modern software design patterns in your Django project. This allows you to use similar concepts and design patterns as in C# ASP.NET environment in your Django project.
+Ninja-Extra APIController is responsible for handling incoming requests and returning responses to the client.
 
-### Why APIController in Django.
+In Ninja-Extra, there are major components to creating a controller model
 
-Coming from a background of modeling objects using class-based approaches, and having experience working with various API tools such as DRF, FastAPI, and Flask-Restful, you have likely noticed that these libraries primarily use function-based or class-tailored function-based approaches in writing route functions. This approach may not fully utilize the concepts of object-oriented programming when designing RESTful APIs. But despite this, these libraries are still great.
-
-I have designed the APIController in Django Ninja Extra to bring a more traditional controller-based approach to Django Ninja, providing more flexibility and adaptability to recent software design patterns. 
-If you prefer using class-based controls for building APIs, Django Ninja Extra's APIController is a great option for you.
+- ControllerBase
+- APIController Decorator
 
 ## ControllerBase
 
 The `ControllerBase` class is the base class for all controllers in Django Ninja Extra. 
 It provides the core functionality for handling requests, validating input, and returning responses in a class-based approach.
 
 The class includes properties and methods that are common to all controllers, such as the `request` object, `permission_classes`, and `response` object which are part of the `RouteContext`. 
@@ -28,15 +25,14 @@
 from ninja_extra import ControllerBase, api_controller
 
 @api_controller('/users')
 class UserControllerBase(ControllerBase):
     ...
 ```
 
-
 ## APIController Decorator
 The `api_controller` decorator is used to define a class-based controller in Django Ninja Extra. 
 It is applied to a ControllerBase class and takes several arguments to configure the routes and functionality of the controller.
 
 The first argument, `prefix_or_class`, is either a prefix string for grouping all routes registered under the controller or the class object that the decorator is applied on.
 
 The second argument, `auth`, is a list of all Django Ninja Auth classes that should be applied to the controller's routes.
```

### Comparing `django-ninja-extra-0.18.7/docs/images/benchmark.png` & `django-ninja-extra-0.18.8/docs/images/benchmark.png`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/images/custom_exception.gif` & `django-ninja-extra-0.18.8/docs/images/custom_exception.gif`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/images/pagination_example.gif` & `django-ninja-extra-0.18.8/docs/images/pagination_example.gif`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/images/ui_swagger_preview_readme.gif` & `django-ninja-extra-0.18.8/docs/images/ui_swagger_preview_readme.gif`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/index.md` & `django-ninja-extra-0.18.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/route_context.md` & `django-ninja-extra-0.18.8/docs/route_context.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/service_module_injector.md` & `django-ninja-extra-0.18.8/docs/service_module_injector.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/tutorial/body_request.md` & `django-ninja-extra-0.18.8/docs/tutorial/body_request.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/tutorial/custom_exception.md` & `django-ninja-extra-0.18.8/docs/tutorial/custom_exception.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/tutorial/form.md` & `django-ninja-extra-0.18.8/docs/tutorial/form.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/tutorial/index.md` & `django-ninja-extra-0.18.8/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/tutorial/pagination.md` & `django-ninja-extra-0.18.8/docs/tutorial/pagination.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/tutorial/path.md` & `django-ninja-extra-0.18.8/docs/tutorial/path.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/tutorial/query.md` & `django-ninja-extra-0.18.8/docs/tutorial/query.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/tutorial/schema.md` & `django-ninja-extra-0.18.8/docs/tutorial/schema.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/tutorial/testing.md` & `django-ninja-extra-0.18.8/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/tutorial/throttling.md` & `django-ninja-extra-0.18.8/docs/tutorial/throttling.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/docs/tutorial/versioning.md` & `django-ninja-extra-0.18.8/docs/tutorial/versioning.md`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/mkdocs.yml` & `django-ninja-extra-0.18.8/mkdocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 site_name: Django Ninja Extra
 site_description: Django Ninja Extra - Adds more power to Django Ninja RESTful api library
 site_url: https://eadwincode.github.io/django-ninja-extra/
 repo_name: eadwinCode/django-ninja
 repo_url: https://github.com/eadwinCode/django-ninja-extra
-edit_uri: ''
+edit_uri: blob/master/docs
 
 theme:
   name: material
   palette:
     - media: "(prefers-color-scheme: light)"
       scheme: default
       primary: deeppurple
@@ -42,14 +42,17 @@
   - Authentication: tutorial/authentication.md
   - Path Parameter: tutorial/path.md
   - Query Request: tutorial/query.md
   - Body Request: tutorial/body_request.md
   - Form Request: tutorial/form.md
   - Schema: tutorial/schema.md
   - Pagination: tutorial/pagination.md
+  - Filtering:
+    - Ordering: tutorial/ordering.md
+    - Searching: tutorial/searching.md
   - Error Handling: tutorial/custom_exception.md
   - Versioning: tutorial/versioning.md
   - Throttling: tutorial/throttling.md
   - Testing: tutorial/testing.md
 - RouteContext: route_context.md
 - Settings: settings.md
 - Dependency Injection: service_module_injector.md
```

### Comparing `django-ninja-extra-0.18.7/ninja_extra/__init__.py` & `django-ninja-extra-0.18.8/ninja_extra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Django Ninja Extra - Class Based Utility and more for Django Ninja(Fast Django REST framework)"""
 
-__version__ = "0.18.7"
+__version__ = "0.18.8"
 
 import django
 
 from ninja_extra.controllers import (
     ControllerBase,
     api_controller,
     http_delete,
```

### Comparing `django-ninja-extra-0.18.7/ninja_extra/apps.py` & `django-ninja-extra-0.18.8/ninja_extra/apps.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/conf/settings.py` & `django-ninja-extra-0.18.8/ninja_extra/conf/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     INJECTOR_MODULES=[],
     PAGINATION_CLASS="ninja_extra.pagination.LimitOffsetPagination",
     THROTTLE_CLASSES=[
         "ninja_extra.throttling.AnonRateThrottle",
         "ninja_extra.throttling.UserRateThrottle",
     ],
     THROTTLE_RATES={"user": None, "anon": None},
+    ORDERING_CLASS="ninja_extra.ordering.Ordering",
+    SEARCHING_CLASS="ninja_extra.searching.Searching",
 )
 
 USER_SETTINGS = UserDefinedSettingsMapper(
     getattr(django_settings, "NINJA_EXTRA", NinjaExtra_SETTINGS_DEFAULTS)
 )
 
 
@@ -39,14 +41,20 @@
     PAGINATION_PER_PAGE: int = Field(100)
     THROTTLE_RATES: Dict[str, Optional[str]] = Field(
         {"user": "1000/day", "anon": "100/day"}
     )
     THROTTLE_CLASSES: List[Any] = []
     NUM_PROXIES: Optional[int] = None
     INJECTOR_MODULES: List[Any] = []
+    ORDERING_CLASS: Any = Field(
+        "ninja_extra.ordering.Ordering",
+    )
+    SEARCHING_CLASS: Any = Field(
+        "ninja_extra.searching.Searching",
+    )
 
     @validator("INJECTOR_MODULES", pre=True)
     def pre_injector_module_validate(cls, value: Any) -> Any:
         if not isinstance(value, list):
             raise ValueError("Invalid data type")
         return value
 
@@ -58,14 +66,26 @@
 
     @validator("PAGINATION_CLASS", pre=True)
     def pre_pagination_class_validate(cls, value: Any) -> Any:
         if isinstance(value, list):
             raise ValueError("Invalid data type")
         return value
 
+    @validator("ORDERING_CLASS", pre=True)
+    def pre_ordering_class_validate(cls, value: Any) -> Any:
+        if isinstance(value, list):
+            raise ValueError("Invalid data type")
+        return value
+
+    @validator("SEARCHING_CLASS", pre=True)
+    def pre_searching_class_validate(cls, value: Any) -> Any:
+        if isinstance(value, list):
+            raise ValueError("Invalid data type")
+        return value
+
     @root_validator
     def validate_ninja_extra_settings(cls, values: Any) -> Any:
         for item in NinjaExtra_SETTINGS_DEFAULTS.keys():
             if (
                 isinstance(values[item], (tuple, list))
                 and values[item]
                 and isinstance(values[item][0], str)
```

### Comparing `django-ninja-extra-0.18.7/ninja_extra/controllers/__init__.py` & `django-ninja-extra-0.18.8/ninja_extra/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/controllers/base.py` & `django-ninja-extra-0.18.8/ninja_extra/controllers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from injector import inject, is_decorated_with_inject
 from ninja import NinjaAPI, Router
 from ninja.constants import NOT_SET
 from ninja.security.base import AuthBase
 from ninja.signature import is_async
 from ninja.utils import normalize_path
 
-from ninja_extra.constants import THROTTLED_FUNCTION
+from ninja_extra.constants import ROUTE_FUNCTION, THROTTLED_FUNCTION
 from ninja_extra.exceptions import APIException, NotFound, PermissionDenied, bad_request
 from ninja_extra.helper import get_function_name
 from ninja_extra.operation import ControllerPathView, Operation
 from ninja_extra.permissions import AllowAny, BasePermission
 from ninja_extra.permissions.base import OperationHolderMixin
 from ninja_extra.shortcuts import (
     fail_silently,
@@ -55,21 +55,21 @@
 
 class MissingAPIControllerDecoratorException(Exception):
     pass
 
 
 def get_route_functions(cls: Type) -> Iterable[RouteFunction]:
     for method in cls.__dict__.values():
-        if isinstance(method, RouteFunction):
-            yield method
+        if hasattr(method, ROUTE_FUNCTION):
+            yield getattr(method, ROUTE_FUNCTION)
 
 
 def get_all_controller_route_function(
     controller: Union[Type["ControllerBase"], Type]
-) -> List[RouteFunction]:
+) -> List[RouteFunction]:  # pragma: no cover
     route_functions: List[RouteFunction] = []
     for item in dir(controller):
         attr = getattr(controller, item)
         if isinstance(attr, RouteFunction):
             route_functions.append(attr)
     return route_functions
 
@@ -313,15 +313,15 @@
     @tags.setter
     def tags(self, value: Union[str, List[str], None]) -> None:
         tag: Optional[List[str]] = cast(Optional[List[str]], value)
         if tag and isinstance(value, str):
             tag = [value]
         self._tags = tag
 
-    def __call__(self, cls: Type) -> Type["ControllerBase"]:
+    def __call__(self, cls: Type) -> Union[Type, Type["ControllerBase"]]:
         from ninja_extra.throttling import throttle
 
         self.auto_import = getattr(cls, "auto_import", self.auto_import)
         if not issubclass(cls, ControllerBase):
             # We force the cls to inherit from `ControllerBase` by creating another type.
             cls = type(cls.__name__, (ControllerBase, cls), {"_api_controller": self})
         else:
@@ -464,46 +464,50 @@
             include_in_schema=include_in_schema,
             openapi_extra=openapi_extra,
         )
         return operation
 
 
 @overload
-def api_controller(prefix_or_class: Type) -> Type[ControllerBase]:  # pragma: no cover
+def api_controller(
+    prefix_or_class: Type,
+) -> Union[Type[ControllerBase], Callable[..., Any], Any]:  # pragma: no cover
     ...
 
 
 @overload
 def api_controller(
     prefix_or_class: str = "",
     auth: Any = NOT_SET,
     tags: Union[Optional[List[str]], str] = None,
     permissions: Optional["PermissionType"] = None,
     auto_import: bool = True,
-) -> APIController:  # pragma: no cover
+) -> Union[Type[ControllerBase], Callable[..., Any], Any]:  # pragma: no cover
     ...
 
 
 def api_controller(
     prefix_or_class: Union[str, Type] = "",
     auth: Any = NOT_SET,
     tags: Union[Optional[List[str]], str] = None,
     permissions: Optional["PermissionType"] = None,
     auto_import: bool = True,
-) -> Union[Type[ControllerBase], APIController]:
+) -> Union[Type[ControllerBase], Callable[..., Any], Any]:
     if isinstance(prefix_or_class, type):
-        _api_controller = APIController(
+        return APIController(
             prefix="",
             auth=auth,
             tags=tags,
             permissions=permissions,
             auto_import=auto_import,
-        )
-        return _api_controller(prefix_or_class)
+        )(prefix_or_class)
+
+    def _decorator(cls: Type) -> Union[Type[ControllerBase], Any]:
+        return APIController(
+            prefix=str(prefix_or_class),
+            auth=auth,
+            tags=tags,
+            permissions=permissions,
+            auto_import=auto_import,
+        )(cls)
 
-    return APIController(
-        prefix=prefix_or_class,
-        auth=auth,
-        tags=tags,
-        permissions=permissions,
-        auto_import=auto_import,
-    )
+    return _decorator
```

### Comparing `django-ninja-extra-0.18.7/ninja_extra/controllers/registry.py` & `django-ninja-extra-0.18.8/ninja_extra/controllers/registry.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/controllers/response.py` & `django-ninja-extra-0.18.8/ninja_extra/controllers/response.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/controllers/route/__init__.py` & `django-ninja-extra-0.18.8/ninja_extra/controllers/route/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,23 @@
     get_type_hints,
 )
 
 from ninja.constants import NOT_SET
 from ninja.signature import is_async
 from ninja.types import TCallable
 
-from ninja_extra.constants import DELETE, GET, PATCH, POST, PUT, ROUTE_METHODS
+from ninja_extra.constants import (
+    DELETE,
+    GET,
+    PATCH,
+    POST,
+    PUT,
+    ROUTE_FUNCTION,
+    ROUTE_METHODS,
+)
 from ninja_extra.controllers.response import ControllerResponse, ControllerResponseMeta
 from ninja_extra.permissions import BasePermission
 from ninja_extra.schemas import RouteParameter
 
 from .route_functions import AsyncRouteFunction, RouteFunction
 
 
@@ -137,15 +145,15 @@
         exclude_none: bool = False,
         url_name: Optional[str] = None,
         include_in_schema: bool = True,
         permissions: Optional[
             List[Union[Type[BasePermission], BasePermission, Any]]
         ] = None,
         openapi_extra: Optional[Dict[str, Any]] = None,
-    ) -> RouteFunction:
+    ) -> TCallable:
         if response is NOT_SET:
             response = get_type_hints(view_func).get("return") or NOT_SET
         route_obj = cls(
             view_func,
             path=path,
             methods=methods,
             auth=auth,
@@ -164,15 +172,16 @@
             permissions=permissions,
             openapi_extra=openapi_extra,
         )
         route_function_class = RouteFunction
         if route_obj.is_async:
             route_function_class = AsyncRouteFunction
 
-        return route_function_class(route=route_obj)
+        setattr(view_func, ROUTE_FUNCTION, route_function_class(route=route_obj))
+        return view_func
 
     @classmethod
     def get(
         cls,
         path: str = "",
         *,
         auth: Any = NOT_SET,
@@ -188,15 +197,15 @@
         exclude_none: bool = False,
         url_name: Optional[str] = None,
         include_in_schema: bool = True,
         permissions: Optional[
             List[Union[Type[BasePermission], BasePermission, Any]]
         ] = None,
         openapi_extra: Optional[Dict[str, Any]] = None,
-    ) -> Callable[[TCallable], RouteFunction]:
+    ) -> Callable[[TCallable], TCallable]:
         """
         A GET Operation method decorator
          eg.
 
         ```python
         @http_get()
         def get_operation(self):
@@ -216,15 +225,15 @@
         :param exclude_none: pydantic schema filters applied to `response` schema object. default: `False`
         :param url_name: a name to an endpoint which can be resolved using `reverse` function in django. default: `None`
         :param include_in_schema: indicates whether an endpoint should appear on the swagger documentation
         :param permissions: collection permission classes. default: `None`
         :return: Route[GET]
         """
 
-        def decorator(view_func: TCallable) -> RouteFunction:
+        def decorator(view_func: TCallable) -> TCallable:
             return cls._create_route_function(
                 view_func,
                 path=path,
                 methods=[GET],
                 auth=auth,
                 response=response,
                 operation_id=operation_id,
@@ -262,15 +271,15 @@
         exclude_none: bool = False,
         url_name: Optional[str] = None,
         include_in_schema: bool = True,
         permissions: Optional[
             List[Union[Type[BasePermission], BasePermission, Any]]
         ] = None,
         openapi_extra: Optional[Dict[str, Any]] = None,
-    ) -> Callable[[TCallable], RouteFunction]:
+    ) -> Callable[[TCallable], TCallable]:
         """
         A POST Operation method decorator
         eg.
 
         ```python
          @http_post()
          def post_operation(self,  create_schema: Schema):
@@ -290,15 +299,15 @@
         :param exclude_none: pydantic schema filters applied to `response` schema object. default: `False`
         :param url_name: a name to an endpoint which can be resolved using `reverse` function in django. default: `None`
         :param include_in_schema: indicates whether an endpoint should appear on the swagger documentation
         :param permissions: collection permission classes. default: `None`
         :return: Route[POST]
         """
 
-        def decorator(view_func: TCallable) -> RouteFunction:
+        def decorator(view_func: TCallable) -> TCallable:
             return cls._create_route_function(
                 view_func,
                 path=path,
                 methods=[POST],
                 auth=auth,
                 response=response,
                 operation_id=operation_id,
@@ -336,15 +345,15 @@
         exclude_none: bool = False,
         url_name: Optional[str] = None,
         include_in_schema: bool = True,
         permissions: Optional[
             List[Union[Type[BasePermission], BasePermission, Any]]
         ] = None,
         openapi_extra: Optional[Dict[str, Any]] = None,
-    ) -> Callable[[TCallable], RouteFunction]:
+    ) -> Callable[[TCallable], TCallable]:
         """
         A DELETE Operation method decorator
         eg.
 
         ```python
         @http_delete('/{int:some_id}')
         def delete_operation(self, some_id: int):
@@ -364,15 +373,15 @@
         :param exclude_none: pydantic schema filters applied to `response` schema object. default: `False`
         :param url_name: a name to an endpoint which can be resolved using `reverse` function in django. default: `None`
         :param include_in_schema: indicates whether an endpoint should appear on the swagger documentation
         :param permissions: collection permission classes. default: `None`
         :return: Route[DELETE]
         """
 
-        def decorator(view_func: TCallable) -> RouteFunction:
+        def decorator(view_func: TCallable) -> TCallable:
             return cls._create_route_function(
                 view_func,
                 path=path,
                 methods=[DELETE],
                 auth=auth,
                 response=response,
                 operation_id=operation_id,
@@ -410,15 +419,15 @@
         exclude_none: bool = False,
         url_name: Optional[str] = None,
         include_in_schema: bool = True,
         permissions: Optional[
             List[Union[Type[BasePermission], BasePermission, Any]]
         ] = None,
         openapi_extra: Optional[Dict[str, Any]] = None,
-    ) -> Callable[[TCallable], RouteFunction]:
+    ) -> Callable[[TCallable], TCallable]:
         """
         A PATCH Operation method decorator
         eg.
 
         ```python
 
         @http_patch('/{int:some_id}')
@@ -439,15 +448,15 @@
         :param exclude_none: pydantic schema filters applied to `response` schema object. default: `False`
         :param url_name: a name to an endpoint which can be resolved using `reverse` function in django. default: `None`
         :param include_in_schema: indicates whether an endpoint should appear on the swagger documentation
         :param permissions: collection permission classes. default: `None`
         :return: Route[PATCH]
         """
 
-        def decorator(view_func: TCallable) -> RouteFunction:
+        def decorator(view_func: TCallable) -> TCallable:
             return cls._create_route_function(
                 view_func,
                 path=path,
                 methods=[PATCH],
                 auth=auth,
                 response=response,
                 operation_id=operation_id,
@@ -485,15 +494,15 @@
         exclude_none: bool = False,
         url_name: Optional[str] = None,
         include_in_schema: bool = True,
         permissions: Optional[
             List[Union[Type[BasePermission], BasePermission, Any]]
         ] = None,
         openapi_extra: Optional[Dict[str, Any]] = None,
-    ) -> Callable[[TCallable], RouteFunction]:
+    ) -> Callable[[TCallable], TCallable]:
         """
          A PUT Operation method decorator
         eg.
 
         ```python
 
         @http_put('/{int:some_id}')
@@ -514,15 +523,15 @@
          :param exclude_none: pydantic schema filters applied to `response` schema object. default: `False`
          :param url_name: a name to an endpoint which can be resolved using `reverse` function in django. default: `None`
          :param include_in_schema: indicates whether an endpoint should appear on the swagger documentation
          :param permissions: collection permission classes. default: `None`
          :return: Route[PUT]
         """
 
-        def decorator(view_func: TCallable) -> RouteFunction:
+        def decorator(view_func: TCallable) -> TCallable:
             return cls._create_route_function(
                 view_func,
                 path=path,
                 methods=[PUT],
                 auth=auth,
                 response=response,
                 operation_id=operation_id,
@@ -561,15 +570,15 @@
         exclude_none: bool = False,
         url_name: Optional[str] = None,
         include_in_schema: bool = True,
         permissions: Optional[
             List[Union[Type[BasePermission], BasePermission, Any]]
         ] = None,
         openapi_extra: Optional[Dict[str, Any]] = None,
-    ) -> Callable[[TCallable], RouteFunction]:
+    ) -> Callable[[TCallable], TCallable]:
         """
         A Custom Operation method decorator, for creating route with more than one operation
         eg.
 
         ```python
 
         @http_generic('', methods=['POST', 'GET'])
@@ -591,15 +600,15 @@
         :param exclude_none: pydantic schema filters applied to `response` schema object. default: `False`
         :param url_name: a name to an endpoint which can be resolved using `reverse` function in django. default: `None`
         :param include_in_schema: indicates whether an endpoint should appear on the swagger documentation
         :param permissions: collection permission classes. default: `None`
         :return: Route[PATCH]
         """
 
-        def decorator(view_func: TCallable) -> RouteFunction:
+        def decorator(view_func: TCallable) -> TCallable:
             return cls._create_route_function(
                 view_func,
                 path=path,
                 methods=methods,
                 auth=auth,
                 response=response,
                 operation_id=operation_id,
```

### Comparing `django-ninja-extra-0.18.7/ninja_extra/controllers/route/context.py` & `django-ninja-extra-0.18.8/ninja_extra/controllers/route/context.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/controllers/route/route_functions.py` & `django-ninja-extra-0.18.8/ninja_extra/controllers/route/route_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.http import HttpRequest, HttpResponse
 
 from ninja_extra.controllers.response import ControllerResponse
 
 from ...dependency_resolver import get_injector, service_resolver
 from .context import RouteContext, get_route_execution_context
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from ninja_extra.operation import ControllerOperation
 
     from ...controllers.base import APIController, ControllerBase
     from ...controllers.route import Route
 
 
 class RouteFunctionContext:
```

### Comparing `django-ninja-extra-0.18.7/ninja_extra/dependency_resolver.py` & `django-ninja-extra-0.18.8/ninja_extra/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/details.py` & `django-ninja-extra-0.18.8/ninja_extra/details.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/exceptions.py` & `django-ninja-extra-0.18.8/ninja_extra/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/generic.py` & `django-ninja-extra-0.18.8/ninja_extra/generic.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/lazy.py` & `django-ninja-extra-0.18.8/ninja_extra/lazy.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/main.py` & `django-ninja-extra-0.18.8/ninja_extra/main.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/modules.py` & `django-ninja-extra-0.18.8/ninja_extra/modules.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/operation.py` & `django-ninja-extra-0.18.8/ninja_extra/operation.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/pagination.py` & `django-ninja-extra-0.18.8/ninja_extra/pagination.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 import inspect
 import logging
 from collections import OrderedDict
 from functools import wraps
-from typing import TYPE_CHECKING, Any, Callable, Optional, Type, Union, cast, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+    cast,
+    overload,
+)
 
 from asgiref.sync import sync_to_async
 from django.core.paginator import InvalidPage, Page, Paginator
 from django.db.models import QuerySet
 from django.http import HttpRequest
 from ninja import Schema
 from ninja.constants import NOT_SET
@@ -176,27 +187,31 @@
         paginator_kwargs_name: str = "pagination",
     ) -> None:
         self.paginator = paginator
         self.paginator_kwargs_name = paginator_kwargs_name
         self.view_func = view_func
 
         paginator_view = self.get_view_function()
+        _ninja_contribute_args: List[Tuple] = getattr(
+            self.view_func, "_ninja_contribute_args", []
+        )
+        setattr(paginator_view, "_ninja_contribute_args", _ninja_contribute_args)
         add_ninja_contribute_args(
             paginator_view,
             (
                 self.paginator_kwargs_name,
                 self.paginator.Input,
                 self.paginator.InputSource,
             ),
         )
         setattr(paginator_view, "paginator_operation", self)
         self.as_view = wraps(view_func)(paginator_view)
 
     @property
-    def view_func_has_kwargs(self) -> bool:
+    def view_func_has_kwargs(self) -> bool:  # pragma: no cover
         return self.paginator.pass_parameter is not None
 
     def get_view_function(self) -> Callable:
         def as_view(controller: "ControllerBase", *args: Any, **kw: Any) -> Any:
             func_kwargs = dict(**kw)
             pagination_params = func_kwargs.pop(self.paginator_kwargs_name)
             if self.paginator.pass_parameter:
```

### Comparing `django-ninja-extra-0.18.7/ninja_extra/permissions/base.py` & `django-ninja-extra-0.18.8/ninja_extra/permissions/base.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/permissions/common.py` & `django-ninja-extra-0.18.8/ninja_extra/permissions/common.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/router.py` & `django-ninja-extra-0.18.8/ninja_extra/router.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/schemas/response.py` & `django-ninja-extra-0.18.8/ninja_extra/schemas/response.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/security/__init__.py` & `django-ninja-extra-0.18.8/ninja_extra/security/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/security/api_key.py` & `django-ninja-extra-0.18.8/ninja_extra/security/api_key.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/security/http.py` & `django-ninja-extra-0.18.8/ninja_extra/security/http.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/security/session.py` & `django-ninja-extra-0.18.8/ninja_extra/security/session.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/shortcuts.py` & `django-ninja-extra-0.18.8/ninja_extra/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/status.py` & `django-ninja-extra-0.18.8/ninja_extra/status.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/testing/client.py` & `django-ninja-extra-0.18.8/ninja_extra/testing/client.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/throttling/decorator.py` & `django-ninja-extra-0.18.8/ninja_extra/throttling/decorator.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/throttling/model.py` & `django-ninja-extra-0.18.8/ninja_extra/throttling/model.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/ninja_extra/urls.py` & `django-ninja-extra-0.18.8/ninja_extra/urls.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/pyproject.toml` & `django-ninja-extra-0.18.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/conftest.py` & `django-ninja-extra-0.18.8/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import django
 
 
 def pytest_configure(config):
     from django.conf import settings
 
     os.environ.setdefault("NINJA_SKIP_REGISTRY", "True")
+
     settings.configure(
         ALLOWED_HOSTS=["*"],
         DEBUG_PROPAGATE_EXCEPTIONS=True,
         DATABASES={
             "default": {"ENGINE": "django.db.backends.sqlite3", "NAME": ":memory:"}
         },
         SITE_ID=1,
```

### Comparing `django-ninja-extra-0.18.7/tests/controllers.py` & `django-ninja-extra-0.18.8/tests/controllers.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_api_instance.py` & `django-ninja-extra-0.18.8/tests/test_api_instance.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_async_auth.py` & `django-ninja-extra-0.18.8/tests/test_async_auth.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_controller.py` & `django-ninja-extra-0.18.8/tests/test_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,21 @@
     api_controller,
     exceptions,
     http_get,
     http_post,
     testing,
 )
 from ninja_extra.controllers import ControllerBase, RouteContext, RouteFunction
-from ninja_extra.controllers.base import APIController, get_route_functions
+from ninja_extra.controllers.base import (
+    APIController,
+    MissingAPIControllerDecoratorException,
+    get_route_functions,
+)
 from ninja_extra.controllers.response import Detail, Id, Ok
+from ninja_extra.helper import get_route_function
 from ninja_extra.permissions.common import AllowAny
 
 from .schemas import UserSchema
 from .utils import AsyncFakeAuth, FakeAuth
 
 
 @api_controller
@@ -72,31 +77,40 @@
 @api_controller("", tags=["new tag"])
 class DisableAutoImportController:
     auto_import = False  # disable auto_import of the controller
 
 
 class TestAPIController:
     def test_api_controller_as_decorator(self):
-        api_controller_instance = api_controller(
-            "prefix", tags="new_tag", auth=FakeAuth()
+        controller_type = api_controller("prefix", tags="new_tag", auth=FakeAuth())(
+            type("Any", (), {})
         )
+        api_controller_instance = controller_type.get_api_controller()
 
         assert not api_controller_instance.has_auth_async
         assert not api_controller_instance._prefix_has_route_param
         assert api_controller_instance.prefix == "prefix"
         assert api_controller_instance.tags == ["new_tag"]
         assert api_controller_instance.permission_classes == [AllowAny]
 
-        api_controller_instance = api_controller()
+        controller_type = api_controller()(controller_type)
+        api_controller_instance = controller_type.get_api_controller()
         assert api_controller_instance.prefix == ""
-        assert api_controller_instance.tags is None
+        assert api_controller_instance.tags == ["any"]
         assert "abc" in SomeController.__module__
         assert "tests.test_controller" in Some2Controller.__module__
         assert Some2Controller.get_api_controller()
 
+    def test_controller_get_api_controller_raise_exception(self):
+        class BController(ControllerBase):
+            pass
+
+        with pytest.raises(MissingAPIControllerDecoratorException):
+            BController.get_api_controller()
+
     def test_api_controller_prefix_with_parameter(self):
         @api_controller("/{int:organisation_id}")
         class UsersController:
             @http_get("")
             def example_with_id_response(self, organisation_id: int):
                 return dict(organisation_id=organisation_id)
 
@@ -126,40 +140,40 @@
         assert not hasattr(SomeController.__init__, "__bindings__")
         assert hasattr(SomeControllerWithInject.__init__, "__bindings__")
 
     def test_controller_should_have_path_operation_list(self):
         _api_controller = SomeControllerWithRoute.get_api_controller()
         assert len(_api_controller._path_operations) == 7
 
-        route_function: RouteFunction = SomeControllerWithRoute.example
+        route_function: RouteFunction = get_route_function(
+            SomeControllerWithRoute().example
+        )
         path_view = _api_controller._path_operations.get(str(route_function))
         assert path_view, "route doesn't exist in controller"
         assert len(path_view.operations) == 1
 
         operation = path_view.operations[0]
         assert operation.methods == route_function.route.route_params.methods
         assert operation.operation_id == route_function.route.route_params.operation_id
 
     def test_get_route_function_should_return_instance_route_definitions(self):
         for route_definition in get_route_functions(SomeControllerWithRoute):
             assert isinstance(route_definition, RouteFunction)
 
     def test_compute_api_route_function_works(self):
-        _api_controller = api_controller()
-
+        @api_controller()
         class AnyClassTypeWithRoute:
             @http_get("/example")
             def example(self):
                 pass
 
-        _api_controller(AnyClassTypeWithRoute)
-        assert len(_api_controller.path_operations) == 1
-        path_view = _api_controller.path_operations.get(
-            str(AnyClassTypeWithRoute.example)
-        )
+        api_controller_instance = AnyClassTypeWithRoute.get_api_controller()
+        assert len(api_controller_instance.path_operations) == 1
+        route_function = get_route_function(AnyClassTypeWithRoute().example)
+        path_view = api_controller_instance.path_operations.get(str(route_function))
         assert path_view
 
     @pytest.mark.django_db
     def test_controller_base_get_object_or_exception_works(self):
         group_instance = Group.objects.create(name="_groupowner")
 
         controller_object = SomeController()
@@ -203,37 +217,40 @@
             with patch.object(AllowAny, "has_object_permission", return_value=False):
                 controller_object.get_object_or_none(Group, id=group_instance.id)
                 assert isinstance(ex, exceptions.PermissionDenied)
 
 
 @pytest.mark.skipif(django.VERSION < (3, 1), reason="requires django 3.1 or higher")
 def test_async_controller():
-    api_controller_instance = api_controller(
+    api_controller_decorator = api_controller(
         "prefix", tags="any_Tag", auth=AsyncFakeAuth()
     )
-    assert api_controller_instance.has_auth_async
 
     with pytest.raises(Exception) as ex:
 
-        @api_controller_instance
+        @api_controller_decorator
         class NonAsyncRouteInControllerWithAsyncAuth:
             @http_get("/example")
             def example(self):
                 pass
 
     assert "NonAsyncRouteInControllerWithAsyncAuth" in str(ex) and "example" in str(ex)
 
-    @api_controller_instance
+    @api_controller_decorator
     class AsyncRouteInControllerWithAsyncAuth:
         @http_get("/example")
         async def example(self):
             pass
 
+    example_route_function = get_route_function(
+        AsyncRouteInControllerWithAsyncAuth().example
+    )
+    assert AsyncRouteInControllerWithAsyncAuth.get_api_controller().has_auth_async
     assert isinstance(
-        AsyncRouteInControllerWithAsyncAuth.example.operation.auth_callbacks[0],
+        example_route_function.operation.auth_callbacks[0],
         AsyncFakeAuth,
     )
 
 
 class TestAPIControllerResponse:
     ok_response = Ok("OK")
     id_response = Id("ID")
@@ -287,37 +304,40 @@
         assert response.status_code == 201
         assert (
             str(Id[uuid.UUID](_uuid_value).convert_to_schema().dict()["id"])
             == response.json()["id"]
         )
 
         ok_response = Ok[UserSchema](dict(name="John", age=56))
-        result = SomeControllerWithRoute.example_with_ok_schema_response(
-            request=Mock(), user=UserSchema(name="John", age=56)
+        route_function = get_route_function(
+            SomeControllerWithRoute().example_with_ok_schema_response
         )
+        result = route_function(request=Mock(), user=UserSchema(name="John", age=56))
         assert isinstance(result, tuple)
         assert result[1] == ok_response.convert_to_schema()
         assert result[0] == ok_response.status_code
 
     def test_controller_response_in_route_functions_works(self):
         detail = Detail("5242", status_code=302)
         client = testing.TestClient(SomeControllerWithRoute)
         response = client.get("/example/5242")
 
         assert response.status_code == 302
         assert detail.convert_to_schema().dict() == response.json()
 
         ok_response = Ok("5242")
-        result = SomeControllerWithRoute.example_with_ok_response(
-            request=Mock(), ex_id="5242"
+        route_function = get_route_function(
+            SomeControllerWithRoute().example_with_ok_response
         )
+        result = route_function(request=Mock(), ex_id="5242")
         assert isinstance(result, tuple)
         assert result[1] == ok_response.convert_to_schema()
         assert result[0] == ok_response.status_code
 
         id_response = Id("5242")
-        result = SomeControllerWithRoute.example_with_id_response(
-            request=Mock(), ex_id="5242"
+        route_function = get_route_function(
+            SomeControllerWithRoute().example_with_id_response
         )
+        result = route_function(request=Mock(), ex_id="5242")
         assert isinstance(result, tuple)
         assert result[1] == id_response.convert_to_schema()
         assert result[0] == id_response.status_code
```

### Comparing `django-ninja-extra-0.18.7/tests/test_controller_registry.py` & `django-ninja-extra-0.18.8/tests/test_controller_registry.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_controller_response.py` & `django-ninja-extra-0.18.8/tests/test_controller_response.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_dependency_resolver.py` & `django-ninja-extra-0.18.8/tests/test_dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_django_model.py` & `django-ninja-extra-0.18.8/tests/test_django_model.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_django_ninja_router.py` & `django-ninja-extra-0.18.8/tests/test_django_ninja_router.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_event_controller.py` & `django-ninja-extra-0.18.8/tests/test_event_controller.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_exceptions.py` & `django-ninja-extra-0.18.8/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_generic_patch.py` & `django-ninja-extra-0.18.8/tests/test_generic_patch.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_operation.py` & `django-ninja-extra-0.18.8/tests/test_operation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import django
 import pytest
 
 from ninja_extra import api_controller, route
 from ninja_extra.controllers import AsyncRouteFunction, RouteFunction
+from ninja_extra.helper import get_route_function
 from ninja_extra.operation import AsyncOperation, Operation
 from ninja_extra.testing import TestAsyncClient, TestClient
 
 from .utils import AsyncFakeAuth, FakeAuth, mock_log_call, mock_signal_call
 
 
 class TestOperation:
@@ -21,56 +22,63 @@
             raise Exception()
 
     @mock_signal_call("route_context_started")
     @mock_signal_call("route_context_finished")
     @mock_log_call("info")
     def test_route_operation_execution_works(self):
         client = TestClient(self.SomeTestController)
-        response = client.get(str(self.SomeTestController.example))
+        response = client.get("/example")
         assert response.json() == {"message": "example"}
 
     @mock_signal_call("route_context_started")
     @mock_signal_call("route_context_finished")
     @mock_log_call("error")
     def test_route_operation_execution_should_log_execution(self):
         client = TestClient(self.SomeTestController)
         with pytest.raises(Exception):
-            client.get(str(self.SomeTestController.example_exception))
+            client.get("/example_exception")
 
 
 @pytest.mark.skipif(django.VERSION < (3, 1), reason="requires django 3.1 or higher")
 def test_operation_auth_configs():
-    api_controller_instance = api_controller("prefix", tags="any_Tag")
+    @api_controller("prefix", tags="any_Tag")
+    class AController:
+        pass
+
+    api_controller_instance = AController.get_api_controller()
 
     async def async_endpoint(self, request):
         pass
 
     def sync_endpoint(self, request):
         pass
 
     sync_auth_http_get = route.get("/example", auth=[FakeAuth()])
     async_auth_http_get = route.get("/example/async", auth=[AsyncFakeAuth()])
 
-    route_function = sync_auth_http_get(async_endpoint)
-    assert isinstance(route_function, AsyncRouteFunction)
-    async_route_function = async_auth_http_get(async_endpoint)
+    sync_auth_http_get(async_endpoint)
+    async_route_function = get_route_function(async_endpoint)
+    assert isinstance(async_route_function, AsyncRouteFunction)
 
-    api_controller_instance._add_operation_from_route_function(route_function)
-    assert isinstance(route_function.operation, AsyncOperation)
+    api_controller_instance._add_operation_from_route_function(async_route_function)
+    assert isinstance(async_route_function.operation, AsyncOperation)
     api_controller_instance._add_operation_from_route_function(async_route_function)
     assert isinstance(async_route_function.operation, AsyncOperation)
 
-    sync_route_function = sync_auth_http_get(sync_endpoint)
+    sync_auth_http_get(sync_endpoint)
+    sync_route_function = get_route_function(sync_endpoint)
     api_controller_instance._add_operation_from_route_function(sync_route_function)
     assert isinstance(sync_route_function.operation, Operation)
     assert isinstance(sync_route_function, RouteFunction)
 
     with pytest.raises(Exception) as ex:
+        new_sync_endpoint = async_auth_http_get(sync_endpoint)
+        new_sync_route_function = get_route_function(new_sync_endpoint)
         api_controller_instance._add_operation_from_route_function(
-            async_auth_http_get(sync_endpoint)
+            new_sync_route_function
         )
     assert "sync_endpoint" in str(ex) and "AsyncFakeAuth" in str(ex)
 
 
 @pytest.mark.skipif(django.VERSION < (3, 1), reason="requires django 3.1 or higher")
 @pytest.mark.asyncio
 class TestAsyncOperations:
@@ -87,17 +95,17 @@
                 raise Exception()
 
         @mock_signal_call("route_context_started")
         @mock_signal_call("route_context_finished")
         @mock_log_call("info")
         async def test_async_route_operation_execution_works(self):
             client = TestAsyncClient(self.SomeTestController)
-            response = await client.get(str(self.SomeTestController.example))
+            response = await client.get("/example")
             assert response.json() == {"message": "example"}
 
         @mock_signal_call("route_context_started")
         @mock_signal_call("route_context_finished")
         @mock_log_call("error")
         async def test_async_route_operation_execution_should_log_execution(self):
             client = TestAsyncClient(self.SomeTestController)
             with pytest.raises(Exception):
-                await client.get(str(self.SomeTestController.example_exception))
+                await client.get("/example_exception")
```

### Comparing `django-ninja-extra-0.18.7/tests/test_pagination.py` & `django-ninja-extra-0.18.8/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_permissions.py` & `django-ninja-extra-0.18.8/tests/test_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,18 @@
         request = self.get_real_user_request()
         composed_perm = permissions.IsAuthenticated | permissions.AllowAny
         assert composed_perm().has_permission(request, None) is True
 
     def test_not_false(self):
         composed_perm = ~permissions.IsAuthenticated
         assert composed_perm().has_permission(anonymous_request, None) is True
+        assert (
+            composed_perm().has_object_permission(anonymous_request, None, None)
+            is False
+        )
 
     @pytest.mark.django_db
     def test_not_true(self):
         request = self.get_real_user_request()
         composed_perm = ~permissions.AllowAny
         assert composed_perm().has_permission(request, None) is False
```

### Comparing `django-ninja-extra-0.18.7/tests/test_route.py` & `django-ninja-extra-0.18.8/tests/test_route.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 )
 from ninja_extra.controllers.base import get_all_controller_route_function
 from ninja_extra.controllers.route.context import (
     RouteContext,
     get_route_execution_context,
 )
 from ninja_extra.exceptions import PermissionDenied
+from ninja_extra.helper import get_route_function
 from ninja_extra.permissions import AllowAny
 
 from .schemas import UserSchema
 from .utils import FakeAuth
 
 anonymous_request = Mock()
 anonymous_request.user = AnonymousUser()
@@ -110,27 +111,27 @@
             )
             assert len(operations) == 1
             if str(route_func) == "/example/operation-id":
                 assert operations[0].operation_id == "example_post_operation_id"
             assert route_func.route.route_params.methods == operations[0].methods
 
     def test_controller_route_should_right_view_func_type(self):
-        assert isinstance(SomeTestController.example, RouteFunction)
-        assert SomeTestController.example.as_view
-        assert hasattr(SomeTestController.example.as_view, "get_route_function")
-        assert (
-            SomeTestController.example.as_view.get_route_function()
-            == SomeTestController.example
-        )
+        controller = SomeTestController()
+        route_function = get_route_function(controller.example)
+        assert isinstance(route_function, RouteFunction)
+        assert route_function.as_view
+        assert hasattr(route_function.as_view, "get_route_function")
+        assert route_function.as_view.get_route_function() == route_function
 
     def test_controller_route_should_use_userschema_as_response(self):
-        route_function: RouteFunction = SomeTestController.example
+        controller = SomeTestController()
+        route_function = get_route_function(controller.example)
         assert route_function.route.route_params.response == NOT_SET
-        route_function: RouteFunction = (
-            SomeTestController.function_return_as_response_schema
+        route_function: RouteFunction = get_route_function(
+            controller.function_return_as_response_schema
         )
         assert route_function.route.route_params.response == UserSchema
 
     def test_route_generic_invalid_parameters(self):
         with pytest.raises(RouteInvalidParameterException) as ex:
 
             @route.generic("/example/list", methods=["SOMETHING", "GET"])
@@ -168,16 +169,26 @@
         def example_unique_response(self, ex_id: str):
             pass
 
         @route.get("/example/list", response=non_unique_response)
         def example_non_unique_response(self, ex_id: str):
             pass
 
-        assert len(example_unique_response.route.route_params.response) == 4
-        assert len(example_non_unique_response.route.route_params.response) == 2
+        assert (
+            len(get_route_function(example_unique_response).route.route_params.response)
+            == 4
+        )
+        assert (
+            len(
+                get_route_function(
+                    example_non_unique_response
+                ).route.route_params.response
+            )
+            == 2
+        )
 
     @pytest.mark.parametrize(
         "func, methods, kwargs",
         [
             (
                 "get",
                 ["GET"],
@@ -211,79 +222,101 @@
         ],
     )
     def test_route_generates_required_route_definitions(self, func, methods, kwargs):
         def view_func(request):
             pass
 
         route_method = getattr(route, func)
-        route_instance: RouteFunction = (
+        (
             route_method("/", methods=methods, **kwargs)
             if func == "generic"
             else route_method("/", **kwargs)
         )(view_func)
-        assert route_instance.route.route_params.methods == methods
+        route_function = get_route_function(view_func)
+        assert route_function.route.route_params.methods == methods
         for k, v in kwargs.items():
-            assert getattr(route_instance.route.route_params, k) == v
+            assert getattr(route_function.route.route_params, k) == v
 
 
 @pytest.mark.skipif(django.VERSION < (3, 1), reason="requires django 3.1 or higher")
-def test_async_route_function():
+@pytest.mark.asyncio
+async def test_async_route_function():
+    @api_controller()
     class AsyncSomeTestController(SomeTestController):
         @route.get("/example_async")
         async def example_async(self, ex_id: str):
-            pass
+            return {"message": "Okay", "ex_id": ex_id}
+
+    controller = AsyncSomeTestController()
+    example_route_function = get_route_function(controller.example)
+    example_async_route_function = get_route_function(controller.example_async)
+
+    assert isinstance(example_route_function, RouteFunction)
+    assert isinstance(example_async_route_function, AsyncRouteFunction)
 
-    assert isinstance(AsyncSomeTestController.example, RouteFunction)
-    assert isinstance(AsyncSomeTestController.example_async, AsyncRouteFunction)
-    assert AsyncSomeTestController.example_async.as_view
-    assert hasattr(AsyncSomeTestController.example_async.as_view, "get_route_function")
+    assert example_async_route_function.as_view
+    assert hasattr(example_async_route_function.as_view, "get_route_function")
     assert (
-        AsyncSomeTestController.example_async.as_view.get_route_function()
-        == AsyncSomeTestController.example_async
+        example_async_route_function.as_view.get_route_function()
+        == example_async_route_function
     )
+    assert await example_async_route_function(anonymous_request, ex_id="some id") == {
+        "message": "Okay",
+        "ex_id": "some id",
+    }
 
 
 class TestRouteFunction:
+    @staticmethod
     def api_func_with_has_request_param(self, request):
         pass
 
+    @staticmethod
     def api_func(self):
         pass
 
+    @staticmethod
     def api_func_with_param(self, example_id: str):
         pass
 
+    @staticmethod
     async def async_api_func(self):
         pass
 
     def test_get_required_api_func_signature_return_filtered_signature(self):
-        route_function = route.get("")(self.api_func)
+        route.get("")(self.api_func)
+        route_function = get_route_function(self.api_func)
         assert not route_function.has_request_param
         sig_inspect, sig_parameter = route_function._get_required_api_func_signature()
         assert len(sig_parameter) == 0
 
-        route_function = route.get("")(self.api_func_with_has_request_param)
+        route.get("")(self.api_func_with_has_request_param)
+        route_function = get_route_function(self.api_func_with_has_request_param)
         assert route_function.has_request_param
         sig_inspect, sig_parameter = route_function._get_required_api_func_signature()
         assert len(sig_parameter) == 0
 
-        route_function = route.get("")(self.api_func_with_param)
+        route.get("")(self.api_func_with_param)
+        route_function = get_route_function(self.api_func_with_param)
         sig_inspect, sig_parameter = route_function._get_required_api_func_signature()
         assert len(sig_parameter) == 1
         assert str(sig_parameter[0]).replace(" ", "") == "example_id:str"
 
     def test_from_route_returns_route_function_instance(self):
-        route_function = route.get("")(self.api_func)
+        route.get("")(self.api_func)
+        route_function = get_route_function(self.api_func)
         assert isinstance(route_function, RouteFunction)
 
-        route_function = route.get("")(self.async_api_func)
+        route.get("")(self.async_api_func)
+        route_function = get_route_function(self.async_api_func)
         assert isinstance(route_function, AsyncRouteFunction)
 
     def test_get_route_execution_context(self):
-        route_function = route.get("")(self.api_func)
+        route.get("")(self.api_func)
+        route_function = get_route_function(self.api_func)
         with pytest.raises(Exception):
             route_function.get_route_execution_context(
                 anonymous_request, "arg1", "arg2", extra="extra"
             )
         route_function.api_controller = Mock()
         route_function.api_controller.permission_classes = [AllowAny]
 
@@ -292,83 +325,95 @@
         )
         assert isinstance(route_context, RouteContext)
         expected_keywords = ("permission_classes", "request", "args", "kwargs")
         for key in expected_keywords:
             assert getattr(route_context, key)
 
     def test_get_controller_instance_return_controller_instance(self):
-        route_function: RouteFunction = SomeTestController.example
+        route_function: RouteFunction = get_route_function(SomeTestController().example)
         controller_instance = route_function._get_controller_instance()
         assert isinstance(controller_instance, SomeTestController)
         assert isinstance(controller_instance, SomeTestController)
         assert controller_instance.context is None
 
     def test_process_view_function_result_return_tuple_or_input(self):
-        route_function: RouteFunction = SomeTestController.example
+        route_function: RouteFunction = get_route_function(SomeTestController().example)
         mock_result = Detail("Some Message", status_code=302)
         response = route_function._process_view_function_result(mock_result)
         assert isinstance(response, tuple)
         assert response[1] == mock_result.convert_to_schema()
         assert response[0] == mock_result.status_code
 
         mock_result = dict(status=302, message="Some Message")
         response = route_function._process_view_function_result(mock_result)
         assert not isinstance(response, tuple)
         assert response == mock_result
 
 
 @pytest.mark.django_db
 class TestAPIControllerRoutePermission:
+    def setup(self):
+        self.controller = PermissionController()
+
     @classmethod
     def get_real_user_request(cls):
         _request = Mock()
         user = User.objects.create_user(
             username="eadwin",
             email="eadwin@example.com",
             password="password",
             is_staff=True,
         )
         _request.user = user
         return _request
 
     def test_permission_controller_example_allow_any_auth_is_none(self):
-        route_params = PermissionController.example_allow_any.route.route_params
+        example_allow_any_route_function = get_route_function(
+            self.controller.example_allow_any
+        )
+        route_params = example_allow_any_route_function.route.route_params
         assert route_params.auth is None
 
-        response = PermissionController.example_allow_any(anonymous_request)
+        response = example_allow_any_route_function(anonymous_request)
         assert response == {"message": "OK"}
+        assert response == self.controller.example_allow_any()
 
     def test_route_is_protected_by_global_controller_permission(self):
+        example_route_function = get_route_function(self.controller.example)
         with pytest.raises(PermissionDenied) as pex:
-            PermissionController.example(anonymous_request)
+            example_route_function(anonymous_request)
         assert "You do not have permission to perform this action." in str(
             pex.value.detail
         )
 
     def test_route_protected_by_global_controller_permission_works(self):
+        example_route_function = get_route_function(self.controller.example)
         request = self.get_real_user_request()
-        response = PermissionController.example(request)
+        response = example_route_function(request)
         assert response == {"message": "OK"}
 
     def test_route_is_protected_by_its_permissions_paramater(self):
-        response = PermissionController.example_allow_any(anonymous_request)
+        example_allow_any_route_function = get_route_function(
+            self.controller.example_allow_any
+        )
+        response = example_allow_any_route_function(anonymous_request)
         assert response == {"message": "OK"}
 
     def test_route_prep_controller_route_execution_context_works(self):
-        route_function: RouteFunction = SomeTestController.example
+        route_function: RouteFunction = get_route_function(SomeTestController().example)
         context = get_route_execution_context(request=anonymous_request)
         with route_function._prep_controller_route_execution(context=context) as ctx:
             assert isinstance(ctx.controller_instance, SomeTestController)
             assert ctx.controller_instance.context
         assert ctx.controller_instance.context is None
 
     def test_route_prep_controller_route_execution_context_cleans_controller_after_route_execution(
         self,
     ):
-        route_function: RouteFunction = SomeTestController.example
+        route_function: RouteFunction = get_route_function(SomeTestController().example)
         context = get_route_execution_context(request=anonymous_request)
         with pytest.raises(Exception):
             with route_function._prep_controller_route_execution(
                 context=context
             ) as ctx:
                 assert isinstance(ctx.controller_instance, SomeTestController)
                 assert ctx.controller_instance.context
```

### Comparing `django-ninja-extra-0.18.7/tests/test_settings.py` & `django-ninja-extra-0.18.8/tests/test_settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,22 @@
     pass
 
 
 class CustomThrottlingClassImport:
     pass
 
 
+class CustomOrderingClassImport:
+    pass
+
+
+class CustomSearchClassImport:
+    pass
+
+
 def test_setting_imports_string_works(monkeypatch):
     with monkeypatch.context() as m:
         m.setattr(
             settings,
             "INJECTOR_MODULES",
             [
                 "tests.test_settings.CustomModuleImport",
@@ -31,18 +39,26 @@
         m.setattr(
             settings,
             "THROTTLE_CLASSES",
             [
                 "tests.test_settings.CustomThrottlingClassImport",
             ],
         )
+        m.setattr(
+            settings, "ORDERING_CLASS", "tests.test_settings.CustomOrderingClassImport"
+        )
+        m.setattr(
+            settings, "SEARCHING_CLASS", "tests.test_settings.CustomSearchClassImport"
+        )
 
         assert isinstance(settings.INJECTOR_MODULES[0](), CustomModuleImport)
         assert isinstance(settings.PAGINATION_CLASS(), CustomPaginationImport)
         assert isinstance(settings.THROTTLE_CLASSES[0](), CustomThrottlingClassImport)
+        assert isinstance(settings.ORDERING_CLASS(), CustomOrderingClassImport)
+        assert isinstance(settings.SEARCHING_CLASS(), CustomSearchClassImport)
 
     with pytest.raises(ValidationError):
         monkeypatch.setattr(
             settings, "PAGINATION_CLASS", ["tests.test_settings.CustomModuleImport"]
         )
 
     with pytest.raises(ValidationError):
@@ -50,7 +66,17 @@
             settings, "THROTTLE_CLASSES", "tests.test_settings.CustomModuleImport"
         )
 
     with pytest.raises(ValidationError):
         monkeypatch.setattr(
             settings, "INJECTOR_MODULES", "tests.test_settings.CustomModuleImport"
         )
+
+    with pytest.raises(ValidationError):
+        monkeypatch.setattr(
+            settings, "ORDERING_CLASS", ["tests.test_settings.CustomModuleImport"]
+        )
+
+    with pytest.raises(ValidationError):
+        monkeypatch.setattr(
+            settings, "SEARCHING_CLASS", ["tests.test_settings.CustomModuleImport"]
+        )
```

### Comparing `django-ninja-extra-0.18.7/tests/test_shortcuts.py` & `django-ninja-extra-0.18.8/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_status.py` & `django-ninja-extra-0.18.8/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_testclient.py` & `django-ninja-extra-0.18.8/tests/test_testclient.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_throthling/test_decorator.py` & `django-ninja-extra-0.18.8/tests/test_throthling/test_decorator.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_throthling/test_models.py` & `django-ninja-extra-0.18.8/tests/test_throthling/test_models.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_throthling/test_throttle_controller.py` & `django-ninja-extra-0.18.8/tests/test_throthling/test_throttle_controller.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_throthling/test_throttle_decorator_on_controllers.py` & `django-ninja-extra-0.18.8/tests/test_throthling/test_throttle_decorator_on_controllers.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/test_throthling/test_throttling_xxf.py` & `django-ninja-extra-0.18.8/tests/test_throthling/test_throttling_xxf.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/tests/utils.py` & `django-ninja-extra-0.18.8/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-ninja-extra-0.18.7/PKG-INFO` & `django-ninja-extra-0.18.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ninja-extra
-Version: 0.18.7
+Version: 0.18.8
 Summary: Django Ninja Extra - Class Based Utility and more for Django Ninja(Fast Django REST framework)
 Home-page: https://github.com/eadwinCode/django-ninja-extra
 Author: Ezeudoh Tochukwu
 Author-email: tochukwu.ezeudoh@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -67,15 +67,15 @@
 
 ![Test](https://github.com/eadwinCode/django-ninja-extra/workflows/Test/badge.svg)
 [![PyPI version](https://badge.fury.io/py/django-ninja-extra.svg)](https://badge.fury.io/py/django-ninja-extra)
 [![PyPI version](https://img.shields.io/pypi/v/django-ninja-extra.svg)](https://pypi.python.org/pypi/django-ninja-extra)
 [![PyPI version](https://img.shields.io/pypi/pyversions/django-ninja-extra.svg)](https://pypi.python.org/pypi/django-ninja-extra)
 [![PyPI version](https://img.shields.io/pypi/djversions/django-ninja-extra.svg)](https://pypi.python.org/pypi/django-ninja-extra)
 [![Codecov](https://img.shields.io/codecov/c/gh/eadwinCode/django-ninja-extra)](https://codecov.io/gh/eadwinCode/django-ninja-extra)
-[![Downloads](https://pepy.tech/badge/django-ninja-extra/month)](https://pepy.tech/project/django-ninja-extra)
+[![Downloads](https://static.pepy.tech/badge/django-ninja-extra)](https://pepy.tech/project/django-ninja-extra)
 
 # Django Ninja Extra
 
 The **Django Ninja Extra** package offers a convenient, **class-based** approach to quickly building and configuring high-performance APIs. 
 Utilizing the core features of [**Django Ninja**](https://django-ninja.rest-framework.com), it allows for speedy development without sacrificing performance."
 
 **Key features:**
```

