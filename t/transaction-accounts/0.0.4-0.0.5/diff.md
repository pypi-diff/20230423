# Comparing `tmp/transaction-accounts-0.0.4.tar.gz` & `tmp/transaction-accounts-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction-accounts-0.0.4.tar", last modified: Sat Apr 22 15:43:52 2023, max compression
+gzip compressed data, was "transaction-accounts-0.0.5.tar", last modified: Sun Apr 23 04:01:49 2023, max compression
```

## Comparing `transaction-accounts-0.0.4.tar` & `transaction-accounts-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 15:43:52.161280 transaction-accounts-0.0.4/
--rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.0.4/LICENSE.txt
--rw-r--r--   0 igormusic   (501) staff       (20)     7382 2023-04-22 15:43:52.161448 transaction-accounts-0.0.4/PKG-INFO
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 15:43:52.154827 transaction-accounts-0.0.4/accounts/
--rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.0.4/accounts/__init__.py
--rw-r--r--   0 igormusic   (501) staff       (20)     8251 2023-04-22 13:55:27.000000 transaction-accounts-0.0.4/accounts/metadata.py
--rw-r--r--   0 igormusic   (501) staff       (20)    11134 2023-04-22 15:23:52.000000 transaction-accounts-0.0.4/accounts/runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-04-22 15:43:52.162097 transaction-accounts-0.0.4/setup.cfg
--rw-r--r--   0 igormusic   (501) staff       (20)     7655 2023-04-22 15:43:43.000000 transaction-accounts-0.0.4/setup.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 15:43:52.158023 transaction-accounts-0.0.4/tests/
--rw-r--r--   0 igormusic   (501) staff       (20)     3204 2023-04-22 13:49:23.000000 transaction-accounts-0.0.4/tests/test_config.py
--rw-r--r--   0 igormusic   (501) staff       (20)      960 2023-04-22 14:02:47.000000 transaction-accounts-0.0.4/tests/test_configuration.py
--rw-r--r--   0 igormusic   (501) staff       (20)     1917 2023-04-22 14:06:37.000000 transaction-accounts-0.0.4/tests/test_rate_type.py
--rw-r--r--   0 igormusic   (501) staff       (20)     2556 2023-04-22 15:20:57.000000 transaction-accounts-0.0.4/tests/test_runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)     3915 2023-04-22 15:27:27.000000 transaction-accounts-0.0.4/tests/test_schedule.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-22 15:43:52.160676 transaction-accounts-0.0.4/transaction_accounts.egg-info/
--rw-r--r--   0 igormusic   (501) staff       (20)     7382 2023-04-22 15:43:52.000000 transaction-accounts-0.0.4/transaction_accounts.egg-info/PKG-INFO
--rw-r--r--   0 igormusic   (501) staff       (20)      429 2023-04-22 15:43:52.000000 transaction-accounts-0.0.4/transaction_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-04-22 15:43:52.000000 transaction-accounts-0.0.4/transaction_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 igormusic   (501) staff       (20)       25 2023-04-22 15:43:52.000000 transaction-accounts-0.0.4/transaction_accounts.egg-info/requires.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-04-22 15:43:52.000000 transaction-accounts-0.0.4/transaction_accounts.egg-info/top_level.txt
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 04:01:49.872895 transaction-accounts-0.0.5/
+-rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.0.5/LICENSE.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)     6737 2023-04-23 04:01:49.873030 transaction-accounts-0.0.5/PKG-INFO
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 04:01:49.868031 transaction-accounts-0.0.5/accounts/
+-rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.0.5/accounts/__init__.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     7044 2023-04-23 03:44:55.000000 transaction-accounts-0.0.5/accounts/metadata.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    10797 2023-04-23 03:47:22.000000 transaction-accounts-0.0.5/accounts/runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-04-23 04:01:49.873533 transaction-accounts-0.0.5/setup.cfg
+-rw-r--r--   0 igormusic   (501) staff       (20)     7019 2023-04-23 04:01:44.000000 transaction-accounts-0.0.5/setup.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 04:01:49.870513 transaction-accounts-0.0.5/tests/
+-rw-r--r--   0 igormusic   (501) staff       (20)     2847 2023-04-23 03:49:18.000000 transaction-accounts-0.0.5/tests/test_config.py
+-rw-r--r--   0 igormusic   (501) staff       (20)      982 2023-04-23 03:03:07.000000 transaction-accounts-0.0.5/tests/test_configuration.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     1917 2023-04-22 14:06:37.000000 transaction-accounts-0.0.5/tests/test_rate_type.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     2209 2023-04-23 03:53:57.000000 transaction-accounts-0.0.5/tests/test_runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     3915 2023-04-22 15:27:27.000000 transaction-accounts-0.0.5/tests/test_schedule.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-04-23 04:01:49.872578 transaction-accounts-0.0.5/transaction_accounts.egg-info/
+-rw-r--r--   0 igormusic   (501) staff       (20)     6737 2023-04-23 04:01:49.000000 transaction-accounts-0.0.5/transaction_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 igormusic   (501) staff       (20)      429 2023-04-23 04:01:49.000000 transaction-accounts-0.0.5/transaction_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-04-23 04:01:49.000000 transaction-accounts-0.0.5/transaction_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)       25 2023-04-23 04:01:49.000000 transaction-accounts-0.0.5/transaction_accounts.egg-info/requires.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-04-23 04:01:49.000000 transaction-accounts-0.0.5/transaction_accounts.egg-info/top_level.txt
```

### Comparing `transaction-accounts-0.0.4/LICENSE.txt` & `transaction-accounts-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.0.4/PKG-INFO` & `transaction-accounts-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.4.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
@@ -83,90 +83,82 @@
 variables: - account: Account - transaction: Transaction - config:
 Configuration
 
 Here is a code that will create this configuration:
 
 .. code:: python
 
-    def create_savings_account() -> Configuration:
-        config: Configuration = Configuration(version="v1")
-    
-        current = config.add_position_type("current", "current balance")
-        interest_accrued = config.add_position_type("accrued", "interest accrued")
-        withholding = config.add_position_type("withholding", "withholding tax")
-    
-        deposit = config.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
-    
-        interest_accrued_tt = config.add_transaction_type("interestAccrued", "Interest Accrued")
-        interest_accrued_tt.add_position_rule(TransactionOperation.CREDIT, interest_accrued)
-    
-        capitalized = config.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(
-            TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
-    
-        withholding_txn = config.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(
-            TransactionOperation.CREDIT, withholding)
-    
-        savings_account = config.add_account_type("savingsAccount", "Savings Account")
-    
-        savings_account.add_transaction_type(deposit)
-        savings_account.add_transaction_type(interest_accrued_tt)
-        savings_account.add_transaction_type(capitalized)
-        savings_account.add_transaction_type(withholding_txn)
-    
-        accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
+ def create_savings_account() -> AccountType:
+    acc = AccountType(name="savingsAccount", label="Savings Account")
+
+    current = acc.add_position_type("current", "current balance")
+    interest_accrued = acc.add_position_type("accrued", "interest accrued")
+    withholding = acc.add_position_type("withholding", "withholding tax")
+
+    acc.add_transaction_type("deposit", "Deposit")        .add_position_rule(TransactionOperation.CREDIT, current)
+
+    interest_accrued_tt = acc.add_transaction_type("interestAccrued", "Interest Accrued")         .add_position_rule(TransactionOperation.CREDIT, interest_accrued)
+
+    capitalized_tt = acc.add_transaction_type("capitalized", "Interest Capitalized")         .add_position_rule(TransactionOperation.CREDIT, current)         .add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+
+    withholding_tt = acc.add_transaction_type("withholdingTax", "Withholding Tax")         .add_position_rule(TransactionOperation.CREDIT, withholding)
+
+    accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
+                                    end_type=ScheduleEndType.NO_END,
+                                    business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
+                                    interval_expression="1", start_date_expression="account.start_date")
+
+    acc.add_schedule_type(accrual_schedule)
+
+    compounding_schedule = ScheduleType(name="compounding", label="Compounding Schedule",
+                                        frequency=ScheduleFrequency.MONTHLY,
                                         end_type=ScheduleEndType.NO_END,
                                         business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
-                                        interval_expression="1", start_date_expression="account.start_date")
-    
-        savings_account.add_schedule_type(accrual_schedule)
-    
-        compounding_schedule = ScheduleType(name="compounding", label="Compounding Schedule", frequency=ScheduleFrequency.MONTHLY,
-                                            end_type=ScheduleEndType.NO_END,
-                                            business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
-                                            interval_expression="1",
-                                            start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
-    
-        savings_account.add_schedule_type(compounding_schedule)
-    
-        savings_account.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                  interest_accrued_tt,
-                                                  "account.current * config.interest.get_rate(account.current) / Decimal(365)")
-    
-        savings_account.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                  capitalized, "account.accrued")
-    
-        interest_rate = config.add_rate_type("interest", "Interest Rate")
-    
-        interest_rate.add_tier(Decimal(10000), Decimal(0.03))
-        interest_rate.add_tier(Decimal(100000), Decimal(0.035))
-        interest_rate.add_tier(Decimal(50000), Decimal(0.04))
-    
-        config.add_trigger_transaction(capitalized, withholding_txn, "transaction.amount * Decimal(0.2)")
-    
-        return config
+                                        interval_expression="1",
+                                        start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
+
+    acc.add_schedule_type(compounding_schedule)
+
+    acc.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                  interest_accrued_tt,
+                                  "account.current * accountType.interest.get_rate(account.current) / Decimal(365)")
+
+    acc.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                  capitalized_tt, "account.accrued")
+
+    interest_rate = acc.add_rate_type("interest", "Interest Rate")
+
+    interest_rate.add_tier(Decimal(10000), Decimal(0.03))
+    interest_rate.add_tier(Decimal(100000), Decimal(0.035))
+    interest_rate.add_tier(Decimal(50000), Decimal(0.04))
+
+    acc.add_trigger_transaction(capitalized_tt, withholding_tt, "transaction.amount * Decimal(0.2)")
+
+    return acc
+
 
 
 Given configuration, we can create an account:
 
 .. code:: python
 
-       config: Configuration = create_savings_account()
+ def test_valuation(self):
+        account_type = create_savings_account()
 
-        # account = create_account(config, "savingsAccount", date(2019, 1, 1))
-        account_type = config.get_account_type("savingsAccount")
         account = Account(start_date=date(2019, 1, 1), account_type_name=account_type.name,
-                          config_version= config.version, config=config)
+                          account_type=account_type)
 
-        valuation = AccountValuation(account, account_type, config, date(2020, 1, 1))
+        valuation = AccountValuation(account, account_type, date(2020, 1, 1))
 
-        deposit_transaction_type = config.get_transaction_type("deposit")
+        deposit_transaction_type = account_type.get_transaction_type("deposit")
 
         external_transactions = group_by_date([
             ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
-                                amount= Decimal(1000), value_date=date(2019, 1, 1))])
+                                amount=Decimal(1000), value_date=date(2019, 1, 1))])
 
         valuation.forecast(date(2020, 1, 1), external_transactions)
 
         self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
         self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
+        self.assertAlmostEqual(account.transactions[1].amount, Decimal('0.0821'), places=1)
```

### Comparing `transaction-accounts-0.0.4/accounts/metadata.py` & `transaction-accounts-0.0.5/accounts/metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -148,64 +148,33 @@
     name: str
     label: str
 
 
 class AccountType(BaseModel):
     name: str
     label: str
-    transaction_type_names: List[str] = []
-    schedule_types: List[ScheduleType] = []
-    property_types: List[PropertyType] = []
-    scheduled_transactions: List[ScheduledTransaction] = []
-    triggered_transactions: List[TriggeredTransaction] = []
-
-    def add_transaction_type(self, transaction_type: TransactionType):
-        self.transaction_type_names.append(transaction_type.name)
-
-    def add_schedule_type(self, schedule_type: ScheduleType):
-        self.schedule_types.append(schedule_type)
-
-    def add_scheduled_transaction(self, schedule_type: ScheduleType, timing: ScheduledTransactionTiming,
-                                  generated_transaction_type: TransactionType, amount_expression: str):
-        scheduled_transaction = ScheduledTransaction(schedule_name=schedule_type.name, timing=timing,
-                                                     generated_transaction_type=generated_transaction_type.name,
-                                                     amount_expression=amount_expression)
-        self.scheduled_transactions.append(scheduled_transaction)
-
-    def add_trigger_transaction(self, trigger_transaction_type: TransactionType,
-                                generated_transaction_type: TransactionType, amount_expression: str):
-        triggered_transaction = TriggeredTransaction(name=trigger_transaction_type.name,
-                                                     generated_transaction_type=generated_transaction_type.name,
-                                                     amount_expression=amount_expression)
-        self.triggered_transactions.append(triggered_transaction)
-
-
-class Configuration(BaseModel):
-    version: str
     transaction_types: List[TransactionType] = []
     position_types: List[PositionType] = []
-    account_types: List[AccountType] = []
     rate_types: Dict[str, RateType] = {}
     triggered_transactions: List[TriggeredTransaction] = []
+    schedule_types: List[ScheduleType] = []
+    property_types: List[PropertyType] = []
+    scheduled_transactions: List[ScheduledTransaction] = []
+    triggered_transactions: List[TriggeredTransaction] = []
 
     def add_transaction_type(self, name: str, label: str) -> TransactionType:
         transaction_type = TransactionType(name=name, label=label)
         self.transaction_types.append(transaction_type)
         return transaction_type
 
     def add_position_type(self, name: str, label: str) -> PositionType:
         position_type = PositionType(name=name, label=label)
         self.position_types.append(position_type)
         return position_type
 
-    def add_account_type(self, name: str, label: str) -> AccountType:
-        account_type = AccountType(name=name, label=label)
-        self.account_types.append(account_type)
-        return account_type
-
     def add_rate_type(self, name: str, label: str) -> RateType:
         rate_type = RateType(name=name, label=label)
         self.rate_types[name] = rate_type
         return rate_type
 
     def add_trigger_transaction(self, trigger_transaction_type: TransactionType,
                                 generated_transaction_type: TransactionType, amount_expression: str):
@@ -213,24 +182,32 @@
                                                    generated_transaction_type=generated_transaction_type.name,
                                                    amount_expression=amount_expression)
         self.triggered_transactions.append(trigger_transaction)
 
     def get_transaction_type(self, transaction_type_name: str) -> TransactionType:
         return next(tt for tt in self.transaction_types if tt.name == transaction_type_name)
 
-    def get_account_type(self, account_type_name: str):
-        return next(at for at in self.account_types if at.name == account_type_name)
-
     def get_rate_type(self, rate_type_name: str):
         return next(rt for rt in self.rate_types if rt.name == rate_type_name)
 
     def get_trigger_transaction(self, trigger_transaction_type_name: str) -> Optional[TriggeredTransaction]:
         return next((tt for tt in self.triggered_transactions if
                      tt.trigger_transaction_type_name == trigger_transaction_type_name), None)
 
-    def __getattr__(self, method_name: str):
-        # find rate type by method name
+    def add_schedule_type(self, schedule_type: ScheduleType):
+        self.schedule_types.append(schedule_type)
+
+    def add_scheduled_transaction(self, schedule_type: ScheduleType, timing: ScheduledTransactionTiming,
+                                  generated_transaction_type: TransactionType, amount_expression: str):
+        scheduled_transaction = ScheduledTransaction(schedule_name=schedule_type.name, timing=timing,
+                                                     generated_transaction_type=generated_transaction_type.name,
+                                                     amount_expression=amount_expression)
+        self.scheduled_transactions.append(scheduled_transaction)
 
+    def __getattr__(self, method_name):
         if method_name in self.rate_types:
             return self.rate_types[method_name]
         else:
             raise AttributeError(f'No such attribute: {method_name}')
+
+
+
```

### Comparing `transaction-accounts-0.0.4/accounts/runtime.py` & `transaction-accounts-0.0.5/accounts/runtime.py`

 * *Files 16% similar despite different names*

```diff
@@ -119,49 +119,45 @@
     amount: Decimal
     value_date: date
 
 
 class Account(BaseModel):
     start_date: date
     account_type_name: str
-    config_version: str
     positions: dict[str, Position] = {}
     schedules: dict[str, Schedule] = {}
     transactions: list[Transaction] = []
 
-    def __init__(self, *a, **kw):
-        super().__init__(*a, **kw)
+    def __init__(self, **kw):
+        super().__init__(**kw)
+        if "account_type" in kw:
+            account_type: AccountType = kw["account_type"]
+            self.__initialize_positions(account_type)
+            self.__initialize_schedules(account_type)
 
-        if "config" in kw:
-            config: Configuration = kw["config"]
-            account_type: AccountType = config.get_account_type(self.account_type_name)
-            self.__initialize_positions(account_type, config)
-            self.__initialize_schedules(account_type, config)
-
-    def __initialize_schedules(self, account_type: AccountType, config: Configuration):
+    def __initialize_schedules(self, account_type: AccountType):
         for schedule_type in account_type.schedule_types:
             schedule = Schedule(
-                start_date=self.evaluate(schedule_type.start_date_expression, {"config": config, "account": self}),
+                start_date=self.evaluate(schedule_type.start_date_expression, {"accountType": account_type, "account": self}),
                 end_type=schedule_type.end_type,
                 frequency=schedule_type.frequency,
-                interval=self.evaluate(schedule_type.interval_expression, {"config": config, "account": self}),
+                interval=self.evaluate(schedule_type.interval_expression, {"accountType": account_type, "account": self}),
                 adjustment=schedule_type.business_day_adjustment)
 
             if schedule_type.end_date_expression:
                 schedule.end_date = self.evaluate(schedule_type.end_date_expression,
-                                                  {"config": config, "account": self})
+                                                  {"accountType": account_type,  "account": self})
 
             if schedule_type.number_of_repeats_expression:
                 schedule.number_of_repeats = self.evaluate(schedule_type.number_of_repeats_expression)
 
             self.schedules[schedule_type.name] = schedule
 
-    def __initialize_positions(self, account_type, config):
-        for transaction_type_name in account_type.transaction_type_names:
-            transaction_type = config.get_transaction_type(transaction_type_name)
+    def __initialize_positions(self, account_type: AccountType):
+        for transaction_type in account_type.transaction_types:
             for rule in transaction_type.position_rules:
                 if rule.position_type_name not in self.positions:
                     self.positions[rule.position_type_name] = Position()
 
     def add_transaction(self, transaction: Transaction, transaction_type: TransactionType) -> Transaction:
         for rule in transaction_type.position_rules:
             position = self.positions[rule.position_type_name]
@@ -196,18 +192,17 @@
         else:
             grouped[external_transaction.value_date].append(external_transaction)
 
     return grouped
 
 
 class AccountValuation:
-    def __init__(self, account: Account, account_type: AccountType, configuration: Configuration, action_date: date):
+    def __init__(self, account: Account, account_type: AccountType, action_date: date):
         self.account = account
         self.account_type = account_type
-        self.configuration = configuration
         self.action_date = action_date
 
     def forecast(self, to_value_date: date, external_transactions):
         value_date = self.account.start_date
 
         self.start_of_day(value_date)
         self.process_external_transactions(value_date, external_transactions)
@@ -219,55 +214,53 @@
 
             self.start_of_day(value_date)
             self.process_external_transactions(value_date, external_transactions)
 
     def process_external_transactions(self, value_date: date, external_transactions):
         if value_date in external_transactions:
             for external_transaction in external_transactions[value_date]:
-                transaction_type = self.configuration.get_transaction_type(external_transaction.transaction_type_name)
+                transaction_type = self.account_type.get_transaction_type(external_transaction.transaction_type_name)
                 self.__create_transaction(transaction_type, value_date, external_transaction.amount, False)
 
     def start_of_day(self, value_date):
         for scheduled_transaction in self.account_type.scheduled_transactions:
             if scheduled_transaction.timing == ScheduledTransactionTiming.START_OF_DAY:
                 self.__create_transaction_if_due(value_date, scheduled_transaction)
 
     def __create_transaction_if_due(self, value_date: date, scheduled_transaction: ScheduledTransaction):
         schedule = self.account.schedules[scheduled_transaction.schedule_name]
 
         if schedule.is_due(value_date):
-            transaction_type = self.configuration.get_transaction_type(scheduled_transaction.generated_transaction_type)
+            transaction_type = self.account_type.get_transaction_type(scheduled_transaction.generated_transaction_type)
 
             self.__create_calculated_transaction(value_date, transaction_type, scheduled_transaction.amount_expression)
 
     def __create_calculated_transaction(self, value_date: date, transaction_type: TransactionType,
                                         amount_expression: str):
         try:
-            amount = self.account.evaluate(amount_expression, {"config": self.configuration, "account": self.account})
+            amount = self.account.evaluate(amount_expression, {"accountType": self.account_type, "account": self.account})
         except Exception as e:
 
             raise Exception(f'Error evaluating expression: {amount_expression} {e.args}') from e
         else:
             if amount != Decimal(0):
                 self.__create_transaction(transaction_type, value_date, amount, True)
 
     def __create_transaction(self, transaction_type: TransactionType, value_date: date,
                              amount: Decimal, system_generated: bool):
         transaction = Transaction(action_date= self.action_date, value_date=value_date, transaction_type=transaction_type.name,
                                   amount=amount, system_generated=system_generated)
         self.account.add_transaction(transaction, transaction_type)
 
-        triggered_transaction = self.configuration.get_trigger_transaction(transaction_type.name)
+        triggered_transaction = self.account_type.get_trigger_transaction(transaction_type.name)
 
         if triggered_transaction:
             trigger_amount = self.account.evaluate(triggered_transaction.amount_expression,
-                                                   {"transaction": transaction,
-                                                    "config": self.configuration,
+                                                   {"transaction": transaction, "accountType": self.account_type,
                                                     "account": self.account})
-            generated_transaction_type = self.configuration \
-                .get_transaction_type(triggered_transaction.generated_transaction_type)
+            generated_transaction_type = self.account_type.get_transaction_type(triggered_transaction.generated_transaction_type)
             self.__create_transaction(generated_transaction_type, value_date, trigger_amount, True)
 
     def end_of_day(self, value_date):
         for scheduled_transaction in self.account_type.scheduled_transactions:
             if scheduled_transaction.timing == ScheduledTransactionTiming.END_OF_DAY:
                 self.__create_transaction_if_due(value_date, scheduled_transaction)
```

### Comparing `transaction-accounts-0.0.4/setup.py` & `transaction-accounts-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='transaction-accounts',
-    version='0.0.4',
+    version='0.0.5',
     description='Create configuration for transactional accounts and implement account runtime',
     long_description='''
 Transaction Accounts
 ====================
 
 This library provides basic functionality for working with transaction
 accounts.
@@ -72,95 +72,92 @@
 variables: - account: Account - transaction: Transaction - config:
 Configuration
 
 Here is a code that will create this configuration:
 
 .. code:: python
 
-    def create_savings_account() -> Configuration:
-        config: Configuration = Configuration(version="v1")
-    
-        current = config.add_position_type("current", "current balance")
-        interest_accrued = config.add_position_type("accrued", "interest accrued")
-        withholding = config.add_position_type("withholding", "withholding tax")
-    
-        deposit = config.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
-    
-        interest_accrued_tt = config.add_transaction_type("interestAccrued", "Interest Accrued")
-        interest_accrued_tt.add_position_rule(TransactionOperation.CREDIT, interest_accrued)
-    
-        capitalized = config.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(
-            TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
-    
-        withholding_txn = config.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(
-            TransactionOperation.CREDIT, withholding)
-    
-        savings_account = config.add_account_type("savingsAccount", "Savings Account")
-    
-        savings_account.add_transaction_type(deposit)
-        savings_account.add_transaction_type(interest_accrued_tt)
-        savings_account.add_transaction_type(capitalized)
-        savings_account.add_transaction_type(withholding_txn)
-    
-        accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
+ def create_savings_account() -> AccountType:
+    acc = AccountType(name="savingsAccount", label="Savings Account")
+
+    current = acc.add_position_type("current", "current balance")
+    interest_accrued = acc.add_position_type("accrued", "interest accrued")
+    withholding = acc.add_position_type("withholding", "withholding tax")
+
+    acc.add_transaction_type("deposit", "Deposit")\
+        .add_position_rule(TransactionOperation.CREDIT, current)
+
+    interest_accrued_tt = acc.add_transaction_type("interestAccrued", "Interest Accrued") \
+        .add_position_rule(TransactionOperation.CREDIT, interest_accrued)
+
+    capitalized_tt = acc.add_transaction_type("capitalized", "Interest Capitalized") \
+        .add_position_rule(TransactionOperation.CREDIT, current) \
+        .add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+
+    withholding_tt = acc.add_transaction_type("withholdingTax", "Withholding Tax") \
+        .add_position_rule(TransactionOperation.CREDIT, withholding)
+
+    accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
+                                    end_type=ScheduleEndType.NO_END,
+                                    business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
+                                    interval_expression="1", start_date_expression="account.start_date")
+
+    acc.add_schedule_type(accrual_schedule)
+
+    compounding_schedule = ScheduleType(name="compounding", label="Compounding Schedule",
+                                        frequency=ScheduleFrequency.MONTHLY,
                                         end_type=ScheduleEndType.NO_END,
                                         business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
-                                        interval_expression="1", start_date_expression="account.start_date")
-    
-        savings_account.add_schedule_type(accrual_schedule)
-    
-        compounding_schedule = ScheduleType(name="compounding", label="Compounding Schedule", frequency=ScheduleFrequency.MONTHLY,
-                                            end_type=ScheduleEndType.NO_END,
-                                            business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
-                                            interval_expression="1",
-                                            start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
-    
-        savings_account.add_schedule_type(compounding_schedule)
-    
-        savings_account.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                  interest_accrued_tt,
-                                                  "account.current * config.interest.get_rate(account.current) / Decimal(365)")
-    
-        savings_account.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                  capitalized, "account.accrued")
-    
-        interest_rate = config.add_rate_type("interest", "Interest Rate")
-    
-        interest_rate.add_tier(Decimal(10000), Decimal(0.03))
-        interest_rate.add_tier(Decimal(100000), Decimal(0.035))
-        interest_rate.add_tier(Decimal(50000), Decimal(0.04))
-    
-        config.add_trigger_transaction(capitalized, withholding_txn, "transaction.amount * Decimal(0.2)")
-    
-        return config
+                                        interval_expression="1",
+                                        start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
+
+    acc.add_schedule_type(compounding_schedule)
+
+    acc.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                  interest_accrued_tt,
+                                  "account.current * accountType.interest.get_rate(account.current) / Decimal(365)")
+
+    acc.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                  capitalized_tt, "account.accrued")
+
+    interest_rate = acc.add_rate_type("interest", "Interest Rate")
+
+    interest_rate.add_tier(Decimal(10000), Decimal(0.03))
+    interest_rate.add_tier(Decimal(100000), Decimal(0.035))
+    interest_rate.add_tier(Decimal(50000), Decimal(0.04))
+
+    acc.add_trigger_transaction(capitalized_tt, withholding_tt, "transaction.amount * Decimal(0.2)")
+
+    return acc
+
 
 
 Given configuration, we can create an account:
 
 .. code:: python
 
-       config: Configuration = create_savings_account()
+ def test_valuation(self):
+        account_type = create_savings_account()
 
-        # account = create_account(config, "savingsAccount", date(2019, 1, 1))
-        account_type = config.get_account_type("savingsAccount")
         account = Account(start_date=date(2019, 1, 1), account_type_name=account_type.name,
-                          config_version= config.version, config=config)
+                          account_type=account_type)
 
-        valuation = AccountValuation(account, account_type, config, date(2020, 1, 1))
+        valuation = AccountValuation(account, account_type, date(2020, 1, 1))
 
-        deposit_transaction_type = config.get_transaction_type("deposit")
+        deposit_transaction_type = account_type.get_transaction_type("deposit")
 
         external_transactions = group_by_date([
             ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
-                                amount= Decimal(1000), value_date=date(2019, 1, 1))])
+                                amount=Decimal(1000), value_date=date(2019, 1, 1))])
 
         valuation.forecast(date(2020, 1, 1), external_transactions)
 
         self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
         self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
+        self.assertAlmostEqual(account.transactions[1].amount, Decimal('0.0821'), places=1)
     
     ''',
     author='Igor Music',
     author_email='igormusich@gmail.com',
     packages=find_packages(),
     license='MIT',
     url='https://github.com/igormusic/transaction-accounts',
@@ -172,10 +169,9 @@
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',  # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
-
     ],
 )
```

### Comparing `transaction-accounts-0.0.4/tests/test_rate_type.py` & `transaction-accounts-0.0.5/tests/test_rate_type.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.0.4/tests/test_schedule.py` & `transaction-accounts-0.0.5/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.0.4/transaction_accounts.egg-info/PKG-INFO` & `transaction-accounts-0.0.5/transaction_accounts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.4.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
@@ -83,90 +83,82 @@
 variables: - account: Account - transaction: Transaction - config:
 Configuration
 
 Here is a code that will create this configuration:
 
 .. code:: python
 
-    def create_savings_account() -> Configuration:
-        config: Configuration = Configuration(version="v1")
-    
-        current = config.add_position_type("current", "current balance")
-        interest_accrued = config.add_position_type("accrued", "interest accrued")
-        withholding = config.add_position_type("withholding", "withholding tax")
-    
-        deposit = config.add_transaction_type("deposit", "Deposit").add_position_rule(TransactionOperation.CREDIT, current)
-    
-        interest_accrued_tt = config.add_transaction_type("interestAccrued", "Interest Accrued")
-        interest_accrued_tt.add_position_rule(TransactionOperation.CREDIT, interest_accrued)
-    
-        capitalized = config.add_transaction_type("capitalized", "Interest Capitalized").add_position_rule(
-            TransactionOperation.CREDIT, current).add_position_rule(TransactionOperation.DEBIT, interest_accrued)
-    
-        withholding_txn = config.add_transaction_type("withholdingTax", "Withholding Tax").add_position_rule(
-            TransactionOperation.CREDIT, withholding)
-    
-        savings_account = config.add_account_type("savingsAccount", "Savings Account")
-    
-        savings_account.add_transaction_type(deposit)
-        savings_account.add_transaction_type(interest_accrued_tt)
-        savings_account.add_transaction_type(capitalized)
-        savings_account.add_transaction_type(withholding_txn)
-    
-        accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
+ def create_savings_account() -> AccountType:
+    acc = AccountType(name="savingsAccount", label="Savings Account")
+
+    current = acc.add_position_type("current", "current balance")
+    interest_accrued = acc.add_position_type("accrued", "interest accrued")
+    withholding = acc.add_position_type("withholding", "withholding tax")
+
+    acc.add_transaction_type("deposit", "Deposit")        .add_position_rule(TransactionOperation.CREDIT, current)
+
+    interest_accrued_tt = acc.add_transaction_type("interestAccrued", "Interest Accrued")         .add_position_rule(TransactionOperation.CREDIT, interest_accrued)
+
+    capitalized_tt = acc.add_transaction_type("capitalized", "Interest Capitalized")         .add_position_rule(TransactionOperation.CREDIT, current)         .add_position_rule(TransactionOperation.DEBIT, interest_accrued)
+
+    withholding_tt = acc.add_transaction_type("withholdingTax", "Withholding Tax")         .add_position_rule(TransactionOperation.CREDIT, withholding)
+
+    accrual_schedule = ScheduleType(name="accrual", label="Accrual Schedule", frequency=ScheduleFrequency.DAILY,
+                                    end_type=ScheduleEndType.NO_END,
+                                    business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
+                                    interval_expression="1", start_date_expression="account.start_date")
+
+    acc.add_schedule_type(accrual_schedule)
+
+    compounding_schedule = ScheduleType(name="compounding", label="Compounding Schedule",
+                                        frequency=ScheduleFrequency.MONTHLY,
                                         end_type=ScheduleEndType.NO_END,
                                         business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
-                                        interval_expression="1", start_date_expression="account.start_date")
-    
-        savings_account.add_schedule_type(accrual_schedule)
-    
-        compounding_schedule = ScheduleType(name="compounding", label="Compounding Schedule", frequency=ScheduleFrequency.MONTHLY,
-                                            end_type=ScheduleEndType.NO_END,
-                                            business_day_adjustment=BusinessDayAdjustment.NO_ADJUSTMENT,
-                                            interval_expression="1",
-                                            start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
-    
-        savings_account.add_schedule_type(compounding_schedule)
-    
-        savings_account.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                  interest_accrued_tt,
-                                                  "account.current * config.interest.get_rate(account.current) / Decimal(365)")
-    
-        savings_account.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
-                                                  capitalized, "account.accrued")
-    
-        interest_rate = config.add_rate_type("interest", "Interest Rate")
-    
-        interest_rate.add_tier(Decimal(10000), Decimal(0.03))
-        interest_rate.add_tier(Decimal(100000), Decimal(0.035))
-        interest_rate.add_tier(Decimal(50000), Decimal(0.04))
-    
-        config.add_trigger_transaction(capitalized, withholding_txn, "transaction.amount * Decimal(0.2)")
-    
-        return config
+                                        interval_expression="1",
+                                        start_date_expression="account.start_date + relativedelta(month=+1) + relativedelta(days=-1)")
+
+    acc.add_schedule_type(compounding_schedule)
+
+    acc.add_scheduled_transaction(accrual_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                  interest_accrued_tt,
+                                  "account.current * accountType.interest.get_rate(account.current) / Decimal(365)")
+
+    acc.add_scheduled_transaction(compounding_schedule, ScheduledTransactionTiming.END_OF_DAY,
+                                  capitalized_tt, "account.accrued")
+
+    interest_rate = acc.add_rate_type("interest", "Interest Rate")
+
+    interest_rate.add_tier(Decimal(10000), Decimal(0.03))
+    interest_rate.add_tier(Decimal(100000), Decimal(0.035))
+    interest_rate.add_tier(Decimal(50000), Decimal(0.04))
+
+    acc.add_trigger_transaction(capitalized_tt, withholding_tt, "transaction.amount * Decimal(0.2)")
+
+    return acc
+
 
 
 Given configuration, we can create an account:
 
 .. code:: python
 
-       config: Configuration = create_savings_account()
+ def test_valuation(self):
+        account_type = create_savings_account()
 
-        # account = create_account(config, "savingsAccount", date(2019, 1, 1))
-        account_type = config.get_account_type("savingsAccount")
         account = Account(start_date=date(2019, 1, 1), account_type_name=account_type.name,
-                          config_version= config.version, config=config)
+                          account_type=account_type)
 
-        valuation = AccountValuation(account, account_type, config, date(2020, 1, 1))
+        valuation = AccountValuation(account, account_type, date(2020, 1, 1))
 
-        deposit_transaction_type = config.get_transaction_type("deposit")
+        deposit_transaction_type = account_type.get_transaction_type("deposit")
 
         external_transactions = group_by_date([
             ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
-                                amount= Decimal(1000), value_date=date(2019, 1, 1))])
+                                amount=Decimal(1000), value_date=date(2019, 1, 1))])
 
         valuation.forecast(date(2020, 1, 1), external_transactions)
 
         self.assertAlmostEqual(account.positions['current'].amount, Decimal(1030.41), places=1)
         self.assertAlmostEqual(account.positions['withholding'].amount, Decimal(30.41) * Decimal(0.2), places=1)
+        self.assertAlmostEqual(account.transactions[1].amount, Decimal('0.0821'), places=1)
```

