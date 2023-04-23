# Comparing `tmp/xray_bot-0.1.3-py3-none-any.whl.zip` & `tmp/xray_bot-0.1.4rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11044 bytes, number of entries: 12
--rw-r--r--  2.0 unx      164 b- defN 23-Mar-07 06:51 xraybot/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-17 06:54 xraybot/__version__.py
--rw-r--r--  2.0 unx     4225 b- defN 23-Mar-08 02:07 xraybot/_context.py
--rw-r--r--  2.0 unx      505 b- defN 23-Mar-03 03:43 xraybot/_data.py
--rw-r--r--  2.0 unx      192 b- defN 23-Mar-03 03:43 xraybot/_utils.py
--rw-r--r--  2.0 unx    17733 b- defN 23-Apr-17 03:52 xraybot/_worker.py
--rw-r--r--  2.0 unx    14945 b- defN 23-Apr-17 06:10 xraybot/_xray_bot.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Apr-17 06:54 xray_bot-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      483 b- defN 23-Apr-17 06:54 xray_bot-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-17 06:54 xray_bot-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-17 06:54 xray_bot-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      916 b- defN 23-Apr-17 06:54 xray_bot-0.1.3.dist-info/RECORD
-12 files, 40350 bytes uncompressed, 9520 bytes compressed:  76.4%
+Zip file size: 12334 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      203 b- defN 23-Apr-23 01:52 xraybot/__init__.py
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-23 10:10 xraybot/__version__.py
+-rw-r--r--  2.0 unx     4358 b- defN 23-Apr-21 11:02 xraybot/_context.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-21 10:09 xraybot/_data.py
+-rw-r--r--  2.0 unx      192 b- defN 23-Apr-21 10:34 xraybot/_utils.py
+-rw-r--r--  2.0 unx    19127 b- defN 23-Apr-23 03:08 xraybot/_worker.py
+-rw-r--r--  2.0 unx    20157 b- defN 23-Apr-23 02:52 xraybot/_xray_bot.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-23 10:11 xray_bot-0.1.4rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      486 b- defN 23-Apr-23 10:11 xray_bot-0.1.4rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-23 10:11 xray_bot-0.1.4rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-23 10:11 xray_bot-0.1.4rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      931 b- defN 23-Apr-23 10:11 xray_bot-0.1.4rc1.dist-info/RECORD
+12 files, 47217 bytes uncompressed, 10780 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: xraybot/_worker.py
 Comment: 
 
 Filename: xraybot/_xray_bot.py
 Comment: 
 
-Filename: xray_bot-0.1.3.dist-info/LICENSE
+Filename: xray_bot-0.1.4rc1.dist-info/LICENSE
 Comment: 
 
-Filename: xray_bot-0.1.3.dist-info/METADATA
+Filename: xray_bot-0.1.4rc1.dist-info/METADATA
 Comment: 
 
-Filename: xray_bot-0.1.3.dist-info/WHEEL
+Filename: xray_bot-0.1.4rc1.dist-info/WHEEL
 Comment: 
 
-Filename: xray_bot-0.1.3.dist-info/top_level.txt
+Filename: xray_bot-0.1.4rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: xray_bot-0.1.3.dist-info/RECORD
+Filename: xray_bot-0.1.4rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xraybot/__init__.py

```diff
@@ -1,4 +1,5 @@
 from .__version__ import __version__
 from ._xray_bot import XrayBot
 from ._worker import WorkerType
-from ._data import TestEntity, TestResultEntity, XrayResultType
+from ._data import TestEntity, TestResultEntity, XrayResultType, WorkResult
+from ._utils import logger
```

## xraybot/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.3"
+__version__ = "0.1.4rc1"
```

## xraybot/_context.py

```diff
@@ -100,18 +100,27 @@
         if self._labels:
             fields["labels"] = self._labels
         return fields
 
 
 class XrayBotContext:
     def __init__(
-        self, jira_url: str, jira_username: str, jira_pwd: str, project_key: str
+        self,
+        jira_url: str,
+        jira_username: str,
+        jira_pwd: str,
+        project_key: str,
+        timeout: int,
     ):
-        self._jira: Jira = Jira(url=jira_url, username=jira_username, password=jira_pwd)
-        self._xray: Xray = Xray(url=jira_url, username=jira_username, password=jira_pwd)
+        self._jira: Jira = Jira(
+            url=jira_url, username=jira_username, password=jira_pwd, timeout=timeout
+        )
+        self._xray: Xray = Xray(
+            url=jira_url, username=jira_username, password=jira_pwd, timeout=timeout
+        )
         self._project_key: str = project_key
         self._config = _XrayBotConfig(self._jira)
 
     @property
     def jira_username(self) -> Jira:
         return self._jira.username
```

## xraybot/_data.py

```diff
@@ -1,10 +1,16 @@
 from dataclasses import dataclass
 from enum import Enum
-from typing import Optional
+from typing import Optional, Any
+
+
+@dataclass
+class WorkResult:
+    success: bool
+    data: Any
 
 
 @dataclass
 class TestEntity:
     # store in test custom field "Generic Test Definition"
     # using as the unique identified for one certain test
     unique_identifier: str
```

## xraybot/_worker.py

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 from enum import Enum
 from typing import List
 from concurrent.futures.process import ProcessPoolExecutor
-from ._data import TestEntity
+from ._data import TestEntity, WorkResult
 from ._utils import logger
 from ._context import XrayBotContext
 
 
 class _XrayAPIWrapper:
     def __init__(self, context: XrayBotContext):
         self.context = context
@@ -134,15 +134,15 @@
 
     def finalize_test_from_any_status(self, test_entity: TestEntity):
         logger.info(f"Start finalizing marked test: {test_entity.key}")
         status = self.context.jira.get_issue_status(test_entity.key)
         if status == "Finalized":
             return
 
-        for status in ["Ready for Review", "In Review", "Finalized"]:
+        for status in ["In-Draft", "Ready for Review", "In Review", "Finalized"]:
             try:
                 self.context.jira.set_issue_status(test_entity.key, status)
             except Exception as e:
                 # ignore errors from any status
                 logger.debug(f"Update test status with error: {e}")
 
         status = self.context.jira.get_issue_status(test_entity.key)
@@ -306,14 +306,33 @@
         self.api_wrapper.finalize_test(test_entity)
         self.api_wrapper.link_test(test_entity)
         self.api_wrapper.add_test_into_folder(
             test_entity, self.api_wrapper.automation_folder_id
         )
 
 
+class _DraftTestCreateWorker(_XrayBotWorker):
+    def run(self, test_entity: TestEntity):
+        logger.info(f"Start creating test draft: {test_entity.summary}")
+
+        fields = {
+            "issuetype": {"name": "Test"},
+            "project": {"key": self.context.project_key},
+            "description": test_entity.description,
+            "summary": f"[🤖Automation Draft] {test_entity.summary}",
+            "assignee": {"name": self.context.jira.username},
+            self.context.config.cf_id_test_definition: test_entity.unique_identifier,
+            **self.context.config.get_tests_cf_label_fields(),
+        }
+
+        test_entity.key = self.context.jira.create_issue(fields)["key"]
+        logger.info(f"Created xray test draft: {test_entity.key}")
+        return test_entity
+
+
 class _NonMarkedTestUpdateWorker(_XrayBotWorker):
     def run(self, test_entity: TestEntity):
         logger.info(f"Start updating test: {test_entity.key}")
         assert test_entity.key is not None, "Jira test key cannot be None"
         fields = {
             "summary": test_entity.summary,
             "description": test_entity.description,
@@ -400,50 +419,62 @@
         if status != "Finalized":
             logger.info(
                 f"Start deleting obsolete test {test_key} from test plan {test_plan_key}"
             )
             self.context.xray.delete_test_from_test_plan(test_plan_key, test_key)
 
 
+class _JiraStatusBulkCheckWorker(_XrayBotWorker):
+    def run(self, jira_keys: List[str]):
+        logger.info(f"Bulk checking jira status: {jira_keys}...")
+        results = self.context.jira.bulk_issue(jira_keys, fields="status")
+        results = [
+            (issue["key"], issue["fields"]["status"]["name"])
+            for issue in results[0]["issues"]
+        ]
+        assert len(results) == len(
+            jira_keys
+        ), f"Not enough jira status found: {results}"
+        return results
+
+
 class WorkerType(Enum):
     NonMarkedTestObsolete = _NonMarkedTestObsoleteWorker
     NonMarkedTestCreate = _NonMarkedTestCreateWorker
     NonMarkedTestUpdate = _NonMarkedTestUpdateWorker
     ExternalMarkedTestUpdate = _ExternalMarkedTestUpdateWorker
     InternalMarkedTestUpdate = _InternalMarkedTestUpdateWorker
     AddTestsToPlan = _AddTestsToPlanWorker
     AddTestsToExecution = _AddTestsToExecutionWorker
     UpdateTestResults = _UpdateTestResultsWorker
     CleanTestExecution = _CleanTestExecutionWorker
     CleanTestPlan = _CleanTestPlanWorker
+    JiraStatusBulkCheck = _JiraStatusBulkCheckWorker
+    DraftTestCreate = _DraftTestCreateWorker
 
 
 class XrayBotWorkerMgr:
     def __init__(self, context: XrayBotContext):
         self.context = context
         self.api_wrapper = _XrayAPIWrapper(self.context)
 
     @staticmethod
-    def _worker_wrapper(worker_func, *iterables):
+    def _worker_wrapper(worker_func, *iterables) -> WorkResult:
         try:
-            worker_func(*iterables)
-            return None
+            ret = worker_func(*iterables)
+            return WorkResult(success=True, data=ret)
         except Exception as e:
             logger.info(
                 f"Worker [{worker_func.__qualname__.split('.')[0].lstrip('_')}] raised error: {e}"
             )
-            converted = []
-            for i in iterables:
-                if isinstance(i, TestEntity):
-                    converted.append(i.__str__())
-                else:
-                    converted.append(i)
-            return f"❌{e} -> 🐛{' | '.join(converted)}"
+            converted = [str(_) for _ in iterables]
+            err_msg = f"❌{e} -> 🐛{' | '.join(converted)}"
+            return WorkResult(success=False, data=err_msg)
 
-    def start_worker(self, worker_type: WorkerType, *iterables):
+    def start_worker(self, worker_type: WorkerType, *iterables) -> List[WorkResult]:
         worker: _XrayBotWorker = worker_type.value(self.api_wrapper)
         with ProcessPoolExecutor(self.context.config.worker_num) as executor:
             results = executor.map(
                 self._worker_wrapper,
                 [worker.run for _ in range(len(iterables[0]))],
                 *iterables,
             )
```

## xraybot/_xray_bot.py

```diff
@@ -1,7 +1,8 @@
+import copy
 from typing import List, Tuple, Union
 from ._context import XrayBotContext
 from ._data import TestEntity, TestResultEntity
 from ._utils import logger
 from ._worker import WorkerType, XrayBotWorkerMgr
 
 
@@ -9,30 +10,36 @@
 _CF_TEST_TYPE = "Test Type"
 _CF_TEST_TYPE_VAL_GENERIC = "Generic"
 _CF_TEST_TYPE_VAL_MANUAL = "Manual"
 _CF_TEST_TYPE_VAL_CUCUMBER = "Cucumber"
 
 
 class XrayBot:
-
+    _JIRA_API_TIMEOUT = 75
     _QUERY_PAGE_LIMIT = 100
     _MULTI_PROCESS_WORKER_NUM = 30
     _AUTOMATION_TESTS_FOLDER_NAME = "Automation Test"
     _AUTOMATION_OBSOLETE_TESTS_FOLDER_NAME = "Obsolete"
 
     def __init__(
         self, jira_url: str, jira_username: str, jira_pwd: str, project_key: str
     ):
         """
         :param jira_url: str
         :param jira_username: str
         :param jira_pwd: str
         :param project_key: str, jira project key, e.g: "TEST"
         """
-        self.context = XrayBotContext(jira_url, jira_username, jira_pwd, project_key)
+        self.context = XrayBotContext(
+            jira_url,
+            jira_username,
+            jira_pwd,
+            project_key,
+            timeout=self._JIRA_API_TIMEOUT,
+        )
         self.config = self.context.config
         self.config.configure_query_page_limit(self._QUERY_PAGE_LIMIT)
         self.config.configure_worker_num(self._MULTI_PROCESS_WORKER_NUM)
         self.config.configure_automation_folder_name(self._AUTOMATION_TESTS_FOLDER_NAME)
         self.config.configure_obsolete_automation_folder_name(
             self._AUTOMATION_OBSOLETE_TESTS_FOLDER_NAME
         )
@@ -146,16 +153,61 @@
                 non_marked_local_tests.append(local_test)
         return (
             non_marked_local_tests,
             internal_marked_local_tests,
             external_marked_local_tests,
         )
 
-    def sync_tests(self, local_tests: List[TestEntity]) -> List[str]:
-        errors = []
+    def create_tests_draft(self, local_tests: List[TestEntity]) -> List[TestEntity]:
+        """
+        Input: local tests including no existing jira key
+        Output: local tests with draft tests created and key has been appended to test entity
+        """
+        local_tests_with_keys = copy.deepcopy(local_tests)
+        # make sure all local test keys will be considered as upper case
+        for local_test in local_tests_with_keys:
+            if local_test.key is not None:
+                local_test.key = local_test.key.upper()
+
+        self._check_duplicated_uniqueness(
+            local_tests_with_keys,
+            "Duplicated key/unique_identifier found in local tests",
+        )
+        xray_tests = self.get_xray_tests()
+
+        def get_test_key_by_unique_identifier(_local_test: TestEntity):
+            for xray_test in xray_tests:
+                if xray_test.unique_identifier == local_test.unique_identifier:
+                    return xray_test.key
+            return None
+
+        to_be_created = []
+        to_be_remained = []
+        for local_test in local_tests_with_keys:
+            if local_test.key is None:
+                # tests have no key but already synced by unique identifier
+                existing_key = get_test_key_by_unique_identifier(local_test)
+                if existing_key is not None:
+                    local_test.key = existing_key
+                else:
+                    to_be_created.append(local_test)
+                    continue
+            to_be_remained.append(local_test)
+
+        worker_results = self.worker_mgr.start_worker(
+            WorkerType.DraftTestCreate, to_be_created
+        )
+        errors = [result.data for result in worker_results if not result.success]
+        err_msg = "\n".join(errors)
+        assert len(errors) == 0, f"Create draft test failed:\n {err_msg}"
+        results = to_be_remained + [_.data for _ in worker_results]
+        return results
+
+    def sync_tests(self, local_tests: List[TestEntity]):
+        worker_results = []
         # make sure all local test keys will be considered as upper case
         for local_test in local_tests:
             if local_test.key is not None:
                 local_test.key = local_test.key.upper()
 
         self._check_duplicated_uniqueness(
             local_tests, "Duplicated key/unique_identifier found in local_tests"
@@ -165,30 +217,30 @@
         (
             non_marked_local_tests,
             internal_marked_local_tests,
             external_marked_local_tests,
         ) = self._categorize_local_tests(xray_tests, local_tests)
         if external_marked_local_tests:
             # external marked test -> strategy: update and move to automation folder
-            errors.extend(
+            worker_results.extend(
                 self.worker_mgr.start_worker(
                     WorkerType.ExternalMarkedTestUpdate, external_marked_local_tests
                 )
             )
         if internal_marked_local_tests:
             # internal marked test -> strategy: update all fields including unique identifier
             filtered_xray_tests = [
                 xray_test
                 for xray_test in xray_tests
                 if xray_test.key in [_.key for _ in internal_marked_local_tests]
             ]
             to_be_updated = self._get_internal_marked_tests_diff(
                 filtered_xray_tests, internal_marked_local_tests
             )
-            errors.extend(
+            worker_results.extend(
                 self.worker_mgr.start_worker(
                     WorkerType.InternalMarkedTestUpdate, to_be_updated
                 )
             )
 
         # non marked test -> strategy: unique identifier sync
         # exclude internal marked local tests in xray tests
@@ -199,26 +251,31 @@
             if xray_test.key not in [_.key for _ in internal_marked_local_tests]
         ]
         (
             to_be_deleted,
             to_be_appended,
             to_be_updated,
         ) = self._get_non_marked_tests_diff(filtered_xray_tests, non_marked_local_tests)
-        errors.extend(
+        worker_results.extend(
             self.worker_mgr.start_worker(
                 WorkerType.NonMarkedTestObsolete, to_be_deleted
             )
         )
-        errors.extend(
+        worker_results.extend(
             self.worker_mgr.start_worker(WorkerType.NonMarkedTestCreate, to_be_appended)
         )
-        errors.extend(
+        worker_results.extend(
             self.worker_mgr.start_worker(WorkerType.NonMarkedTestUpdate, to_be_updated)
         )
-        return errors
+        errors = [_.data for _ in worker_results if not _.success]
+        if len(errors) > 0:
+            err_msg = ""
+            for idx, err in enumerate(errors):
+                err_msg = f"{err_msg}\n({idx + 1}) {err}"
+            raise AssertionError(f"Sync failed with the following errors:\n{err_msg}.")
 
     @staticmethod
     def _get_internal_marked_tests_diff(
         filtered_xray_tests: List[TestEntity],
         internal_marked_local_tests: List[TestEntity],
     ):
         to_be_updated = list()
@@ -324,15 +381,15 @@
         # delete obsolete tests from test plan
         self.worker_mgr.start_worker(
             WorkerType.CleanTestPlan,
             [test_plan_key for _ in range(len(test_plan_tests))],
             test_plan_tests,
         )
 
-    def upload_automation_results(
+    def upload_test_results(
         self,
         test_plan_name: str,
         test_execution_name: str,
         test_results: List[TestResultEntity],
         clean_test_plan_and_execution: bool = False,
     ):
         test_plan_key = self.worker_mgr.api_wrapper.create_test_plan(test_plan_name)
@@ -366,7 +423,79 @@
         # update test execution result
         self.worker_mgr.start_worker(
             WorkerType.UpdateTestResults,
             [result.key for result in test_results],
             [result.result.value for result in test_results],
             [test_execution_key for _ in range(len(test_results))],
         )
+
+    def upload_test_results_by_execution_key(
+        self,
+        test_results: List[TestResultEntity],
+        test_execution_key: str,
+    ):
+        # add tests to test execution based on local tests execution
+        self.worker_mgr.start_worker(
+            WorkerType.AddTestsToExecution,
+            [test_execution_key for _ in range(len(test_results))],
+            [_.key for _ in test_results],
+        )
+
+        # update test execution result
+        self.worker_mgr.start_worker(
+            WorkerType.UpdateTestResults,
+            [result.key for result in test_results],
+            [result.result.value for result in test_results],
+            [test_execution_key for _ in range(len(test_results))],
+        )
+
+    def sync_check(self, local_tests: List[TestEntity]):
+        """
+        1. make sure all local tests have been marked with keys
+        2. make sure all the uniqueness of local tests keys and unique identifiers
+        2. make sure all test keys are valid and not obsolete
+        3. make sure requirement keys are valid
+        """
+        test_keys = [_.key for _ in local_tests]
+        req_keys = [_.req_key for _ in local_tests]
+        assert (
+            None not in test_keys
+        ), "Some of the tests are not are not marked with test key, run sync prepare firstly."
+
+        self._check_duplicated_uniqueness(
+            local_tests, "Duplicated key/unique_identifier found in local tests"
+        )
+
+        def chunks(xs, n=20):
+            n = max(1, n)
+            return list(xs[i : i + n] for i in range(0, len(xs), n))
+
+        results = self.worker_mgr.start_worker(
+            WorkerType.JiraStatusBulkCheck, chunks(test_keys)
+        )
+        errors = []
+        test_status_results = []
+        for result in results:
+            if not result.success:
+                errors.append(f"Get test status failed: {result}")
+            else:
+                test_status_results.extend(result.data)
+        for test_key, status in test_status_results:
+            if status == "Obsolete":
+                errors.append(f"Test status is obsolete: {test_key}")
+
+        merged_req_keys = []
+        for req_key in req_keys:
+            if req_key:
+                merged_req_keys.extend(req_key.split(","))
+        merged_req_keys = list(set(merged_req_keys))
+        results = self.worker_mgr.start_worker(
+            WorkerType.JiraStatusBulkCheck, chunks(merged_req_keys)
+        )
+        for result in results:
+            if not result.success:
+                errors.append(f"Get requirement status failed: {result}")
+        if errors:
+            err_msg = ""
+            for idx, err in enumerate(errors):
+                err_msg = f"{err_msg}\n({idx + 1}) {err}"
+            raise AssertionError(f"Found following errors:{err_msg}")
```

## Comparing `xray_bot-0.1.3.dist-info/LICENSE` & `xray_bot-0.1.4rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xray_bot-0.1.3.dist-info/RECORD` & `xray_bot-0.1.4rc1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xraybot/__init__.py,sha256=Jv8SYQOZLM9nxZZczIc52DaNbDK8-XV5qR4WS4NIUl0,164
-xraybot/__version__.py,sha256=XEqb2aiIn8fzGE68Mph4ck1FtQqsR_am0wRWvrYPffQ,22
-xraybot/_context.py,sha256=AaKSlGLXu8ZKfM9zE4KB74XlgJvNiatkAsXFwIU3DQg,4225
-xraybot/_data.py,sha256=KKrdEdyOEyvK-EMN7cPJFI59Z-Mxwn6-CUO5uP5zh1w,505
+xraybot/__init__.py,sha256=9vptE2bh-sEH1jh9NFrm70D5vYw9-boQi9XgNA8_cn4,203
+xraybot/__version__.py,sha256=GIpwzbbPGQ9L-Oth25lm6mP4T9eA5Rwe9Ik85ZYTcz4,25
+xraybot/_context.py,sha256=9U4UnphDAvNTvi-WjjAhJ2IYOlmY3PlkLyoqIXxr24o,4358
+xraybot/_data.py,sha256=E4dsHZxyxioIqpc7I3c8TmNU8Kkj6JKZ6dKzO4Mrjb0,573
 xraybot/_utils.py,sha256=s7UwsTSNkSpDu73B-CeKaOjEXU8oQwDrF75FEhZAj_I,192
-xraybot/_worker.py,sha256=xda6s0p1mWtgen2WROcAZuBmyGxD6hkR-kgZfnIlFH0,17733
-xraybot/_xray_bot.py,sha256=h8eVynlEimemZxAxekFrRUgGR2RdmMSTkP6ysfAo9c8,14945
-xray_bot-0.1.3.dist-info/LICENSE,sha256=2V4UacA-K7TqPsdWQUP2it4zb9rJmDW5rW27r6Fho0U,1065
-xray_bot-0.1.3.dist-info/METADATA,sha256=SzeHqsNsJf5IN-VdM-HkreiuTT5q__Ern3VTwizhKLE,483
-xray_bot-0.1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-xray_bot-0.1.3.dist-info/top_level.txt,sha256=xQlj4RDuEOf9bM5ryJNYButwxv-W_pXRvRl46gky_7Q,8
-xray_bot-0.1.3.dist-info/RECORD,,
+xraybot/_worker.py,sha256=_gpmO4O98eNqDFQcXs-ggjjdOkNTXLDzlYNBkUdYHPs,19127
+xraybot/_xray_bot.py,sha256=9EAGIFDShB0Idt4CBwVDZCU0-AHzHAJPdZwJaY0pM4c,20157
+xray_bot-0.1.4rc1.dist-info/LICENSE,sha256=2V4UacA-K7TqPsdWQUP2it4zb9rJmDW5rW27r6Fho0U,1065
+xray_bot-0.1.4rc1.dist-info/METADATA,sha256=Ku_uoW8J_lne6jEzfoOGLXYjK-4k5vh9XQKhLQ1l18U,486
+xray_bot-0.1.4rc1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+xray_bot-0.1.4rc1.dist-info/top_level.txt,sha256=xQlj4RDuEOf9bM5ryJNYButwxv-W_pXRvRl46gky_7Q,8
+xray_bot-0.1.4rc1.dist-info/RECORD,,
```

