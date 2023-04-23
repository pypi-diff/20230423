# Comparing `tmp/lunchable-0.6.0.tar.gz` & `tmp/lunchable-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunchable-0.6.0.tar", max compression
+gzip compressed data, was "lunchable-0.7.0.tar", max compression
```

## Comparing `lunchable-0.6.0.tar` & `lunchable-0.7.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1071 2023-04-23 02:03:25.658808 lunchable-0.6.0/LICENSE
--rw-r--r--   0        0        0     2215 2023-04-23 02:03:25.658808 lunchable-0.6.0/README.md
--rw-r--r--   0        0        0      537 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/__init__.py
--rw-r--r--   0        0        0       98 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/__main__.py
--rw-r--r--   0        0        0    12928 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_cli.py
--rw-r--r--   0        0        0      160 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_config/__init__.py
--rw-r--r--   0        0        0     4687 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_config/api_config.py
--rw-r--r--   0        0        0      379 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_config/file_config.py
--rw-r--r--   0        0        0     2216 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_config/logging_config.py
--rw-r--r--   0        0        0      147 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_version.py
--rw-r--r--   0        0        0      502 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/exceptions.py
--rw-r--r--   0        0        0      917 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/__init__.py
--rw-r--r--   0        0        0      322 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/_base.py
--rw-r--r--   0        0        0     6250 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/_core.py
--rw-r--r--   0        0        0     1895 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/_lunchmoney.py
--rw-r--r--   0        0        0     9126 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/assets.py
--rw-r--r--   0        0        0     6752 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/budgets.py
--rw-r--r--   0        0        0    15170 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/categories.py
--rw-r--r--   0        0        0     5188 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/crypto.py
--rw-r--r--   0        0        0     4626 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/plaid_accounts.py
--rw-r--r--   0        0        0     6857 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/recurring_expenses.py
--rw-r--r--   0        0        0     1271 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/tags.py
--rw-r--r--   0        0        0    32901 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/transactions.py
--rw-r--r--   0        0        0     1535 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/user.py
--rw-r--r--   0        0        0      220 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/__init__.py
--rw-r--r--   0        0        0      205 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/base/__init__.py
--rw-r--r--   0        0        0    12165 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/base/base_app.py
--rw-r--r--   0        0        0     1598 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/base/pandas_app.py
--rw-r--r--   0        0        0     2809 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/primelunch/README.md
--rw-r--r--   0        0        0       26 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/primelunch/__init__.py
--rw-r--r--   0        0        0    14911 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/primelunch/primelunch.py
--rw-r--r--   0        0        0     2104 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/pushlunch/README.md
--rw-r--r--   0        0        0      100 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/pushlunch/__init__.py
--rw-r--r--   0        0        0    11661 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/pushlunch/pushover.py
--rw-r--r--   0        0        0     1707 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/README.md
--rw-r--r--   0        0        0      230 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/__init__.py
--rw-r--r--   0        0        0      320 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/_config.py
--rw-r--r--   0        0        0      150 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/exceptions.py
--rw-r--r--   0        0        0    48829 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py
--rw-r--r--   0        0        0      598 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/models.py
--rw-r--r--   0        0        0        0 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/py.typed
--rw-r--r--   0        0        0     1800 2023-04-23 02:03:25.662808 lunchable-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 lunchable-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-23 04:32:09.089263 lunchable-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2215 2023-04-23 04:32:09.089263 lunchable-0.7.0/README.md
+-rw-r--r--   0        0        0      537 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/__init__.py
+-rw-r--r--   0        0        0       98 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/__main__.py
+-rw-r--r--   0        0        0    13208 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_cli.py
+-rw-r--r--   0        0        0      160 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_config/__init__.py
+-rw-r--r--   0        0        0     4687 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_config/api_config.py
+-rw-r--r--   0        0        0      379 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_config/file_config.py
+-rw-r--r--   0        0        0     2216 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_config/logging_config.py
+-rw-r--r--   0        0        0      147 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/_version.py
+-rw-r--r--   0        0        0      502 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/exceptions.py
+-rw-r--r--   0        0        0      917 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/models/__init__.py
+-rw-r--r--   0        0        0      322 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/models/_base.py
+-rw-r--r--   0        0        0     6250 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/models/_core.py
+-rw-r--r--   0        0        0     1895 2023-04-23 04:32:09.089263 lunchable-0.7.0/lunchable/models/_lunchmoney.py
+-rw-r--r--   0        0        0     9126 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/assets.py
+-rw-r--r--   0        0        0     6752 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/budgets.py
+-rw-r--r--   0        0        0    15170 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/categories.py
+-rw-r--r--   0        0        0     5188 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/crypto.py
+-rw-r--r--   0        0        0     4626 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/plaid_accounts.py
+-rw-r--r--   0        0        0     6857 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/recurring_expenses.py
+-rw-r--r--   0        0        0     1271 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/tags.py
+-rw-r--r--   0        0        0    32901 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/transactions.py
+-rw-r--r--   0        0        0     1535 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/models/user.py
+-rw-r--r--   0        0        0      220 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/__init__.py
+-rw-r--r--   0        0        0      205 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/base/__init__.py
+-rw-r--r--   0        0        0    12165 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/base/base_app.py
+-rw-r--r--   0        0        0     1598 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/base/pandas_app.py
+-rw-r--r--   0        0        0     2809 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/primelunch/README.md
+-rw-r--r--   0        0        0       26 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/primelunch/__init__.py
+-rw-r--r--   0        0        0    14911 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/primelunch/primelunch.py
+-rw-r--r--   0        0        0     2104 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/pushlunch/README.md
+-rw-r--r--   0        0        0      100 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/pushlunch/__init__.py
+-rw-r--r--   0        0        0    11661 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/pushlunch/pushover.py
+-rw-r--r--   0        0        0     1707 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/README.md
+-rw-r--r--   0        0        0      230 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/__init__.py
+-rw-r--r--   0        0        0      320 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/_config.py
+-rw-r--r--   0        0        0      150 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/exceptions.py
+-rw-r--r--   0        0        0    49243 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py
+-rw-r--r--   0        0        0      598 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/plugins/splitlunch/models.py
+-rw-r--r--   0        0        0        0 2023-04-23 04:32:09.093263 lunchable-0.7.0/lunchable/py.typed
+-rw-r--r--   0        0        0     1800 2023-04-23 04:32:09.093263 lunchable-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 lunchable-0.7.0/PKG-INFO
```

### Comparing `lunchable-0.6.0/LICENSE` & `lunchable-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/README.md` & `lunchable-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/__init__.py` & `lunchable-0.7.0/lunchable/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/_cli.py` & `lunchable-0.7.0/lunchable/_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Lunchmoney CLI
 """
 
+import datetime
 import logging
 from json import JSONDecodeError
 from typing import Any, Dict, Optional, Union
 
 import click
 import requests
 from pydantic.json import pydantic_encoder
@@ -148,32 +149,36 @@
 def splitlunch() -> None:
     """
     Splitwise Plugin for lunchable, SplitLunch 💲🍱
     """
     pass
 
 
-@splitlunch.command("expenses")
-@click.option(
-    "--limit", default=None, help="Limit the amount of Results. 0 returns everything."
-)
-@click.option("--offset", default=None, help="Number of expenses to be skipped")
-@click.option("--limit", default=None, help="Number of expenses to be returned")
-@click.option("--group-id", default=None, help="GroupID of the expenses")
-@click.option("--friendship-id", default=None, help="FriendshipID of the expenses")
-@click.option(
+dated_after = click.option(
     "--dated-after",
     default=None,
     help="ISO 8601 Date time. Return expenses later that this date",
 )
-@click.option(
+dated_before = click.option(
     "--dated-before",
     default=None,
     help="ISO 8601 Date time. Return expenses earlier than this date",
 )
+
+
+@splitlunch.command("expenses")
+@click.option(
+    "--limit", default=None, help="Limit the amount of Results. 0 returns everything."
+)
+@click.option("--offset", default=None, help="Number of expenses to be skipped")
+@click.option("--limit", default=None, help="Number of expenses to be returned")
+@click.option("--group-id", default=None, help="GroupID of the expenses")
+@click.option("--friendship-id", default=None, help="FriendshipID of the expenses")
+@dated_after
+@dated_before
 @click.option(
     "--updated-after",
     default=None,
     help="ISO 8601 Date time. Return expenses updated after this date",
 )
 @click.option(
     "--updated-before",
@@ -307,37 +312,47 @@
 
     splitlunch = SplitLunch()
     updated_asset = splitlunch.update_splitwise_balance()
     print_json(data=updated_asset, default=pydantic_encoder)
 
 
 @splitlunch.command("refresh")
+@dated_after
+@dated_before
 @click.option(
     "--allow-self-paid/--no-allow-self-paid",
     default=False,
     help="Allow self-paid expenses to be imported (filtered out by default).",
 )
 @click.option(
     "--allow-payments/--no-allow-payments",
     default=False,
     help="Allow payments to be imported (filtered out by default).",
 )
-def refresh_splitwise_transactions(allow_self_paid: bool, allow_payments: bool) -> None:
+def refresh_splitwise_transactions(
+    dated_before: Optional[datetime.datetime],
+    dated_after: Optional[datetime.datetime],
+    allow_self_paid: bool,
+    allow_payments: bool,
+) -> None:
     """
     Import New Splitwise Transactions to Lunch Money and
 
     This function gets all transactions from Splitwise, all transactions from
     your Lunch Money Splitwise account and compares the two. This also updates
     the account balance.
     """
     from lunchable.plugins.splitlunch import SplitLunch
 
     splitlunch = SplitLunch()
     response = splitlunch.refresh_splitwise_transactions(
-        allow_self_paid=allow_self_paid, allow_payments=allow_payments
+        dated_before=dated_before,
+        dated_after=dated_after,
+        allow_self_paid=allow_self_paid,
+        allow_payments=allow_payments,
     )
     print_json(data=response, default=pydantic_encoder)
 
 
 @plugins.group()
 def pushlunch() -> None:
     """
```

### Comparing `lunchable-0.6.0/lunchable/_config/api_config.py` & `lunchable-0.7.0/lunchable/_config/api_config.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/_config/logging_config.py` & `lunchable-0.7.0/lunchable/_config/logging_config.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/__init__.py` & `lunchable-0.7.0/lunchable/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/_core.py` & `lunchable-0.7.0/lunchable/models/_core.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/_lunchmoney.py` & `lunchable-0.7.0/lunchable/models/_lunchmoney.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/assets.py` & `lunchable-0.7.0/lunchable/models/assets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/budgets.py` & `lunchable-0.7.0/lunchable/models/budgets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/categories.py` & `lunchable-0.7.0/lunchable/models/categories.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/crypto.py` & `lunchable-0.7.0/lunchable/models/crypto.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/plaid_accounts.py` & `lunchable-0.7.0/lunchable/models/plaid_accounts.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/recurring_expenses.py` & `lunchable-0.7.0/lunchable/models/recurring_expenses.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/tags.py` & `lunchable-0.7.0/lunchable/models/tags.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/transactions.py` & `lunchable-0.7.0/lunchable/models/transactions.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/models/user.py` & `lunchable-0.7.0/lunchable/models/user.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/plugins/base/base_app.py` & `lunchable-0.7.0/lunchable/plugins/base/base_app.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/plugins/base/pandas_app.py` & `lunchable-0.7.0/lunchable/plugins/base/pandas_app.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/plugins/primelunch/README.md` & `lunchable-0.7.0/lunchable/plugins/primelunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/plugins/primelunch/primelunch.py` & `lunchable-0.7.0/lunchable/plugins/primelunch/primelunch.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/plugins/pushlunch/README.md` & `lunchable-0.7.0/lunchable/plugins/pushlunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/plugins/pushlunch/pushover.py` & `lunchable-0.7.0/lunchable/plugins/pushlunch/pushover.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/plugins/splitlunch/README.md` & `lunchable-0.7.0/lunchable/plugins/splitlunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py` & `lunchable-0.7.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1117,14 +1117,16 @@
             self.splitwise_asset = updated_asset
         return self.splitwise_asset
 
     _deleted_payee = "[DELETED FROM SPLITWISE]"
 
     def get_new_transactions(
         self,
+        dated_after: Optional[datetime.datetime] = None,
+        dated_before: Optional[datetime.datetime] = None,
     ) -> Tuple[List[SplitLunchExpense], List[TransactionObject]]:
         """
         Get Splitwise Transactions that don't exist in Lunch Money
 
         Also return deleted transaction from LunchMoney
 
         Returns
@@ -1141,15 +1143,19 @@
             end_date=datetime.datetime(2300, 12, 31),
         )
         splitlunch_ids = {
             int(item.external_id)
             for item in splitlunch_expenses
             if item.external_id is not None
         }
-        splitwise_expenses = self.get_expenses(limit=0)
+        splitwise_expenses = self.get_expenses(
+            limit=0,
+            dated_after=dated_after,
+            dated_before=dated_before,
+        )
         splitwise_ids = {item.splitwise_id for item in splitwise_expenses}
         new_ids = splitwise_ids.difference(splitlunch_ids)
         new_expenses = [
             expense for expense in splitwise_expenses if expense.splitwise_id in new_ids
         ]
         deleted_transactions = self.get_deleted_transactions(
             splitlunch_expenses=splitlunch_expenses,
@@ -1195,28 +1201,33 @@
             and int(tran.external_id) in untethered_transactions
             and tran.payee != self._deleted_payee
         ]
         return transactions_to_delete
 
     def refresh_splitwise_transactions(
         self,
+        dated_after: Optional[datetime.datetime] = None,
+        dated_before: Optional[datetime.datetime] = None,
         allow_self_paid: bool = False,
         allow_payments: bool = False,
     ) -> Dict[str, Any]:
         """
         Import New Splitwise Transactions to Lunch Money
 
         This function get's all transactions from Splitwise, all transactions from
         your Lunch Money Splitwise account and compares the two.
 
         Returns
         -------
         List[SplitLunchExpense]
         """
-        new_transactions, deleted_transactions = self.get_new_transactions()
+        new_transactions, deleted_transactions = self.get_new_transactions(
+            dated_after=dated_after,
+            dated_before=dated_before,
+        )
         self.splitwise_to_lunchmoney(
             expenses=new_transactions,
             allow_self_paid=allow_self_paid,
             allow_payments=allow_payments,
         )
         splitwise_asset = self.update_splitwise_balance()
         self.handle_deleted_transactions(deleted_transactions=deleted_transactions)
```

### Comparing `lunchable-0.6.0/lunchable/plugins/splitlunch/models.py` & `lunchable-0.7.0/lunchable/plugins/splitlunch/models.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.6.0/pyproject.toml` & `lunchable-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 documentation = "https://juftin.github.io/lunchable"
 homepage = "https://github.com/juftin/lunchable"
 include = ["lunchable/py.typed"]
 license = "MIT"
 name = "lunchable"
 readme = "README.md"
 repository = "https://github.com/juftin/lunchable"
-version = "0.6.0"
+version = "0.7.0"
 
 [tool.poetry.dependencies]
 click = ">=8.0.1"
 pandas = {version = "^1.3", optional = true}
 pydantic = ">=1.2.0,<2.0.0"
 python = ">=3.7.1,<4.0"
 python-dateutil = {version = "^2.8.2", optional = true}
```

### Comparing `lunchable-0.6.0/PKG-INFO` & `lunchable-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunchable
-Version: 0.6.0
+Version: 0.7.0
 Summary: A simple Python SDK around the Lunch Money Developer API
 Home-page: https://github.com/juftin/lunchable
 License: MIT
 Author: Justin Flannery
 Author-email: juftin@juftin.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lunchable Version: 0.6.0 Summary: A simple Python
+Metadata-Version: 2.1 Name: lunchable Version: 0.7.0 Summary: A simple Python
 SDK around the Lunch Money Developer API Home-page: https://github.com/juftin/
 lunchable License: MIT Author: Justin Flannery Author-email: juftin@juftin.com
 Requires-Python: >=3.7.1,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

