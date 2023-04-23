# Comparing `tmp/lunchable-0.5.1.tar.gz` & `tmp/lunchable-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunchable-0.5.1.tar", max compression
+gzip compressed data, was "lunchable-0.6.0.tar", max compression
```

## Comparing `lunchable-0.5.1.tar` & `lunchable-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1071 2023-04-09 16:23:36.735018 lunchable-0.5.1/LICENSE
--rw-r--r--   0        0        0     2215 2023-04-09 16:23:36.735018 lunchable-0.5.1/README.md
--rw-r--r--   0        0        0      537 2023-04-09 16:23:36.735018 lunchable-0.5.1/lunchable/__init__.py
--rw-r--r--   0        0        0       98 2023-04-09 16:23:36.735018 lunchable-0.5.1/lunchable/__main__.py
--rw-r--r--   0        0        0    12499 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_cli.py
--rw-r--r--   0        0        0      160 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_config/__init__.py
--rw-r--r--   0        0        0     4687 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_config/api_config.py
--rw-r--r--   0        0        0      379 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_config/file_config.py
--rw-r--r--   0        0        0     2216 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_config/logging_config.py
--rw-r--r--   0        0        0      147 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/_version.py
--rw-r--r--   0        0        0      502 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/exceptions.py
--rw-r--r--   0        0        0      917 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/__init__.py
--rw-r--r--   0        0        0      322 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/_base.py
--rw-r--r--   0        0        0     6250 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/_core.py
--rw-r--r--   0        0        0     1895 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/_lunchmoney.py
--rw-r--r--   0        0        0     9126 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/assets.py
--rw-r--r--   0        0        0     6752 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/budgets.py
--rw-r--r--   0        0        0    15170 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/categories.py
--rw-r--r--   0        0        0     5188 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/crypto.py
--rw-r--r--   0        0        0     4626 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/plaid_accounts.py
--rw-r--r--   0        0        0     6857 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/recurring_expenses.py
--rw-r--r--   0        0        0     1271 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/tags.py
--rw-r--r--   0        0        0    32901 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/transactions.py
--rw-r--r--   0        0        0     1535 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/models/user.py
--rw-r--r--   0        0        0      220 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/__init__.py
--rw-r--r--   0        0        0      205 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/base/__init__.py
--rw-r--r--   0        0        0    12165 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/base/base_app.py
--rw-r--r--   0        0        0     1598 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/base/pandas_app.py
--rw-r--r--   0        0        0     2809 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/primelunch/README.md
--rw-r--r--   0        0        0       26 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/primelunch/__init__.py
--rw-r--r--   0        0        0    14911 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/primelunch/primelunch.py
--rw-r--r--   0        0        0     2104 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/pushlunch/README.md
--rw-r--r--   0        0        0      100 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/pushlunch/__init__.py
--rw-r--r--   0        0        0    11661 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/pushlunch/pushover.py
--rw-r--r--   0        0        0     1707 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/README.md
--rw-r--r--   0        0        0      230 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/__init__.py
--rw-r--r--   0        0        0      320 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/_config.py
--rw-r--r--   0        0        0      150 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/exceptions.py
--rw-r--r--   0        0        0    49826 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/lunchmoney_splitwise.py
--rw-r--r--   0        0        0      624 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/plugins/splitlunch/models.py
--rw-r--r--   0        0        0        0 2023-04-09 16:23:36.739018 lunchable-0.5.1/lunchable/py.typed
--rw-r--r--   0        0        0     1800 2023-04-09 16:23:36.739018 lunchable-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 lunchable-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-23 02:03:25.658808 lunchable-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2215 2023-04-23 02:03:25.658808 lunchable-0.6.0/README.md
+-rw-r--r--   0        0        0      537 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/__init__.py
+-rw-r--r--   0        0        0       98 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/__main__.py
+-rw-r--r--   0        0        0    12928 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_cli.py
+-rw-r--r--   0        0        0      160 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_config/__init__.py
+-rw-r--r--   0        0        0     4687 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_config/api_config.py
+-rw-r--r--   0        0        0      379 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_config/file_config.py
+-rw-r--r--   0        0        0     2216 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_config/logging_config.py
+-rw-r--r--   0        0        0      147 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/_version.py
+-rw-r--r--   0        0        0      502 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/exceptions.py
+-rw-r--r--   0        0        0      917 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/__init__.py
+-rw-r--r--   0        0        0      322 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/_base.py
+-rw-r--r--   0        0        0     6250 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/_core.py
+-rw-r--r--   0        0        0     1895 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/_lunchmoney.py
+-rw-r--r--   0        0        0     9126 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/assets.py
+-rw-r--r--   0        0        0     6752 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/budgets.py
+-rw-r--r--   0        0        0    15170 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/categories.py
+-rw-r--r--   0        0        0     5188 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/crypto.py
+-rw-r--r--   0        0        0     4626 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/plaid_accounts.py
+-rw-r--r--   0        0        0     6857 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/recurring_expenses.py
+-rw-r--r--   0        0        0     1271 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/tags.py
+-rw-r--r--   0        0        0    32901 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/transactions.py
+-rw-r--r--   0        0        0     1535 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/models/user.py
+-rw-r--r--   0        0        0      220 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/__init__.py
+-rw-r--r--   0        0        0      205 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/base/__init__.py
+-rw-r--r--   0        0        0    12165 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/base/base_app.py
+-rw-r--r--   0        0        0     1598 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/base/pandas_app.py
+-rw-r--r--   0        0        0     2809 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/primelunch/README.md
+-rw-r--r--   0        0        0       26 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/primelunch/__init__.py
+-rw-r--r--   0        0        0    14911 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/primelunch/primelunch.py
+-rw-r--r--   0        0        0     2104 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/pushlunch/README.md
+-rw-r--r--   0        0        0      100 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/pushlunch/__init__.py
+-rw-r--r--   0        0        0    11661 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/pushlunch/pushover.py
+-rw-r--r--   0        0        0     1707 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/README.md
+-rw-r--r--   0        0        0      230 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/__init__.py
+-rw-r--r--   0        0        0      320 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/_config.py
+-rw-r--r--   0        0        0      150 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/exceptions.py
+-rw-r--r--   0        0        0    48829 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py
+-rw-r--r--   0        0        0      598 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/plugins/splitlunch/models.py
+-rw-r--r--   0        0        0        0 2023-04-23 02:03:25.662808 lunchable-0.6.0/lunchable/py.typed
+-rw-r--r--   0        0        0     1800 2023-04-23 02:03:25.662808 lunchable-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4063 1970-01-01 00:00:00.000000 lunchable-0.6.0/PKG-INFO
```

### Comparing `lunchable-0.5.1/LICENSE` & `lunchable-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/README.md` & `lunchable-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/__init__.py` & `lunchable-0.6.0/lunchable/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/_cli.py` & `lunchable-0.6.0/lunchable/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,26 +307,38 @@
 
     splitlunch = SplitLunch()
     updated_asset = splitlunch.update_splitwise_balance()
     print_json(data=updated_asset, default=pydantic_encoder)
 
 
 @splitlunch.command("refresh")
-def refresh_splitwise_transactions() -> None:
+@click.option(
+    "--allow-self-paid/--no-allow-self-paid",
+    default=False,
+    help="Allow self-paid expenses to be imported (filtered out by default).",
+)
+@click.option(
+    "--allow-payments/--no-allow-payments",
+    default=False,
+    help="Allow payments to be imported (filtered out by default).",
+)
+def refresh_splitwise_transactions(allow_self_paid: bool, allow_payments: bool) -> None:
     """
     Import New Splitwise Transactions to Lunch Money and
 
     This function gets all transactions from Splitwise, all transactions from
     your Lunch Money Splitwise account and compares the two. This also updates
     the account balance.
     """
     from lunchable.plugins.splitlunch import SplitLunch
 
     splitlunch = SplitLunch()
-    response = splitlunch.refresh_splitwise_transactions()
+    response = splitlunch.refresh_splitwise_transactions(
+        allow_self_paid=allow_self_paid, allow_payments=allow_payments
+    )
     print_json(data=response, default=pydantic_encoder)
 
 
 @plugins.group()
 def pushlunch() -> None:
     """
     Push Notifications for Lunch Money: PushLunch 📲
```

### Comparing `lunchable-0.5.1/lunchable/_config/api_config.py` & `lunchable-0.6.0/lunchable/_config/api_config.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/_config/logging_config.py` & `lunchable-0.6.0/lunchable/_config/logging_config.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/__init__.py` & `lunchable-0.6.0/lunchable/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/_core.py` & `lunchable-0.6.0/lunchable/models/_core.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/_lunchmoney.py` & `lunchable-0.6.0/lunchable/models/_lunchmoney.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/assets.py` & `lunchable-0.6.0/lunchable/models/assets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/budgets.py` & `lunchable-0.6.0/lunchable/models/budgets.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/categories.py` & `lunchable-0.6.0/lunchable/models/categories.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/crypto.py` & `lunchable-0.6.0/lunchable/models/crypto.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/plaid_accounts.py` & `lunchable-0.6.0/lunchable/models/plaid_accounts.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/recurring_expenses.py` & `lunchable-0.6.0/lunchable/models/recurring_expenses.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/tags.py` & `lunchable-0.6.0/lunchable/models/tags.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/transactions.py` & `lunchable-0.6.0/lunchable/models/transactions.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/models/user.py` & `lunchable-0.6.0/lunchable/models/user.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/plugins/base/base_app.py` & `lunchable-0.6.0/lunchable/plugins/base/base_app.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/plugins/base/pandas_app.py` & `lunchable-0.6.0/lunchable/plugins/base/pandas_app.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/plugins/primelunch/README.md` & `lunchable-0.6.0/lunchable/plugins/primelunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/plugins/primelunch/primelunch.py` & `lunchable-0.6.0/lunchable/plugins/primelunch/primelunch.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/plugins/pushlunch/README.md` & `lunchable-0.6.0/lunchable/plugins/pushlunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/plugins/pushlunch/pushover.py` & `lunchable-0.6.0/lunchable/plugins/pushlunch/pushover.py`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/plugins/splitlunch/README.md` & `lunchable-0.6.0/lunchable/plugins/splitlunch/README.md`

 * *Files identical despite different names*

### Comparing `lunchable-0.5.1/lunchable/plugins/splitlunch/lunchmoney_splitwise.py` & `lunchable-0.6.0/lunchable/plugins/splitlunch/lunchmoney_splitwise.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,44 @@
     _pip_extra_error = (
         "Looks like you don't have the Splitwise plugin installed: "
         f"`pip install {__application__}[splitlunch]`"
     )
     raise LunchMoneyImportError(_pip_extra_error)
 
 
+def _get_splitwise_impact(
+    expense: splitwise.Expense, current_user_id: int
+) -> Tuple[float, bool]:
+    """
+    Get the Financial Impact of a Splitwise Transaction
+
+    Parameters
+    ----------
+    expense: splitwise.Expense
+
+    Returns
+    -------
+    Tuple[float, bool]
+    """
+    financial_impact = 0.00
+    self_paid = False
+    if len(expense.repayments) >= 1:
+        for debt in expense.repayments:
+            if debt.fromUser == current_user_id:
+                financial_impact += float(debt.amount)
+            elif debt.toUser == current_user_id:
+                self_paid = True
+                financial_impact -= float(debt.amount)
+    elif len(expense.repayments) == 0:
+        assert len(expense.users) == 1
+        if expense.users[0].id == current_user_id:
+            self_paid = True
+    return financial_impact, self_paid
+
+
 class SplitLunch(splitwise.Splitwise):
     """
     Lunchable Plugin For Interacting With Splitwise
 
     This plugin supports different operations, and some of those operations
     have prerequisites:
 
@@ -478,94 +508,35 @@
         ----------
         expense: splitwise.Expense
 
         Returns
         -------
         SplitLunchExpense
         """
-        financial_impact, self_paid = self._get_splitwise_impact(expense=expense)
-        if expense.payment is True and financial_impact < 0:
-            personal_share = abs(financial_impact)
-        elif expense.payment is True and financial_impact > 0:
-            personal_share = 0
-        elif self_paid is True:
-            personal_share = round(float(expense.cost) - financial_impact, 2)
-        else:
-            personal_share = abs(financial_impact)
+        financial_impact, self_paid = _get_splitwise_impact(
+            expense=expense, current_user_id=self.current_user.id
+        )
         expense = SplitLunchExpense(
             splitwise_id=expense.id,
             original_amount=expense.cost,
             financial_impact=financial_impact,
-            personal_share=personal_share,
             self_paid=self_paid,
             description=expense.description,
             category=expense.category.name,
             details=expense.details,
             payment=expense.payment,
             date=expense.date,
             users=[user.id for user in expense.users],
             created_at=expense.created_at,
             updated_at=expense.updated_at,
             deleted_at=expense.deleted_at,
             deleted=True if expense.deleted_at is not None else False,
         )
         return expense
 
-    def _get_expense_impact(self, expense: splitwise.Expense) -> Tuple[float, bool]:
-        """
-        Get the Financial Impact of a Splitwise Expense
-
-        Parameters
-        ----------
-        expense: splitwise.Expense
-
-        Returns
-        -------
-        Tuple[float, bool]
-        """
-        financial_impact = 0.00
-        self_paid = True
-        if len(expense.repayments) >= 1:
-            for debt in expense.repayments:
-                if debt.fromUser == self.current_user.id:
-                    self_paid = False
-                    financial_impact -= float(debt.amount)
-                elif debt.toUser == self.current_user.id:
-                    financial_impact += float(debt.amount)
-        elif len(expense.repayments) == 0:
-            assert len(expense.users) == 1
-            assert expense.users[0].id == self.current_user.id
-        return financial_impact, self_paid
-
-    def _get_payment_impact(self, expense: splitwise.Expense) -> Tuple[float, bool]:
-        """
-        Get the Financial Impact of a Splitwise Payment
-
-        Parameters
-        ----------
-        expense: splitwise.Expense
-
-        Returns
-        -------
-        Tuple[float, bool]
-        """
-        financial_impact = 0.00
-        self_paid = True
-        if len(expense.repayments) >= 1:
-            for debt in expense.repayments:
-                if debt.fromUser == self.current_user.id:
-                    self_paid = False
-                    financial_impact += float(debt.amount)
-                elif debt.toUser == self.current_user.id:
-                    financial_impact -= float(debt.amount)
-        elif len(expense.repayments) == 0:
-            assert expense.users[0].id == self.current_user.id
-            financial_impact -= float(expense.cost)
-        return financial_impact, self_paid
-
     def _get_splitwise_asset(self) -> Optional[AssetsObject]:
         """
         Get the Splitwise asset
 
         Parse a user's Lunch Money accounts and return the manually managed
         Splitwise account asset object
 
@@ -608,32 +579,14 @@
         for category in categories:
             if "reimbursement" == category.name.strip().lower():
                 reimbursement_list.append(category)
         if len(reimbursement_list) != 1:
             return None
         return reimbursement_list[0]
 
-    def _get_splitwise_impact(self, expense: splitwise.Expense) -> Tuple[float, bool]:
-        """
-        Get the Financial Impact of a Splitwise Transaction
-
-        Parameters
-        ----------
-        expense: splitwise.Expense
-
-        Returns
-        -------
-        Tuple[float, bool]
-        """
-        if expense.payment is True:
-            financial_impact, self_paid = self._get_payment_impact(expense=expense)
-        else:
-            financial_impact, self_paid = self._get_expense_impact(expense=expense)
-        return financial_impact, self_paid
-
     def _get_splitwise_tags(self) -> None:
         """
         Get Lunch Money Tags to Interact with
 
         Returns
         -------
         Dict[str, int]
@@ -913,20 +866,21 @@
             notes = f"Splitwise ID: {new_transaction.splitwise_id}"
             if transaction.notes is not None:
                 notes = f"{transaction.notes} || {notes}"
             split_object = TransactionSplitObject(
                 date=transaction.date,
                 category_id=transaction.category_id,
                 notes=notes,
-                amount=new_transaction.personal_share,
+                # financial_impact for self-paid transactions will be negative
+                amount=round(
+                    transaction.amount - abs(new_transaction.financial_impact), 2
+                ),
             )
             reimbursement_object = split_object.copy()
-            reimbursement_object.amount = round(
-                transaction.amount - new_transaction.personal_share, 2
-            )
+            reimbursement_object.amount = new_transaction.financial_impact
             reimbursement_object.category_id = self.reimbursement_category.id
             logger.debug(
                 f"Transaction split by Splitwise: {transaction.amount} -> "
                 f"({split_object.amount}, {reimbursement_object.amount})"
             )
             update_response = self.lunchable.update_transaction(
                 transaction_id=transaction.id,
@@ -1019,21 +973,26 @@
                 splitwise_id=new_transaction.splitwise_id,
                 updated=response["updated"],
                 split=None,
             )
             update_responses.append(formatted_update_response)
         return update_responses
 
-    def splitwise_to_lunchmoney(self, expenses: List[SplitLunchExpense]) -> List[int]:
+    def splitwise_to_lunchmoney(
+        self,
+        expenses: List[SplitLunchExpense],
+        allow_self_paid: bool = False,
+        allow_payments: bool = False,
+    ) -> List[int]:
         """
         Ingest Splitwise Expenses into Lunch Money
 
-        This function inserts splitwise expenses into Lunch Money. If an expense
-        is not a payment, not deleted, and not self-paid it qualifies for ingestion. Otherwise
-        it will be ignored.
+        This function inserts splitwise expenses into Lunch Money. If an expense not deleted and has
+        a non-0 impact on the user's splitwise balance it qualifies for ingestion. By default,
+        payments and self-paid transactions are also ineligible. Otherwise it will be ignored.
 
         Parameters
         ----------
         expenses: List[SplitLunchExpense]
 
         Returns
         -------
@@ -1041,20 +1000,24 @@
             New Lunch Money transaction IDs
         """
         if self.splitwise_asset is None:
             self._raise_splitwise_asset_error()
             raise ValueError("SplitwiseAsset")
         batch = []
         new_transaction_ids = []
-        filtered_expenses = self.filter_relevant_splitwise_expenses(expenses=expenses)
+        filtered_expenses = self.filter_relevant_splitwise_expenses(
+            expenses=expenses,
+            allow_self_paid=allow_self_paid,
+            allow_payments=allow_payments,
+        )
         for splitwise_transaction in filtered_expenses:
             new_lunchmoney_transaction = TransactionInsertObject(
                 date=splitwise_transaction.date.astimezone(tzlocal()),
                 payee=splitwise_transaction.description,
-                amount=splitwise_transaction.personal_share,
+                amount=splitwise_transaction.financial_impact,
                 asset_id=self.splitwise_asset.id,
                 external_id=splitwise_transaction.splitwise_id,
             )
             batch.append(new_lunchmoney_transaction)
             if len(batch) == 10:
                 new_ids = self.lunchable.insert_transactions(
                     transactions=batch, apply_rules=True
@@ -1067,45 +1030,53 @@
             )
             new_transaction_ids += new_ids
         return new_transaction_ids
 
     @staticmethod
     def filter_relevant_splitwise_expenses(
         expenses: List[SplitLunchExpense],
+        allow_self_paid: bool = False,
+        allow_payments: bool = False,
     ) -> List[SplitLunchExpense]:
         """
         Filter Expenses in Splitwise into relevant expenses.
 
         This filtering action is important to understand when seeing why not
         all transactions from Splitwise end up flowing into Lunch Money.
 
         1) It filters out deleted expenses
 
-        2) It filters out `self-paid` expenses. A `self-paid` expense is an expense in Splitwise
-        where you originated the payment. This is excluded because it is assumed that these
-        transactions will have already been imported via a different account.
+        2) It filters out expenses with a financial impact of 0, implying that the user was not
+        involved in the expense.
 
-        3) It filters out payments. Payments are excluded because it is assumed that these
-        transactions will have already been imported via a different account.
+        3) If the --allow-self-paid flag is not provided, it filters out `self-paid` expenses. A
+        `self-paid` expense is an expense in Splitwise where you originated the payment. This is
+        excluded because it is assumed that these transactions will have already been imported via a
+        different account.
+
+        4) If the --allow-payments flag is not provided, it filters out payments. Payments are
+        excluded because it is assumed that these transactions will have already been imported via a
+        different account.
 
         Parameters
         ----------
         expenses: List[SplitLunchExpense]
 
         Returns
         -------
         List[SplitLunchExpense]
         """
         filtered_expenses = list()
         for splitwise_transaction in expenses:
             if all(
                 [
                     splitwise_transaction.deleted is False,
-                    splitwise_transaction.payment is False,
-                    splitwise_transaction.self_paid is False,
+                    splitwise_transaction.financial_impact != 0.00,
+                    allow_self_paid or (splitwise_transaction.self_paid is False),
+                    allow_payments or (splitwise_transaction.payment is False),
                 ]
             ):
                 filtered_expenses.append(splitwise_transaction)
 
         return filtered_expenses
 
     def get_splitwise_balance(self) -> float:
@@ -1173,19 +1144,16 @@
             int(item.external_id)
             for item in splitlunch_expenses
             if item.external_id is not None
         }
         splitwise_expenses = self.get_expenses(limit=0)
         splitwise_ids = {item.splitwise_id for item in splitwise_expenses}
         new_ids = splitwise_ids.difference(splitlunch_ids)
-        filtered_expenses = self.filter_relevant_splitwise_expenses(
-            expenses=splitwise_expenses
-        )
         new_expenses = [
-            expense for expense in filtered_expenses if expense.splitwise_id in new_ids
+            expense for expense in splitwise_expenses if expense.splitwise_id in new_ids
         ]
         deleted_transactions = self.get_deleted_transactions(
             splitlunch_expenses=splitlunch_expenses,
             splitwise_transactions=splitwise_expenses,
         )
         return new_expenses, deleted_transactions
 
@@ -1225,27 +1193,35 @@
             for tran in splitlunch_expenses
             if tran.external_id is not None
             and int(tran.external_id) in untethered_transactions
             and tran.payee != self._deleted_payee
         ]
         return transactions_to_delete
 
-    def refresh_splitwise_transactions(self) -> Dict[str, Any]:
+    def refresh_splitwise_transactions(
+        self,
+        allow_self_paid: bool = False,
+        allow_payments: bool = False,
+    ) -> Dict[str, Any]:
         """
         Import New Splitwise Transactions to Lunch Money
 
         This function get's all transactions from Splitwise, all transactions from
         your Lunch Money Splitwise account and compares the two.
 
         Returns
         -------
         List[SplitLunchExpense]
         """
         new_transactions, deleted_transactions = self.get_new_transactions()
-        self.splitwise_to_lunchmoney(expenses=new_transactions)
+        self.splitwise_to_lunchmoney(
+            expenses=new_transactions,
+            allow_self_paid=allow_self_paid,
+            allow_payments=allow_payments,
+        )
         splitwise_asset = self.update_splitwise_balance()
         self.handle_deleted_transactions(deleted_transactions=deleted_transactions)
         return dict(
             balance=splitwise_asset.balance,
             new=new_transactions,
             deleted=deleted_transactions,
         )
```

### Comparing `lunchable-0.5.1/lunchable/plugins/splitlunch/models.py` & `lunchable-0.6.0/lunchable/plugins/splitlunch/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     SplitLunch Object for Splitwise Expenses
     """
 
     splitwise_id: int
     original_amount: float
     self_paid: bool
     financial_impact: float
-    personal_share: float
     description: str
     category: str
     details: Optional[str]
     payment: bool
     date: datetime.datetime
     users: List[int]
     created_at: datetime.datetime
```

### Comparing `lunchable-0.5.1/pyproject.toml` & `lunchable-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 documentation = "https://juftin.github.io/lunchable"
 homepage = "https://github.com/juftin/lunchable"
 include = ["lunchable/py.typed"]
 license = "MIT"
 name = "lunchable"
 readme = "README.md"
 repository = "https://github.com/juftin/lunchable"
-version = "0.5.1"
+version = "0.6.0"
 
 [tool.poetry.dependencies]
 click = ">=8.0.1"
 pandas = {version = "^1.3", optional = true}
 pydantic = ">=1.2.0,<2.0.0"
 python = ">=3.7.1,<4.0"
 python-dateutil = {version = "^2.8.2", optional = true}
```

### Comparing `lunchable-0.5.1/PKG-INFO` & `lunchable-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunchable
-Version: 0.5.1
+Version: 0.6.0
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
-Metadata-Version: 2.1 Name: lunchable Version: 0.5.1 Summary: A simple Python
+Metadata-Version: 2.1 Name: lunchable Version: 0.6.0 Summary: A simple Python
 SDK around the Lunch Money Developer API Home-page: https://github.com/juftin/
 lunchable License: MIT Author: Justin Flannery Author-email: juftin@juftin.com
 Requires-Python: >=3.7.1,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

