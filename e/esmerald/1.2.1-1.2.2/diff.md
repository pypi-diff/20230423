# Comparing `tmp/esmerald-1.2.1.tar.gz` & `tmp/esmerald-1.2.2.tar.gz`

## Comparing `esmerald-1.2.1.tar` & `esmerald-1.2.2.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/__init__.py
--rw-r--r--   0        0        0    32270 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/applications.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/concurrency.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/enums.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/exceptions.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/injector.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/logging.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/param_functions.py
--rw-r--r--   0        0        0    14351 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/params.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/py.typed
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/requests.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/staticfiles.py
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/testclient.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/types.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/typing.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/websockets.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/enums.py
--rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/cors.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/csrf.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/jwt.py
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/openapi.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/session.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/static_files.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/crypto.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/tortoise/__init__.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/tortoise/base_user.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/tortoise/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/databases/__init__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/databases/tortoise/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/json.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/basic.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/cors.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/https.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/apiview.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/parameters.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/path_item.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/request_body.py
--rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/schema.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/types.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/utils.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/permissions/base.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/template.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/responses/base.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/responses/json.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/__init__.py
--rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/base.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/events.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/gateways.py
--rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    40060 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/router.py
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/helpers.py
--rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/model.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/signature.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/types.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/utils.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/urls/__init__.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/urls/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/constants.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/helpers.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/model.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/pydantic.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/sync.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/timezone.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/url.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.2.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.2.1/LICENSE
--rw-r--r--   0        0        0    15138 2020-02-02 00:00:00.000000 esmerald-1.2.1/README.md
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 esmerald-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    20137 2020-02-02 00:00:00.000000 esmerald-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/__init__.py
+-rw-r--r--   0        0        0    32270 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/applications.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/concurrency.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/enums.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/exceptions.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/injector.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/logging.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/param_functions.py
+-rw-r--r--   0        0        0    14351 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/params.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/py.typed
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/requests.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/testclient.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/types.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/typing.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/websockets.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/app_template/v1/views.py-tpl
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/config/cors.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/config/csrf.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/config/jwt.py
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/config/openapi.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/config/session.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/config/static_files.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/crypto.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/tortoise/__init__.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/tortoise/base_user.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/auth/tortoise/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/databases/__init__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/contrib/databases/tortoise/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/basic.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/openapi/apiview.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/openapi/parameters.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/openapi/path_item.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/openapi/request_body.py
+-rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/openapi/schema.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/openapi/types.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/protocols/template.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/responses/base.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/routing/events.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    40060 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/routing/router.py
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/routing/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/transformers/helpers.py
+-rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/transformers/types.py
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/urls/__init__.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/urls/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/constants.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/model.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/pydantic.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/sync.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/timezone.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.2.2/esmerald/utils/url.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.2.2/LICENSE
+-rw-r--r--   0        0        0    15138 2020-02-02 00:00:00.000000 esmerald-1.2.2/README.md
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 esmerald-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    20115 2020-02-02 00:00:00.000000 esmerald-1.2.2/PKG-INFO
```

### Comparing `esmerald-1.2.1/esmerald/__init__.py` & `esmerald-1.2.2/esmerald/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Esmerald: Highly scalable, performant, easy to learn and for every application.
 """
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 
 from starlette import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.injector import Inject
```

### Comparing `esmerald-1.2.1/esmerald/applications.py` & `esmerald-1.2.2/esmerald/applications.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/backgound.py` & `esmerald-1.2.2/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/enums.py` & `esmerald-1.2.2/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/exception_handlers.py` & `esmerald-1.2.2/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/exceptions.py` & `esmerald-1.2.2/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/injector.py` & `esmerald-1.2.2/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/logging.py` & `esmerald-1.2.2/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/params.py` & `esmerald-1.2.2/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/parsers.py` & `esmerald-1.2.2/esmerald/parsers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/requests.py` & `esmerald-1.2.2/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/testclient.py` & `esmerald-1.2.2/esmerald/testclient.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/types.py` & `esmerald-1.2.2/esmerald/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/websockets.py` & `esmerald-1.2.2/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/conf/__init__.py` & `esmerald-1.2.2/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/conf/global_settings.py` & `esmerald-1.2.2/esmerald/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/conf/project_template/.gitignore.e-tpl` & `esmerald-1.2.2/esmerald/conf/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/conf/project_template/Makefile.e-tpl` & `esmerald-1.2.2/esmerald/conf/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/conf/project_template/project_name/main.py-tpl` & `esmerald-1.2.2/esmerald/conf/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/conf/project_template/project_name/serve.py-tpl` & `esmerald-1.2.2/esmerald/conf/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/conf/project_template/project_name/urls.py-tpl` & `esmerald-1.2.2/esmerald/conf/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/settings.py-tpl` & `esmerald-1.2.2/esmerald/conf/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/config/jwt.py` & `esmerald-1.2.2/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/config/openapi.py` & `esmerald-1.2.2/esmerald/config/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/config/session.py` & `esmerald-1.2.2/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/config/static_files.py` & `esmerald-1.2.2/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/contrib/encoding.py` & `esmerald-1.2.2/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/contrib/auth/hashers.py` & `esmerald-1.2.2/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/contrib/auth/common/middleware.py` & `esmerald-1.2.2/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-1.2.2/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-1.2.2/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/contrib/auth/tortoise/base_user.py` & `esmerald-1.2.2/esmerald/contrib/auth/tortoise/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/contrib/auth/tortoise/middleware.py` & `esmerald-1.2.2/esmerald/contrib/auth/tortoise/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/contrib/databases/tortoise/__init__.py` & `esmerald-1.2.2/esmerald/contrib/databases/tortoise/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/directives/base.py` & `esmerald-1.2.2/esmerald/core/directives/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/directives/cli.py` & `esmerald-1.2.2/esmerald/core/directives/cli.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/directives/env.py` & `esmerald-1.2.2/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/directives/templates.py` & `esmerald-1.2.2/esmerald/core/directives/templates.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/directives/utils.py` & `esmerald-1.2.2/esmerald/core/directives/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     return directive_list
 
 
 def load_directive_class(app_name: str, name: str) -> Any:
     """
     Loads the directive class from native Esmerald.
     """
-    module = import_module("%s.directives.operations.%s" % (app_name, name))
+    module = import_module("{}.directives.operations.{}".format(app_name, name))
     return module.Directive()
 
 
 def load_directive_class_by_filename(app_name: str, location: str) -> Any:
     """
     Loads the directive by filename.
 
@@ -99,35 +99,44 @@
 
 def fetch_custom_directive(subdirective: Any, location: str) -> Any:
     """Fetches the directive classes custom and native"""
     directives = get_application_directives(location)
 
     counter = 0
     matches = []
+    app_name = None
 
     for directive in sorted(directives, key=lambda d: d["location"]):
         try:
             for key, _ in directive.items():
                 if key == subdirective:
                     app_name = key
                     location = directive["location"]
                     break
         except KeyError:
             counter += 1
-
             directive = {k: v for k, v in directive.items() if k != "location"}
             matches.extend(get_close_matches(subdirective, directive))
 
             if matches and len(directives) == counter:
                 printer.write_error("Did you mean %s?" % matches[0])
 
             if len(directives) == counter:
                 return None
             continue
 
+    if not app_name:
+        directive = {k: v for k, v in directive.items() if k != "location"}
+        matches.extend(get_close_matches(subdirective, directive))
+
+        if matches:
+            printer.write_error("Did you mean %s?" % matches[0])
+            return None
+        return None
+
     name = f"{location}/{app_name}.py"
     klass = load_directive_class_by_filename(app_name, name)
 
     if not isinstance(klass, BaseDirective):
         raise DirectiveError(detail="The directive must be a subclass of BaseDirective")
     return klass
```

### Comparing `esmerald-1.2.1/esmerald/core/directives/operations/createapp.py` & `esmerald-1.2.2/esmerald/core/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/directives/operations/createproject.py` & `esmerald-1.2.2/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/directives/operations/list.py` & `esmerald-1.2.2/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/directives/operations/run.py` & `esmerald-1.2.2/esmerald/core/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/directives/operations/runserver.py` & `esmerald-1.2.2/esmerald/core/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/directives/operations/show_urls.py` & `esmerald-1.2.2/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/terminal/base.py` & `esmerald-1.2.2/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/terminal/print.py` & `esmerald-1.2.2/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/core/terminal/terminal.py` & `esmerald-1.2.2/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/datastructures/__init__.py` & `esmerald-1.2.2/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/datastructures/base.py` & `esmerald-1.2.2/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/datastructures/encoders.py` & `esmerald-1.2.2/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/datastructures/file.py` & `esmerald-1.2.2/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/datastructures/json.py` & `esmerald-1.2.2/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/datastructures/redirect.py` & `esmerald-1.2.2/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/datastructures/stream.py` & `esmerald-1.2.2/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/datastructures/template.py` & `esmerald-1.2.2/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/interceptors/interceptor.py` & `esmerald-1.2.2/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/middleware/__init__.py` & `esmerald-1.2.2/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/middleware/asyncexitstack.py` & `esmerald-1.2.2/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/middleware/authentication.py` & `esmerald-1.2.2/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/middleware/basic.py` & `esmerald-1.2.2/esmerald/middleware/basic.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/middleware/csrf.py` & `esmerald-1.2.2/esmerald/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/middleware/errors.py` & `esmerald-1.2.2/esmerald/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/middleware/exceptions.py` & `esmerald-1.2.2/esmerald/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/middleware/settings_middleware.py` & `esmerald-1.2.2/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/openapi/apiview.py` & `esmerald-1.2.2/esmerald/openapi/apiview.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/openapi/enums.py` & `esmerald-1.2.2/esmerald/openapi/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/openapi/parameters.py` & `esmerald-1.2.2/esmerald/openapi/parameters.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/openapi/path_item.py` & `esmerald-1.2.2/esmerald/openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/openapi/request_body.py` & `esmerald-1.2.2/esmerald/openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/openapi/responses.py` & `esmerald-1.2.2/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/openapi/schema.py` & `esmerald-1.2.2/esmerald/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/openapi/utils.py` & `esmerald-1.2.2/esmerald/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/permissions/base.py` & `esmerald-1.2.2/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/permissions/utils.py` & `esmerald-1.2.2/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/pluggables/base.py` & `esmerald-1.2.2/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/protocols/asyncdao.py` & `esmerald-1.2.2/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/protocols/dao.py` & `esmerald-1.2.2/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/protocols/interceptor.py` & `esmerald-1.2.2/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/protocols/template.py` & `esmerald-1.2.2/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/responses/base.py` & `esmerald-1.2.2/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/responses/encoders.py` & `esmerald-1.2.2/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/responses/json.py` & `esmerald-1.2.2/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/responses/template.py` & `esmerald-1.2.2/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/routing/base.py` & `esmerald-1.2.2/esmerald/routing/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/routing/events.py` & `esmerald-1.2.2/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/routing/gateways.py` & `esmerald-1.2.2/esmerald/routing/gateways.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/routing/handlers.py` & `esmerald-1.2.2/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/routing/router.py` & `esmerald-1.2.2/esmerald/routing/router.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/routing/views.py` & `esmerald-1.2.2/esmerald/routing/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/security/jwt/token.py` & `esmerald-1.2.2/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/template/jinja.py` & `esmerald-1.2.2/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/template/mako.py` & `esmerald-1.2.2/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/transformers/datastructures.py` & `esmerald-1.2.2/esmerald/transformers/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/transformers/helpers.py` & `esmerald-1.2.2/esmerald/transformers/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/transformers/model.py` & `esmerald-1.2.2/esmerald/transformers/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/transformers/signature.py` & `esmerald-1.2.2/esmerald/transformers/signature.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/transformers/types.py` & `esmerald-1.2.2/esmerald/transformers/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/transformers/utils.py` & `esmerald-1.2.2/esmerald/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/urls/base.py` & `esmerald-1.2.2/esmerald/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/utils/constants.py` & `esmerald-1.2.2/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/utils/crypto.py` & `esmerald-1.2.2/esmerald/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/utils/functional.py` & `esmerald-1.2.2/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/utils/helpers.py` & `esmerald-1.2.2/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/utils/model.py` & `esmerald-1.2.2/esmerald/utils/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/utils/module_loading.py` & `esmerald-1.2.2/esmerald/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/utils/pydantic.py` & `esmerald-1.2.2/esmerald/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/utils/sync.py` & `esmerald-1.2.2/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/esmerald/utils/timezone.py` & `esmerald-1.2.2/esmerald/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/LICENSE` & `esmerald-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/README.md` & `esmerald-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.1/pyproject.toml` & `esmerald-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 dependencies = [
     "a2wsgi>=1.7.0,<2",
     "aiofiles>=0.8.0,<24",
     "anyio>=3.6.2,<4.0.0",
     "awesome-slugify>=1.6.5,<2",
     "httpx>=0.24.0,<0.30.0",
     "itsdangerous>=2.1.2,<3.0.0",
+    "jinja2>=3.1.2,<4.0.0",
     "jsonschema_rs>=0.16.2,<0.20.0",
     "loguru>=0.6.0,<0.7.0",
     "pydantic>=1.10.7,<2.0.0",
     "pydantic-factories==1.17.2",
     "python-multipart>=0.0.5,<0.0.7",
     "openapi-schemas-pydantic>=1.1.0",
     "rich>=13.3.1,<14.0.0",
@@ -73,15 +74,15 @@
 Documentation = "https://esmerald.dymmond.com/"
 Changelog = "https://esmerald.dymmond.com/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
 Source = "https://github.com/dymmond/esmerald"
 
 [project.optional-dependencies]
 test = [
-    "pytest>=7.1.3,<8.0.0",
+    "pytest>=7.3.1,<8.0.0",
     "pytest-cov>=2.12.0,<5.0.0",
     "pytest-asyncio>=0.19.0",
     "mypy==1.1.1",
     "flake8>=5.0.4",
     "black== 23.3.0",
     "isort>=5.0.6,<6.0.0",
     "aiofiles>=0.8.0,<24",
@@ -93,15 +94,15 @@
     "jinja2>=3.1.2,<4.0.0",
     "flask>=1.1.2,<3.0.0",
     "freezegun>=1.2.2,<2.0.0",
     "mock==5.0.1",
     "passlib==1.7.4",
     "python-jose>=3.3.0,<4",
     "orjson>=3.8.5,<4.0.0",
-    "saffier[postgres]>=0.6.1",
+    "saffier[postgres]==0.6.1",
     "requests>=2.28.2,<3.0.0",
     "ruff>=0.0.256,<1.0.0",
     "ujson>=5.7.0,<6",
 
     # types
     "types-ujson==5.7.0.1",
     "types-orjson==3.6.2",
@@ -121,15 +122,15 @@
     "mkdocs-material>=9.0.13,<10.0.0",
     "mdx-include>=1.4.2,<2.0.0",
     "mkdocs-markdownextradata-plugin>=0.2.5,<0.3.0",
     "mkdocstrings>=0.20.0,<0.30.0",
     "pyyaml>=6.0,<7.0.0",
 ]
 
-templates = ["jinja2>=3.1.2,<4.0.0", "mako==1.2.4"]
+templates = ["mako==1.2.4"]
 
 jwt = ["passlib==1.7.4", "python-jose>=3.3.0,<4"]
 
 encoders = ["orjson>=3.8.5,<4.0.0", "ujson>=5.7.0,<6"]
 
 schedulers = ["asyncz>=0.2.0"]
```

### Comparing `esmerald-1.2.1/PKG-INFO` & `esmerald-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald
-Version: 1.2.1
+Version: 1.2.2
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
@@ -38,14 +38,15 @@
 Requires-Python: >=3.8
 Requires-Dist: a2wsgi<2,>=1.7.0
 Requires-Dist: aiofiles<24,>=0.8.0
 Requires-Dist: anyio<4.0.0,>=3.6.2
 Requires-Dist: awesome-slugify<2,>=1.6.5
 Requires-Dist: httpx<0.30.0,>=0.24.0
 Requires-Dist: itsdangerous<3.0.0,>=2.1.2
+Requires-Dist: jinja2<4.0.0,>=3.1.2
 Requires-Dist: jsonschema-rs<0.20.0,>=0.16.2
 Requires-Dist: loguru<0.7.0,>=0.6.0
 Requires-Dist: openapi-schemas-pydantic>=1.1.0
 Requires-Dist: pydantic-factories==1.17.2
 Requires-Dist: pydantic<2.0.0,>=1.10.7
 Requires-Dist: python-multipart<0.0.7,>=0.0.5
 Requires-Dist: rich<14.0.0,>=13.3.1
@@ -69,15 +70,14 @@
 Requires-Dist: ujson<6,>=5.7.0; extra == 'encoders'
 Provides-Extra: jwt
 Requires-Dist: passlib==1.7.4; extra == 'jwt'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'jwt'
 Provides-Extra: schedulers
 Requires-Dist: asyncz>=0.2.0; extra == 'schedulers'
 Provides-Extra: templates
-Requires-Dist: jinja2<4.0.0,>=3.1.2; extra == 'templates'
 Requires-Dist: mako==1.2.4; extra == 'templates'
 Provides-Extra: test
 Requires-Dist: a2wsgi<2,>=1.7.0; extra == 'test'
 Requires-Dist: aiofiles<24,>=0.8.0; extra == 'test'
 Requires-Dist: anyio[trio]<4.0.0,>=3.6.2; extra == 'test'
 Requires-Dist: asyncio[trio]<4.0.0,>=3.4.3; extra == 'test'
 Requires-Dist: asyncz>=0.2.0; extra == 'test'
@@ -90,19 +90,19 @@
 Requires-Dist: jinja2<4.0.0,>=3.1.2; extra == 'test'
 Requires-Dist: mock==5.0.1; extra == 'test'
 Requires-Dist: mypy==1.1.1; extra == 'test'
 Requires-Dist: orjson<4.0.0,>=3.8.5; extra == 'test'
 Requires-Dist: passlib==1.7.4; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.19.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
-Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
+Requires-Dist: pytest<8.0.0,>=7.3.1; extra == 'test'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'test'
 Requires-Dist: requests<3.0.0,>=2.28.2; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
-Requires-Dist: saffier[postgres]>=0.6.1; extra == 'test'
+Requires-Dist: saffier[postgres]==0.6.1; extra == 'test'
 Requires-Dist: types-orjson==3.6.2; extra == 'test'
 Requires-Dist: types-ujson==5.7.0.1; extra == 'test'
 Requires-Dist: ujson<6,>=5.7.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Esmerald
```

