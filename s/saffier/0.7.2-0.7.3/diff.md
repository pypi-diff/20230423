# Comparing `tmp/saffier-0.7.2.tar.gz` & `tmp/saffier-0.7.3.tar.gz`

## Comparing `saffier-0.7.2.tar` & `saffier-0.7.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/__init__.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/exceptions.py
--rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/fields.py
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/metaclass.py
--rw-r--r--   0        0        0     9039 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/models.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/py.typed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/testclient.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/types.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/conf/enums.py
--rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/conf/functional.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/conf/global_settings.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/conf/module_import.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/__init__.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/base.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/datastructures.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/events.py
--rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/formats.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/registry.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/schemas.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/sync.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/unique.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/terminal/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/terminal/base.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/terminal/print.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/core/terminal/terminal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/db/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/db/connection.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/db/constants.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/db/datastructures.py
--rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/db/fields.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/db/manager.py
--rw-r--r--   0        0        0    23146 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/db/queryset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/db/query/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/db/query/protocols.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/__init__.py
--rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/base.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/cli.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/constants.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/decorators.py
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/env.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/branches.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/check.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/current.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/downgrade.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/edit.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/heads.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/history.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/init.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/list_templates.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/makemigrations.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/merge.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/migrate.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/revision.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/show.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/stamp.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/shell/__init__.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/shell/enums.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/shell/ipython.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/shell/ptpython.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/operations/shell/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/templates/default/README
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/templates/default/alembic.ini.mako
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/templates/default/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/migrations/templates/default/script.py.mako
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/sqlalchemy/fields.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/sqlalchemy/protocols.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.7.2/saffier/sqlalchemy/types.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.7.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.7.2/LICENSE
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.7.2/README.md
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 saffier-0.7.2/pyproject.toml
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 saffier-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/__init__.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/exceptions.py
+-rw-r--r--   0        0        0    10792 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/fields.py
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/metaclass.py
+-rw-r--r--   0        0        0     9039 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/models.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/py.typed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/testclient.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/types.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/conf/enums.py
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/conf/functional.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/conf/global_settings.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/conf/module_import.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/__init__.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/base.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/datastructures.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/events.py
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/formats.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/registry.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/schemas.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/sync.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/unique.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/terminal/base.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/terminal/print.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/core/terminal/terminal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/connection.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/constants.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/datastructures.py
+-rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/fields.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/manager.py
+-rw-r--r--   0        0        0    23146 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/query/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/db/query/protocols.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/__init__.py
+-rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/base.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/cli.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/constants.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/decorators.py
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/env.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/branches.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/check.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/current.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/downgrade.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/edit.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/heads.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/history.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/init.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/list_templates.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/makemigrations.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/merge.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/migrate.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/revision.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/show.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/stamp.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/enums.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/operations/shell/utils.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/templates/default/README
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/templates/default/alembic.ini.mako
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/templates/default/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/migrations/templates/default/script.py.mako
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/sqlalchemy/fields.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/sqlalchemy/protocols.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.7.3/saffier/sqlalchemy/types.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.7.3/LICENSE
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.7.3/README.md
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 saffier-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0    11270 2020-02-02 00:00:00.000000 saffier-0.7.3/PKG-INFO
```

### Comparing `saffier-0.7.2/saffier/__init__.py` & `saffier-0.7.3/saffier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 from saffier.conf import settings
 from saffier.conf.global_settings import SaffierSettings
 
 from .core.registry import Registry
 from .db.connection import Database
 from .db.constants import CASCADE, RESTRICT, SET_NULL
```

### Comparing `saffier-0.7.2/saffier/exceptions.py` & `saffier-0.7.3/saffier/exceptions.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/fields.py` & `saffier-0.7.3/saffier/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/metaclass.py` & `saffier-0.7.3/saffier/metaclass.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/models.py` & `saffier-0.7.3/saffier/models.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/conf/__init__.py` & `saffier-0.7.3/saffier/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/conf/functional.py` & `saffier-0.7.3/saffier/conf/functional.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/conf/global_settings.py` & `saffier-0.7.3/saffier/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/conf/module_import.py` & `saffier-0.7.3/saffier/conf/module_import.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/base.py` & `saffier-0.7.3/saffier/core/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/datastructures.py` & `saffier-0.7.3/saffier/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/events.py` & `saffier-0.7.3/saffier/core/events.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/formats.py` & `saffier-0.7.3/saffier/core/formats.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/registry.py` & `saffier-0.7.3/saffier/core/registry.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/schemas.py` & `saffier-0.7.3/saffier/core/schemas.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/sync.py` & `saffier-0.7.3/saffier/core/sync.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/unique.py` & `saffier-0.7.3/saffier/core/unique.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/utils.py` & `saffier-0.7.3/saffier/core/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/terminal/base.py` & `saffier-0.7.3/saffier/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/terminal/print.py` & `saffier-0.7.3/saffier/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/core/terminal/terminal.py` & `saffier-0.7.3/saffier/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/db/datastructures.py` & `saffier-0.7.3/saffier/db/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/db/fields.py` & `saffier-0.7.3/saffier/db/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/db/manager.py` & `saffier-0.7.3/saffier/db/manager.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/db/queryset.py` & `saffier-0.7.3/saffier/db/queryset.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/db/query/protocols.py` & `saffier-0.7.3/saffier/db/query/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/base.py` & `saffier-0.7.3/saffier/migrations/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/cli.py` & `saffier-0.7.3/saffier/migrations/cli.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/env.py` & `saffier-0.7.3/saffier/migrations/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/__init__.py` & `saffier-0.7.3/saffier/migrations/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/branches.py` & `saffier-0.7.3/saffier/migrations/operations/branches.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/current.py` & `saffier-0.7.3/saffier/migrations/operations/current.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/downgrade.py` & `saffier-0.7.3/saffier/migrations/operations/downgrade.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/heads.py` & `saffier-0.7.3/saffier/migrations/operations/heads.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/history.py` & `saffier-0.7.3/saffier/migrations/operations/history.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/init.py` & `saffier-0.7.3/saffier/migrations/operations/init.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/makemigrations.py` & `saffier-0.7.3/saffier/migrations/operations/makemigrations.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/merge.py` & `saffier-0.7.3/saffier/migrations/operations/merge.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/migrate.py` & `saffier-0.7.3/saffier/migrations/operations/migrate.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/revision.py` & `saffier-0.7.3/saffier/migrations/operations/revision.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/stamp.py` & `saffier-0.7.3/saffier/migrations/operations/stamp.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/shell/base.py` & `saffier-0.7.3/saffier/migrations/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/shell/ipython.py` & `saffier-0.7.3/saffier/migrations/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/shell/ptpython.py` & `saffier-0.7.3/saffier/migrations/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/operations/shell/utils.py` & `saffier-0.7.3/saffier/migrations/operations/shell/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "BaseModel": pydantic.BaseModel,
         "BaseConfig": pydantic.BaseConfig,
         "settings": saffier.settings,
     }
 )
 
 
-def welcome_message(app: Any):
+def welcome_message(app: Any) -> None:
     """Displays the welcome message for the user"""
     now = datetime.datetime.now().strftime("%b %d %Y, %H:%M:%S")
     saffier_info_date = f"Saffier {saffier.__version__} (interactive shell, {now})"
     info = "Interactive shell that imports the application models and some python defaults."
 
     application_text = printer.message("Application: ", colour=OutputColour.CYAN3)
     application_name = printer.message(app.__class__.__name__, colour=OutputColour.GREEN3)
@@ -49,31 +49,32 @@
 
     def import_defaults():
         for name, module in defaults.items():
             directive = import_statement.format(module_path=module.__module__, model=name)
             printer.write_success(directive, colour=OutputColour.CYAN3)
             imported_objects[name] = module
 
-    def import_models():
-        # Creates a dict map with module path and model to import
-        printer.write_success("Models".center(79, "-"), colour=OutputColour.CYAN3)
-        for _, model in sorted(registry.models.items()):
+    def _import_objects(lookup_dict: Dict[Any, Any]) -> Any:
+        for _, model in sorted(lookup_dict.items()):
             directive = import_statement.format(module_path=model.__module__, model=model.__name__)
             printer.write_success(directive, colour=OutputColour.CYAN3)
             imported_objects[model.__name__] = model
 
+    def import_models():
+        if not registry.models:
+            return
+
+        printer.write_success("Models".center(79, "-"), colour=OutputColour.CYAN3)
+        _import_objects(registry.models)
+
     def import_reflected_models():
-        # Creates a dict map with module path and model to import
         if not registry.reflected:
             return
 
         printer.write_success("Reflected models".center(79, "-"), colour=OutputColour.CYAN3)
-        for _, model in sorted(registry.reflected.items()):
-            directive = import_statement.format(module_path=model.__module__, model=model.__name__)
-            printer.write_success(directive, colour=OutputColour.CYAN3)
-            imported_objects[model.__name__] = model
+        _import_objects(registry.reflected)
 
     import_defaults()
     import_models()
     import_reflected_models()
 
     return imported_objects
```

### Comparing `saffier-0.7.2/saffier/migrations/templates/default/alembic.ini.mako` & `saffier-0.7.3/saffier/migrations/templates/default/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/migrations/templates/default/env.py` & `saffier-0.7.3/saffier/migrations/templates/default/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/sqlalchemy/fields.py` & `saffier-0.7.3/saffier/sqlalchemy/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/saffier/sqlalchemy/protocols.py` & `saffier-0.7.3/saffier/sqlalchemy/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/LICENSE` & `saffier-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/README.md` & `saffier-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `saffier-0.7.2/pyproject.toml` & `saffier-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     "mdx-include>=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin>=0.1.7,<0.3.0",
     "mkdocstrings>=0.19.0,<0.21.0",
     "pyyaml>=5.3.1,<7.0.0",
 ]
 
 testing = ["sqlalchemy_utils>=0.40.0"]
-postgres = ["databasez[postgressql]"]
+postgres = ["databasez[postgresql]"]
 mysql = ["databasez[mysql]"]
 sqlite = ["databasez[sqlite]"]
 
 ptpython = ["ptpython>=3.0.23,<4.0.0"]
 ipython = ["ipython>=8.10.0,<9.0.0"]
 
 all = [
```

### Comparing `saffier-0.7.2/PKG-INFO` & `saffier-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saffier
-Version: 0.7.2
+Version: 0.7.3
 Summary: The only python ORM you will ever need.
 Project-URL: Homepage, https://github.com/tarsil/saffier
 Project-URL: Documentation, https://saffier.tarsild.io/
 Project-URL: Changelog, https://saffier.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/saffier
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -68,15 +68,15 @@
 Requires-Dist: mkdocstrings<0.21.0,>=0.19.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=5.3.1; extra == 'doc'
 Provides-Extra: ipython
 Requires-Dist: ipython<9.0.0,>=8.10.0; extra == 'ipython'
 Provides-Extra: mysql
 Requires-Dist: databasez[mysql]; extra == 'mysql'
 Provides-Extra: postgres
-Requires-Dist: databasez[postgressql]; extra == 'postgres'
+Requires-Dist: databasez[postgresql]; extra == 'postgres'
 Provides-Extra: ptpython
 Requires-Dist: ptpython<4.0.0,>=3.0.23; extra == 'ptpython'
 Provides-Extra: sqlite
 Requires-Dist: databasez[sqlite]; extra == 'sqlite'
 Provides-Extra: test
 Requires-Dist: asyncmy<0.3.0,>=0.2.7; extra == 'test'
 Requires-Dist: asyncpg<1,>=0.27.0; extra == 'test'
```

