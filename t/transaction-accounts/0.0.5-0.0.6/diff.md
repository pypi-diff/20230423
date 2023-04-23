# Comparing `tmp/transaction-accounts-0.0.5.tar.gz` & `tmp/transaction-accounts-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction-accounts-0.0.5.tar", last modified: Sun Apr 23 04:01:49 2023, max compression
+gzip compressed data, was "transaction-accounts-0.0.6.tar", last modified: Sun Apr 23 15:22:45 2023, max compression
```

## Comparing `transaction-accounts-0.0.5.tar` & `transaction-accounts-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 04:01:49.872895 transaction-accounts-0.0.5/
--rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.0.5/LICENSE.txt
--rw-r--r--   0 igormusic   (501) staff       (20)     6737 2023-04-23 04:01:49.873030 transaction-accounts-0.0.5/PKG-INFO
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 04:01:49.868031 transaction-accounts-0.0.5/accounts/
--rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.0.5/accounts/__init__.py
--rw-r--r--   0 igormusic   (501) staff       (20)     7044 2023-04-23 03:44:55.000000 transaction-accounts-0.0.5/accounts/metadata.py
--rw-r--r--   0 igormusic   (501) staff       (20)    10797 2023-04-23 03:47:22.000000 transaction-accounts-0.0.5/accounts/runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-04-23 04:01:49.873533 transaction-accounts-0.0.5/setup.cfg
--rw-r--r--   0 igormusic   (501) staff       (20)     7019 2023-04-23 04:01:44.000000 transaction-accounts-0.0.5/setup.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 04:01:49.870513 transaction-accounts-0.0.5/tests/
--rw-r--r--   0 igormusic   (501) staff       (20)     2847 2023-04-23 03:49:18.000000 transaction-accounts-0.0.5/tests/test_config.py
--rw-r--r--   0 igormusic   (501) staff       (20)      982 2023-04-23 03:03:07.000000 transaction-accounts-0.0.5/tests/test_configuration.py
--rw-r--r--   0 igormusic   (501) staff       (20)     1917 2023-04-22 14:06:37.000000 transaction-accounts-0.0.5/tests/test_rate_type.py
--rw-r--r--   0 igormusic   (501) staff       (20)     2209 2023-04-23 03:53:57.000000 transaction-accounts-0.0.5/tests/test_runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)     3915 2023-04-22 15:27:27.000000 transaction-accounts-0.0.5/tests/test_schedule.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 04:01:49.872578 transaction-accounts-0.0.5/transaction_accounts.egg-info/
--rw-r--r--   0 igormusic   (501) staff       (20)     6737 2023-04-23 04:01:49.000000 transaction-accounts-0.0.5/transaction_accounts.egg-info/PKG-INFO
--rw-r--r--   0 igormusic   (501) staff       (20)      429 2023-04-23 04:01:49.000000 transaction-accounts-0.0.5/transaction_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-04-23 04:01:49.000000 transaction-accounts-0.0.5/transaction_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 igormusic   (501) staff       (20)       25 2023-04-23 04:01:49.000000 transaction-accounts-0.0.5/transaction_accounts.egg-info/requires.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-04-23 04:01:49.000000 transaction-accounts-0.0.5/transaction_accounts.egg-info/top_level.txt
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 15:22:45.482520 transaction-accounts-0.0.6/
+-rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.0.6/LICENSE.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-04-23 15:22:45.482666 transaction-accounts-0.0.6/PKG-INFO
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 15:22:45.478129 transaction-accounts-0.0.6/accounts/
+-rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.0.6/accounts/__init__.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     7401 2023-04-23 14:17:53.000000 transaction-accounts-0.0.6/accounts/metadata.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    10924 2023-04-23 14:19:31.000000 transaction-accounts-0.0.6/accounts/runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-04-23 15:22:45.483187 transaction-accounts-0.0.6/setup.cfg
+-rw-r--r--   0 igormusic   (501) staff       (20)     7614 2023-04-23 15:22:39.000000 transaction-accounts-0.0.6/setup.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 15:22:45.480202 transaction-accounts-0.0.6/tests/
+-rw-r--r--   0 igormusic   (501) staff       (20)     3254 2023-04-23 14:51:14.000000 transaction-accounts-0.0.6/tests/test_config.py
+-rw-r--r--   0 igormusic   (501) staff       (20)      982 2023-04-23 03:03:07.000000 transaction-accounts-0.0.6/tests/test_configuration.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     1917 2023-04-22 14:06:37.000000 transaction-accounts-0.0.6/tests/test_rate_type.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     2242 2023-04-23 14:55:48.000000 transaction-accounts-0.0.6/tests/test_runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     3915 2023-04-22 15:27:27.000000 transaction-accounts-0.0.6/tests/test_schedule.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 15:22:45.482223 transaction-accounts-0.0.6/transaction_accounts.egg-info/
+-rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-04-23 15:22:45.000000 transaction-accounts-0.0.6/transaction_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 igormusic   (501) staff       (20)      429 2023-04-23 15:22:45.000000 transaction-accounts-0.0.6/transaction_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-04-23 15:22:45.000000 transaction-accounts-0.0.6/transaction_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)       25 2023-04-23 15:22:45.000000 transaction-accounts-0.0.6/transaction_accounts.egg-info/requires.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-04-23 15:22:45.000000 transaction-accounts-0.0.6/transaction_accounts.egg-info/top_level.txt
```

### Comparing `transaction-accounts-0.0.5/LICENSE.txt` & `transaction-accounts-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.0.5/PKG-INFO` & `transaction-accounts-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,110 +1,109 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.0.5
+Version: 0.0.6
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
-Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.4.tar.gz
+Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE.txt
 
 
 Transaction Accounts
 ====================
 
-This library provides basic functionality for working with transaction
-accounts.
+This library provides basic functionality for working with transaction accounts.
 
-You can use it to make any type of transaction account, such as a
-savings account, a credit card, or a loan.
+You can use it to make any type of transaction account, such as a savings account, a credit card, or a loan.
 
-Assume we would like to create simple Savings Account that has 3 types
-of balances:
- 
-- current balance 
-- interest accrued 
+Assume we would like to create simple Savings Account that has 3 types of balances:
+
+- current balance
+- interest accrued
 - withholding tax
 
-We would like to have 4 types of transactions: 
+We would like to have 4 types of transactions:
 
-- deposit 
-- interest accrued 
-- interest capitalized 
+- deposit
+- interest accrued
+- interest capitalized
 - withholding tax
 
-We would like to have 2 types of schedules: 
+We would like to have 2 types of schedules:
 
-- accrual schedule 
+- accrual schedule
 - compounding schedule
 
-We would like to have interest rate with 3 tiers: 
+We would like to have interest rate with 3 tiers:
 
-- 0 - 10000: 3% 
-- 10000 - 50000: 3.5% 
+- 0 - 10000: 3%
+- 10000 - 50000: 3.5%
 - 50000+: 4%
 
-Deposit transaction will increase current balance, and it will be used
-to deposit money to the account. This transaction will be externally
-created and posted to the account.
-
-Interest accrued transaction will increase interest accrued balance, and
-it will be used to accrue interest on the account.
-
-Interest will be accrued daily, and it will be calculated based on
-current balance and interest rate.
-
-Interest capitalized transaction will increase current balance and
-decrease interest accrued balance. This transaction will be internally
-created and posted to the account at the end of each month.
-
-Withholding tax transaction will decrease withholding tax balance, and
-it will be used to pay withholding tax on the account. It will be
-calculated as 20% of interest capitalized transaction.
+We would like to have monthly fee of 1.00 charged at the end of each month to the account before interest is accrued.
+
+Deposit transaction will increase current balance, and it will be used to deposit money to the account. 
+This transaction will be externally created and posted to the account.
+
+Interest accrued transaction will increase interest accrued balance, and it will be used to accrue interest on the account.
+
+Interest will be accrued daily, and it will be calculated based on current balance and interest rate.
+
+Interest capitalized transaction will increase current balance and decrease interest accrued balance.
+This transaction will be internally created and posted to the account at the end of each month.
+
+Withholding tax transaction will decrease withholding tax balance, and it will be used to pay withholding tax on the account. 
+It will be calculated as 20% of interest capitalized transaction.
 
-We will use accrual schedule to accrue interest daily, and we will use
-compounding schedule to capitalize interest at the end of each month.
+We will use accrual schedule to accrue interest daily, and we will use compounding schedule to capitalize interest at the end of each month.
 
 We will use interest rate to calculate interest.
 
 We will use trigger transaction to calculate withholding tax.
 
-Note that this framework is not limited to this configuration, and it
-can be used to create any type of transaction account.
+We will use monthly fee property to specify monthly fee. This amount will be charged at the end of each month.
 
-You can define custom calculations when calculating either schedules or
-transactions. In this context you can use any of the following
-variables: - account: Account - transaction: Transaction - config:
-Configuration
+Note that this framework is not limited to this configuration, and it can be used to create any type of transaction account.
+
+You can define custom calculations when calculating either schedules or transactions. In this context you can use any of the following variables:
+
+- account: Account
+- transaction: Transaction
+- config: Configuration
 
 Here is a code that will create this configuration:
 
 .. code:: python
 
  def create_savings_account() -> AccountType:
     acc = AccountType(name="savingsAccount", label="Savings Account")
 
     current = acc.add_position_type("current", "current balance")
     interest_accrued = acc.add_position_type("accrued", "interest accrued")
     withholding = acc.add_position_type("withholding", "withholding tax")
 
-    acc.add_transaction_type("deposit", "Deposit")        .add_position_rule(TransactionOperation.CREDIT, current)
+    montly_fee = acc.add_property_type("monthlyFee", "Monthly Fee", DataType.DECIMAL, True)
+
+    acc.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
 
-    interest_accrued_tt = acc.add_transaction_type("interestAccrued", "Interest Accrued")         .add_position_rule(TransactionOperation.CREDIT, interest_accrued)
+    fee_tt = acc.add_transaction_type("fee", "Fee").add_position_rule(TransactionOperation.DEBIT, current)
 
-    capitalized_tt = acc.add_transaction_type("capitalized", "Interest Capitalized")         .add_position_rule(TransactionOperation.CREDIT, current)         .add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+    interest_accrued_tt = acc.add_transaction_type("interestAccrued", "Interest Accrued").add_position_rule(TransactionOperation.CREDIT, interest_accrued)
 
-    withholding_tt = acc.add_transaction_type("withholdingTax", "Withholding Tax")         .add_position_rule(TransactionOperation.CREDIT, withholding)
+    capitalized_tt = acc.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+
+    withholding_tt = acc.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(TransactionOperation.CREDIT, withholding)
 
     accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
                                     end_type=ScheduleEndType.NO_END,
                                     business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
                                     interval_expression="1", start_date_expression="account.start_date")
 
     acc.add_schedule_type(accrual_schedule)
@@ -114,14 +113,18 @@
                                         end_type=ScheduleEndType.NO_END,
                                         business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
                                         interval_expression="1",
                                         start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
 
     acc.add_schedule_type(compounding_schedule)
 
+    acc.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                  fee_tt,
+                                  "account.monthlyFee")
+
     acc.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
                                   interest_accrued_tt,
                                   "account.current * accountType.interest.get_rate(account.current) / Decimal(365)")
 
     acc.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
                                   capitalized_tt, "account.accrued")
 
@@ -141,24 +144,24 @@
 
 .. code:: python
 
  def test_valuation(self):
         account_type = create_savings_account()
 
         account = Account(start_date=date(2019, 1, 1), account_type_name=account_type.name,
-                          account_type=account_type)
+                          account_type=account_type, properties={"monthlyFee": Decimal(1.00)})
 
         valuation = AccountValuation(account, account_type, date(2020, 1, 1))
 
         deposit_transaction_type = account_type.get_transaction_type("deposit")
 
         external_transactions = group_by_date([
             ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
                                 amount=Decimal(1000), value_date=date(2019, 1, 1))])
 
         valuation.forecast(date(2020, 1, 1), external_transactions)
 
-        self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
-        self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
-        self.assertAlmostEqual(account.transactions[1].amount, Decimal('0.0821'), places=1)
+        self.assertAlmostEqual(account.positions['current'].amount, Decimal(1018.24775), places=4)
+        self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(6.04955), places=4)
+        self.assertAlmostEqual(account.transactions[1].amount, Decimal('0.08219'), places=4)
```

### Comparing `transaction-accounts-0.0.5/accounts/metadata.py` & `transaction-accounts-0.0.6/accounts/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class TransactionOperation(Enum):
     CREDIT = 'credit'
     DEBIT = 'debit'
     SET = 'set'
 
 
 class DataType(Enum):
-    NUMBER = 'number'
+    DECIMAL = 'decimal'
     STRING = 'string'
     BOOLEAN = 'boolean'
 
 
 class ScheduleEndType(Enum):
     NO_END = "no_end"
     END_REPEATS = "end_repeats"
@@ -143,28 +143,35 @@
     generated_transaction_type: str
     amount_expression: str
 
 
 class PropertyType(BaseModel):
     name: str
     label: str
+    data_type: DataType
+    required: bool = True
 
 
 class AccountType(BaseModel):
     name: str
     label: str
     transaction_types: List[TransactionType] = []
     position_types: List[PositionType] = []
     rate_types: Dict[str, RateType] = {}
     triggered_transactions: List[TriggeredTransaction] = []
     schedule_types: List[ScheduleType] = []
     property_types: List[PropertyType] = []
     scheduled_transactions: List[ScheduledTransaction] = []
     triggered_transactions: List[TriggeredTransaction] = []
 
+    def add_property_type(self, name: str, label: str, data_type: DataType, required: bool = True) -> PropertyType:
+        property_type = PropertyType(name=name, label=label, data_type=data_type.value, required=required)
+        self.property_types.append(property_type)
+        return property_type
+
     def add_transaction_type(self, name: str, label: str) -> TransactionType:
         transaction_type = TransactionType(name=name, label=label)
         self.transaction_types.append(transaction_type)
         return transaction_type
 
     def add_position_type(self, name: str, label: str) -> PositionType:
         position_type = PositionType(name=name, label=label)
@@ -179,33 +186,35 @@
     def add_trigger_transaction(self, trigger_transaction_type: TransactionType,
                                 generated_transaction_type: TransactionType, amount_expression: str):
         trigger_transaction = TriggeredTransaction(trigger_transaction_type_name=trigger_transaction_type.name,
                                                    generated_transaction_type=generated_transaction_type.name,
                                                    amount_expression=amount_expression)
         self.triggered_transactions.append(trigger_transaction)
 
+    def add_schedule_type(self, schedule_type: ScheduleType):
+        self.schedule_types.append(schedule_type)
+
+    def add_scheduled_transaction(self, schedule_type: ScheduleType, timing: ScheduledTransactionTiming,
+                                  generated_transaction_type: TransactionType, amount_expression: str):
+        scheduled_transaction = ScheduledTransaction(schedule_name=schedule_type.name, timing=timing,
+                                                     generated_transaction_type=generated_transaction_type.name,
+                                                     amount_expression=amount_expression)
+        self.scheduled_transactions.append(scheduled_transaction)
+
     def get_transaction_type(self, transaction_type_name: str) -> TransactionType:
         return next(tt for tt in self.transaction_types if tt.name == transaction_type_name)
 
     def get_rate_type(self, rate_type_name: str):
         return next(rt for rt in self.rate_types if rt.name == rate_type_name)
 
     def get_trigger_transaction(self, trigger_transaction_type_name: str) -> Optional[TriggeredTransaction]:
         return next((tt for tt in self.triggered_transactions if
                      tt.trigger_transaction_type_name == trigger_transaction_type_name), None)
 
-    def add_schedule_type(self, schedule_type: ScheduleType):
-        self.schedule_types.append(schedule_type)
 
-    def add_scheduled_transaction(self, schedule_type: ScheduleType, timing: ScheduledTransactionTiming,
-                                  generated_transaction_type: TransactionType, amount_expression: str):
-        scheduled_transaction = ScheduledTransaction(schedule_name=schedule_type.name, timing=timing,
-                                                     generated_transaction_type=generated_transaction_type.name,
-                                                     amount_expression=amount_expression)
-        self.scheduled_transactions.append(scheduled_transaction)
 
     def __getattr__(self, method_name):
         if method_name in self.rate_types:
             return self.rate_types[method_name]
         else:
             raise AttributeError(f'No such attribute: {method_name}')
```

### Comparing `transaction-accounts-0.0.5/accounts/runtime.py` & `transaction-accounts-0.0.6/accounts/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
     value_date: date
 
 
 class Account(BaseModel):
     start_date: date
     account_type_name: str
     positions: dict[str, Position] = {}
+    properties: dict[str, Any] = {}
     schedules: dict[str, Schedule] = {}
     transactions: list[Transaction] = []
 
     def __init__(self, **kw):
         super().__init__(**kw)
         if "account_type" in kw:
             account_type: AccountType = kw["account_type"]
@@ -172,14 +173,16 @@
             raise ValueError(f'Error evaluating expression: {expression} {e.args}') from e
         else:
             return value
 
     def __getattr__(self, method_name):
         if method_name in self.positions:
             return self.positions[method_name].amount
+        if method_name in self.properties:
+            return self.properties[method_name]
         else:
             raise AttributeError(f'No such attribute: {method_name}')
 
     class Config:
         exclude = {"config"}
```

### Comparing `transaction-accounts-0.0.5/setup.py` & `transaction-accounts-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,104 +1,98 @@
 from setuptools import setup, find_packages
 
 setup(
     name='transaction-accounts',
-    version='0.0.5',
+    version='0.0.6',
     description='Create configuration for transactional accounts and implement account runtime',
     long_description='''
 Transaction Accounts
 ====================
 
-This library provides basic functionality for working with transaction
-accounts.
+This library provides basic functionality for working with transaction accounts.
 
-You can use it to make any type of transaction account, such as a
-savings account, a credit card, or a loan.
+You can use it to make any type of transaction account, such as a savings account, a credit card, or a loan.
 
-Assume we would like to create simple Savings Account that has 3 types
-of balances:
- 
-- current balance 
-- interest accrued 
+Assume we would like to create simple Savings Account that has 3 types of balances:
+
+- current balance
+- interest accrued
 - withholding tax
 
-We would like to have 4 types of transactions: 
+We would like to have 4 types of transactions:
 
-- deposit 
-- interest accrued 
-- interest capitalized 
+- deposit
+- interest accrued
+- interest capitalized
 - withholding tax
 
-We would like to have 2 types of schedules: 
+We would like to have 2 types of schedules:
 
-- accrual schedule 
+- accrual schedule
 - compounding schedule
 
-We would like to have interest rate with 3 tiers: 
+We would like to have interest rate with 3 tiers:
 
-- 0 - 10000: 3% 
-- 10000 - 50000: 3.5% 
+- 0 - 10000: 3%
+- 10000 - 50000: 3.5%
 - 50000+: 4%
 
-Deposit transaction will increase current balance, and it will be used
-to deposit money to the account. This transaction will be externally
-created and posted to the account.
-
-Interest accrued transaction will increase interest accrued balance, and
-it will be used to accrue interest on the account.
-
-Interest will be accrued daily, and it will be calculated based on
-current balance and interest rate.
-
-Interest capitalized transaction will increase current balance and
-decrease interest accrued balance. This transaction will be internally
-created and posted to the account at the end of each month.
-
-Withholding tax transaction will decrease withholding tax balance, and
-it will be used to pay withholding tax on the account. It will be
-calculated as 20% of interest capitalized transaction.
+We would like to have monthly fee of 1.00 charged at the end of each month to the account before interest is accrued.
+
+Deposit transaction will increase current balance, and it will be used to deposit money to the account. 
+This transaction will be externally created and posted to the account.
+
+Interest accrued transaction will increase interest accrued balance, and it will be used to accrue interest on the account.
+
+Interest will be accrued daily, and it will be calculated based on current balance and interest rate.
+
+Interest capitalized transaction will increase current balance and decrease interest accrued balance.
+This transaction will be internally created and posted to the account at the end of each month.
+
+Withholding tax transaction will decrease withholding tax balance, and it will be used to pay withholding tax on the account. 
+It will be calculated as 20% of interest capitalized transaction.
 
-We will use accrual schedule to accrue interest daily, and we will use
-compounding schedule to capitalize interest at the end of each month.
+We will use accrual schedule to accrue interest daily, and we will use compounding schedule to capitalize interest at the end of each month.
 
 We will use interest rate to calculate interest.
 
 We will use trigger transaction to calculate withholding tax.
 
-Note that this framework is not limited to this configuration, and it
-can be used to create any type of transaction account.
+We will use monthly fee property to specify monthly fee. This amount will be charged at the end of each month.
 
-You can define custom calculations when calculating either schedules or
-transactions. In this context you can use any of the following
-variables: - account: Account - transaction: Transaction - config:
-Configuration
+Note that this framework is not limited to this configuration, and it can be used to create any type of transaction account.
+
+You can define custom calculations when calculating either schedules or transactions. In this context you can use any of the following variables:
+
+- account: Account
+- transaction: Transaction
+- config: Configuration
 
 Here is a code that will create this configuration:
 
 .. code:: python
 
  def create_savings_account() -> AccountType:
     acc = AccountType(name="savingsAccount", label="Savings Account")
 
     current = acc.add_position_type("current", "current balance")
     interest_accrued = acc.add_position_type("accrued", "interest accrued")
     withholding = acc.add_position_type("withholding", "withholding tax")
 
-    acc.add_transaction_type("deposit", "Deposit")\
-        .add_position_rule(TransactionOperation.CREDIT, current)
+    montly_fee = acc.add_property_type("monthlyFee", "Monthly Fee", DataType.DECIMAL, True)
+
+    acc.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
 
-    interest_accrued_tt = acc.add_transaction_type("interestAccrued", "Interest Accrued") \
-        .add_position_rule(TransactionOperation.CREDIT, interest_accrued)
+    fee_tt = acc.add_transaction_type("fee", "Fee").add_position_rule(TransactionOperation.DEBIT, current)
 
-    capitalized_tt = acc.add_transaction_type("capitalized", "Interest Capitalized") \
-        .add_position_rule(TransactionOperation.CREDIT, current) \
-        .add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+    interest_accrued_tt = acc.add_transaction_type("interestAccrued", "Interest Accrued").add_position_rule(TransactionOperation.CREDIT, interest_accrued)
 
-    withholding_tt = acc.add_transaction_type("withholdingTax", "Withholding Tax") \
-        .add_position_rule(TransactionOperation.CREDIT, withholding)
+    capitalized_tt = acc.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+
+    withholding_tt = acc.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(TransactionOperation.CREDIT, withholding)
 
     accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
                                     end_type=ScheduleEndType.NO_END,
                                     business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
                                     interval_expression="1", start_date_expression="account.start_date")
 
     acc.add_schedule_type(accrual_schedule)
@@ -108,14 +102,18 @@
                                         end_type=ScheduleEndType.NO_END,
                                         business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
                                         interval_expression="1",
                                         start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
 
     acc.add_schedule_type(compounding_schedule)
 
+    acc.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                  fee_tt,
+                                  "account.monthlyFee")
+
     acc.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
                                   interest_accrued_tt,
                                   "account.current * accountType.interest.get_rate(account.current) / Decimal(365)")
 
     acc.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
                                   capitalized_tt, "account.accrued")
 
@@ -135,43 +133,43 @@
 
 .. code:: python
 
  def test_valuation(self):
         account_type = create_savings_account()
 
         account = Account(start_date=date(2019, 1, 1), account_type_name=account_type.name,
-                          account_type=account_type)
+                          account_type=account_type, properties={"monthlyFee": Decimal(1.00)})
 
         valuation = AccountValuation(account, account_type, date(2020, 1, 1))
 
         deposit_transaction_type = account_type.get_transaction_type("deposit")
 
         external_transactions = group_by_date([
             ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
                                 amount=Decimal(1000), value_date=date(2019, 1, 1))])
 
         valuation.forecast(date(2020, 1, 1), external_transactions)
 
-        self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
-        self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
-        self.assertAlmostEqual(account.transactions[1].amount, Decimal('0.0821'), places=1)
+        self.assertAlmostEqual(account.positions['current'].amount, Decimal(1018.24775), places=4)
+        self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(6.04955), places=4)
+        self.assertAlmostEqual(account.transactions[1].amount, Decimal('0.08219'), places=4)
     
     ''',
     author='Igor Music',
     author_email='igormusich@gmail.com',
     packages=find_packages(),
     license='MIT',
     url='https://github.com/igormusic/transaction-accounts',
-    download_url='https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.4.tar.gz',
+    download_url='https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz',
     keywords=['TRANSACTION PROCESSING', 'LOANS', 'SAVINGS', 'ACCOUNTS', 'FINANCE', 'BANKING'],
     install_requires=[
         'python-dateutil',
         'pydantic'
     ],
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',  # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
     ],
 )
```

### Comparing `transaction-accounts-0.0.5/tests/test_config.py` & `transaction-accounts-0.0.6/tests/test_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,22 @@
 def create_savings_account() -> AccountType:
     acc = AccountType(name="savingsAccount", label="Savings Account")
 
     current = acc.add_position_type("current", "current balance")
     interest_accrued = acc.add_position_type("accrued", "interest accrued")
     withholding = acc.add_position_type("withholding", "withholding tax")
 
-    acc.add_transaction_type("deposit", "Deposit")\
+    montly_fee = acc.add_property_type("monthlyFee", "Monthly Fee", DataType.DECIMAL, True)
+
+    acc.add_transaction_type("deposit", "Deposit") \
         .add_position_rule(TransactionOperation.CREDIT, current)
 
+    fee_tt = acc.add_transaction_type("fee", "Fee") \
+        .add_position_rule(TransactionOperation.DEBIT, current)
+
     interest_accrued_tt = acc.add_transaction_type("interestAccrued", "Interest Accrued") \
         .add_position_rule(TransactionOperation.CREDIT, interest_accrued)
 
     capitalized_tt = acc.add_transaction_type("capitalized", "Interest Capitalized") \
         .add_position_rule(TransactionOperation.CREDIT, current) \
         .add_position_rule(TransactionOperation.DEBIT, interest_accrued)
 
@@ -33,14 +38,18 @@
                                         end_type=ScheduleEndType.NO_END,
                                         business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
                                         interval_expression="1",
                                         start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
 
     acc.add_schedule_type(compounding_schedule)
 
+    acc.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                  fee_tt,
+                                  "account.monthlyFee")
+
     acc.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
                                   interest_accrued_tt,
                                   "account.current * accountType.interest.get_rate(account.current) / Decimal(365)")
 
     acc.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
                                   capitalized_tt, "account.accrued")
```

### Comparing `transaction-accounts-0.0.5/tests/test_configuration.py` & `transaction-accounts-0.0.6/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.0.5/tests/test_rate_type.py` & `transaction-accounts-0.0.6/tests/test_rate_type.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.0.5/tests/test_runtime.py` & `transaction-accounts-0.0.6/tests/test_runtime.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,26 +32,26 @@
                          account.evaluate("self.start_date + relativedelta(months=+1) + relativedelta(days=-1)",
                                           None))
 
     def test_valuation(self):
         account_type = create_savings_account()
 
         account = Account(start_date=date(2019, 1, 1), account_type_name=account_type.name,
-                          account_type=account_type)
+                          account_type=account_type, properties={"monthlyFee": Decimal(1.00)})
 
         valuation = AccountValuation(account, account_type, date(2020, 1, 1))
 
         deposit_transaction_type = account_type.get_transaction_type("deposit")
 
         external_transactions = group_by_date([
             ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
                                 amount=Decimal(1000), value_date=date(2019, 1, 1))])
 
         valuation.forecast(date(2020, 1, 1), external_transactions)
 
-        self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
-        self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
-        self.assertAlmostEqual(account.transactions[1].amount, Decimal('0.0821'), places=1)
+        self.assertAlmostEqual(account.positions['current'].amount, Decimal(1018.24775), places=4)
+        self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(6.04955), places=4)
+        self.assertAlmostEqual(account.transactions[1].amount, Decimal('0.08219'), places=4)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `transaction-accounts-0.0.5/tests/test_schedule.py` & `transaction-accounts-0.0.6/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.0.5/transaction_accounts.egg-info/PKG-INFO` & `transaction-accounts-0.0.6/transaction_accounts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,110 +1,109 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.0.5
+Version: 0.0.6
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
-Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.4.tar.gz
+Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE.txt
 
 
 Transaction Accounts
 ====================
 
-This library provides basic functionality for working with transaction
-accounts.
+This library provides basic functionality for working with transaction accounts.
 
-You can use it to make any type of transaction account, such as a
-savings account, a credit card, or a loan.
+You can use it to make any type of transaction account, such as a savings account, a credit card, or a loan.
 
-Assume we would like to create simple Savings Account that has 3 types
-of balances:
- 
-- current balance 
-- interest accrued 
+Assume we would like to create simple Savings Account that has 3 types of balances:
+
+- current balance
+- interest accrued
 - withholding tax
 
-We would like to have 4 types of transactions: 
+We would like to have 4 types of transactions:
 
-- deposit 
-- interest accrued 
-- interest capitalized 
+- deposit
+- interest accrued
+- interest capitalized
 - withholding tax
 
-We would like to have 2 types of schedules: 
+We would like to have 2 types of schedules:
 
-- accrual schedule 
+- accrual schedule
 - compounding schedule
 
-We would like to have interest rate with 3 tiers: 
+We would like to have interest rate with 3 tiers:
 
-- 0 - 10000: 3% 
-- 10000 - 50000: 3.5% 
+- 0 - 10000: 3%
+- 10000 - 50000: 3.5%
 - 50000+: 4%
 
-Deposit transaction will increase current balance, and it will be used
-to deposit money to the account. This transaction will be externally
-created and posted to the account.
-
-Interest accrued transaction will increase interest accrued balance, and
-it will be used to accrue interest on the account.
-
-Interest will be accrued daily, and it will be calculated based on
-current balance and interest rate.
-
-Interest capitalized transaction will increase current balance and
-decrease interest accrued balance. This transaction will be internally
-created and posted to the account at the end of each month.
-
-Withholding tax transaction will decrease withholding tax balance, and
-it will be used to pay withholding tax on the account. It will be
-calculated as 20% of interest capitalized transaction.
+We would like to have monthly fee of 1.00 charged at the end of each month to the account before interest is accrued.
+
+Deposit transaction will increase current balance, and it will be used to deposit money to the account. 
+This transaction will be externally created and posted to the account.
+
+Interest accrued transaction will increase interest accrued balance, and it will be used to accrue interest on the account.
+
+Interest will be accrued daily, and it will be calculated based on current balance and interest rate.
+
+Interest capitalized transaction will increase current balance and decrease interest accrued balance.
+This transaction will be internally created and posted to the account at the end of each month.
+
+Withholding tax transaction will decrease withholding tax balance, and it will be used to pay withholding tax on the account. 
+It will be calculated as 20% of interest capitalized transaction.
 
-We will use accrual schedule to accrue interest daily, and we will use
-compounding schedule to capitalize interest at the end of each month.
+We will use accrual schedule to accrue interest daily, and we will use compounding schedule to capitalize interest at the end of each month.
 
 We will use interest rate to calculate interest.
 
 We will use trigger transaction to calculate withholding tax.
 
-Note that this framework is not limited to this configuration, and it
-can be used to create any type of transaction account.
+We will use monthly fee property to specify monthly fee. This amount will be charged at the end of each month.
 
-You can define custom calculations when calculating either schedules or
-transactions. In this context you can use any of the following
-variables: - account: Account - transaction: Transaction - config:
-Configuration
+Note that this framework is not limited to this configuration, and it can be used to create any type of transaction account.
+
+You can define custom calculations when calculating either schedules or transactions. In this context you can use any of the following variables:
+
+- account: Account
+- transaction: Transaction
+- config: Configuration
 
 Here is a code that will create this configuration:
 
 .. code:: python
 
  def create_savings_account() -> AccountType:
     acc = AccountType(name="savingsAccount", label="Savings Account")
 
     current = acc.add_position_type("current", "current balance")
     interest_accrued = acc.add_position_type("accrued", "interest accrued")
     withholding = acc.add_position_type("withholding", "withholding tax")
 
-    acc.add_transaction_type("deposit", "Deposit")        .add_position_rule(TransactionOperation.CREDIT, current)
+    montly_fee = acc.add_property_type("monthlyFee", "Monthly Fee", DataType.DECIMAL, True)
+
+    acc.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
 
-    interest_accrued_tt = acc.add_transaction_type("interestAccrued", "Interest Accrued")         .add_position_rule(TransactionOperation.CREDIT, interest_accrued)
+    fee_tt = acc.add_transaction_type("fee", "Fee").add_position_rule(TransactionOperation.DEBIT, current)
 
-    capitalized_tt = acc.add_transaction_type("capitalized", "Interest Capitalized")         .add_position_rule(TransactionOperation.CREDIT, current)         .add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+    interest_accrued_tt = acc.add_transaction_type("interestAccrued", "Interest Accrued").add_position_rule(TransactionOperation.CREDIT, interest_accrued)
 
-    withholding_tt = acc.add_transaction_type("withholdingTax", "Withholding Tax")         .add_position_rule(TransactionOperation.CREDIT, withholding)
+    capitalized_tt = acc.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+
+    withholding_tt = acc.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(TransactionOperation.CREDIT, withholding)
 
     accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
                                     end_type=ScheduleEndType.NO_END,
                                     business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
                                     interval_expression="1", start_date_expression="account.start_date")
 
     acc.add_schedule_type(accrual_schedule)
@@ -114,14 +113,18 @@
                                         end_type=ScheduleEndType.NO_END,
                                         business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
                                         interval_expression="1",
                                         start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
 
     acc.add_schedule_type(compounding_schedule)
 
+    acc.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                  fee_tt,
+                                  "account.monthlyFee")
+
     acc.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
                                   interest_accrued_tt,
                                   "account.current * accountType.interest.get_rate(account.current) / Decimal(365)")
 
     acc.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
                                   capitalized_tt, "account.accrued")
 
@@ -141,24 +144,24 @@
 
 .. code:: python
 
  def test_valuation(self):
         account_type = create_savings_account()
 
         account = Account(start_date=date(2019, 1, 1), account_type_name=account_type.name,
-                          account_type=account_type)
+                          account_type=account_type, properties={"monthlyFee": Decimal(1.00)})
 
         valuation = AccountValuation(account, account_type, date(2020, 1, 1))
 
         deposit_transaction_type = account_type.get_transaction_type("deposit")
 
         external_transactions = group_by_date([
             ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
                                 amount=Decimal(1000), value_date=date(2019, 1, 1))])
 
         valuation.forecast(date(2020, 1, 1), external_transactions)
 
-        self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
-        self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
-        self.assertAlmostEqual(account.transactions[1].amount, Decimal('0.0821'), places=1)
+        self.assertAlmostEqual(account.positions['current'].amount, Decimal(1018.24775), places=4)
+        self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(6.04955), places=4)
+        self.assertAlmostEqual(account.transactions[1].amount, Decimal('0.08219'), places=4)
```

