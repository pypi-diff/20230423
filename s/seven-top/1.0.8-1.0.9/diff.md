# Comparing `tmp/seven_top-1.0.8.tar.gz` & `tmp/seven_top-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\seven_top-1.0.8.tar", last modified: Tue Aug 11 05:43:54 2020, max compression
+gzip compressed data, was "dist\seven_top-1.0.9.tar", last modified: Mon Sep  7 11:02:59 2020, max compression
```

## Comparing `seven_top-1.0.8.tar` & `seven_top-1.0.9.tar`

### file list

```diff
@@ -1,110 +1,112 @@
-drwxrwxrwx   0        0        0        0 2020-08-11 05:43:54.922015 seven_top-1.0.8/
--rw-rw-rw-   0        0        0      993 2020-08-11 05:43:54.921017 seven_top-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      149 2020-08-11 05:43:13.000000 seven_top-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2020-08-11 05:43:54.923012 seven_top-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1274 2020-08-11 05:43:19.000000 seven_top-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2020-08-11 05:43:54.704089 seven_top-1.0.8/seven_top/
--rw-rw-rw-   0        0        0      139 2020-07-08 04:42:06.000000 seven_top-1.0.8/seven_top/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-11 05:43:54.716057 seven_top-1.0.8/seven_top/top/
--rw-rw-rw-   0        0        0      530 2020-08-11 03:49:13.000000 seven_top-1.0.8/seven_top/top/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-11 05:43:54.719049 seven_top-1.0.8/seven_top/top/api/
--rw-rw-rw-   0        0        0      247 2020-08-11 03:52:12.000000 seven_top-1.0.8/seven_top/top/api/__init__.py
--rw-rw-rw-   0        0        0    10731 2020-08-11 03:47:36.000000 seven_top-1.0.8/seven_top/top/api/base.py
-drwxrwxrwx   0        0        0        0 2020-08-11 05:43:54.919022 seven_top-1.0.8/seven_top/top/api/rest/
--rw-rw-rw-   0        0        0      428 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/AlibabaAliqinTaNumberSinglecallbyttsRequest.py
--rw-rw-rw-   0        0        0      434 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/AlibabaAliqinTaNumberSinglecallbyvoiceRequest.py
--rw-rw-rw-   0        0        0      430 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/AlibabaAliqinTaSmsNumQueryRequest.py
--rw-rw-rw-   0        0        0      519 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/AlibabaAliqinTaSmsNumSendRequest.py
--rw-rw-rw-   0        0        0      488 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/AlibabaAliqinTaVoiceNumDoublecallRequest.py
--rw-rw-rw-   0        0        0      273 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/AppipGetRequest.py
--rw-rw-rw-   0        0        0      342 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/AppstoreSubscribeGetRequest.py
--rw-rw-rw-   0        0        0      345 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/FilesGetRequest.py
--rw-rw-rw-   0        0        0      334 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/FuwuSaleLinkGenRequest.py
--rw-rw-rw-   0        0        0      357 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/FuwuScoresGetRequest.py
--rw-rw-rw-   0        0        0      277 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/HttpdnsGetRequest.py
--rw-rw-rw-   0        0        0      329 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ItemSellerGetRequest.py
--rw-rw-rw-   0        0        0      345 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ItemSkuGetRequest.py
--rw-rw-rw-   0        0        0      326 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ItemSkusGetRequest.py
--rw-rw-rw-   0        0        0      320 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ItemcatsAuthorizeGetRequest.py
--rw-rw-rw-   0        0        0      371 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ItemcatsGetRequest.py
--rw-rw-rw-   0        0        0      631 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ItempropsGetRequest.py
--rw-rw-rw-   0        0        0      420 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ItempropvaluesGetRequest.py
--rw-rw-rw-   0        0        0      332 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ItemsCustomGetRequest.py
--rw-rw-rw-   0        0        0      631 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ItemsInventoryGetRequest.py
--rw-rw-rw-   0        0        0      680 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ItemsOnsaleGetRequest.py
--rw-rw-rw-   0        0        0      341 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ItemsSellerListGetRequest.py
--rw-rw-rw-   0        0        0      342 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/JstSmsExtendcodeQueryRequest.py
--rw-rw-rw-   0        0        0      339 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/JstSmsMenuinfoReportRequest.py
--rw-rw-rw-   0        0        0      345 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/JstSmsMessageBatchsendRequest.py
--rw-rw-rw-   0        0        0      329 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/JstSmsMessageSendRequest.py
--rw-rw-rw-   0        0        0      349 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/JstSmsOfficialaccountCancelRequest.py
--rw-rw-rw-   0        0        0      355 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/JstSmsOfficialaccountOfflineRequest.py
--rw-rw-rw-   0        0        0      360 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/JstSmsOfficialaccountOnlineRequest.py
--rw-rw-rw-   0        0        0      357 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/JstSmsOfficialaccountOrderRequest.py
--rw-rw-rw-   0        0        0      365 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/JstSmsOfficialaccountReportRequest.py
--rw-rw-rw-   0        0        0      346 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/JstSmsStatusQueryRequest.py
--rw-rw-rw-   0        0        0      354 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/KfcKeywordSearchRequest.py
--rw-rw-rw-   0        0        0      392 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/MiniappDistributionItemsBindRequest.py
--rw-rw-rw-   0        0        0      334 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/MiniappItemsGetRequest.py
--rw-rw-rw-   0        0        0      483 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/MiniappTemplateInstantiateRequest.py
--rw-rw-rw-   0        0        0      437 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/MiniappTemplateOnlineappRequest.py
--rw-rw-rw-   0        0        0      380 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/MiniappTemplateQueryappRequest.py
--rw-rw-rw-   0        0        0      424 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/MiniappTemplateUpdateRequest.py
--rw-rw-rw-   0        0        0      434 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/MiniappTemplateUpdateappRequest.py
--rw-rw-rw-   0        0        0      294 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/MiniappUserInfoGetRequest.py
--rw-rw-rw-   0        0        0      485 2020-08-11 03:56:43.000000 seven_top-1.0.8/seven_top/top/api/rest/MiniapppTemplateInstantiateRequest.py
--rw-rw-rw-   0        0        0      323 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/OpenTradeGetRequest.py
--rw-rw-rw-   0        0        0      544 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/OpenTradesSoldGetRequest.py
--rw-rw-rw-   0        0        0      314 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/OpenlinkSessionGetRequest.py
--rw-rw-rw-   0        0        0      337 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/OpenuidChangeRequest.py
--rw-rw-rw-   0        0        0      320 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/OpenuidGetBymixnickRequest.py
--rw-rw-rw-   0        0        0      311 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/OpenuidGetBytradeRequest.py
--rw-rw-rw-   0        0        0      277 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/OpenuidGetRequest.py
--rw-rw-rw-   0        0        0      314 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SellercatsListGetRequest.py
--rw-rw-rw-   0        0        0      395 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SellercenterRoleAddRequest.py
--rw-rw-rw-   0        0        0      328 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SellercenterRoleInfoGetRequest.py
--rw-rw-rw-   0        0        0      333 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SellercenterRolemembersGetRequest.py
--rw-rw-rw-   0        0        0      318 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SellercenterRolesGetRequest.py
--rw-rw-rw-   0        0        0      356 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SellercenterSubuserPermissionsRolesGetRequest.py
--rw-rw-rw-   0        0        0      324 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SellercenterSubusersGetRequest.py
--rw-rw-rw-   0        0        0      339 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SellercenterUserPermissionsGetRequest.py
--rw-rw-rw-   0        0        0      306 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ShopSellerGetRequest.py
--rw-rw-rw-   0        0        0      310 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/ShopcatsListGetRequest.py
--rw-rw-rw-   0        0        0      330 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SkusCustomGetRequest.py
--rw-rw-rw-   0        0        0      325 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SubuserDepartmentsGetRequest.py
--rw-rw-rw-   0        0        0      313 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SubuserDutysGetRequest.py
--rw-rw-rw-   0        0        0      673 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SubuserEmployeeAddRequest.py
--rw-rw-rw-   0        0        0      362 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SubuserFullinfoGetRequest.py
--rw-rw-rw-   0        0        0      378 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SubuserInfoUpdateRequest.py
--rw-rw-rw-   0        0        0      304 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/SubusersGetRequest.py
--rw-rw-rw-   0        0        0      271 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TimeGetRequest.py
--rw-rw-rw-   0        0        0      299 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcAuthGetRequest.py
--rw-rw-rw-   0        0        0      356 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcGroupAddRequest.py
--rw-rw-rw-   0        0        0      362 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcGroupDeleteRequest.py
--rw-rw-rw-   0        0        0      357 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcGroupsGetRequest.py
--rw-rw-rw-   0        0        0      697 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcMessageProduceRequest.py
--rw-rw-rw-   0        0        0      378 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcMessagesConfirmRequest.py
--rw-rw-rw-   0        0        0      344 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcMessagesConsumeRequest.py
--rw-rw-rw-   0        0        0      318 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcMessagesProduceRequest.py
--rw-rw-rw-   0        0        0      339 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcTopicGroupAddRequest.py
--rw-rw-rw-   0        0        0      369 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcTopicGroupDeleteRequest.py
--rw-rw-rw-   0        0        0      333 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcUserCancelRequest.py
--rw-rw-rw-   0        0        0      349 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcUserGetRequest.py
--rw-rw-rw-   0        0        0      306 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TmcUserPermitRequest.py
--rw-rw-rw-   0        0        0      335 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TopAuthTokenCreateRequest.py
--rw-rw-rw-   0        0        0      326 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TopAuthTokenRefreshRequest.py
--rw-rw-rw-   0        0        0      280 2020-08-11 03:56:41.000000 seven_top-1.0.8/seven_top/top/api/rest/TopIpoutGetRequest.py
--rw-rw-rw-   0        0        0      342 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TopSdkFeedbackUploadRequest.py
--rw-rw-rw-   0        0        0      370 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TopSecretGetRequest.py
--rw-rw-rw-   0        0        0      315 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/TopSecretRegisterRequest.py
--rw-rw-rw-   0        0        0      306 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/UserSellerGetRequest.py
--rw-rw-rw-   0        0        0      539 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/VasOrderSearchRequest.py
--rw-rw-rw-   0        0        0      539 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/VasSubscSearchRequest.py
--rw-rw-rw-   0        0        0      336 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/VasSubscribeGetRequest.py
--rw-rw-rw-   0        0        0     8116 2020-08-11 03:56:40.000000 seven_top-1.0.8/seven_top/top/api/rest/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-11 05:43:54.714062 seven_top-1.0.8/seven_top.egg-info/
--rw-rw-rw-   0        0        0      993 2020-08-11 05:43:54.000000 seven_top-1.0.8/seven_top.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5016 2020-08-11 05:43:54.000000 seven_top-1.0.8/seven_top.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-08-11 05:43:54.000000 seven_top-1.0.8/seven_top.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2020-08-11 05:43:54.000000 seven_top-1.0.8/seven_top.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2020-08-11 05:43:54.000000 seven_top-1.0.8/seven_top.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-09-07 11:02:59.298192 seven_top-1.0.9/
+-rw-rw-rw-   0        0        0     1141 2020-09-07 11:02:59.298192 seven_top-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2020-09-07 11:02:13.000000 seven_top-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2020-09-07 11:02:59.300187 seven_top-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1274 2020-09-07 11:01:32.000000 seven_top-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2020-09-07 11:02:59.028406 seven_top-1.0.9/seven_top/
+-rw-rw-rw-   0        0        0      139 2020-07-08 04:42:06.000000 seven_top-1.0.9/seven_top/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-07 11:02:59.044363 seven_top-1.0.9/seven_top/top/
+-rw-rw-rw-   0        0        0      530 2020-08-11 03:49:13.000000 seven_top-1.0.9/seven_top/top/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-07 11:02:59.051345 seven_top-1.0.9/seven_top/top/api/
+-rw-rw-rw-   0        0        0      247 2020-08-11 03:52:12.000000 seven_top-1.0.9/seven_top/top/api/__init__.py
+-rw-rw-rw-   0        0        0    10731 2020-08-11 03:47:36.000000 seven_top-1.0.9/seven_top/top/api/base.py
+drwxrwxrwx   0        0        0        0 2020-09-07 11:02:59.296198 seven_top-1.0.9/seven_top/top/api/rest/
+-rw-rw-rw-   0        0        0      428 2020-09-07 10:55:30.000000 seven_top-1.0.9/seven_top/top/api/rest/AlibabaAliqinTaNumberSinglecallbyttsRequest.py
+-rw-rw-rw-   0        0        0      434 2020-09-07 10:55:30.000000 seven_top-1.0.9/seven_top/top/api/rest/AlibabaAliqinTaNumberSinglecallbyvoiceRequest.py
+-rw-rw-rw-   0        0        0      430 2020-09-07 10:55:24.000000 seven_top-1.0.9/seven_top/top/api/rest/AlibabaAliqinTaSmsNumQueryRequest.py
+-rw-rw-rw-   0        0        0      519 2020-09-07 10:55:24.000000 seven_top-1.0.9/seven_top/top/api/rest/AlibabaAliqinTaSmsNumSendRequest.py
+-rw-rw-rw-   0        0        0      488 2020-09-07 10:55:24.000000 seven_top-1.0.9/seven_top/top/api/rest/AlibabaAliqinTaVoiceNumDoublecallRequest.py
+-rw-rw-rw-   0        0        0      273 2020-09-07 10:55:24.000000 seven_top-1.0.9/seven_top/top/api/rest/AppipGetRequest.py
+-rw-rw-rw-   0        0        0      342 2020-09-07 10:55:24.000000 seven_top-1.0.9/seven_top/top/api/rest/AppstoreSubscribeGetRequest.py
+-rw-rw-rw-   0        0        0      405 2020-09-07 10:58:06.000000 seven_top-1.0.9/seven_top/top/api/rest/CrmMemberIdentityGetRequest.py
+-rw-rw-rw-   0        0        0      381 2020-09-07 10:58:10.000000 seven_top-1.0.9/seven_top/top/api/rest/CrmMemberJoinurlGetRequest.py
+-rw-rw-rw-   0        0        0      345 2020-09-07 10:55:24.000000 seven_top-1.0.9/seven_top/top/api/rest/FilesGetRequest.py
+-rw-rw-rw-   0        0        0      334 2020-09-07 10:55:25.000000 seven_top-1.0.9/seven_top/top/api/rest/FuwuSaleLinkGenRequest.py
+-rw-rw-rw-   0        0        0      357 2020-09-07 10:55:30.000000 seven_top-1.0.9/seven_top/top/api/rest/FuwuScoresGetRequest.py
+-rw-rw-rw-   0        0        0      277 2020-09-07 10:55:30.000000 seven_top-1.0.9/seven_top/top/api/rest/HttpdnsGetRequest.py
+-rw-rw-rw-   0        0        0      329 2020-09-07 10:55:30.000000 seven_top-1.0.9/seven_top/top/api/rest/ItemSellerGetRequest.py
+-rw-rw-rw-   0        0        0      345 2020-09-07 10:55:35.000000 seven_top-1.0.9/seven_top/top/api/rest/ItemSkuGetRequest.py
+-rw-rw-rw-   0        0        0      326 2020-09-07 10:55:35.000000 seven_top-1.0.9/seven_top/top/api/rest/ItemSkusGetRequest.py
+-rw-rw-rw-   0        0        0      320 2020-09-07 10:55:30.000000 seven_top-1.0.9/seven_top/top/api/rest/ItemcatsAuthorizeGetRequest.py
+-rw-rw-rw-   0        0        0      371 2020-09-07 10:55:30.000000 seven_top-1.0.9/seven_top/top/api/rest/ItemcatsGetRequest.py
+-rw-rw-rw-   0        0        0      631 2020-09-07 10:55:30.000000 seven_top-1.0.9/seven_top/top/api/rest/ItempropsGetRequest.py
+-rw-rw-rw-   0        0        0      420 2020-09-07 10:55:30.000000 seven_top-1.0.9/seven_top/top/api/rest/ItempropvaluesGetRequest.py
+-rw-rw-rw-   0        0        0      332 2020-09-07 10:55:30.000000 seven_top-1.0.9/seven_top/top/api/rest/ItemsCustomGetRequest.py
+-rw-rw-rw-   0        0        0      631 2020-09-07 10:55:35.000000 seven_top-1.0.9/seven_top/top/api/rest/ItemsInventoryGetRequest.py
+-rw-rw-rw-   0        0        0      680 2020-09-07 10:55:35.000000 seven_top-1.0.9/seven_top/top/api/rest/ItemsOnsaleGetRequest.py
+-rw-rw-rw-   0        0        0      341 2020-09-07 10:55:35.000000 seven_top-1.0.9/seven_top/top/api/rest/ItemsSellerListGetRequest.py
+-rw-rw-rw-   0        0        0      342 2020-09-07 10:55:35.000000 seven_top-1.0.9/seven_top/top/api/rest/JstSmsExtendcodeQueryRequest.py
+-rw-rw-rw-   0        0        0      339 2020-09-07 10:55:35.000000 seven_top-1.0.9/seven_top/top/api/rest/JstSmsMenuinfoReportRequest.py
+-rw-rw-rw-   0        0        0      345 2020-09-07 10:55:35.000000 seven_top-1.0.9/seven_top/top/api/rest/JstSmsMessageBatchsendRequest.py
+-rw-rw-rw-   0        0        0      329 2020-09-07 10:55:35.000000 seven_top-1.0.9/seven_top/top/api/rest/JstSmsMessageSendRequest.py
+-rw-rw-rw-   0        0        0      349 2020-09-07 10:55:35.000000 seven_top-1.0.9/seven_top/top/api/rest/JstSmsOfficialaccountCancelRequest.py
+-rw-rw-rw-   0        0        0      355 2020-09-07 10:55:40.000000 seven_top-1.0.9/seven_top/top/api/rest/JstSmsOfficialaccountOfflineRequest.py
+-rw-rw-rw-   0        0        0      360 2020-09-07 10:55:40.000000 seven_top-1.0.9/seven_top/top/api/rest/JstSmsOfficialaccountOnlineRequest.py
+-rw-rw-rw-   0        0        0      357 2020-09-07 10:55:40.000000 seven_top-1.0.9/seven_top/top/api/rest/JstSmsOfficialaccountOrderRequest.py
+-rw-rw-rw-   0        0        0      365 2020-09-07 10:55:40.000000 seven_top-1.0.9/seven_top/top/api/rest/JstSmsOfficialaccountReportRequest.py
+-rw-rw-rw-   0        0        0      346 2020-09-07 10:55:40.000000 seven_top-1.0.9/seven_top/top/api/rest/JstSmsStatusQueryRequest.py
+-rw-rw-rw-   0        0        0      354 2020-09-07 10:55:40.000000 seven_top-1.0.9/seven_top/top/api/rest/KfcKeywordSearchRequest.py
+-rw-rw-rw-   0        0        0      392 2020-09-07 10:55:40.000000 seven_top-1.0.9/seven_top/top/api/rest/MiniappDistributionItemsBindRequest.py
+-rw-rw-rw-   0        0        0      334 2020-09-07 10:55:40.000000 seven_top-1.0.9/seven_top/top/api/rest/MiniappItemsGetRequest.py
+-rw-rw-rw-   0        0        0      483 2020-09-07 10:55:40.000000 seven_top-1.0.9/seven_top/top/api/rest/MiniappTemplateInstantiateRequest.py
+-rw-rw-rw-   0        0        0      437 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/MiniappTemplateOnlineappRequest.py
+-rw-rw-rw-   0        0        0      380 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/MiniappTemplateQueryappRequest.py
+-rw-rw-rw-   0        0        0      424 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/MiniappTemplateUpdateRequest.py
+-rw-rw-rw-   0        0        0      434 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/MiniappTemplateUpdateappRequest.py
+-rw-rw-rw-   0        0        0      294 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/MiniappUserInfoGetRequest.py
+-rw-rw-rw-   0        0        0      485 2020-09-07 10:55:40.000000 seven_top-1.0.9/seven_top/top/api/rest/MiniapppTemplateInstantiateRequest.py
+-rw-rw-rw-   0        0        0      323 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/OpenTradeGetRequest.py
+-rw-rw-rw-   0        0        0      544 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/OpenTradesSoldGetRequest.py
+-rw-rw-rw-   0        0        0      314 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/OpenlinkSessionGetRequest.py
+-rw-rw-rw-   0        0        0      337 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/OpenuidChangeRequest.py
+-rw-rw-rw-   0        0        0      320 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/OpenuidGetBymixnickRequest.py
+-rw-rw-rw-   0        0        0      311 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/OpenuidGetBytradeRequest.py
+-rw-rw-rw-   0        0        0      277 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/OpenuidGetRequest.py
+-rw-rw-rw-   0        0        0      314 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SellercatsListGetRequest.py
+-rw-rw-rw-   0        0        0      395 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SellercenterRoleAddRequest.py
+-rw-rw-rw-   0        0        0      328 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SellercenterRoleInfoGetRequest.py
+-rw-rw-rw-   0        0        0      333 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SellercenterRolemembersGetRequest.py
+-rw-rw-rw-   0        0        0      318 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SellercenterRolesGetRequest.py
+-rw-rw-rw-   0        0        0      356 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SellercenterSubuserPermissionsRolesGetRequest.py
+-rw-rw-rw-   0        0        0      324 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SellercenterSubusersGetRequest.py
+-rw-rw-rw-   0        0        0      339 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SellercenterUserPermissionsGetRequest.py
+-rw-rw-rw-   0        0        0      306 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/ShopSellerGetRequest.py
+-rw-rw-rw-   0        0        0      310 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/ShopcatsListGetRequest.py
+-rw-rw-rw-   0        0        0      330 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SkusCustomGetRequest.py
+-rw-rw-rw-   0        0        0      325 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SubuserDepartmentsGetRequest.py
+-rw-rw-rw-   0        0        0      313 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SubuserDutysGetRequest.py
+-rw-rw-rw-   0        0        0      673 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SubuserEmployeeAddRequest.py
+-rw-rw-rw-   0        0        0      362 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SubuserFullinfoGetRequest.py
+-rw-rw-rw-   0        0        0      378 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SubuserInfoUpdateRequest.py
+-rw-rw-rw-   0        0        0      304 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/SubusersGetRequest.py
+-rw-rw-rw-   0        0        0      271 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/TimeGetRequest.py
+-rw-rw-rw-   0        0        0      299 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcAuthGetRequest.py
+-rw-rw-rw-   0        0        0      356 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcGroupAddRequest.py
+-rw-rw-rw-   0        0        0      362 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcGroupDeleteRequest.py
+-rw-rw-rw-   0        0        0      357 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcGroupsGetRequest.py
+-rw-rw-rw-   0        0        0      697 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcMessageProduceRequest.py
+-rw-rw-rw-   0        0        0      378 2020-09-07 10:55:53.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcMessagesConfirmRequest.py
+-rw-rw-rw-   0        0        0      344 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcMessagesConsumeRequest.py
+-rw-rw-rw-   0        0        0      318 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcMessagesProduceRequest.py
+-rw-rw-rw-   0        0        0      339 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcTopicGroupAddRequest.py
+-rw-rw-rw-   0        0        0      369 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcTopicGroupDeleteRequest.py
+-rw-rw-rw-   0        0        0      333 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcUserCancelRequest.py
+-rw-rw-rw-   0        0        0      349 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcUserGetRequest.py
+-rw-rw-rw-   0        0        0      306 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TmcUserPermitRequest.py
+-rw-rw-rw-   0        0        0      335 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TopAuthTokenCreateRequest.py
+-rw-rw-rw-   0        0        0      326 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TopAuthTokenRefreshRequest.py
+-rw-rw-rw-   0        0        0      280 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TopIpoutGetRequest.py
+-rw-rw-rw-   0        0        0      342 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TopSdkFeedbackUploadRequest.py
+-rw-rw-rw-   0        0        0      370 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TopSecretGetRequest.py
+-rw-rw-rw-   0        0        0      315 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/TopSecretRegisterRequest.py
+-rw-rw-rw-   0        0        0      306 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/UserSellerGetRequest.py
+-rw-rw-rw-   0        0        0      539 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/VasOrderSearchRequest.py
+-rw-rw-rw-   0        0        0      539 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/VasSubscSearchRequest.py
+-rw-rw-rw-   0        0        0      336 2020-09-07 10:55:54.000000 seven_top-1.0.9/seven_top/top/api/rest/VasSubscribeGetRequest.py
+-rw-rw-rw-   0        0        0     8298 2020-09-07 10:56:54.000000 seven_top-1.0.9/seven_top/top/api/rest/__init__.py
+drwxrwxrwx   0        0        0        0 2020-09-07 11:02:59.040386 seven_top-1.0.9/seven_top.egg-info/
+-rw-rw-rw-   0        0        0     1141 2020-09-07 11:02:58.000000 seven_top-1.0.9/seven_top.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5123 2020-09-07 11:02:58.000000 seven_top-1.0.9/seven_top.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-09-07 11:02:58.000000 seven_top-1.0.9/seven_top.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2020-09-07 11:02:58.000000 seven_top-1.0.9/seven_top.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2020-09-07 11:02:58.000000 seven_top-1.0.9/seven_top.egg-info/top_level.txt
```

### Comparing `seven_top-1.0.8/PKG-INFO` & `seven_top-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven_top
-Version: 1.0.8
+Version: 1.0.9
 Summary: seven top
 Home-page: http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_top
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: 
         # seven_top
@@ -12,14 +12,19 @@
         ## 天志互联Python淘宝top库
         
         ### 1.0.5 更新内容
         * 淘宝top库初始工程
         
         ### 1.0.8 更新内容
         * 增加新的api
+        
+        ### 1.0.9 更新内容
+        * 增加新的api
+        CrmMemberIdentityGetRequest.py
+        CrmMemberJoinurlGetRequest.py
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `seven_top-1.0.8/setup.py` & `seven_top-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="seven_top",
-    version="1.0.8",
+    version="1.0.9",
     author="seven",
     author_email="tech@gao7.com",
     description="seven top",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_top",
```

### Comparing `seven_top-1.0.8/seven_top/top/__init__.py` & `seven_top-1.0.9/seven_top/top/__init__.py`

 * *Files identical despite different names*

### Comparing `seven_top-1.0.8/seven_top/top/api/base.py` & `seven_top-1.0.9/seven_top/top/api/base.py`

 * *Files identical despite different names*

### Comparing `seven_top-1.0.8/seven_top/top/api/rest/AlibabaAliqinTaSmsNumSendRequest.py` & `seven_top-1.0.9/seven_top/top/api/rest/AlibabaAliqinTaSmsNumSendRequest.py`

 * *Files identical despite different names*

### Comparing `seven_top-1.0.8/seven_top/top/api/rest/ItempropsGetRequest.py` & `seven_top-1.0.9/seven_top/top/api/rest/ItempropsGetRequest.py`

 * *Files identical despite different names*

### Comparing `seven_top-1.0.8/seven_top/top/api/rest/ItemsInventoryGetRequest.py` & `seven_top-1.0.9/seven_top/top/api/rest/ItemsInventoryGetRequest.py`

 * *Files identical despite different names*

### Comparing `seven_top-1.0.8/seven_top/top/api/rest/ItemsOnsaleGetRequest.py` & `seven_top-1.0.9/seven_top/top/api/rest/ItemsOnsaleGetRequest.py`

 * *Files identical despite different names*

### Comparing `seven_top-1.0.8/seven_top/top/api/rest/OpenTradesSoldGetRequest.py` & `seven_top-1.0.9/seven_top/top/api/rest/OpenTradesSoldGetRequest.py`

 * *Files identical despite different names*

### Comparing `seven_top-1.0.8/seven_top/top/api/rest/SubuserEmployeeAddRequest.py` & `seven_top-1.0.9/seven_top/top/api/rest/SubuserEmployeeAddRequest.py`

 * *Files identical despite different names*

### Comparing `seven_top-1.0.8/seven_top/top/api/rest/TmcMessageProduceRequest.py` & `seven_top-1.0.9/seven_top/top/api/rest/TmcMessageProduceRequest.py`

 * *Files identical despite different names*

### Comparing `seven_top-1.0.8/seven_top/top/api/rest/VasOrderSearchRequest.py` & `seven_top-1.0.9/seven_top/top/api/rest/VasOrderSearchRequest.py`

 * *Files identical despite different names*

### Comparing `seven_top-1.0.8/seven_top/top/api/rest/VasSubscSearchRequest.py` & `seven_top-1.0.9/seven_top/top/api/rest/VasSubscSearchRequest.py`

 * *Files identical despite different names*

### Comparing `seven_top-1.0.8/seven_top/top/api/rest/__init__.py` & `seven_top-1.0.9/seven_top/top/api/rest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,98 +1,100 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJingCan
 @Date: 2020-07-08 10:14:46
-@LastEditTime: 2020-08-11 11:56:19
+@LastEditTime: 2020-09-07 18:56:54
 @LastEditors: HuangJingCan
 @Description: 
 """
-from seven_top.top.api.rest.OpenlinkSessionGetRequest import OpenlinkSessionGetRequest
-from seven_top.top.api.rest.SubuserDutysGetRequest import SubuserDutysGetRequest
-from seven_top.top.api.rest.OpenuidGetBymixnickRequest import OpenuidGetBymixnickRequest
-from seven_top.top.api.rest.MiniappTemplateUpdateappRequest import MiniappTemplateUpdateappRequest
-from seven_top.top.api.rest.SellercatsListGetRequest import SellercatsListGetRequest
-from seven_top.top.api.rest.AlibabaAliqinTaSmsNumQueryRequest import AlibabaAliqinTaSmsNumQueryRequest
-from seven_top.top.api.rest.SellercenterSubuserPermissionsRolesGetRequest import SellercenterSubuserPermissionsRolesGetRequest
-from seven_top.top.api.rest.TmcGroupDeleteRequest import TmcGroupDeleteRequest
-from seven_top.top.api.rest.TmcAuthGetRequest import TmcAuthGetRequest
-from seven_top.top.api.rest.TopSdkFeedbackUploadRequest import TopSdkFeedbackUploadRequest
-from seven_top.top.api.rest.SubuserInfoUpdateRequest import SubuserInfoUpdateRequest
-from seven_top.top.api.rest.MiniappItemsGetRequest import MiniappItemsGetRequest
-from seven_top.top.api.rest.AlibabaAliqinTaVoiceNumDoublecallRequest import AlibabaAliqinTaVoiceNumDoublecallRequest
-from seven_top.top.api.rest.TmcTopicGroupAddRequest import TmcTopicGroupAddRequest
-from seven_top.top.api.rest.SubuserFullinfoGetRequest import SubuserFullinfoGetRequest
-from seven_top.top.api.rest.AppstoreSubscribeGetRequest import AppstoreSubscribeGetRequest
-from seven_top.top.api.rest.TopSecretRegisterRequest import TopSecretRegisterRequest
-from seven_top.top.api.rest.SellercenterRolemembersGetRequest import SellercenterRolemembersGetRequest
-from seven_top.top.api.rest.SellercenterUserPermissionsGetRequest import SellercenterUserPermissionsGetRequest
-from seven_top.top.api.rest.ShopSellerGetRequest import ShopSellerGetRequest
-from seven_top.top.api.rest.SellercenterRolesGetRequest import SellercenterRolesGetRequest
-from seven_top.top.api.rest.MiniappTemplateQueryappRequest import MiniappTemplateQueryappRequest
-from seven_top.top.api.rest.ItemSkuGetRequest import ItemSkuGetRequest
-from seven_top.top.api.rest.TmcGroupAddRequest import TmcGroupAddRequest
+from seven_top.top.api.rest.AlibabaAliqinTaNumberSinglecallbyttsRequest import AlibabaAliqinTaNumberSinglecallbyttsRequest
+from seven_top.top.api.rest.SkusCustomGetRequest import SkusCustomGetRequest
+from seven_top.top.api.rest.JstSmsOfficialaccountReportRequest import JstSmsOfficialaccountReportRequest
+from seven_top.top.api.rest.TmcMessageProduceRequest import TmcMessageProduceRequest
+from seven_top.top.api.rest.ItemsCustomGetRequest import ItemsCustomGetRequest
+from seven_top.top.api.rest.FuwuSaleLinkGenRequest import FuwuSaleLinkGenRequest
+from seven_top.top.api.rest.AlibabaAliqinTaNumberSinglecallbyvoiceRequest import AlibabaAliqinTaNumberSinglecallbyvoiceRequest
+from seven_top.top.api.rest.ItemSellerGetRequest import ItemSellerGetRequest
+from seven_top.top.api.rest.KfcKeywordSearchRequest import KfcKeywordSearchRequest
+from seven_top.top.api.rest.TmcMessagesProduceRequest import TmcMessagesProduceRequest
 from seven_top.top.api.rest.SubuserDepartmentsGetRequest import SubuserDepartmentsGetRequest
-from seven_top.top.api.rest.ItemsInventoryGetRequest import ItemsInventoryGetRequest
-from seven_top.top.api.rest.OpenTradeGetRequest import OpenTradeGetRequest
-from seven_top.top.api.rest.TmcMessagesConfirmRequest import TmcMessagesConfirmRequest
-from seven_top.top.api.rest.SellercenterSubusersGetRequest import SellercenterSubusersGetRequest
-from seven_top.top.api.rest.AppipGetRequest import AppipGetRequest
-from seven_top.top.api.rest.ItempropsGetRequest import ItempropsGetRequest
-from seven_top.top.api.rest.ItemcatsAuthorizeGetRequest import ItemcatsAuthorizeGetRequest
-from seven_top.top.api.rest.TimeGetRequest import TimeGetRequest
-from seven_top.top.api.rest.JstSmsMenuinfoReportRequest import JstSmsMenuinfoReportRequest
 from seven_top.top.api.rest.OpenuidGetRequest import OpenuidGetRequest
-from seven_top.top.api.rest.SubuserEmployeeAddRequest import SubuserEmployeeAddRequest
-from seven_top.top.api.rest.JstSmsMessageBatchsendRequest import JstSmsMessageBatchsendRequest
 from seven_top.top.api.rest.MiniappTemplateUpdateRequest import MiniappTemplateUpdateRequest
-from seven_top.top.api.rest.AlibabaAliqinTaNumberSinglecallbyttsRequest import AlibabaAliqinTaNumberSinglecallbyttsRequest
-from seven_top.top.api.rest.JstSmsOfficialaccountOfflineRequest import JstSmsOfficialaccountOfflineRequest
-from seven_top.top.api.rest.MiniappTemplateOnlineappRequest import MiniappTemplateOnlineappRequest
-from seven_top.top.api.rest.KfcKeywordSearchRequest import KfcKeywordSearchRequest
-from seven_top.top.api.rest.TmcTopicGroupDeleteRequest import TmcTopicGroupDeleteRequest
-from seven_top.top.api.rest.AlibabaAliqinTaSmsNumSendRequest import AlibabaAliqinTaSmsNumSendRequest
-from seven_top.top.api.rest.MiniappTemplateInstantiateRequest import MiniappTemplateInstantiateRequest
-from seven_top.top.api.rest.MiniappDistributionItemsBindRequest import MiniappDistributionItemsBindRequest
+from seven_top.top.api.rest.ItemsOnsaleGetRequest import ItemsOnsaleGetRequest
 from seven_top.top.api.rest.OpenuidChangeRequest import OpenuidChangeRequest
-from seven_top.top.api.rest.TopSecretGetRequest import TopSecretGetRequest
-from seven_top.top.api.rest.OpenTradesSoldGetRequest import OpenTradesSoldGetRequest
-from seven_top.top.api.rest.ItemSkusGetRequest import ItemSkusGetRequest
-from seven_top.top.api.rest.JstSmsOfficialaccountOrderRequest import JstSmsOfficialaccountOrderRequest
-from seven_top.top.api.rest.VasOrderSearchRequest import VasOrderSearchRequest
-from seven_top.top.api.rest.TmcUserCancelRequest import TmcUserCancelRequest
+from seven_top.top.api.rest.SellercenterSubusersGetRequest import SellercenterSubusersGetRequest
+from seven_top.top.api.rest.SellercenterRolemembersGetRequest import SellercenterRolemembersGetRequest
+from seven_top.top.api.rest.MiniappTemplateQueryappRequest import MiniappTemplateQueryappRequest
+from seven_top.top.api.rest.FuwuScoresGetRequest import FuwuScoresGetRequest
+from seven_top.top.api.rest.ItempropvaluesGetRequest import ItempropvaluesGetRequest
+from seven_top.top.api.rest.MiniappTemplateOnlineappRequest import MiniappTemplateOnlineappRequest
 from seven_top.top.api.rest.FilesGetRequest import FilesGetRequest
-from seven_top.top.api.rest.MiniapppTemplateInstantiateRequest import MiniapppTemplateInstantiateRequest
 from seven_top.top.api.rest.TopAuthTokenCreateRequest import TopAuthTokenCreateRequest
-from seven_top.top.api.rest.TmcGroupsGetRequest import TmcGroupsGetRequest
-from seven_top.top.api.rest.JstSmsStatusQueryRequest import JstSmsStatusQueryRequest
-from seven_top.top.api.rest.ItemsOnsaleGetRequest import ItemsOnsaleGetRequest
-from seven_top.top.api.rest.FuwuSaleLinkGenRequest import FuwuSaleLinkGenRequest
-from seven_top.top.api.rest.JstSmsOfficialaccountReportRequest import JstSmsOfficialaccountReportRequest
 from seven_top.top.api.rest.TmcMessagesConsumeRequest import TmcMessagesConsumeRequest
-from seven_top.top.api.rest.VasSubscribeGetRequest import VasSubscribeGetRequest
-from seven_top.top.api.rest.TmcUserPermitRequest import TmcUserPermitRequest
-from seven_top.top.api.rest.TmcMessageProduceRequest import TmcMessageProduceRequest
-from seven_top.top.api.rest.TopIpoutGetRequest import TopIpoutGetRequest
-from seven_top.top.api.rest.ItemsCustomGetRequest import ItemsCustomGetRequest
-from seven_top.top.api.rest.FuwuScoresGetRequest import FuwuScoresGetRequest
+from seven_top.top.api.rest.SellercenterRolesGetRequest import SellercenterRolesGetRequest
 from seven_top.top.api.rest.VasSubscSearchRequest import VasSubscSearchRequest
-from seven_top.top.api.rest.SellercenterRoleAddRequest import SellercenterRoleAddRequest
-from seven_top.top.api.rest.ItemSellerGetRequest import ItemSellerGetRequest
-from seven_top.top.api.rest.TmcUserGetRequest import TmcUserGetRequest
 from seven_top.top.api.rest.ItemcatsGetRequest import ItemcatsGetRequest
+from seven_top.top.api.rest.SellercatsListGetRequest import SellercatsListGetRequest
+from seven_top.top.api.rest.AlibabaAliqinTaSmsNumSendRequest import AlibabaAliqinTaSmsNumSendRequest
+from seven_top.top.api.rest.JstSmsOfficialaccountOnlineRequest import JstSmsOfficialaccountOnlineRequest
+from seven_top.top.api.rest.JstSmsOfficialaccountCancelRequest import JstSmsOfficialaccountCancelRequest
 from seven_top.top.api.rest.SellercenterRoleInfoGetRequest import SellercenterRoleInfoGetRequest
-from seven_top.top.api.rest.SubusersGetRequest import SubusersGetRequest
-from seven_top.top.api.rest.SkusCustomGetRequest import SkusCustomGetRequest
-from seven_top.top.api.rest.TopAuthTokenRefreshRequest import TopAuthTokenRefreshRequest
-from seven_top.top.api.rest.UserSellerGetRequest import UserSellerGetRequest
-from seven_top.top.api.rest.JstSmsExtendcodeQueryRequest import JstSmsExtendcodeQueryRequest
+from seven_top.top.api.rest.JstSmsMessageSendRequest import JstSmsMessageSendRequest
+from seven_top.top.api.rest.TopIpoutGetRequest import TopIpoutGetRequest
+from seven_top.top.api.rest.TmcGroupDeleteRequest import TmcGroupDeleteRequest
+from seven_top.top.api.rest.ShopSellerGetRequest import ShopSellerGetRequest
+from seven_top.top.api.rest.SellercenterUserPermissionsGetRequest import SellercenterUserPermissionsGetRequest
+from seven_top.top.api.rest.CrmMemberIdentityGetRequest import CrmMemberIdentityGetRequest
+from seven_top.top.api.rest.TmcTopicGroupAddRequest import TmcTopicGroupAddRequest
+from seven_top.top.api.rest.ShopcatsListGetRequest import ShopcatsListGetRequest
+from seven_top.top.api.rest.TmcGroupsGetRequest import TmcGroupsGetRequest
+from seven_top.top.api.rest.CrmMemberJoinurlGetRequest import CrmMemberJoinurlGetRequest
+from seven_top.top.api.rest.VasOrderSearchRequest import VasOrderSearchRequest
+from seven_top.top.api.rest.JstSmsStatusQueryRequest import JstSmsStatusQueryRequest
 from seven_top.top.api.rest.HttpdnsGetRequest import HttpdnsGetRequest
+from seven_top.top.api.rest.TmcTopicGroupDeleteRequest import TmcTopicGroupDeleteRequest
+from seven_top.top.api.rest.AppipGetRequest import AppipGetRequest
+from seven_top.top.api.rest.OpenTradeGetRequest import OpenTradeGetRequest
+from seven_top.top.api.rest.TimeGetRequest import TimeGetRequest
+from seven_top.top.api.rest.TmcMessagesConfirmRequest import TmcMessagesConfirmRequest
+from seven_top.top.api.rest.TopSecretGetRequest import TopSecretGetRequest
+from seven_top.top.api.rest.MiniappTemplateUpdateappRequest import MiniappTemplateUpdateappRequest
 from seven_top.top.api.rest.ItemsSellerListGetRequest import ItemsSellerListGetRequest
-from seven_top.top.api.rest.ShopcatsListGetRequest import ShopcatsListGetRequest
-from seven_top.top.api.rest.TmcMessagesProduceRequest import TmcMessagesProduceRequest
-from seven_top.top.api.rest.ItempropvaluesGetRequest import ItempropvaluesGetRequest
-from seven_top.top.api.rest.JstSmsOfficialaccountOnlineRequest import JstSmsOfficialaccountOnlineRequest
-from seven_top.top.api.rest.JstSmsOfficialaccountCancelRequest import JstSmsOfficialaccountCancelRequest
+from seven_top.top.api.rest.SellercenterRoleAddRequest import SellercenterRoleAddRequest
+from seven_top.top.api.rest.TmcUserPermitRequest import TmcUserPermitRequest
+from seven_top.top.api.rest.ItempropsGetRequest import ItempropsGetRequest
 from seven_top.top.api.rest.OpenuidGetBytradeRequest import OpenuidGetBytradeRequest
+from seven_top.top.api.rest.JstSmsOfficialaccountOfflineRequest import JstSmsOfficialaccountOfflineRequest
 from seven_top.top.api.rest.MiniappUserInfoGetRequest import MiniappUserInfoGetRequest
-from seven_top.top.api.rest.AlibabaAliqinTaNumberSinglecallbyvoiceRequest import AlibabaAliqinTaNumberSinglecallbyvoiceRequest
-from seven_top.top.api.rest.JstSmsMessageSendRequest import JstSmsMessageSendRequest
+from seven_top.top.api.rest.ItemcatsAuthorizeGetRequest import ItemcatsAuthorizeGetRequest
+from seven_top.top.api.rest.UserSellerGetRequest import UserSellerGetRequest
+from seven_top.top.api.rest.ItemsInventoryGetRequest import ItemsInventoryGetRequest
+from seven_top.top.api.rest.VasSubscribeGetRequest import VasSubscribeGetRequest
+from seven_top.top.api.rest.ItemSkusGetRequest import ItemSkusGetRequest
+from seven_top.top.api.rest.SubuserDutysGetRequest import SubuserDutysGetRequest
+from seven_top.top.api.rest.SubuserInfoUpdateRequest import SubuserInfoUpdateRequest
+from seven_top.top.api.rest.TmcUserCancelRequest import TmcUserCancelRequest
+from seven_top.top.api.rest.MiniappItemsGetRequest import MiniappItemsGetRequest
+from seven_top.top.api.rest.AlibabaAliqinTaVoiceNumDoublecallRequest import AlibabaAliqinTaVoiceNumDoublecallRequest
+from seven_top.top.api.rest.TopAuthTokenRefreshRequest import TopAuthTokenRefreshRequest
+from seven_top.top.api.rest.SubuserFullinfoGetRequest import SubuserFullinfoGetRequest
+from seven_top.top.api.rest.TmcGroupAddRequest import TmcGroupAddRequest
+from seven_top.top.api.rest.JstSmsMessageBatchsendRequest import JstSmsMessageBatchsendRequest
+from seven_top.top.api.rest.OpenlinkSessionGetRequest import OpenlinkSessionGetRequest
+from seven_top.top.api.rest.MiniapppTemplateInstantiateRequest import MiniapppTemplateInstantiateRequest
+from seven_top.top.api.rest.MiniappTemplateInstantiateRequest import MiniappTemplateInstantiateRequest
+from seven_top.top.api.rest.ItemSkuGetRequest import ItemSkuGetRequest
+from seven_top.top.api.rest.JstSmsOfficialaccountOrderRequest import JstSmsOfficialaccountOrderRequest
+from seven_top.top.api.rest.TopSecretRegisterRequest import TopSecretRegisterRequest
+from seven_top.top.api.rest.JstSmsMenuinfoReportRequest import JstSmsMenuinfoReportRequest
+from seven_top.top.api.rest.MiniappDistributionItemsBindRequest import MiniappDistributionItemsBindRequest
+from seven_top.top.api.rest.OpenuidGetBymixnickRequest import OpenuidGetBymixnickRequest
+from seven_top.top.api.rest.AlibabaAliqinTaSmsNumQueryRequest import AlibabaAliqinTaSmsNumQueryRequest
+from seven_top.top.api.rest.OpenTradesSoldGetRequest import OpenTradesSoldGetRequest
+from seven_top.top.api.rest.TopSdkFeedbackUploadRequest import TopSdkFeedbackUploadRequest
+from seven_top.top.api.rest.SellercenterSubuserPermissionsRolesGetRequest import SellercenterSubuserPermissionsRolesGetRequest
+from seven_top.top.api.rest.SubusersGetRequest import SubusersGetRequest
+from seven_top.top.api.rest.TmcUserGetRequest import TmcUserGetRequest
+from seven_top.top.api.rest.JstSmsExtendcodeQueryRequest import JstSmsExtendcodeQueryRequest
+from seven_top.top.api.rest.SubuserEmployeeAddRequest import SubuserEmployeeAddRequest
+from seven_top.top.api.rest.AppstoreSubscribeGetRequest import AppstoreSubscribeGetRequest
+from seven_top.top.api.rest.TmcAuthGetRequest import TmcAuthGetRequest
```

### Comparing `seven_top-1.0.8/seven_top.egg-info/PKG-INFO` & `seven_top-1.0.9/seven_top.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven-top
-Version: 1.0.8
+Version: 1.0.9
 Summary: seven top
 Home-page: http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_top
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: 
         # seven_top
@@ -12,14 +12,19 @@
         ## 天志互联Python淘宝top库
         
         ### 1.0.5 更新内容
         * 淘宝top库初始工程
         
         ### 1.0.8 更新内容
         * 增加新的api
+        
+        ### 1.0.9 更新内容
+        * 增加新的api
+        CrmMemberIdentityGetRequest.py
+        CrmMemberJoinurlGetRequest.py
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `seven_top-1.0.8/seven_top.egg-info/SOURCES.txt` & `seven_top-1.0.9/seven_top.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 seven_top/top/api/rest/AlibabaAliqinTaNumberSinglecallbyttsRequest.py
 seven_top/top/api/rest/AlibabaAliqinTaNumberSinglecallbyvoiceRequest.py
 seven_top/top/api/rest/AlibabaAliqinTaSmsNumQueryRequest.py
 seven_top/top/api/rest/AlibabaAliqinTaSmsNumSendRequest.py
 seven_top/top/api/rest/AlibabaAliqinTaVoiceNumDoublecallRequest.py
 seven_top/top/api/rest/AppipGetRequest.py
 seven_top/top/api/rest/AppstoreSubscribeGetRequest.py
+seven_top/top/api/rest/CrmMemberIdentityGetRequest.py
+seven_top/top/api/rest/CrmMemberJoinurlGetRequest.py
 seven_top/top/api/rest/FilesGetRequest.py
 seven_top/top/api/rest/FuwuSaleLinkGenRequest.py
 seven_top/top/api/rest/FuwuScoresGetRequest.py
 seven_top/top/api/rest/HttpdnsGetRequest.py
 seven_top/top/api/rest/ItemSellerGetRequest.py
 seven_top/top/api/rest/ItemSkuGetRequest.py
 seven_top/top/api/rest/ItemSkusGetRequest.py
```

