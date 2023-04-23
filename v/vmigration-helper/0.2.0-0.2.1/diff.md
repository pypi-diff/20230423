# Comparing `tmp/vmigration_helper-0.2.0.tar.gz` & `tmp/vmigration_helper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmigration_helper-0.2.0.tar", max compression
+gzip compressed data, was "vmigration_helper-0.2.1.tar", max compression
```

## Comparing `vmigration_helper-0.2.0.tar` & `vmigration_helper-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2021-06-15 02:31:59.417332 vmigration_helper-0.2.0/LICENSE
--rw-r--r--   0        0        0     6250 2023-03-31 01:36:59.331626 vmigration_helper-0.2.0/README.md
--rw-r--r--   0        0        0      578 2023-03-31 07:00:28.819017 vmigration_helper-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-06-15 02:31:59.428646 vmigration_helper-0.2.0/vmigration_helper/__init__.py
--rw-r--r--   0        0        0      165 2021-06-21 02:44:18.433874 vmigration_helper-0.2.0/vmigration_helper/apps.py
--rw-r--r--   0        0        0        0 2023-03-22 05:48:58.166198 vmigration_helper-0.2.0/vmigration_helper/helpers/__init__.py
--rw-r--r--   0        0        0     1950 2023-03-31 02:03:24.501310 vmigration_helper-0.2.0/vmigration_helper/helpers/command.py
--rw-r--r--   0        0        0     3426 2023-03-31 01:39:36.011432 vmigration_helper-0.2.0/vmigration_helper/helpers/migration_records.py
--rw-r--r--   0        0        0        0 2021-06-15 02:31:59.431441 vmigration_helper-0.2.0/vmigration_helper/management/__init__.py
--rw-r--r--   0        0        0        0 2021-06-15 02:31:59.432096 vmigration_helper-0.2.0/vmigration_helper/management/commands/__init__.py
--rw-r--r--   0        0        0      872 2023-03-31 01:30:36.972945 vmigration_helper-0.2.0/vmigration_helper/management/commands/migration_current_id.py
--rw-r--r--   0        0        0     1889 2023-03-31 01:32:13.499983 vmigration_helper-0.2.0/vmigration_helper/management/commands/migration_delete.py
--rw-r--r--   0        0        0     2819 2023-03-31 01:32:01.406392 vmigration_helper-0.2.0/vmigration_helper/management/commands/migration_records.py
--rw-r--r--   0        0        0     3346 2023-03-31 01:31:44.660584 vmigration_helper-0.2.0/vmigration_helper/management/commands/migration_rollback.py
--rw-r--r--   0        0        0        0 2021-06-15 02:31:59.435089 vmigration_helper-0.2.0/vmigration_helper/migrations/__init__.py
--rw-r--r--   0        0        0     6906 1970-01-01 00:00:00.000000 vmigration_helper-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1084 2021-09-05 02:57:41.133752 vmigration_helper-0.2.1/LICENSE
+-rwxr-xr-x   0        0        0     6436 2023-04-02 02:56:46.322165 vmigration_helper-0.2.1/README.md
+-rwxr-xr-x   0        0        0      606 2023-04-23 03:59:13.893771 vmigration_helper-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2021-09-05 02:57:41.149378 vmigration_helper-0.2.1/vmigration_helper/__init__.py
+-rwxr-xr-x   0        0        0      171 2021-09-05 02:57:41.149378 vmigration_helper-0.2.1/vmigration_helper/apps.py
+-rwxr-xr-x   0        0        0        0 2023-03-26 20:31:46.863353 vmigration_helper-0.2.1/vmigration_helper/helpers/__init__.py
+-rwxr-xr-x   0        0        0     2002 2023-04-02 02:56:46.327188 vmigration_helper-0.2.1/vmigration_helper/helpers/command.py
+-rwxr-xr-x   0        0        0     3517 2023-04-02 02:56:46.328164 vmigration_helper-0.2.1/vmigration_helper/helpers/migration_records.py
+-rwxr-xr-x   0        0        0        0 2021-09-05 02:57:41.149378 vmigration_helper-0.2.1/vmigration_helper/management/__init__.py
+-rwxr-xr-x   0        0        0        0 2021-09-05 02:57:41.149378 vmigration_helper-0.2.1/vmigration_helper/management/commands/__init__.py
+-rwxr-xr-x   0        0        0      898 2023-04-02 02:56:46.329164 vmigration_helper-0.2.1/vmigration_helper/management/commands/migration_current_id.py
+-rwxr-xr-x   0        0        0     1942 2023-04-02 02:56:46.330166 vmigration_helper-0.2.1/vmigration_helper/management/commands/migration_delete.py
+-rwxr-xr-x   0        0        0     2895 2023-04-02 02:56:46.331179 vmigration_helper-0.2.1/vmigration_helper/management/commands/migration_records.py
+-rwxr-xr-x   0        0        0     3434 2023-04-02 02:56:46.332186 vmigration_helper-0.2.1/vmigration_helper/management/commands/migration_rollback.py
+-rwxr-xr-x   0        0        0        0 2021-09-05 02:57:41.149378 vmigration_helper-0.2.1/vmigration_helper/migrations/__init__.py
+-rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 vmigration_helper-0.2.1/PKG-INFO
```

### Comparing `vmigration_helper-0.2.0/README.md` & `vmigration_helper-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: vmigration-helper
+Version: 0.2.1
+Summary: Van's Django Migration Helper
+Home-page: https://github.com/bluedenim/vmigration-helper
+Keywords: django,migration,rollback
+Author: bluedenim
+Author-email: vancly@hotmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Django (>=1.11.17,<4)
+Description-Content-Type: text/markdown
+
 # Van's Migration Helper
 
 Django commands to help with running Django migrations.
 
 ## Installation
 
 * Add the dependency to your environment:
@@ -180,7 +198,8 @@
 * Run `migration_current_id` and capture the current ID
 * Run migration normally
 * Run your automated tests normally
   * If tests pass, you're done!
   * If tests fail, and you need to rollback, run
   `migration_rollback <captured ID>`
   
+
```

### Comparing `vmigration_helper-0.2.0/pyproject.toml` & `vmigration_helper-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[tool.poetry]
-name = "vmigration-helper"
-version = "0.2.0"
-homepage = "https://github.com/bluedenim/vmigration-helper"
-description = "Van's Django Migration Helper"
-authors = ["bluedenim <vancly@hotmail.com>"]
-readme = "README.md"
-packages = [
-    { include = "vmigration_helper" },
-]
-exclude = ["main"]
-keywords = ["django","migration","rollback"]
-
-[tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-Django = "^1.11.17"
-
-[tool.poetry.dev-dependencies]
-twine = "^3.4.1"
-wheel = "^0.36.2"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "vmigration-helper"
+version = "0.2.1"
+homepage = "https://github.com/bluedenim/vmigration-helper"
+description = "Van's Django Migration Helper"
+authors = ["bluedenim <vancly@hotmail.com>"]
+readme = "README.md"
+packages = [
+    { include = "vmigration_helper" },
+]
+exclude = ["main"]
+keywords = ["django","migration","rollback"]
+
+[tool.poetry.dependencies]
+python = ">=3.7,<4.0"
+Django = ">=1.11.17,<4"
+
+[tool.poetry.dev-dependencies]
+twine = "^3.4.1"
+wheel = "^0.36.2"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `vmigration_helper-0.2.0/vmigration_helper/helpers/command.py` & `vmigration_helper-0.2.1/vmigration_helper/helpers/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from abc import ABC
-
-from django.core.management import BaseCommand
-from django.db import connections, DEFAULT_DB_ALIAS
-from django.db.migrations.recorder import MigrationRecorder
-
-from vmigration_helper.helpers.migration_records import MigrationRecordsHelper
-
-
-class MigrationCommand(BaseCommand, ABC):
-    """
-    Abstract base class for migration commands in this app.
-
-    This class provides a place for common concerns to all migration commands to be implemented. For instance, it
-    registers the "connection-name" optional parameter to the command and surfaces the parameter as
-    the "connection_name" property.
-    """
-
-    def add_arguments(self, parser):
-        parser.add_argument(
-            '--connection-name',
-            default=DEFAULT_DB_ALIAS,
-            help=f'The connection to use for migration commands. Defaults to settings.DEFAULT_DB_ALIAS'
-        )
-
-    def execute(self, *args, **options):
-        self.connection_name = options["connection_name"]
-        super().execute(*args, **options)
-
-    def create_migration_helper(self, connection=None) -> MigrationRecordsHelper:
-        """
-        Initializes a connection and returns an instance of MigrationRecordsHelper initialized to the connection
-        provided.
-
-        :param connection: optional connection to use. If not provided, a connection to the current connection name
-            is created and used. If a connection is provided, its prepare_database() MUST have been called.
-
-        :returns: an instance of MigrationRecordsHelper
-        """
-        if not connection:
-            connection = connections[self.connection_name]
-            connection.prepare_database()
-        return MigrationRecordsHelper(MigrationRecorder(connection))
-
-    @property
-    def connection_name(self) -> str:
-        return self._connection_name
-
-    @connection_name.setter
-    def connection_name(self, value: str) -> None:
-        self._connection_name = value
+from abc import ABC
+
+from django.core.management import BaseCommand
+from django.db import connections, DEFAULT_DB_ALIAS
+from django.db.migrations.recorder import MigrationRecorder
+
+from vmigration_helper.helpers.migration_records import MigrationRecordsHelper
+
+
+class MigrationCommand(BaseCommand, ABC):
+    """
+    Abstract base class for migration commands in this app.
+
+    This class provides a place for common concerns to all migration commands to be implemented. For instance, it
+    registers the "connection-name" optional parameter to the command and surfaces the parameter as
+    the "connection_name" property.
+    """
+
+    def add_arguments(self, parser):
+        parser.add_argument(
+            '--connection-name',
+            default=DEFAULT_DB_ALIAS,
+            help=f'The connection to use for migration commands. Defaults to django.db.DEFAULT_DB_ALIAS'
+        )
+
+    def execute(self, *args, **options):
+        self.connection_name = options["connection_name"]
+        super().execute(*args, **options)
+
+    def create_migration_helper(self, connection=None) -> MigrationRecordsHelper:
+        """
+        Initializes a connection and returns an instance of MigrationRecordsHelper initialized to the connection
+        provided.
+
+        :param connection: optional connection to use. If not provided, a connection to the current connection name
+            is created and used. If a connection is provided, its prepare_database() MUST have been called.
+
+        :returns: an instance of MigrationRecordsHelper
+        """
+        if not connection:
+            connection = connections[self.connection_name]
+            connection.prepare_database()
+        return MigrationRecordsHelper(MigrationRecorder(connection))
+
+    @property
+    def connection_name(self) -> str:
+        return self._connection_name
+
+    @connection_name.setter
+    def connection_name(self, value: str) -> None:
+        self._connection_name = value
```

### Comparing `vmigration_helper-0.2.0/vmigration_helper/helpers/migration_records.py` & `vmigration_helper-0.2.1/vmigration_helper/helpers/migration_records.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from typing import List, Optional
-
-from django.db import connections, DEFAULT_DB_ALIAS
-from django.db.migrations.recorder import MigrationRecorder
-from django.db.models import QuerySet
-
-
-class MigrationRecordsHelper:
-    """
-    Helper for migration records
-    """
-
-    def __init__(self, migration_recorder: Optional[MigrationRecorder] = None) -> None:
-        if not migration_recorder:
-            connection = connections[DEFAULT_DB_ALIAS]
-            connection.prepare_database()
-
-            migration_recorder = MigrationRecorder(connection)
-        self.migration_recorder = migration_recorder
-
-    def get_migration_records_qs(self) -> QuerySet:
-        """
-        Gets a QuerySet from which MigrationRecorder.Migration records can be acquired.
-
-        Args:
-            migration_recorder - instance of MigrationRecorder used to get migration records
-        Returns:
-            query set to use to get migration records
-        """
-        return self.migration_recorder.migration_qs
-
-    def previous_migration(self, migration: MigrationRecorder.Migration) -> Optional[MigrationRecorder.Migration]:
-        """
-        Retrieve the previous migration record (based on the app and ID) from the DB if one exists.
-
-        :param migration_recorder: the MigrationRecorder instance to use to access migration records.
-        :param migration: the migration to retrieve the previous migration for.
-
-        :returns: the previous migration if one exists
-        """
-        return self.migration_recorder.migration_qs.filter(
-            app=migration.app, id__lt=migration.id
-        ).order_by('-id').first()
-
-    def delete_migration(self, app: str, name: str) -> bool:
-        """
-        Delete the migration matching the app and name given.
-
-        :returns: True if a record was deleted
-        """
-        deleted, _ = self.migration_recorder.migration_qs.filter(app=app, name=name).delete()
-        return deleted
-
-    @staticmethod
-    def squash_migrations(migrations: List[MigrationRecorder.Migration]) -> List[MigrationRecorder.Migration]:
-        """
-        Find contiguous migrations for the same app and squash them by omitting all but the last entry. The incoming
-        list, therefore, must be ordered such that the last entry of a contiguous group is the one to keep (e.g.
-        in descending order when rolling back).
-
-        For example:
-          input: app 1, migration 5
-                 app 1, migration 4
-                 app 1, migration 3
-                 app 2, migration 11
-                 app 2, migration 10
-
-          output: app 1, migration 3
-                  app 2, migration 10
-
-        :param migrations: the migrations to squash
-
-        :returns: the squashed migrations
-        """
-        lowest_migrations = []  # type: List[MigrationRecorder.Migration]
-        curr_app = None
-        curr_migration = None
-        for migration in migrations:
-            if curr_app is None:
-                curr_app = migration.app
-                curr_migration = migration
-            else:
-                if curr_app == migration.app:
-                    curr_migration = migration
-                else:
-                    lowest_migrations.append(curr_migration)
-                    curr_app = migration.app
-                    curr_migration = migration
-        if curr_migration:
-            lowest_migrations.append(curr_migration)
-        return lowest_migrations
+from typing import List, Optional
+
+from django.db import connections, DEFAULT_DB_ALIAS
+from django.db.migrations.recorder import MigrationRecorder
+from django.db.models import QuerySet
+
+
+class MigrationRecordsHelper:
+    """
+    Helper for migration records
+    """
+
+    def __init__(self, migration_recorder: Optional[MigrationRecorder] = None) -> None:
+        if not migration_recorder:
+            connection = connections[DEFAULT_DB_ALIAS]
+            connection.prepare_database()
+
+            migration_recorder = MigrationRecorder(connection)
+        self.migration_recorder = migration_recorder
+
+    def get_migration_records_qs(self) -> QuerySet:
+        """
+        Gets a QuerySet from which MigrationRecorder.Migration records can be acquired.
+
+        Args:
+            migration_recorder - instance of MigrationRecorder used to get migration records
+        Returns:
+            query set to use to get migration records
+        """
+        return self.migration_recorder.migration_qs
+
+    def previous_migration(self, migration: MigrationRecorder.Migration) -> Optional[MigrationRecorder.Migration]:
+        """
+        Retrieve the previous migration record (based on the app and ID) from the DB if one exists.
+
+        :param migration_recorder: the MigrationRecorder instance to use to access migration records.
+        :param migration: the migration to retrieve the previous migration for.
+
+        :returns: the previous migration if one exists
+        """
+        return self.migration_recorder.migration_qs.filter(
+            app=migration.app, id__lt=migration.id
+        ).order_by('-id').first()
+
+    def delete_migration(self, app: str, name: str) -> bool:
+        """
+        Delete the migration matching the app and name given.
+
+        :returns: True if a record was deleted
+        """
+        deleted, _ = self.migration_recorder.migration_qs.filter(app=app, name=name).delete()
+        return deleted
+
+    @staticmethod
+    def squash_migrations(migrations: List[MigrationRecorder.Migration]) -> List[MigrationRecorder.Migration]:
+        """
+        Find contiguous migrations for the same app and squash them by omitting all but the last entry. The incoming
+        list, therefore, must be ordered such that the last entry of a contiguous group is the one to keep (e.g.
+        in descending order when rolling back).
+
+        For example:
+          input: app 1, migration 5
+                 app 1, migration 4
+                 app 1, migration 3
+                 app 2, migration 11
+                 app 2, migration 10
+
+          output: app 1, migration 3
+                  app 2, migration 10
+
+        :param migrations: the migrations to squash
+
+        :returns: the squashed migrations
+        """
+        lowest_migrations = []  # type: List[MigrationRecorder.Migration]
+        curr_app = None
+        curr_migration = None
+        for migration in migrations:
+            if curr_app is None:
+                curr_app = migration.app
+                curr_migration = migration
+            else:
+                if curr_app == migration.app:
+                    curr_migration = migration
+                else:
+                    lowest_migrations.append(curr_migration)
+                    curr_app = migration.app
+                    curr_migration = migration
+        if curr_migration:
+            lowest_migrations.append(curr_migration)
+        return lowest_migrations
```

### Comparing `vmigration_helper-0.2.0/vmigration_helper/management/commands/migration_current_id.py` & `vmigration_helper-0.2.1/vmigration_helper/management/commands/migration_current_id.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from django.db import OperationalError
-from django.db.models import Max
-
-from vmigration_helper.helpers.command import MigrationCommand
-
-
-class Command(MigrationCommand):
-    """
-    Displays the ID of the last entry in the migration records (from the ``django_migrations`` table).
-    """
-
-    def create_snapshot_name(self) -> int:
-        """
-        Returns the current max ID of the migration records table (django_migrations). If there are no records,
-        0 is returned.
-        """
-        helper = self.create_migration_helper()
-        latest_migration_id = helper.get_migration_records_qs().aggregate(Max('id'))['id__max']
-        return latest_migration_id or 0
-
-    def handle(self, *args, **options):
-        try:
-            print(self.create_snapshot_name())
-        except OperationalError as e:
-            print(f'DB ERROR: {e}')
-            exit(1)
+from django.db import OperationalError
+from django.db.models import Max
+
+from vmigration_helper.helpers.command import MigrationCommand
+
+
+class Command(MigrationCommand):
+    """
+    Displays the ID of the last entry in the migration records (from the ``django_migrations`` table).
+    """
+
+    def create_snapshot_name(self) -> int:
+        """
+        Returns the current max ID of the migration records table (django_migrations). If there are no records,
+        0 is returned.
+        """
+        helper = self.create_migration_helper()
+        latest_migration_id = helper.get_migration_records_qs().aggregate(Max('id'))['id__max']
+        return latest_migration_id or 0
+
+    def handle(self, *args, **options):
+        try:
+            print(self.create_snapshot_name())
+        except OperationalError as e:
+            print(f'DB ERROR: {e}')
+            exit(1)
```

### Comparing `vmigration_helper-0.2.0/vmigration_helper/management/commands/migration_records.py` & `vmigration_helper-0.2.1/vmigration_helper/management/commands/migration_records.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from django.db import OperationalError
-from django.db.migrations.recorder import MigrationRecorder
-from django.db.models import QuerySet
-
-from vmigration_helper.helpers.command import MigrationCommand
-
-FORMAT_CSV = 'csv'
-FORMAT_CONSOLE = 'console'
-DATETIME_FORMAT = '%Y-%m-%dT%H:%M:%S%z'
-
-
-class Command(MigrationCommand):
-    """
-    Displays all the migration records (from the ``django_migrations`` table).
-
-    Optional parameter:
-        --format ("csv" | "console") show all the records of past migrations in CSV or human-friendly format (default)
-    """
-
-    @staticmethod
-    def _format_csv(record: MigrationRecorder.Migration) -> str:
-        return f"{record.id},{record.applied.strftime(DATETIME_FORMAT)},{record.app},{record.name}"
-
-    @staticmethod
-    def _format_console(record: MigrationRecorder.Migration, app_name_width: int) -> str:
-        return (
-            f"{str(record.id).rjust(6, ' ')} {record.applied.strftime(DATETIME_FORMAT).ljust(24, ' ')} "
-            f"{record.app.rjust(app_name_width, ' ')} {record.name}"
-        )
-
-    @staticmethod
-    def _format_header_console(app_name_width: int) -> str:
-        # alloc width 6 for IDs
-        # alloc width 24 for the date: YYYY-MM-DDTHH:MM:SSZZZZZ (DATETIME_FORMAT)
-        return (
-            f"{'ID'.rjust(6, ' ')} {'Applied'.ljust(24, ' ')} "
-            f"{'App'.rjust(app_name_width, ' ')} Name"
-        )
-
-    @staticmethod
-    def _find_max_app_name_width(migration_query_set: QuerySet) -> int:
-        widths = [len(m['app']) for m in migration_query_set.values('app').distinct()]
-        if widths:
-            return max(*widths)
-        return 0
-
-    def add_arguments(self, parser):
-        super().add_arguments(parser)
-        parser.add_argument(
-            '--format',
-            default=FORMAT_CONSOLE,
-            help=f'The format to display the migration records (csv or console). Default is: "{FORMAT_CONSOLE}"'
-        )
-
-    def handle(self, *args, **options):
-        print_format = options['format']
-        try:
-            helper = self.create_migration_helper()
-            migrations_queryset = helper.get_migration_records_qs().all()
-
-            app_name_width = 0
-            header = "ID,Applied,App,Name"
-            if print_format == FORMAT_CONSOLE:
-                app_name_width = max(self._find_max_app_name_width(migrations_queryset), 5)
-                header = self._format_header_console(app_name_width)
-
-            print(header)
-            for record in migrations_queryset:
-                if print_format == FORMAT_CSV:
-                    row = self._format_csv(record)
-                else:
-                    row = self._format_console(record, app_name_width)
-                print(row)
-        except OperationalError as e:
-            print(f'DB ERROR: {e}')
-            exit(1)
+from django.db import OperationalError
+from django.db.migrations.recorder import MigrationRecorder
+from django.db.models import QuerySet
+
+from vmigration_helper.helpers.command import MigrationCommand
+
+FORMAT_CSV = 'csv'
+FORMAT_CONSOLE = 'console'
+DATETIME_FORMAT = '%Y-%m-%dT%H:%M:%S%z'
+
+
+class Command(MigrationCommand):
+    """
+    Displays all the migration records (from the ``django_migrations`` table).
+
+    Optional parameter:
+        --format ("csv" | "console") show all the records of past migrations in CSV or human-friendly format (default)
+    """
+
+    @staticmethod
+    def _format_csv(record: MigrationRecorder.Migration) -> str:
+        return f"{record.id},{record.applied.strftime(DATETIME_FORMAT)},{record.app},{record.name}"
+
+    @staticmethod
+    def _format_console(record: MigrationRecorder.Migration, app_name_width: int) -> str:
+        return (
+            f"{str(record.id).rjust(6, ' ')} {record.applied.strftime(DATETIME_FORMAT).ljust(24, ' ')} "
+            f"{record.app.rjust(app_name_width, ' ')} {record.name}"
+        )
+
+    @staticmethod
+    def _format_header_console(app_name_width: int) -> str:
+        # alloc width 6 for IDs
+        # alloc width 24 for the date: YYYY-MM-DDTHH:MM:SSZZZZZ (DATETIME_FORMAT)
+        return (
+            f"{'ID'.rjust(6, ' ')} {'Applied'.ljust(24, ' ')} "
+            f"{'App'.rjust(app_name_width, ' ')} Name"
+        )
+
+    @staticmethod
+    def _find_max_app_name_width(migration_query_set: QuerySet) -> int:
+        widths = [len(m['app']) for m in migration_query_set.values('app').distinct()]
+        if widths:
+            return max(*widths)
+        return 0
+
+    def add_arguments(self, parser):
+        super().add_arguments(parser)
+        parser.add_argument(
+            '--format',
+            default=FORMAT_CONSOLE,
+            help=f'The format to display the migration records (csv or console). Default is: "{FORMAT_CONSOLE}"'
+        )
+
+    def handle(self, *args, **options):
+        print_format = options['format']
+        try:
+            helper = self.create_migration_helper()
+            migrations_queryset = helper.get_migration_records_qs().all()
+
+            app_name_width = 0
+            header = "ID,Applied,App,Name"
+            if print_format == FORMAT_CONSOLE:
+                app_name_width = max(self._find_max_app_name_width(migrations_queryset), 5)
+                header = self._format_header_console(app_name_width)
+
+            print(header)
+            for record in migrations_queryset:
+                if print_format == FORMAT_CSV:
+                    row = self._format_csv(record)
+                else:
+                    row = self._format_console(record, app_name_width)
+                print(row)
+        except OperationalError as e:
+            print(f'DB ERROR: {e}')
+            exit(1)
```

### Comparing `vmigration_helper-0.2.0/vmigration_helper/management/commands/migration_rollback.py` & `vmigration_helper-0.2.1/vmigration_helper/management/commands/migration_rollback.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-import subprocess
-from typing import List
-
-from django.db import OperationalError
-from django.db.migrations.recorder import MigrationRecorder
-
-from vmigration_helper.helpers.command import MigrationCommand
-
-MIGRATE_COMMAND = 'python manage.py migrate {app} {name}'
-
-
-class Command(MigrationCommand):
-    """
-    Rolls back migrations by unapplying entries in the migration records (django_migrations) whose IDs are greater
-    than the ID provided.
-
-    **NOTE**: the process is **NOT** atomic; As soon as any of the migrations fail, the process will halt. However,
-    successfully rolled-back migrations so far will remain rolled back.
-
-    For example, to roll back all migrations *after* ID 7::
-
-        python manage.py migration_rollback 7
-
-    Optional parameters:
-
-        * --dry-run
-            only print the commands; don't run them
-        * --migrate-cmd "command template"
-            use the template provided to invoke the migrations (default is "python manage.py migrate {app} {name}")
-            the placeholders "{app}" and "{name}" indicate the app name and migration file name, respectively
-
-        For example, to see the rollback commands using pipevn (without running them):
-
-        python manage.py migration_rollback 7 --dry-run --migrate-cmd "pipenv run python manage.py migrate {app} {name}"
-
-    """
-
-    def add_arguments(self, parser):
-        super().add_arguments(parser)
-        parser.add_argument(
-            'to_id',
-            type=int,
-            help=(
-                'The ID of the migration record to rollback to. '
-                'All migrations done after this ID will be rolled back. '
-                'Use "migration_records" to see all records.'
-            )
-        )
-
-        parser.add_argument(
-            '--dry-run',
-            action='store_true',
-            help=f'Show the commands that would have run but do not run them'
-        )
-
-        parser.add_argument(
-            '--migrate-cmd',
-            default=MIGRATE_COMMAND,
-            help=f'The migration command template (accepts {{app}} and {{name}}). Default is: "{MIGRATE_COMMAND}"'
-        )
-
-    def handle(self, *args, **options):
-        rollback_to_id = options['to_id']
-        dry_run = options['dry_run']
-        migrate_cmd = options['migrate_cmd']
-
-        try:
-            helper = self.create_migration_helper()
-            qs = helper.get_migration_records_qs().filter(id__gt=rollback_to_id).order_by('-id')
-            migration_records = list(qs)  # type: List[MigrationRecorder.Migration]
-            squashed_migrations = helper.squash_migrations(migration_records)
-            targets = []
-            for migration in squashed_migrations:
-                previous_migration = helper.previous_migration(migration)
-                if previous_migration:
-                    targets.append((migration.app, previous_migration.name))
-                else:
-                    targets.append((migration.app, 'zero'))
-
-            for target in targets:
-                command_to_run = migrate_cmd.format(app=target[0], name=target[1])
-                print(command_to_run)
-                if not dry_run:
-                    subprocess.run(command_to_run, check=True, shell=True)
-                    print()
-        except OperationalError as e:
-            print(f'DB ERROR: {e}')
-            exit(1)
+import subprocess
+from typing import List
+
+from django.db import OperationalError
+from django.db.migrations.recorder import MigrationRecorder
+
+from vmigration_helper.helpers.command import MigrationCommand
+
+MIGRATE_COMMAND = 'python manage.py migrate {app} {name}'
+
+
+class Command(MigrationCommand):
+    """
+    Rolls back migrations by unapplying entries in the migration records (django_migrations) whose IDs are greater
+    than the ID provided.
+
+    **NOTE**: the process is **NOT** atomic; As soon as any of the migrations fail, the process will halt. However,
+    successfully rolled-back migrations so far will remain rolled back.
+
+    For example, to roll back all migrations *after* ID 7::
+
+        python manage.py migration_rollback 7
+
+    Optional parameters:
+
+        * --dry-run
+            only print the commands; don't run them
+        * --migrate-cmd "command template"
+            use the template provided to invoke the migrations (default is "python manage.py migrate {app} {name}")
+            the placeholders "{app}" and "{name}" indicate the app name and migration file name, respectively
+
+        For example, to see the rollback commands using pipevn (without running them):
+
+        python manage.py migration_rollback 7 --dry-run --migrate-cmd "pipenv run python manage.py migrate {app} {name}"
+
+    """
+
+    def add_arguments(self, parser):
+        super().add_arguments(parser)
+        parser.add_argument(
+            'to_id',
+            type=int,
+            help=(
+                'The ID of the migration record to rollback to. '
+                'All migrations done after this ID will be rolled back. '
+                'Use "migration_records" to see all records.'
+            )
+        )
+
+        parser.add_argument(
+            '--dry-run',
+            action='store_true',
+            help=f'Show the commands that would have run but do not run them'
+        )
+
+        parser.add_argument(
+            '--migrate-cmd',
+            default=MIGRATE_COMMAND,
+            help=f'The migration command template (accepts {{app}} and {{name}}). Default is: "{MIGRATE_COMMAND}"'
+        )
+
+    def handle(self, *args, **options):
+        rollback_to_id = options['to_id']
+        dry_run = options['dry_run']
+        migrate_cmd = options['migrate_cmd']
+
+        try:
+            helper = self.create_migration_helper()
+            qs = helper.get_migration_records_qs().filter(id__gt=rollback_to_id).order_by('-id')
+            migration_records = list(qs)  # type: List[MigrationRecorder.Migration]
+            squashed_migrations = helper.squash_migrations(migration_records)
+            targets = []
+            for migration in squashed_migrations:
+                previous_migration = helper.previous_migration(migration)
+                if previous_migration:
+                    targets.append((migration.app, previous_migration.name))
+                else:
+                    targets.append((migration.app, 'zero'))
+
+            for target in targets:
+                command_to_run = migrate_cmd.format(app=target[0], name=target[1])
+                print(command_to_run)
+                if not dry_run:
+                    subprocess.run(command_to_run, check=True, shell=True)
+                    print()
+        except OperationalError as e:
+            print(f'DB ERROR: {e}')
+            exit(1)
```

### Comparing `vmigration_helper-0.2.0/PKG-INFO` & `vmigration_helper-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,205 +1,186 @@
-Metadata-Version: 2.1
-Name: vmigration-helper
-Version: 0.2.0
-Summary: Van's Django Migration Helper
-Home-page: https://github.com/bluedenim/vmigration-helper
-Keywords: django,migration,rollback
-Author: bluedenim
-Author-email: vancly@hotmail.com
-Requires-Python: >=3.7,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Django (>=1.11.17,<2.0.0)
-Description-Content-Type: text/markdown
-
-# Van's Migration Helper
-
-Django commands to help with running Django migrations.
-
-## Installation
-
-* Add the dependency to your environment:
-
-  ```
-  pip install vmigration-helper
-  ```
-
-* Add the app `vmgration_helper.apps.VMigrationHelperConfig` to your list of installed apps in your settings:
-
-  ```
-  INSTALLED_APPS = [
-    ...
-    'vmigration_helper.apps.VMigrationHelperConfig',
-    ...
-  ]
-  ```
-
-
-## Commands
-
-### migration_records
-
-Shows existing migration records in your `django_migration` table.
-
-```
-> python manage.py migration_records --format csv
-ID,Applied,App,Name
-175,2021-06-13T20:41:28.683900+00:00,contenttypes,0001_initial
-176,2021-06-13T20:41:28.717886+00:00,auth,0001_initial
-177,2021-06-13T20:41:28.742930+00:00,admin,0001_initial
-178,2021-06-13T20:41:28.761938+00:00,admin,0002_logentry_remove_auto_add
-179,2021-06-13T20:41:28.770319+00:00,admin,0003_logentry_add_action_flag_choices
-180,2021-06-13T20:41:28.791287+00:00,contenttypes,0002_remove_content_type_name
-...
-192,2021-06-13T20:41:28.991814+00:00,sessions,0001_initial
-```
-
-These are the records of migrations applied. The fields indicate:
-  * ID - the ID of the record
-  * Applied - when the migration was applied 
-  * App - name of the Django app
-  * Name - name of the migration 
-
-#### Optional parameters:
-
-  * `--format (console | csv)` print the info in CSV or friendlier console format (default)
-  * `--connection-name {connection}` the connection name to use (default is `django.db.DEFAULT_DB_ALIAS`)
-
-### migration_current_id
-
-Shows the ID of the latest migration record in your `django_migration` table.
-
-```
-> python manage.py migration_current_id
-192
-```
-
-192 is the ID of the latest record as shown above.
-
-#### Optional parameters:
-
-  * `--connection-name {connection}` the connection name to use (default is `django.db.DEFAULT_DB_ALIAS`)
-
-### migration_rollback
-
-Roll-back (unapply) previously applied migrations _after_ (but not including) the migration ID provided.
-
-```
-> python manage.py migration_rollback 176
-```
-
-The above will rollback migrations after `0001_initial` of the `auth` app:
-
-```
-python manage.py migrate sessions zero
-Operations to perform:
-  Unapply all migrations: sessions
-Running migrations:
-  Rendering model states... DONE
-  Unapplying sessions.0001_initial... OK
-
-python manage.py migrate auth 0001_initial
-Operations to perform:
-  Target specific migration: 0001_initial, from auth
-Running migrations:
-  Rendering model states... DONE
-  Unapplying auth.0012_alter_user_first_name_max_length... OK
-  Unapplying auth.0011_update_proxy_permissions... OK
-  Unapplying auth.0010_alter_group_name_max_length... OK
-  Unapplying auth.0009_alter_user_last_name_max_length... OK
-  Unapplying auth.0008_alter_user_username_max_length... OK
-  Unapplying auth.0007_alter_validators_add_error_messages... OK
-  Unapplying auth.0006_require_contenttypes_0002... OK
-  Unapplying auth.0005_alter_user_last_login_null... OK
-  Unapplying auth.0004_alter_user_username_opts... OK
-  Unapplying auth.0003_alter_user_email_max_length... OK
-  Unapplying auth.0002_alter_permission_name_max_length... OK
-
-python manage.py migrate contenttypes 0001_initial
-Operations to perform:
-  Target specific migration: 0001_initial, from contenttypes
-Running migrations:
-  Rendering model states... DONE
-  Unapplying contenttypes.0002_remove_content_type_name... OK
-
-python manage.py migrate admin zero
-Operations to perform:
-  Unapply all migrations: admin
-Running migrations:
-  Rendering model states... DONE
-  Unapplying admin.0003_logentry_add_action_flag_choices... OK
-  Unapplying admin.0002_logentry_remove_auto_add... OK
-  Unapplying admin.0001_initial... OK
-```
-
-#### Optional parameters:
-
-  * `--connection-name {connection}` the connection name to use (default is `django.db.DEFAULT_DB_ALIAS`)
-  * `--dry-run` will print the commands but will not actually run them
-  * `--migrate-cmd <command to run migrations>` sets the command to run migrations with. The command must accept 
-    the app and migration name as the `{app}` and `{name}` placeholders, respectively.  
-    
-    For example:
-    
-    ```
-    --migrate-cmd "pipenv run python manage.py migrate {app} {name}" 
-    ```
-    
-    can be used to have the command run migrations using `pipenv`.
-
-    For example:
-
-    ```
-    > pipenv run python manage.py migration_rollback 0 --dry-run --migrate-cmd "pipenv run python manage.py migrate {app} {name}"
-    pipenv run python manage.py migrate sessions zero
-    pipenv run python manage.py migrate auth 0001_initial
-    pipenv run python manage.py migrate contenttypes 0001_initial
-    pipenv run python manage.py migrate admin zero
-    pipenv run python manage.py migrate auth zero
-    pipenv run python manage.py migrate contenttypes zero
-    ```
-
-### migration_delete
-
-Deletes an entry from Django's migration records. This command should be
-used only as a last resort to fix up migration records that cannot be rolled back. No migration up/down is performed; 
-the record is simply removed from `django_migrations`.
-
-NOTE also that migrations that depend on the record being deleted will be "broken" after the deletion, so this 
-command should only be run on "leaf" migration records unless you plan to also delete other migration records that
-depend on the one being deleted.
-
-```
-python manage.py migration_delete myapp 0003_some_migration
-Confirm deletion of myapp:0003_some_migration (yes or no): yes
-```
-The command above deletes the migration `0003_some_migration` for the app `myapp` (after
-getting confirmation).
-
-To delete without confirmation, use the `--yes` option:
-```
-python manage.py migration_delete myapp 0003_some_migration --yes
-```
-
-#### Optional parameters:
-  * `--connection-name {connection}` the connection name to use (default is `django.db.DEFAULT_DB_ALIAS`)
-  * `--yes` will proceed to deleting the record without asking for confirmation
-
-
-## Ideas for automation
-
-Here's an idea for automating the deployment of your Django app using these utilities:
-
-* Deploy new code
-* Run `migration_current_id` and capture the current ID
-* Run migration normally
-* Run your automated tests normally
-  * If tests pass, you're done!
-  * If tests fail, and you need to rollback, run
-  `migration_rollback <captured ID>`
-  
-
+# Van's Migration Helper
+
+Django commands to help with running Django migrations.
+
+## Installation
+
+* Add the dependency to your environment:
+
+  ```
+  pip install vmigration-helper
+  ```
+
+* Add the app `vmgration_helper.apps.VMigrationHelperConfig` to your list of installed apps in your settings:
+
+  ```
+  INSTALLED_APPS = [
+    ...
+    'vmigration_helper.apps.VMigrationHelperConfig',
+    ...
+  ]
+  ```
+
+
+## Commands
+
+### migration_records
+
+Shows existing migration records in your `django_migration` table.
+
+```
+> python manage.py migration_records --format csv
+ID,Applied,App,Name
+175,2021-06-13T20:41:28.683900+00:00,contenttypes,0001_initial
+176,2021-06-13T20:41:28.717886+00:00,auth,0001_initial
+177,2021-06-13T20:41:28.742930+00:00,admin,0001_initial
+178,2021-06-13T20:41:28.761938+00:00,admin,0002_logentry_remove_auto_add
+179,2021-06-13T20:41:28.770319+00:00,admin,0003_logentry_add_action_flag_choices
+180,2021-06-13T20:41:28.791287+00:00,contenttypes,0002_remove_content_type_name
+...
+192,2021-06-13T20:41:28.991814+00:00,sessions,0001_initial
+```
+
+These are the records of migrations applied. The fields indicate:
+  * ID - the ID of the record
+  * Applied - when the migration was applied 
+  * App - name of the Django app
+  * Name - name of the migration 
+
+#### Optional parameters:
+
+  * `--format (console | csv)` print the info in CSV or friendlier console format (default)
+  * `--connection-name {connection}` the connection name to use (default is `django.db.DEFAULT_DB_ALIAS`)
+
+### migration_current_id
+
+Shows the ID of the latest migration record in your `django_migration` table.
+
+```
+> python manage.py migration_current_id
+192
+```
+
+192 is the ID of the latest record as shown above.
+
+#### Optional parameters:
+
+  * `--connection-name {connection}` the connection name to use (default is `django.db.DEFAULT_DB_ALIAS`)
+
+### migration_rollback
+
+Roll-back (unapply) previously applied migrations _after_ (but not including) the migration ID provided.
+
+```
+> python manage.py migration_rollback 176
+```
+
+The above will rollback migrations after `0001_initial` of the `auth` app:
+
+```
+python manage.py migrate sessions zero
+Operations to perform:
+  Unapply all migrations: sessions
+Running migrations:
+  Rendering model states... DONE
+  Unapplying sessions.0001_initial... OK
+
+python manage.py migrate auth 0001_initial
+Operations to perform:
+  Target specific migration: 0001_initial, from auth
+Running migrations:
+  Rendering model states... DONE
+  Unapplying auth.0012_alter_user_first_name_max_length... OK
+  Unapplying auth.0011_update_proxy_permissions... OK
+  Unapplying auth.0010_alter_group_name_max_length... OK
+  Unapplying auth.0009_alter_user_last_name_max_length... OK
+  Unapplying auth.0008_alter_user_username_max_length... OK
+  Unapplying auth.0007_alter_validators_add_error_messages... OK
+  Unapplying auth.0006_require_contenttypes_0002... OK
+  Unapplying auth.0005_alter_user_last_login_null... OK
+  Unapplying auth.0004_alter_user_username_opts... OK
+  Unapplying auth.0003_alter_user_email_max_length... OK
+  Unapplying auth.0002_alter_permission_name_max_length... OK
+
+python manage.py migrate contenttypes 0001_initial
+Operations to perform:
+  Target specific migration: 0001_initial, from contenttypes
+Running migrations:
+  Rendering model states... DONE
+  Unapplying contenttypes.0002_remove_content_type_name... OK
+
+python manage.py migrate admin zero
+Operations to perform:
+  Unapply all migrations: admin
+Running migrations:
+  Rendering model states... DONE
+  Unapplying admin.0003_logentry_add_action_flag_choices... OK
+  Unapplying admin.0002_logentry_remove_auto_add... OK
+  Unapplying admin.0001_initial... OK
+```
+
+#### Optional parameters:
+
+  * `--connection-name {connection}` the connection name to use (default is `django.db.DEFAULT_DB_ALIAS`)
+  * `--dry-run` will print the commands but will not actually run them
+  * `--migrate-cmd <command to run migrations>` sets the command to run migrations with. The command must accept 
+    the app and migration name as the `{app}` and `{name}` placeholders, respectively.  
+    
+    For example:
+    
+    ```
+    --migrate-cmd "pipenv run python manage.py migrate {app} {name}" 
+    ```
+    
+    can be used to have the command run migrations using `pipenv`.
+
+    For example:
+
+    ```
+    > pipenv run python manage.py migration_rollback 0 --dry-run --migrate-cmd "pipenv run python manage.py migrate {app} {name}"
+    pipenv run python manage.py migrate sessions zero
+    pipenv run python manage.py migrate auth 0001_initial
+    pipenv run python manage.py migrate contenttypes 0001_initial
+    pipenv run python manage.py migrate admin zero
+    pipenv run python manage.py migrate auth zero
+    pipenv run python manage.py migrate contenttypes zero
+    ```
+
+### migration_delete
+
+Deletes an entry from Django's migration records. This command should be
+used only as a last resort to fix up migration records that cannot be rolled back. No migration up/down is performed; 
+the record is simply removed from `django_migrations`.
+
+NOTE also that migrations that depend on the record being deleted will be "broken" after the deletion, so this 
+command should only be run on "leaf" migration records unless you plan to also delete other migration records that
+depend on the one being deleted.
+
+```
+python manage.py migration_delete myapp 0003_some_migration
+Confirm deletion of myapp:0003_some_migration (yes or no): yes
+```
+The command above deletes the migration `0003_some_migration` for the app `myapp` (after
+getting confirmation).
+
+To delete without confirmation, use the `--yes` option:
+```
+python manage.py migration_delete myapp 0003_some_migration --yes
+```
+
+#### Optional parameters:
+  * `--connection-name {connection}` the connection name to use (default is `django.db.DEFAULT_DB_ALIAS`)
+  * `--yes` will proceed to deleting the record without asking for confirmation
+
+
+## Ideas for automation
+
+Here's an idea for automating the deployment of your Django app using these utilities:
+
+* Deploy new code
+* Run `migration_current_id` and capture the current ID
+* Run migration normally
+* Run your automated tests normally
+  * If tests pass, you're done!
+  * If tests fail, and you need to rollback, run
+  `migration_rollback <captured ID>`
+
```

