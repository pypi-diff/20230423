# Comparing `tmp/mtsql-1.3.202304072016-py3-none-any.whl.zip` & `tmp/mtsql-1.4.202304230628-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 18946 bytes, number of entries: 11
+Zip file size: 19131 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       44 b- defN 23-Jan-22 22:24 mt/sql/__init__.py
--rw-r--r--  2.0 unx     9605 b- defN 23-Feb-28 20:18 mt/sql/base.py
+-rw-r--r--  2.0 unx     9989 b- defN 23-Apr-23 06:23 mt/sql/base.py
 -rw-r--r--  2.0 unx     4894 b- defN 23-Feb-15 11:50 mt/sql/mysql.py
--rw-r--r--  2.0 unx    61173 b- defN 23-Apr-07 20:16 mt/sql/psql.py
+-rw-r--r--  2.0 unx    64376 b- defN 23-Apr-23 06:28 mt/sql/psql.py
 -rw-r--r--  2.0 unx     8678 b- defN 23-Feb-23 10:22 mt/sql/sqlite.py
--rw-r--r--  2.0 unx      396 b- defN 23-Apr-07 20:16 mt/sql/version.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Apr-07 20:17 mtsql-1.3.202304072016.dist-info/LICENSE
--rw-r--r--  2.0 unx      597 b- defN 23-Apr-07 20:17 mtsql-1.3.202304072016.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 20:17 mtsql-1.3.202304072016.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 23-Apr-07 20:17 mtsql-1.3.202304072016.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      863 b- defN 23-Apr-07 20:17 mtsql-1.3.202304072016.dist-info/RECORD
-11 files, 87415 bytes uncompressed, 17492 bytes compressed:  80.0%
+-rw-r--r--  2.0 unx      396 b- defN 23-Apr-23 06:28 mt/sql/version.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Apr-23 06:29 mtsql-1.4.202304230628.dist-info/LICENSE
+-rw-r--r--  2.0 unx      597 b- defN 23-Apr-23 06:29 mtsql-1.4.202304230628.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 06:29 mtsql-1.4.202304230628.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-Apr-23 06:29 mtsql-1.4.202304230628.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      863 b- defN 23-Apr-23 06:29 mtsql-1.4.202304230628.dist-info/RECORD
+11 files, 91002 bytes uncompressed, 17677 bytes compressed:  80.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: mt/sql/sqlite.py
 Comment: 
 
 Filename: mt/sql/version.py
 Comment: 
 
-Filename: mtsql-1.3.202304072016.dist-info/LICENSE
+Filename: mtsql-1.4.202304230628.dist-info/LICENSE
 Comment: 
 
-Filename: mtsql-1.3.202304072016.dist-info/METADATA
+Filename: mtsql-1.4.202304230628.dist-info/METADATA
 Comment: 
 
-Filename: mtsql-1.3.202304072016.dist-info/WHEEL
+Filename: mtsql-1.4.202304230628.dist-info/WHEEL
 Comment: 
 
-Filename: mtsql-1.3.202304072016.dist-info/top_level.txt
+Filename: mtsql-1.4.202304230628.dist-info/top_level.txt
 Comment: 
 
-Filename: mtsql-1.3.202304072016.dist-info/RECORD
+Filename: mtsql-1.4.202304230628.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mt/sql/base.py

```diff
@@ -1,17 +1,15 @@
 """Base functions dealing with an SQL database."""
 
-import typing as tp
-
 import sqlalchemy as sa
 import sqlalchemy.exc as se
 import psycopg2 as ps
 from halo import Halo
 
-from mt import pd, ctx
+from mt import tp, logg, pd, ctx
 from mt.base import deprecated_func
 
 
 __all__ = [
     "frame_sql",
     "run_func",
     "conn_ctx",
@@ -27,26 +25,32 @@
 def frame_sql(frame_name, schema: tp.Optional[str] = None):
     return frame_name if schema is None else "{}.{}".format(schema, frame_name)
 
 
 # ----- functions dealing with sql queries to overcome OperationalError -----
 
 
-def run_func(func, *args, nb_trials: int = 3, logger=None, **kwargs):
+def run_func(
+    func,
+    *args,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
+    **kwargs
+):
     """Attempt to run a function a number of times to overcome OperationalError exceptions.
 
     Parameters
     ----------
     func: function
         function to be invoked
     args: sequence
         arguments to be passed to the function
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
     kwargs: dict
         keyword arguments to be passed to the function
     """
     for x in range(nb_trials):
         try:
             return func(*args, **kwargs)
@@ -88,15 +92,15 @@
 def read_sql(
     sql,
     engine,
     index_col: tp.Union[str, tp.List[str], None] = None,
     chunksize: tp.Optional[int] = None,
     nb_trials: int = 3,
     exception_handling: str = "raise",
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
     **kwargs
 ) -> pd.DataFrame:
     """Read an SQL query with a number of trials to overcome OperationalError.
 
     The function wraps :func:`pandas.read_sql_query`. However, when `chunksize` is not None, it
     iterates over chunks and concatenates them. In addition, if `logger` is not None, a progress
     bar is shown in that case.
@@ -119,15 +123,15 @@
         number of query trials. If `chunksize` is provided, this is only effective before an
         iterator is returned from pandas.
     exception_handling : {'warn', 'raise'}
         policy for handling SQL-raised exceptions when iterating over many chunks to completely
         download the result. Only valid when `chunksize` is provided. Right now there are only
         2 policies. Either to raise the exception as-is ('raise'), or to raise the exception as a
         warning ('warn') and return whatever has been downloaded.
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
     kwargs: dict
         other keyword arguments to be passed directly to :func:`pandas.read_sql_query`
 
     Returns
     -------
     pandas.DataFrame
@@ -204,15 +208,15 @@
 )
 def read_sql_query(
     sql,
     engine,
     index_col=None,
     set_index_after=False,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
     **kwargs
 ):
     """Read an SQL query with a number of trials to overcome OperationalError.
 
     Parameters
     ----------
     sql : str
@@ -222,15 +226,15 @@
     index_col: string or list of strings, optional, default: None
         Column(s) to set as index(MultiIndex). See :func:`pandas.read_sql_query`.
     set_index_after: bool
         whether to set index specified by index_col via the pandas.read_sql_query() function or
         after the function has been invoked
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
     kwargs: dict
         other keyword arguments to be passed directly to :func:`pandas.read_sql_query`
 
     See Also
     --------
     pandas.read_sql_query
@@ -246,26 +250,32 @@
         **kwargs
     )
     if index_col is None or not set_index_after:
         return df
     return df.set_index(index_col, drop=True)
 
 
-def read_sql_table(table_name, engine, nb_trials: int = 3, logger=None, **kwargs):
+def read_sql_table(
+    table_name,
+    engine,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
+    **kwargs
+):
     """Read an SQL table with a number of trials to overcome OperationalError.
 
     Parameters
     ----------
     table_name : str
         name of the table to be read
     engine : sqlalchemy.engine.Engine
         connection engine to the server
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     See Also
     --------
     pandas.read_sql_table
 
     """
@@ -275,30 +285,41 @@
         engine,
         nb_trials=nb_trials,
         logger=logger,
         **kwargs
     )
 
 
-def exec_sql(sql, engine, *args, nb_trials: int = 3, logger=None, **kwargs):
-    """Execute an SQL query with a number of trials to overcome OperationalError. See :func:`sqlalchemy.engine.Engine.execute` for more details.
+def exec_sql(
+    sql,
+    engine,
+    *args,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
+    **kwargs
+):
+    """Execute an SQL query with a number of trials to overcome OperationalError.
 
     Parameters
     ----------
     sql : str
         SQL query to be executed
     engine : sqlalchemy.engine.Engine
         connection engine to the server
     args : list
         positional arguments to be passed as-is to :func:`sqlalchemy.engine.Engine.execute`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
+    See Also
+    --------
+    sqlalchemy.engine.Engine.execute
+        for more details
     """
 
     return run_func(
         engine_execute, engine, sql, *args, nb_trials=nb_trials, logger=logger, **kwargs
     )
```

## mt/sql/psql.py

```diff
@@ -1,18 +1,16 @@
 """Useful modules for accessing PostgreSQL"""
 
-from typing import Optional
-
 import sqlalchemy as sa
 import re
 import psycopg2 as ps
 import sqlalchemy.exc as se
 from tqdm import tqdm  # nice progress bar
 
-from mt import pd, np
+from mt import tp, logg, pd, np
 import mt.base.path as _p
 from mt.base.bg_invoke import BgInvoke
 from mt.base.with_utils import dummy_scope
 
 from .base import *
 
 
@@ -34,14 +32,15 @@
     "get_frame_dependencies",
     "get_view_sql_code",
     "rename_table",
     "drop_table",
     "rename_view",
     "drop_view",
     "rename_matview",
+    "refresh_matview",
     "drop_matview",
     "frame_exists",
     "drop_frame",
     "list_columns_ext",
     "list_columns",
     "list_primary_columns_ext",
     "list_primary_columns",
@@ -52,23 +51,24 @@
     "writesync_table",
 ]
 
 
 # ----- debugging functions -----
 
 
-def pg_get_locked_transactions(engine, schema: Optional[str] = None):
+def pg_get_locked_transactions(engine, schema: tp.Optional[str] = None):
     """Obtains a dataframe representing transactions which have been locked by the server.
 
     Parameters
     ----------
     engine: sqlalchemy.engine.Engine
         connection engine
     schema: str or None
-        If None, then all schemas are considered and not just the public schema. Else, scope down to a single schema.
+        If None, then all schemas are considered and not just the public schema. Else, scope down
+        to a single schema.
 
     Returns
     -------
     pd.DataFrame
         A table containing the current backend transactions
     """
     if schema is None:
@@ -105,24 +105,29 @@
     pid: int
         the backend pid to be cancelled
     """
     query_str = "SELECT pg_cancel_backend('{}');".format(pid)
     return read_sql(sa.text(query_str), engine)
 
 
-def pg_cancel_all_backends(engine, schema: Optional[str] = None, logger=None):
+def pg_cancel_all_backends(
+    engine,
+    schema: tp.Optional[str] = None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
+):
     """Cancels all backend transactions.
 
     Parameters
     ----------
     engine: sqlalchemy.engine.Engine
         connection engine
     schema: str or None
-        If None, then all schemas are considered and not just the public schema. Else, scope down to a single schema.
-    logger: logging.Logger or None
+        If None, then all schemas are considered and not just the public schema. Else, scope down
+        to a single schema.
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
     """
     df = pg_get_locked_transactions(engine, schema=schema)
     pids = df["pid"].drop_duplicates().tolist()
     for pid in pids:
         if logger:
             logger.info("Cancelling backend pid {}".format(pid))
@@ -134,16 +139,29 @@
 
 def indices(df):
     """Returns the list of named indices of the dataframe, ignoring any unnamed index."""
     a = list(df.index.names)
     return a if a != [None] else []
 
 
-def compliance_check(df):
-    """Checks if a dataframe is compliant to PSQL. It must have no index, or indices which do not match with any column. Raises ValueError when an error is encountered."""
+def compliance_check(df: pd.DataFrame):
+    """Checks if a dataframe is compliant to PSQL.
+
+    It must have no index, or indices which do not match with any column.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        the input dataframe
+
+    Raises
+    ------
+    ValueError
+        when an error is encountered.
+    """
     for x in indices(df):
         if x in df.columns:
             raise ValueError(
                 "Index '{}' appears as a non-primary column as well".format(x)
             )
 
 
@@ -179,46 +197,55 @@
     return s2
 
 
 def to_sql(
     df,
     name,
     engine,
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     if_exists="fail",
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
     **kwargs,
 ):
-    """Writes records stored in a DataFrame to an SQL database, with a number of trials to overcome OperationalError.
+    """Writes records stored in a DataFrame to an SQL database.
+
+    With a number of trials to overcome OperationalError.
 
     Parameters
     ----------
     df : pandas.DataFrame
         dataframe to be sent to the server
     name : str
         name of the table to be written to
     engine : sqlalchemy.engine.Engine
         connection engine to the server
     schema: string, optional
         Specify the schema. If None, use default schema.
     if_exists: str
-        what to do when the table exists. Beside all options available from pandas.to_sql(), a new option called 'gently_replace' is introduced, in which it will avoid dropping the table by trying to delete all entries and then inserting new entries. But it will only do so if the remote table contains exactly all the columns that the local dataframe has, and vice-versa.
+        what to do when the table exists. Beside all options available from pandas.to_sql(), a new
+        option called 'gently_replace' is introduced, in which it will avoid dropping the table by
+        trying to delete all entries and then inserting new entries. But it will only do so if the
+        remote table contains exactly all the columns that the local dataframe has, and vice-versa.
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Raises
     ------
     sqlalchemy.exc.ProgrammingError if the local and remote frames do not have the same structure
 
     Notes
     -----
-    The original pandas.DataFrame.to_sql() function does not turn any index into a primary key in PSQL. This function attempts to fix that problem. It takes as input a PSQL-compliant dataframe (see `compliance_check()`). It ignores any input `index` or `index_label` keyword. Instead, it considers 2 cases. If the dataframe's has an index or indices, then the tuple of all indices is turned into the primary key. If not, there is no primary key and no index is uploaded.
+    The original pandas.DataFrame.to_sql() function does not turn any index into a primary key in
+    PSQL. This function attempts to fix that problem. It takes as input a PSQL-compliant dataframe
+    (see `compliance_check()`). It ignores any input `index` or `index_label` keyword. Instead, it
+    considers 2 cases. If the dataframe's has an index or indices, then the tuple of all indices is
+    turned into the primary key. If not, there is no primary key and no index is uploaded.
 
     See Also
     --------
     pandas.DataFrame.to_sql()
 
     """
 
@@ -330,50 +357,61 @@
         **kwargs,
     )
 
 
 # ----- simple functions -----
 
 
-def rename_schema(old_schema, new_schema, engine, nb_trials: int = 3, logger=None):
+def rename_schema(
+    old_schema,
+    new_schema,
+    engine,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
+):
     """Renames a schema.
 
     Parameters
     ----------
     old_schema: str
         old schema name
     new_schema: str
         new schema name
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
     """
     exec_sql(
         'ALTER SCHEMA "{}" RENAME TO "{}";'.format(old_schema, new_schema),
         engine,
         nb_trials=nb_trials,
         logger=logger,
     )
 
 
-def list_views(engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None):
+def list_views(
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
+):
     """Lists all views of a given schema.
 
     Parameters
     ----------
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     out: list
         list of all view names
     """
@@ -386,27 +424,30 @@
             )
         )
     df = read_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
     return df["viewname"].tolist()
 
 
 def list_matviews(
-    engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Lists all materialized views of a given schema.
 
     Parameters
     ----------
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     out: list
         list of all materialized view names
     """
@@ -418,27 +459,30 @@
         )
     )
     df = read_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
     return df["matviewname"].tolist()
 
 
 def list_foreign_tables(
-    engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Lists all foreign tables of a given schema.
 
     Parameters
     ----------
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     out: list
         list of all materialized view names
     """
@@ -446,26 +490,31 @@
         schema = "public"
     query_str = f"SELECT foreign_table_name FROM information_schema.foreign_tables WHERE foreign_table_schema='{schema}';"
 
     df = read_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
     return df["foreign_table_name"].tolist()
 
 
-def list_frames(engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None):
+def list_frames(
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
+):
     """Lists all dataframes (tables/views/materialized views/foreign tables) of a given schema.
 
     Parameters
     ----------
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     out: pd.DataFrame(columns=['name', 'type'])
         list of all dataframes of types {'table', 'view', 'matview'}
     """
@@ -482,25 +531,28 @@
         engine, schema=schema, nb_trials=nb_trials, logger=logger
     ):
         data.append((item, "foreign_table"))
     return pd.DataFrame(data=data, columns=["name", "type"])
 
 
 def list_all_frames(
-    engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Lists all dataframes (tables/views/materialized views/foreign tables) across all schemas.
 
     Parameters
     ----------
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     out: pd.DataFrame(columns=['name', 'schema', 'type'])
         list of all dataframes of types {'table', 'view', 'matview'}
     """
@@ -510,27 +562,31 @@
         if len(df) > 0:
             df["schema"] = schema
             dfs.append(df)
     return pd.concat(dfs, sort=False).reset_index(drop=True)
 
 
 def get_frame_length(
-    frame_name, engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None
+    frame_name,
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Gets the number of rows of a dataframes (tables/views/materialized views).
 
     Parameters
     ----------
     frame_name: str
         name of the dataframe
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     out: int
         number of rows
 
@@ -544,15 +600,19 @@
         engine,
         nb_trials=nb_trials,
         logger=logger,
     )["a"][0]
 
 
 def get_frame_dependencies(
-    frame_name, engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None
+    frame_name,
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Gets the list of all frames that depend on the given frame."""
     query_str = """
         SELECT dependent_ns.nspname as dependent_schema
         , dependent_view.relname as dependent_view
         , source_ns.nspname as source_schema
         , source_table.relname as source_table
@@ -573,29 +633,33 @@
     """.format(
         "public" if schema is None else schema, frame_name
     )
     return read_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
 
 
 def get_view_sql_code(
-    view_name, engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None
+    view_name,
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Gets the SQL string of a view.
 
     Parameters
     ----------
     view_name: str
         view name
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     retval: str
         SQL query string defining the view
     """
@@ -609,17 +673,17 @@
     )["a"][0]
 
 
 def rename_table(
     old_table_name,
     new_table_name,
     engine,
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Renames a table of a schema.
 
     Parameters
     ----------
     old_table_name: str
         old table name
@@ -627,15 +691,15 @@
         new table name
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     whatever exec_sql() returns
     """
     frame_sql_str = frame_sql(old_table_name, schema=schema)
@@ -646,34 +710,36 @@
         logger=logger,
     )
 
 
 def drop_table(
     table_name,
     engine,
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     restrict=True,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Drops a table if it exists, with restrict or cascade options.
 
     Parameters
     ----------
     table_name : str
         table name
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     restrict: bool
-        If True, refuses to drop table if there is any object depending on it. Otherwise it is the 'cascade' option which allows you to remove those dependent objects together with the table automatically.
+        If True, refuses to drop table if there is any object depending on it. Otherwise it is the
+        'cascade' option which allows you to remove those dependent objects together with the table
+        automatically.
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     whatever exec_sql() returns
     """
     frame_sql_str = frame_sql(table_name, schema=schema)
@@ -683,17 +749,17 @@
     return exec_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
 
 
 def rename_view(
     old_view_name,
     new_view_name,
     engine,
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Renames a view of a schema.
 
     Parameters
     ----------
     old_view_name: str
         old view name
@@ -701,49 +767,51 @@
         new view name
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
     """
     frame_sql_str = frame_sql(old_view_name, schema=schema)
     exec_sql(
         'ALTER VIEW {} RENAME TO "{}";'.format(frame_sql_str, new_view_name),
         engine,
         nb_trials=nb_trials,
         logger=logger,
     )
 
 
 def drop_view(
     view_name,
     engine,
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     restrict=True,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Drops a view if it exists, with restrict or cascade options.
 
     Parameters
     ----------
     view_name: str
         view name
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     restrict: bool
-        If True, refuses to drop table if there is any object depending on it. Otherwise it is the 'cascade' option which allows you to remove those dependent objects together with the table automatically.
+        If True, refuses to drop table if there is any object depending on it. Otherwise it is the
+        'cascade' option which allows you to remove those dependent objects together with the table
+        automatically.
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     whatever exec_sql() returns
     """
     frame_sql_str = frame_sql(view_name, schema=schema)
@@ -753,17 +821,17 @@
     return exec_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
 
 
 def rename_matview(
     old_matview_name,
     new_matview_name,
     engine,
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Renames a materialized view of a schema.
 
     Parameters
     ----------
     old_matview_name: str
         old materialized view name
@@ -771,80 +839,117 @@
         new materialized view name
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
     """
     frame_sql_str = frame_sql(old_matview_name, schema=schema)
     exec_sql(
         'ALTER MATERIALIZED VIEW {} RENAME TO "{}";'.format(
             frame_sql_str, new_matview_name
         ),
         engine,
         nb_trials=nb_trials,
         logger=logger,
     )
 
 
+def refreesh_matview(
+    matview_name,
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
+):
+    """Refreshes a materialized view of a schema.
+
+    Parameters
+    ----------
+    matview_name: str
+        materialized view name
+    engine: sqlalchemy.engine.Engine
+        an sqlalchemy connection engine created by function `create_engine()`
+    schema: str or None
+        a valid schema name returned from `list_schemas()`
+    nb_trials: int
+        number of query trials
+    logger: mt.logg.IndentedLoggerAdapter, optional
+        logger for debugging
+    """
+    frame_sql_str = frame_sql(matview_name, schema=schema)
+    exec_sql(
+        f"REFRESH MATERIALIZED VIEW {frame_sql_str};",
+        engine,
+        nb_trials=nb_trials,
+        logger=logger,
+    )
+
+
 def drop_matview(
     matview_name,
     engine,
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     restrict=True,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Drops a mateiralized view if it exists, with restrict or cascade options.
 
     Parameters
     ----------
     matview_name: str
         materialized view name
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     restrict: bool
-        If True, refuses to drop table if there is any object depending on it. Otherwise it is the 'cascade' option which allows you to remove those dependent objects together with the table automatically.
+        If True, refuses to drop table if there is any object depending on it. Otherwise it is the
+        'cascade' option which allows you to remove those dependent objects together with the table
+        automatically.
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     whatever exec_sql() returns
     """
     frame_sql_str = frame_sql(matview_name, schema=schema)
     query_str = "DROP MATERIALIZED VIEW IF EXISTS {} {};".format(
         frame_sql_str, "RESTRICT" if restrict else "CASCADE"
     )
     return exec_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
 
 
 def frame_exists(
-    frame_name, engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None
+    frame_name,
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Checks if a frame exists.
 
     Parameters
     ----------
     frame_name: str
         name of table or view
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     retval: bool
         whether a table or a view exists with the given name
     """
@@ -858,34 +963,36 @@
         engine, schema=schema, nb_trials=nb_trials, logger=logger
     )
 
 
 def drop_frame(
     frame_name,
     engine,
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     restrict=True,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Drops a frame (table/view/mateiralized view) if it exists, with restrict or cascade options.
 
     Parameters
     ----------
     frame_name: str
         frame name
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     restrict: bool
-        If True, refuses to drop table if there is any object depending on it. Otherwise it is the 'cascade' option which allows you to remove those dependent objects together with the table automatically.
+        If True, refuses to drop table if there is any object depending on it. Otherwise it is the
+        'cascade' option which allows you to remove those dependent objects together with the table
+        automatically.
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     whatever exec_sql() returns, or False if the frame does not exist
     """
     if frame_name in list_tables(engine, schema=schema):
@@ -919,29 +1026,33 @@
             nb_trials=nb_trials,
             logger=logger,
         )
     return False
 
 
 def list_columns_ext(
-    table_name, engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None
+    table_name,
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Lists all columns of a given table of a given schema.
 
     Parameters
     ----------
     table_name: str
         a valid table name returned from `list_tables()`
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     out: pandas.DataFrame
         a table of details of the columns
     """
@@ -967,56 +1078,64 @@
             schema, table_name
         )
 
     return read_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
 
 
 def list_columns(
-    table_name, engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None
+    table_name,
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Lists all columns of a given table of a given schema.
 
     Parameters
     ----------
     table_name: str
         a valid table name returned from `list_tables()`
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     out: list of all column names
     """
     return list_columns_ext(
         table_name, engine, schema=schema, nb_trials=nb_trials, logger=logger
     )["column_name"].tolist()
 
 
 def list_primary_columns_ext(
-    frame_name, engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None
+    frame_name,
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Lists all primary columns of a given frame of a given schema.
 
     Parameters
     ----------
     frame_name: str
         a valid table/view/matview name returned from `list_frames()`
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     pandas.DataFrame
         dataframe containing primary column names and data types
     """
@@ -1031,29 +1150,33 @@
         """.format(
         frame_sql_str
     )
     return read_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
 
 
 def list_primary_columns(
-    frame_name, engine, schema: Optional[str] = None, nb_trials: int = 3, logger=None
+    frame_name,
+    engine,
+    schema: tp.Optional[str] = None,
+    nb_trials: int = 3,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Lists all primary columns of a given frame of a given schema.
 
     Parameters
     ----------
     frame_name: str
         a valid table/view/matview name returned from `list_frames()`
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         a valid schema name returned from `list_schemas()`
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     list
         list of primary column names
     """
@@ -1063,17 +1186,17 @@
 
 
 def rename_column(
     table_name,
     old_column_name,
     new_column_name,
     engine,
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Renames a column of a table.
 
     Parameters
     ----------
     table_name: str
         table name
@@ -1083,15 +1206,15 @@
         new column name
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         schema name
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
     """
     old_column_name = old_column_name.replace("%", "%%")
     if schema is None:
         query_str = 'ALTER TABLE "{}" RENAME COLUMN "{}" TO "{}";'.format(
             table_name, old_column_name, new_column_name
         )
@@ -1102,17 +1225,17 @@
     exec_sql(query_str, engine, nb_trials=nb_trials, logger=logger)
 
 
 def drop_column(
     table_name,
     column_name,
     engine,
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Drops a column of a table.
 
     Parameters
     ----------
     table_name: str
         table name
@@ -1120,15 +1243,15 @@
         column name
     engine: sqlalchemy.engine.Engine
         an sqlalchemy connection engine created by function `create_engine()`
     schema: str or None
         schema name
     nb_trials: int
         number of query trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
     """
     column_name = column_name.replace("%", "%%")
     if schema is None:
         query_str = 'ALTER TABLE "{}" DROP COLUMN "{}";'.format(table_name, column_name)
     else:
         query_str = 'ALTER TABLE "{}"."{}" DROP COLUMN "{}";'.format(
@@ -1143,48 +1266,52 @@
 def comparesync_table(
     engine,
     df_filepath,
     table_name,
     id_name,
     hash_name="hash",
     columns=["*"],
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     max_records_per_query=None,
     cond=None,
     reading_mode=True,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Compares a local CSV table with a remote PostgreSQL to find out which rows are the same or different.
 
     Parameters
     ----------
     engine: sqlalchemy connectible
         connection to the PostgreSQL database
     df_filepath: path
         path to the local '.csv', '.csv.zip' or '.parquet' file
     table_name: str
         table name
     id_name: str
         index column name. Assumption is only one column for indexing for now.
     hash_name : str
-        Name of the hash field that only changes when the row changes. If reading_mode is True and the field does not exist remotely, it will be generated by the remote server via md5. If reading_mode is False and the field does not exist locally, it will be generate locally using hashlib.
+        Name of the hash field that only changes when the row changes. If reading_mode is True and
+        the field does not exist remotely, it will be generated by the remote server via md5. If
+        reading_mode is False and the field does not exist locally, it will be generate locally
+        using hashlib.
     columns: list
         list of column names the function will read from, ignoring the remaining columns
     schema: str
         schema name, None means using the default one
     max_records_per_query: int or None
-        maximum number of records to be updated in each SQL query. If None, this will be dynamic to make sure each query runs about 5 minute.
+        maximum number of records to be updated in each SQL query. If None, this will be dynamic to
+        make sure each query runs about 5 minute.
     cond: str
         additional condition in selecting rows from the PostgreSQL table
     reading_mode: bool
         whether comparing is for reading or for writing
     nb_trials: int
         number of read_sql() trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     local_df: `pandas.DataFrame(index=id_name, columns=[..., hash_name])` or None
         local dataframe loaded to memory, if it exists
     remote_md5_df: pandas.DataFrame(index=id_name, columns=[hash_name])
@@ -1196,17 +1323,19 @@
     local_only_keys: list
         list of keys containing rows which appear in the local table only
     remote_only_keys: list
         list of keys identifying rows which appear in the remote table only
 
     Notes
     -----
-    The hash field of each table will be used to store and compare the hash values. If it does not exist, it will be generated automatically.
+    The hash field of each table will be used to store and compare the hash values. If it does not
+    exist, it will be generated automatically.
 
-    The id_name field must uniquely identify each record in both tables. Duplicated keys in either table will be treated as diff_keys, so that hopefully next sync will fix them.
+    The id_name field must uniquely identify each record in both tables. Duplicated keys in either
+    table will be treated as diff_keys, so that hopefully next sync will fix them.
     """
     frame_sql_str = frame_sql(table_name, schema=schema)
 
     with logger.scoped_debug(
         "Comparing table: local '{}' <-> remote '{}'".format(
             df_filepath, frame_sql_str
         ),
@@ -1417,21 +1546,21 @@
 
 def writesync_table(
     engine,
     df_filepath,
     table_name,
     id_name,
     hash_name="hash",
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     max_records_per_query=None,
     conn_ro=None,
     engine_ro=None,
     drop_cascade: bool = False,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
 ):
     """Writes and updates a remote PostgreSQL table from a local CSV table by updating only rows which have been changed.
 
     Parameters
     ----------
     engine: sqlalchemy connectible
         connection to the PostgreSQL database
@@ -1444,24 +1573,27 @@
     hash_name : str
         hash column name. See :func:`compare_table` for additional assumptions.
     schema: str
         schema name, None means using the default one
     bg_write_csv: bool
         whether to write the updated CSV file in a background thread
     max_records_per_query: int or None
-        maximum number of records to be updated in each SQL query. If None, this will be dynamic to make sure each query runs about 5 minute.
+        maximum number of records to be updated in each SQL query. If None, this will be dynamic to
+        make sure each query runs about 5 minute.
     conn_ro: sqlalchemy connectible or None
-        read-only connection to the PostgreSQL database. If not specified, it is set to `engine`. This is an old-style keyword argument. It will be replaced by `engine_ro`.
+        read-only connection to the PostgreSQL database. If not specified, it is set to `engine`.
+        This is an old-style keyword argument. It will be replaced by `engine_ro`.
     engine_ro : sqlalchemy.engine.Engine
-        read-only connection engine to the server. If not specified, it is set to `engine`. This new keyword argument will replace `conn_ro`.
+        read-only connection engine to the server. If not specified, it is set to `engine`. This
+        new keyword argument will replace `conn_ro`.
     drop_cascade : bool
         whether or not to drop using the CASCADE option when dropping a table
     nb_trials: int
         number of read_sql() trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
 
     Returns
     -------
     df: pandas.DataFrame
         the data frame representing the local table
 
@@ -1670,20 +1802,20 @@
 def readsync_table(
     engine,
     df_filepath,
     table_name,
     id_name,
     hash_name="hash",
     columns=["*"],
-    schema: Optional[str] = None,
+    schema: tp.Optional[str] = None,
     cond=None,
     bg_write_csv=False,
     max_records_per_query=None,
     nb_trials: int = 3,
-    logger=None,
+    logger: tp.Optional[logg.IndentedLoggerAdapter] = None,
     raise_exception_upon_mismatch=True,
 ):
     """Reads and updates a local CSV table from a PostgreSQL table by updating only rows which have been changed.
 
     Parameters
     ----------
     engine: sqlalchemy connectible
@@ -1701,28 +1833,31 @@
     schema: str
         schema name, None means using the default one
     cond: str
         additional condition in selecting rows from the PostgreSQL table
     bg_write_csv: bool
         whether to write the updated CSV file in a background thread
     max_records_per_query: int or None
-        maximum number of records to be updated in each SQL query. If None, this will be dynamic to make sure each query runs about 5 minute.
+        maximum number of records to be updated in each SQL query. If None, this will be dynamic to
+        make sure each query runs about 5 minute.
     nb_trials: int
         number of read_sql() trials
-    logger: logging.Logger or None
+    logger: mt.logg.IndentedLoggerAdapter, optional
         logger for debugging
     raise_exception_upon_mismatch : bool
-        whether to raise a RuntimeError upon mismatching the number of hashes and the number of records
+        whether to raise a RuntimeError upon mismatching the number of hashes and the number of
+        records
 
     Returns
     -------
     df: pandas.DataFrame
         the data frame representing the read and updated table
     bg: BgInvoke or None, optional
-        If bg_write_csv is True, this represents the background thread for writing the updated CSV file. If no background thread is needed, None is returned.
+        If bg_write_csv is True, this represents the background thread for writing the updated CSV
+        file. If no background thread is needed, None is returned.
     """
     frame_sql_str = frame_sql(table_name, schema=schema)
     with logger.scoped_debug(
         "Reading table: local '{}' <- remote '{}'".format(df_filepath, frame_sql_str),
         curly=False,
     ) if logger else dummy_scope:
         (
```

## mt/sql/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('04')
-VERSION_DAY = int('07')
-VERSION_HOUR = int('20')
-VERSION_MINUTE = int('16')
+VERSION_DAY = int('23')
+VERSION_HOUR = int('06')
+VERSION_MINUTE = int('28')
 MAJOR_VERSION = 1
-MINOR_VERSION = 3
-PATCH_VERSION = 202304072016
-version_date = '2023/04/07 20:16'
+MINOR_VERSION = 4
+PATCH_VERSION = 202304230628
+version_date = '2023/04/23 06:28'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mtsql-1.3.202304072016.dist-info/LICENSE` & `mtsql-1.4.202304230628.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtsql-1.3.202304072016.dist-info/METADATA` & `mtsql-1.4.202304230628.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtsql
-Version: 1.3.202304072016
+Version: 1.4.202304230628
 Summary: Extra Python modules to deal with the interaction between pandas dataframes and remote SQL servers, for Minh-Tri Pham
 Home-page: https://github.com/inteplus/mtsql
 Author: ['Minh-Tri Pham']
 Project-URL: Documentation, https://mtdoc.readthedocs.io/en/latest/mt.sql/mt.sql.html
 Project-URL: Source Code, https://github.com/inteplus/mtsql
 License-File: LICENSE
 Requires-Dist: sqlalchemy (>=2.0)
```

