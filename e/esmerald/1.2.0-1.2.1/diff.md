# Comparing `tmp/esmerald-1.2.0.tar.gz` & `tmp/esmerald-1.2.1.tar.gz`

## Comparing `esmerald-1.2.0.tar` & `esmerald-1.2.1.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/__init__.py
--rw-r--r--   0        0        0    32270 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/applications.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/concurrency.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/enums.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/exceptions.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/injector.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/logging.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/param_functions.py
--rw-r--r--   0        0        0    14351 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/params.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/py.typed
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/requests.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/staticfiles.py
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/testclient.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/types.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/typing.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/websockets.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/enums.py
--rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/cors.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/csrf.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/jwt.py
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/openapi.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/session.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/static_files.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/crypto.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/tortoise/__init__.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/tortoise/base_user.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/auth/tortoise/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/databases/__init__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/contrib/databases/tortoise/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/json.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/basic.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/cors.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/https.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/apiview.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/parameters.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/path_item.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/request_body.py
--rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/schema.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/types.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/openapi/utils.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/permissions/base.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/protocols/template.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/responses/base.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/responses/json.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/__init__.py
--rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/base.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/events.py
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/gateways.py
--rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    40060 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/router.py
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/routing/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/helpers.py
--rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/model.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/signature.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/types.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/transformers/utils.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/urls/__init__.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/urls/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/constants.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/helpers.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/model.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/pydantic.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/sync.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/timezone.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.2.0/esmerald/utils/url.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.2.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.2.0/LICENSE
--rw-r--r--   0        0        0    15138 2020-02-02 00:00:00.000000 esmerald-1.2.0/README.md
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 esmerald-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    20137 2020-02-02 00:00:00.000000 esmerald-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/__init__.py
+-rw-r--r--   0        0        0    32270 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/applications.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/concurrency.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/enums.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/exceptions.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/injector.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/logging.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/param_functions.py
+-rw-r--r--   0        0        0    14351 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/params.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/py.typed
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/requests.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/testclient.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/types.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/typing.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/websockets.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    13177 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/app_template/v1/views.py-tpl
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/cors.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/csrf.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/jwt.py
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/openapi.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/session.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/static_files.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/crypto.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/tortoise/__init__.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/tortoise/base_user.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/auth/tortoise/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/databases/__init__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/contrib/databases/tortoise/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/basic.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/apiview.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/parameters.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/path_item.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/request_body.py
+-rw-r--r--   0        0        0     8557 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/schema.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/types.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/protocols/template.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/responses/base.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/events.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    40060 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/router.py
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/routing/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/helpers.py
+-rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/types.py
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/urls/__init__.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/urls/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/constants.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/model.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/pydantic.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/sync.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/timezone.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-1.2.1/esmerald/utils/url.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-1.2.1/LICENSE
+-rw-r--r--   0        0        0    15138 2020-02-02 00:00:00.000000 esmerald-1.2.1/README.md
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 esmerald-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    20137 2020-02-02 00:00:00.000000 esmerald-1.2.1/PKG-INFO
```

### Comparing `esmerald-1.2.0/esmerald/__init__.py` & `esmerald-1.2.1/esmerald/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Esmerald: Highly scalable, performant, easy to learn and for every application.
 """
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 
 from starlette import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.injector import Inject
```

### Comparing `esmerald-1.2.0/esmerald/applications.py` & `esmerald-1.2.1/esmerald/applications.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/backgound.py` & `esmerald-1.2.1/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/enums.py` & `esmerald-1.2.1/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/exception_handlers.py` & `esmerald-1.2.1/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/exceptions.py` & `esmerald-1.2.1/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/injector.py` & `esmerald-1.2.1/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/logging.py` & `esmerald-1.2.1/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/params.py` & `esmerald-1.2.1/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/parsers.py` & `esmerald-1.2.1/esmerald/parsers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/requests.py` & `esmerald-1.2.1/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/testclient.py` & `esmerald-1.2.1/esmerald/testclient.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/types.py` & `esmerald-1.2.1/esmerald/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/websockets.py` & `esmerald-1.2.1/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/conf/__init__.py` & `esmerald-1.2.1/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/conf/global_settings.py` & `esmerald-1.2.1/esmerald/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/conf/project_template/.gitignore.e-tpl` & `esmerald-1.2.1/esmerald/conf/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/conf/project_template/Makefile.e-tpl` & `esmerald-1.2.1/esmerald/conf/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/conf/project_template/project_name/main.py-tpl` & `esmerald-1.2.1/esmerald/conf/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/conf/project_template/project_name/serve.py-tpl` & `esmerald-1.2.1/esmerald/conf/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/conf/project_template/project_name/urls.py-tpl` & `esmerald-1.2.1/esmerald/conf/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/conf/project_template/project_name/configs/settings.py-tpl` & `esmerald-1.2.1/esmerald/conf/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/config/jwt.py` & `esmerald-1.2.1/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/config/openapi.py` & `esmerald-1.2.1/esmerald/config/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/config/session.py` & `esmerald-1.2.1/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/config/static_files.py` & `esmerald-1.2.1/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/contrib/encoding.py` & `esmerald-1.2.1/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/contrib/auth/hashers.py` & `esmerald-1.2.1/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/contrib/auth/common/middleware.py` & `esmerald-1.2.1/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-1.2.1/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-1.2.1/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/contrib/auth/tortoise/base_user.py` & `esmerald-1.2.1/esmerald/contrib/auth/tortoise/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/contrib/auth/tortoise/middleware.py` & `esmerald-1.2.1/esmerald/contrib/auth/tortoise/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/contrib/databases/tortoise/__init__.py` & `esmerald-1.2.1/esmerald/contrib/databases/tortoise/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/core/directives/base.py` & `esmerald-1.2.1/esmerald/core/directives/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/core/directives/cli.py` & `esmerald-1.2.1/esmerald/core/directives/cli.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/core/directives/env.py` & `esmerald-1.2.1/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/core/directives/templates.py` & `esmerald-1.2.1/esmerald/core/directives/templates.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/core/directives/utils.py` & `esmerald-1.2.1/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/core/directives/operations/createapp.py` & `esmerald-1.2.1/esmerald/core/directives/operations/createapp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""
-Client to interact with Saffier models and migrations.
-"""
-
 import click
 
 from esmerald.core.directives.exceptions import DirectiveError
 from esmerald.core.directives.operations._constants import SECRET_KEY_INSECURE_PREFIX
 from esmerald.core.directives.templates import TemplateDirective
 from esmerald.core.terminal import Print
 from esmerald.utils.crypto import get_random_secret_key
```

### Comparing `esmerald-1.2.0/esmerald/core/directives/operations/createproject.py` & `esmerald-1.2.1/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/core/directives/operations/list.py` & `esmerald-1.2.1/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/core/directives/operations/run.py` & `esmerald-1.2.1/esmerald/core/directives/operations/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import click
 from starlette.types import Lifespan
 
 from esmerald.core.directives.constants import APP_PARAMETER, ESMERALD_DISCOVER_APP
 from esmerald.core.directives.env import DirectiveEnv
 from esmerald.core.directives.utils import fetch_directive
 from esmerald.core.terminal.print import Print
-from esmerald.routing.events import handle_lifespan_events
+from esmerald.routing.events import generate_lifespan_events
 from esmerald.utils.sync import execsync
 
 printer = Print()
 
 
 class Position(int, Enum):
     DEFAULT = 5
@@ -60,15 +60,15 @@
     # Execute the directive
     # The arguments for the directives start at the position 6
     position = get_position()
     program_name = " ".join(value for value in sys.argv[:position])
 
     ## Check if application is up and execute any event
     # Shutting down after
-    lifespan = handle_lifespan_events(env.app.on_startup, env.app.on_shutdown, env.app.lifespan)
+    lifespan = generate_lifespan_events(env.app.on_startup, env.app.on_shutdown, env.app.lifespan)
     execsync(execute_lifespan)(env.app, lifespan, directive, program_name, position)
 
 
 def get_position():
     """
     Gets the position of the arguments to read and pass them
     onto the directive.
```

### Comparing `esmerald-1.2.0/esmerald/core/directives/operations/runserver.py` & `esmerald-1.2.1/esmerald/core/directives/operations/runserver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""
-Client to interact with Saffier models and migrations.
-"""
-
 import sys
 
 import click
 
 from esmerald.core.directives.env import DirectiveEnv
 from esmerald.core.directives.exceptions import DirectiveError
 from esmerald.core.terminal import OutputColour, Print, Terminal
```

### Comparing `esmerald-1.2.0/esmerald/core/directives/operations/show_urls.py` & `esmerald-1.2.1/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/core/terminal/base.py` & `esmerald-1.2.1/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/core/terminal/print.py` & `esmerald-1.2.1/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/core/terminal/terminal.py` & `esmerald-1.2.1/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/datastructures/__init__.py` & `esmerald-1.2.1/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/datastructures/base.py` & `esmerald-1.2.1/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/datastructures/encoders.py` & `esmerald-1.2.1/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/datastructures/file.py` & `esmerald-1.2.1/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/datastructures/json.py` & `esmerald-1.2.1/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/datastructures/redirect.py` & `esmerald-1.2.1/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/datastructures/stream.py` & `esmerald-1.2.1/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/datastructures/template.py` & `esmerald-1.2.1/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/interceptors/interceptor.py` & `esmerald-1.2.1/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/middleware/__init__.py` & `esmerald-1.2.1/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/middleware/asyncexitstack.py` & `esmerald-1.2.1/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/middleware/authentication.py` & `esmerald-1.2.1/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/middleware/basic.py` & `esmerald-1.2.1/esmerald/middleware/basic.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/middleware/csrf.py` & `esmerald-1.2.1/esmerald/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/middleware/errors.py` & `esmerald-1.2.1/esmerald/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/middleware/exceptions.py` & `esmerald-1.2.1/esmerald/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/middleware/settings_middleware.py` & `esmerald-1.2.1/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/openapi/apiview.py` & `esmerald-1.2.1/esmerald/openapi/apiview.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/openapi/enums.py` & `esmerald-1.2.1/esmerald/openapi/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/openapi/parameters.py` & `esmerald-1.2.1/esmerald/openapi/parameters.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/openapi/path_item.py` & `esmerald-1.2.1/esmerald/openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/openapi/request_body.py` & `esmerald-1.2.1/esmerald/openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/openapi/responses.py` & `esmerald-1.2.1/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/openapi/schema.py` & `esmerald-1.2.1/esmerald/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/openapi/utils.py` & `esmerald-1.2.1/esmerald/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/permissions/base.py` & `esmerald-1.2.1/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/permissions/utils.py` & `esmerald-1.2.1/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/pluggables/base.py` & `esmerald-1.2.1/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/protocols/asyncdao.py` & `esmerald-1.2.1/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/protocols/dao.py` & `esmerald-1.2.1/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/protocols/interceptor.py` & `esmerald-1.2.1/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/protocols/template.py` & `esmerald-1.2.1/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/responses/base.py` & `esmerald-1.2.1/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/responses/encoders.py` & `esmerald-1.2.1/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/responses/json.py` & `esmerald-1.2.1/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/responses/template.py` & `esmerald-1.2.1/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/routing/base.py` & `esmerald-1.2.1/esmerald/routing/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/routing/events.py` & `esmerald-1.2.1/esmerald/routing/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,7 +63,17 @@
     for the lifespan.
     """
     if on_startup or on_shutdown:
         return AyncLifespanContextManager(on_startup=on_startup, on_shutdown=on_shutdown)
     elif lifespan:
         return lifespan
     return None
+
+
+def generate_lifespan_events(
+    on_startup: Optional[Sequence[Callable]] = None,
+    on_shutdown: Optional[Sequence[Callable]] = None,
+    lifespan: Optional[Lifespan[Any]] = None,
+) -> Any:
+    if lifespan:
+        return lifespan
+    return AyncLifespanContextManager(on_startup=on_startup, on_shutdown=on_shutdown)
```

### Comparing `esmerald-1.2.0/esmerald/routing/gateways.py` & `esmerald-1.2.1/esmerald/routing/gateways.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/routing/handlers.py` & `esmerald-1.2.1/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/routing/router.py` & `esmerald-1.2.1/esmerald/routing/router.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/routing/views.py` & `esmerald-1.2.1/esmerald/routing/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/security/jwt/token.py` & `esmerald-1.2.1/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/template/jinja.py` & `esmerald-1.2.1/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/template/mako.py` & `esmerald-1.2.1/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/transformers/datastructures.py` & `esmerald-1.2.1/esmerald/transformers/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/transformers/helpers.py` & `esmerald-1.2.1/esmerald/transformers/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/transformers/model.py` & `esmerald-1.2.1/esmerald/transformers/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/transformers/signature.py` & `esmerald-1.2.1/esmerald/transformers/signature.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/transformers/types.py` & `esmerald-1.2.1/esmerald/transformers/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/transformers/utils.py` & `esmerald-1.2.1/esmerald/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/urls/base.py` & `esmerald-1.2.1/esmerald/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/utils/constants.py` & `esmerald-1.2.1/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/utils/crypto.py` & `esmerald-1.2.1/esmerald/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/utils/functional.py` & `esmerald-1.2.1/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/utils/helpers.py` & `esmerald-1.2.1/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/utils/model.py` & `esmerald-1.2.1/esmerald/utils/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/utils/module_loading.py` & `esmerald-1.2.1/esmerald/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/utils/pydantic.py` & `esmerald-1.2.1/esmerald/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/utils/sync.py` & `esmerald-1.2.1/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/esmerald/utils/timezone.py` & `esmerald-1.2.1/esmerald/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/LICENSE` & `esmerald-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/README.md` & `esmerald-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/pyproject.toml` & `esmerald-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esmerald-1.2.0/PKG-INFO` & `esmerald-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald
-Version: 1.2.0
+Version: 1.2.1
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
```

