# Comparing `tmp/printnanny-api-client-0.99.8.tar.gz` & `tmp/printnanny-api-client-0.99.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printnanny-api-client-0.99.8.tar", last modified: Thu Aug  4 02:23:28 2022, max compression
+gzip compressed data, was "printnanny-api-client-0.99.9.tar", last modified: Thu Aug  4 15:39:54 2022, max compression
```

## Comparing `printnanny-api-client-0.99.8.tar` & `printnanny-api-client-0.99.9.tar`

### file list

```diff
@@ -1,352 +1,355 @@
-drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 02:23:28.837936 printnanny-api-client-0.99.8/
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      236 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/MANIFEST.in
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      309 2022-08-04 02:23:28.837936 printnanny-api-client-0.99.8/PKG-INFO
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    21623 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/README.md
-drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 02:23:28.821936 printnanny-api-client-0.99.8/docs/
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    61480 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/AccountsApi.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    23027 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/AlertsApi.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4064 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/BillingApi.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      525 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/BillingSummary.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      510 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/CallbackTokenAuthRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1069 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/CloudiotDevice.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      331 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/CloudiotDeviceRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      299 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/CollectionMethodEnum.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      353 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/DetailResponse.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)   158503 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/DevicesApi.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      630 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/EmailAlertSettings.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      473 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/EmailAlertSettingsRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      443 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/EmailAuthRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      399 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/EmailWaitlist.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      325 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/EmailWaitlistRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      294 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/EndBehaviorEnum.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      342 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/ErrorDetail.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      293 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/EventTypesEnum.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    17456 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/EventsApi.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      480 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/GcodeFile.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      291 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/IntervalEnum.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    23031 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/JanusApi.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      294 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/JanusConfigType.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      346 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/LoginRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      572 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/OctoPrintBackup.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      754 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/OctoPrintServer.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      519 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/OctoPrintServerRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      983 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/OctoPrintSettings.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      909 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/OctoPrintSettingsRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1470 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/OctoPrinterProfile.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1313 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/OctoPrinterProfileRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    98403 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/OctoprintApi.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      288 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/OsEdition.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      496 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedCloudiotDeviceList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      508 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedEmailAlertSettingsList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      481 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedGcodeFileList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      499 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedOctoPrintBackupList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      499 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedOctoPrintServerList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      505 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedOctoPrintSettingsList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      508 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedOctoPrinterProfileList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      460 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedPiList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      484 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedPiSettingsList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      508 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedPolymorphicPiEventList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      481 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedPublicKeyList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      484 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedSystemInfoList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      490 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PaginatedWebrtcStreamList.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      368 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PasswordChangeRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      476 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PasswordResetConfirmRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      376 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PasswordResetRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      349 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PatchedCloudiotDeviceRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      480 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PatchedEmailAlertSettingsRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      537 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PatchedOctoPrintServerRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      927 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PatchedOctoPrintSettingsRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1342 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PatchedOctoPrinterProfileRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      688 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PatchedPiRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      542 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PatchedPiSettingsRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      490 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PatchedPublicKeyRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1086 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PatchedSystemInfoRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      417 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PatchedUserRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      512 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PatchedWebrtcStreamRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1384 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/Pi.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      595 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiBootCommand.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      472 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiBootCommandRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      296 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiBootCommandType.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      589 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiBootEvent.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      466 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiBootEventRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      294 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiBootEventType.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      610 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiGstreamerCommand.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      487 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiGstreamerCommandRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      301 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiGstreamerCommandType.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      681 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      598 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiSettings.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      524 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiSettingsRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      647 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiSoftwareUpdateEvent.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      524 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiSoftwareUpdateEventRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      304 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiSoftwareUpdateEventType.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      344 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PiUrls.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    17393 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PisApi.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      624 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PolymorphicPiEvent.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      501 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PolymorphicPiEventRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      390 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PrintNannyApiConfig.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      415 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PrintNannyLicense.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      549 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PublicKey.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      428 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/PublicKeyRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      380 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/RegisterRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      335 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/ResendEmailVerificationRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      331 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/RestAuthDetail.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      286 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/SbcEnum.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4261 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/SchemaApi.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    23079 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/SettingsApi.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3508 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/StripeCustomer.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4004 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/StripePaymentMethod.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2927 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/StripePlan.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6428 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/StripeSubscription.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2719 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/StripeSubscriptionSchedule.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      315 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/StripeSubscriptionScheduleStatusEnum.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      307 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/StripeSubscriptionStatusEnum.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1090 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/SystemInfo.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      969 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/SystemInfoRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      292 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/TaxExemptEnum.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      336 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/Token.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      351 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/TokenResponse.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      287 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/TypeEnum.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      292 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/UsageTypeEnum.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      473 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/User.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      399 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/UserRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      321 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/VerifyEmailRequest.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1142 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/WebrtcStream.md
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      505 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/docs/WebrtcStreamRequest.md
-drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 02:23:28.821936 printnanny-api-client-0.99.8/printnanny_api_client/
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     9688 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/__init__.py
-drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 02:23:28.825936 printnanny-api-client-0.99.8/printnanny_api_client/api/
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      687 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api/__init__.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    93726 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api/accounts_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    32892 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api/alerts_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6245 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api/billing_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)   250523 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api/devices_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    25756 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api/events_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    36093 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api/janus_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)   152594 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api/octoprint_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    25753 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api/pis_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6690 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api/schema_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    32894 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api/settings_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    28079 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/api_client.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    16995 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/configuration.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5118 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/exceptions.py
-drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 02:23:28.829936 printnanny-api-client-0.99.8/printnanny_api_client/models/
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8539 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/__init__.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6476 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/billing_summary.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6712 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/callback_token_auth_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    19294 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/cloudiot_device.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3966 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/cloudiot_device_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3258 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/collection_method_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3822 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/detail_response.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     9277 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/email_alert_settings.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6099 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/email_alert_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4057 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/email_auth_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5617 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/email_waitlist.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4331 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/email_waitlist_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3181 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/end_behavior_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4530 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/error_detail.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3399 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/event_types_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     7939 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/gcode_file.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3202 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/interval_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3169 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/janus_config_type.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5099 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/login_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    10344 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/octo_print_backup.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    12215 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/octo_print_server.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     9563 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/octo_print_server_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    11651 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/octo_print_settings.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    10519 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/octo_print_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    27869 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/octo_printer_profile.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    26268 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/octo_printer_profile_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3148 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/os_edition.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5803 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_cloudiot_device_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5895 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_email_alert_settings_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5688 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_gcode_file_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5826 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_octo_print_backup_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5826 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_octo_print_server_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5872 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_octo_print_settings_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5895 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_octo_printer_profile_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5527 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_pi_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5711 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_pi_settings_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5895 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_polymorphic_pi_event_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5688 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_public_key_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5711 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_system_info_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5757 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_webrtc_stream_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6064 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/password_change_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8204 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/password_reset_confirm_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4089 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/password_reset_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3862 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/patched_cloudiot_device_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6211 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/patched_email_alert_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     9579 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/patched_octo_print_server_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    10577 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/patched_octo_print_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    26595 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/patched_octo_printer_profile_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8332 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/patched_pi_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5814 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/patched_pi_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8152 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/patched_public_key_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    16204 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/patched_system_info_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6033 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/patched_user_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8897 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/patched_webrtc_stream_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    15619 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8994 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_command.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6772 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_command_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3192 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_command_type.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8924 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_event.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6726 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_event_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3460 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_event_type.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     9169 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_gstreamer_command.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6887 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_gstreamer_command_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3197 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_gstreamer_command_type.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8136 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     7301 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_settings.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     5854 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    10358 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_software_update_event.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8315 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_software_update_event_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3251 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_software_update_event_type.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4624 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/pi_urls.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    10582 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/polymorphic_pi_event.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8575 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/polymorphic_pi_event_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4805 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/print_nanny_api_config.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4169 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/print_nanny_license.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    10278 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/public_key.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8762 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/public_key_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6271 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/register_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4169 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/resend_email_verification_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3822 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/rest_auth_detail.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3113 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/sbc_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    31541 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_customer.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    31348 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_payment_method.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    25067 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_plan.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    49457 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_subscription.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    23298 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_subscription_schedule.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3388 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_subscription_schedule_status_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3446 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_subscription_status_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    18021 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/system_info.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    17444 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/system_info_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3197 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/tax_exempt_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3918 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/token.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3792 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/token_response.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3843 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/type_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3179 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/usage_type_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     7310 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/user.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     6076 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/user_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4023 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/verify_email_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    20012 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/webrtc_stream.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     8729 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/models/webrtc_stream_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)        0 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/py.typed
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     9909 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/printnanny_api_client/rest.py
-drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 02:23:28.821936 printnanny-api-client-0.99.8/printnanny_api_client.egg-info/
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      309 2022-08-04 02:23:28.000000 printnanny-api-client-0.99.8/printnanny_api_client.egg-info/PKG-INFO
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    12954 2022-08-04 02:23:28.000000 printnanny-api-client-0.99.8/printnanny_api_client.egg-info/SOURCES.txt
--rw-rw-r--   0 leigh     (1000) leigh     (1000)        1 2022-08-04 02:23:28.000000 printnanny-api-client-0.99.8/printnanny_api_client.egg-info/dependency_links.txt
--rw-rw-r--   0 leigh     (1000) leigh     (1000)       66 2022-08-04 02:23:28.000000 printnanny-api-client-0.99.8/printnanny_api_client.egg-info/requires.txt
--rw-rw-r--   0 leigh     (1000) leigh     (1000)       27 2022-08-04 02:23:28.000000 printnanny-api-client-0.99.8/printnanny_api_client.egg-info/top_level.txt
--rw-rw-r--   0 leigh     (1000) leigh     (1000)       69 2022-08-04 02:23:28.837936 printnanny-api-client-0.99.8/setup.cfg
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1111 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/setup.py
-drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 02:23:28.837936 printnanny-api-client-0.99.8/test/
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2597 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_accounts_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1385 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_alerts_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      857 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_billing_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    23966 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_billing_summary.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1646 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_callback_token_auth_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2933 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_cloudiot_device.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1535 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_cloudiot_device_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1459 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_collection_method_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1448 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_detail_response.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4969 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_devices_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2144 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_email_alert_settings.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1687 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_email_alert_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1472 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_email_auth_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1701 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_email_waitlist.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1516 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_email_waitlist_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1404 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_end_behavior_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1470 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_error_detail.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1393 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_event_types_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1159 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_events_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1820 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_gcode_file.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1369 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_interval_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1359 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_janus_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1404 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_janus_config_type.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1491 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_login_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2186 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_octo_print_backup.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2219 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_octo_print_server.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1699 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_octo_print_server_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2008 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_octo_print_settings.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1822 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_octo_print_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2985 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_octo_printer_profile.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2534 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_octo_printer_profile_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3555 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_octoprint_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1336 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_os_edition.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2763 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_cloudiot_device_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2408 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_email_alert_settings_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2067 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_gcode_file_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2314 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_octo_print_backup_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2427 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_octo_print_server_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2365 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_octo_print_settings_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3338 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_octo_printer_profile_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2657 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_pi_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2074 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_pi_settings_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1827 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_polymorphic_pi_event_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2236 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_public_key_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2666 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_system_info_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2769 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_paginated_webrtc_stream_list.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1618 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_password_change_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1800 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_password_reset_confirm_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1516 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_password_reset_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1581 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_patched_cloudiot_device_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1766 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_patched_email_alert_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1753 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_patched_octo_print_server_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1862 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_patched_octo_print_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2548 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_patched_octo_printer_profile_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1626 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_patched_pi_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1617 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_patched_pi_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1652 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_patched_public_key_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2019 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_patched_system_info_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1532 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_patched_user_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1695 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_patched_webrtc_stream_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2668 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2003 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_boot_command.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1737 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_boot_command_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1428 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_boot_command_type.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1995 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_boot_event.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1729 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_boot_event_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1406 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_boot_event_type.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2056 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_gstreamer_command.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1790 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_gstreamer_command_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1483 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_gstreamer_command_type.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1547 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1750 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_settings.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1563 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_settings_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2156 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_software_update_event.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1892 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_software_update_event_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1518 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_software_update_event_type.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1429 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pi_urls.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1141 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_pis_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      936 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_polymorphic_pi_event.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      979 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_polymorphic_pi_event_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1598 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_print_nanny_api_config.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1536 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_print_nanny_license.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2124 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_public_key.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1728 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_public_key_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1593 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_register_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1628 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_resend_email_verification_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1450 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_rest_auth_detail.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1314 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_sbc_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)      833 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_schema_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1397 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_settings_api.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3816 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_stripe_customer.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     4288 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_stripe_payment_method.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2861 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_stripe_plan.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)    16691 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_stripe_subscription.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     3342 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_stripe_subscription_schedule.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1639 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_stripe_subscription_schedule_status_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1549 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_stripe_subscription_status_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2743 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_system_info.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2353 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_system_info_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1382 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_tax_exempt_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1341 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_token.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1435 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_token_response.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1325 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_type_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1382 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_usage_type_enum.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1531 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_user.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1482 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_user_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1490 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_verify_email_request.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     2779 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_webrtc_stream.py
--rw-rw-r--   0 leigh     (1000) leigh     (1000)     1616 2022-08-04 02:23:27.000000 printnanny-api-client-0.99.8/test/test_webrtc_stream_request.py
+drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 15:39:54.423238 printnanny-api-client-0.99.9/
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      236 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/MANIFEST.in
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      309 2022-08-04 15:39:54.423238 printnanny-api-client-0.99.9/PKG-INFO
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    21653 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/README.md
+drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 15:39:54.407238 printnanny-api-client-0.99.9/docs/
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    61480 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/AccountsApi.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    23027 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/AlertsApi.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4064 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/BillingApi.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      525 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/docs/BillingSummary.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      510 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/docs/CallbackTokenAuthRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1069 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/docs/CloudiotDevice.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      331 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/docs/CloudiotDeviceRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      299 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/docs/CollectionMethodEnum.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      353 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/DetailResponse.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)   158503 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/DevicesApi.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      630 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/EmailAlertSettings.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      473 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/EmailAlertSettingsRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      443 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/EmailAuthRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      399 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/EmailWaitlist.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      325 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/EmailWaitlistRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      294 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/EndBehaviorEnum.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      342 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/ErrorDetail.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      293 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/EventTypesEnum.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    17456 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/EventsApi.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      480 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/GcodeFile.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      291 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/IntervalEnum.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    23031 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/JanusApi.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      294 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/JanusConfigType.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      346 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/LoginRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      560 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/NatsApp.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      572 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/OctoPrintBackup.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      754 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/OctoPrintServer.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      519 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/OctoPrintServerRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      983 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/OctoPrintSettings.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      909 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/OctoPrintSettingsRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1470 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/OctoPrinterProfile.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1313 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/OctoPrinterProfileRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    98403 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/OctoprintApi.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      288 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/OsEdition.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      496 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedCloudiotDeviceList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      508 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedEmailAlertSettingsList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      481 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedGcodeFileList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      499 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedOctoPrintBackupList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      499 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedOctoPrintServerList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      505 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedOctoPrintSettingsList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      508 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedOctoPrinterProfileList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      460 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedPiList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      484 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedPiSettingsList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      508 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedPolymorphicPiEventList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      481 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedPublicKeyList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      484 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedSystemInfoList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      490 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PaginatedWebrtcStreamList.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      368 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PasswordChangeRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      476 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PasswordResetConfirmRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      376 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PasswordResetRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      349 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PatchedCloudiotDeviceRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      480 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PatchedEmailAlertSettingsRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      537 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PatchedOctoPrintServerRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      927 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PatchedOctoPrintSettingsRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1342 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PatchedOctoPrinterProfileRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      688 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PatchedPiRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      542 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PatchedPiSettingsRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      490 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PatchedPublicKeyRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1086 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PatchedSystemInfoRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      417 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PatchedUserRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      512 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PatchedWebrtcStreamRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1384 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/Pi.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      595 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiBootCommand.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      472 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiBootCommandRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      296 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiBootCommandType.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      589 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiBootEvent.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      466 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiBootEventRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      294 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiBootEventType.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      610 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiGstreamerCommand.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      487 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiGstreamerCommandRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      301 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiGstreamerCommandType.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      681 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      598 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiSettings.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      524 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiSettingsRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      647 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiSoftwareUpdateEvent.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      524 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiSoftwareUpdateEventRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      304 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiSoftwareUpdateEventType.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      344 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PiUrls.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    17393 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PisApi.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      624 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PolymorphicPiEvent.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      501 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PolymorphicPiEventRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      390 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PrintNannyApiConfig.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      473 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PrintNannyLicense.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      549 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PublicKey.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      428 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/PublicKeyRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      380 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/RegisterRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      335 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/ResendEmailVerificationRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      331 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/RestAuthDetail.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      286 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/SbcEnum.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4261 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/SchemaApi.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    23079 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/SettingsApi.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3508 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/StripeCustomer.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4004 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/StripePaymentMethod.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2927 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/StripePlan.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6428 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/StripeSubscription.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2719 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/StripeSubscriptionSchedule.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      315 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/StripeSubscriptionScheduleStatusEnum.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      307 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/StripeSubscriptionStatusEnum.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1090 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/SystemInfo.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      969 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/SystemInfoRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      292 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/TaxExemptEnum.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      336 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/Token.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      351 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/TokenResponse.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      287 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/TypeEnum.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      292 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/UsageTypeEnum.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      473 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/User.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      399 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/UserRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      321 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/VerifyEmailRequest.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1142 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/WebrtcStream.md
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      505 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/docs/WebrtcStreamRequest.md
+drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 15:39:54.407238 printnanny-api-client-0.99.9/printnanny_api_client/
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     9746 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/__init__.py
+drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 15:39:54.407238 printnanny-api-client-0.99.9/printnanny_api_client/api/
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      687 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api/__init__.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    93726 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api/accounts_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    32892 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api/alerts_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6245 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api/billing_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)   250523 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api/devices_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    25756 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api/events_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    36093 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api/janus_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)   152594 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api/octoprint_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    25753 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api/pis_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6690 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api/schema_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    32894 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api/settings_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    28079 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/api_client.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    16995 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/configuration.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5118 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/exceptions.py
+drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 15:39:54.415238 printnanny-api-client-0.99.9/printnanny_api_client/models/
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8597 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/__init__.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6476 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/billing_summary.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6712 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/callback_token_auth_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    19294 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/cloudiot_device.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3966 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/cloudiot_device_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3258 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/collection_method_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3822 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/detail_response.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     9277 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/email_alert_settings.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6099 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/email_alert_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4057 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/email_auth_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5617 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/email_waitlist.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4331 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/email_waitlist_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3181 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/end_behavior_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4530 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/error_detail.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3399 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/event_types_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     7939 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/gcode_file.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3202 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/interval_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3169 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/janus_config_type.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5099 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/login_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8871 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/nats_app.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    10344 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/octo_print_backup.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    12215 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/octo_print_server.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     9563 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/octo_print_server_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    11651 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/octo_print_settings.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    10519 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/octo_print_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    27869 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/octo_printer_profile.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    26268 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/octo_printer_profile_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3148 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/os_edition.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5803 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_cloudiot_device_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5895 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_email_alert_settings_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5688 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_gcode_file_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5826 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_octo_print_backup_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5826 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_octo_print_server_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5872 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_octo_print_settings_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5895 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_octo_printer_profile_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5527 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_pi_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5711 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_pi_settings_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5895 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_polymorphic_pi_event_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5688 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_public_key_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5711 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_system_info_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5757 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_webrtc_stream_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6064 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/password_change_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8204 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/password_reset_confirm_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4089 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/password_reset_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3862 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/patched_cloudiot_device_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6211 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/patched_email_alert_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     9579 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/patched_octo_print_server_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    10577 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/patched_octo_print_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    26595 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/patched_octo_printer_profile_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8332 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/patched_pi_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5814 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/patched_pi_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8152 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/patched_public_key_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    16204 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/patched_system_info_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6033 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/patched_user_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8897 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/patched_webrtc_stream_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    15619 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8994 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_command.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6772 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_command_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3192 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_command_type.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8924 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_event.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6726 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_event_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3460 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_event_type.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     9169 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_gstreamer_command.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6887 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_gstreamer_command_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3197 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_gstreamer_command_type.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8136 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     7301 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_settings.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     5854 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    10358 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_software_update_event.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8315 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_software_update_event_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3251 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_software_update_event_type.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4624 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/pi_urls.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    10582 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/polymorphic_pi_event.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8575 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/polymorphic_pi_event_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4805 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/print_nanny_api_config.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4830 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/print_nanny_license.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    10278 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/public_key.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8762 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/public_key_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6271 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/register_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4169 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/resend_email_verification_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3822 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/rest_auth_detail.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3113 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/sbc_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    31541 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_customer.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    31348 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_payment_method.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    25067 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_plan.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    49457 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_subscription.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    23298 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_subscription_schedule.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3388 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_subscription_schedule_status_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3446 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_subscription_status_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    18021 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/system_info.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    17444 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/system_info_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3197 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/tax_exempt_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3918 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/token.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3792 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/token_response.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3843 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/type_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3179 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/usage_type_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     7310 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/user.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     6076 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/user_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4023 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/verify_email_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    20012 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/webrtc_stream.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     8729 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/models/webrtc_stream_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)        0 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/py.typed
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     9909 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/printnanny_api_client/rest.py
+drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 15:39:54.407238 printnanny-api-client-0.99.9/printnanny_api_client.egg-info/
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      309 2022-08-04 15:39:54.000000 printnanny-api-client-0.99.9/printnanny_api_client.egg-info/PKG-INFO
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    13033 2022-08-04 15:39:54.000000 printnanny-api-client-0.99.9/printnanny_api_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)        1 2022-08-04 15:39:54.000000 printnanny-api-client-0.99.9/printnanny_api_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)       66 2022-08-04 15:39:54.000000 printnanny-api-client-0.99.9/printnanny_api_client.egg-info/requires.txt
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)       27 2022-08-04 15:39:54.000000 printnanny-api-client-0.99.9/printnanny_api_client.egg-info/top_level.txt
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)       69 2022-08-04 15:39:54.427238 printnanny-api-client-0.99.9/setup.cfg
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1111 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/setup.py
+drwxrwxr-x   0 leigh     (1000) leigh     (1000)        0 2022-08-04 15:39:54.423238 printnanny-api-client-0.99.9/test/
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2597 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_accounts_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1385 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_alerts_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      857 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_billing_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    23966 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/test/test_billing_summary.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1646 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/test/test_callback_token_auth_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2933 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/test/test_cloudiot_device.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1535 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/test/test_cloudiot_device_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1459 2022-08-04 15:39:52.000000 printnanny-api-client-0.99.9/test/test_collection_method_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1448 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_detail_response.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4969 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_devices_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2144 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_email_alert_settings.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1687 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_email_alert_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1472 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_email_auth_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1701 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_email_waitlist.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1516 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_email_waitlist_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1404 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_end_behavior_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1470 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_error_detail.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1393 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_event_types_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1159 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_events_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1820 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_gcode_file.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1369 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_interval_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1359 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_janus_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1404 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_janus_config_type.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1491 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_login_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1847 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_nats_app.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2186 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_octo_print_backup.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2219 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_octo_print_server.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1699 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_octo_print_server_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2008 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_octo_print_settings.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1822 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_octo_print_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2985 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_octo_printer_profile.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2534 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_octo_printer_profile_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3555 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_octoprint_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1336 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_os_edition.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2763 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_cloudiot_device_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2408 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_email_alert_settings_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2067 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_gcode_file_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2314 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_octo_print_backup_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2427 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_octo_print_server_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2365 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_octo_print_settings_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3338 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_octo_printer_profile_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2657 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_pi_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2074 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_pi_settings_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1827 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_polymorphic_pi_event_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2236 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_public_key_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2666 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_system_info_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2769 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_paginated_webrtc_stream_list.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1618 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_password_change_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1800 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_password_reset_confirm_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1516 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_password_reset_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1581 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_patched_cloudiot_device_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1766 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_patched_email_alert_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1753 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_patched_octo_print_server_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1862 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_patched_octo_print_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2548 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_patched_octo_printer_profile_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1626 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_patched_pi_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1617 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_patched_pi_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1652 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_patched_public_key_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2019 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_patched_system_info_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1532 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_patched_user_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1695 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_patched_webrtc_stream_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2668 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2003 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_boot_command.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1737 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_boot_command_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1428 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_boot_command_type.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1995 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_boot_event.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1729 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_boot_event_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1406 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_boot_event_type.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2056 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_gstreamer_command.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1790 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_gstreamer_command_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1483 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_gstreamer_command_type.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1547 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1750 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_settings.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1563 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_settings_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2156 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_software_update_event.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1892 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_software_update_event_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1518 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_software_update_event_type.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1429 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pi_urls.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1141 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_pis_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      936 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_polymorphic_pi_event.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      979 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_polymorphic_pi_event_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1598 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_print_nanny_api_config.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1603 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_print_nanny_license.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2124 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_public_key.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1728 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_public_key_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1593 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_register_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1628 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_resend_email_verification_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1450 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_rest_auth_detail.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1314 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_sbc_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)      833 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_schema_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1397 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_settings_api.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3816 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_stripe_customer.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     4288 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_stripe_payment_method.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2861 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_stripe_plan.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)    16691 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_stripe_subscription.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     3342 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_stripe_subscription_schedule.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1639 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_stripe_subscription_schedule_status_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1549 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_stripe_subscription_status_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2743 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_system_info.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2353 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_system_info_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1382 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_tax_exempt_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1341 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_token.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1435 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_token_response.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1325 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_type_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1382 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_usage_type_enum.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1531 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_user.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1482 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_user_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1490 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_verify_email_request.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     2779 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_webrtc_stream.py
+-rw-rw-r--   0 leigh     (1000) leigh     (1000)     1616 2022-08-04 15:39:53.000000 printnanny-api-client-0.99.9/test/test_webrtc_stream_request.py
```

### Comparing `printnanny-api-client-0.99.8/README.md` & `printnanny-api-client-0.99.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # printnanny-api-client
 Official API client library for printnanny.ai
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.99.8
-- Package version: 0.99.8
+- API version: 0.99.9
+- Package version: 0.99.9
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://printnanny.ai](https://printnanny.ai)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -211,14 +211,15 @@
  - [EndBehaviorEnum](docs/EndBehaviorEnum.md)
  - [ErrorDetail](docs/ErrorDetail.md)
  - [EventTypesEnum](docs/EventTypesEnum.md)
  - [GcodeFile](docs/GcodeFile.md)
  - [IntervalEnum](docs/IntervalEnum.md)
  - [JanusConfigType](docs/JanusConfigType.md)
  - [LoginRequest](docs/LoginRequest.md)
+ - [NatsApp](docs/NatsApp.md)
  - [OctoPrintBackup](docs/OctoPrintBackup.md)
  - [OctoPrintServer](docs/OctoPrintServer.md)
  - [OctoPrintServerRequest](docs/OctoPrintServerRequest.md)
  - [OctoPrintSettings](docs/OctoPrintSettings.md)
  - [OctoPrintSettingsRequest](docs/OctoPrintSettingsRequest.md)
  - [OctoPrinterProfile](docs/OctoPrinterProfile.md)
  - [OctoPrinterProfileRequest](docs/OctoPrinterProfileRequest.md)
```

### Comparing `printnanny-api-client-0.99.8/docs/AccountsApi.md` & `printnanny-api-client-0.99.9/docs/AccountsApi.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/AlertsApi.md` & `printnanny-api-client-0.99.9/docs/AlertsApi.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/BillingApi.md` & `printnanny-api-client-0.99.9/docs/BillingApi.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/BillingSummary.md` & `printnanny-api-client-0.99.9/docs/BillingSummary.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/CloudiotDevice.md` & `printnanny-api-client-0.99.9/docs/CloudiotDevice.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/DevicesApi.md` & `printnanny-api-client-0.99.9/docs/DevicesApi.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/EmailAlertSettings.md` & `printnanny-api-client-0.99.9/docs/EmailAlertSettings.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/EventsApi.md` & `printnanny-api-client-0.99.9/docs/EventsApi.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/JanusApi.md` & `printnanny-api-client-0.99.9/docs/JanusApi.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/OctoPrintBackup.md` & `printnanny-api-client-0.99.9/docs/OctoPrintBackup.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/OctoPrintServer.md` & `printnanny-api-client-0.99.9/docs/OctoPrintServer.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/OctoPrintServerRequest.md` & `printnanny-api-client-0.99.9/docs/OctoPrintServerRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/OctoPrintSettings.md` & `printnanny-api-client-0.99.9/docs/OctoPrintSettings.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/OctoPrintSettingsRequest.md` & `printnanny-api-client-0.99.9/docs/OctoPrintSettingsRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/OctoPrinterProfile.md` & `printnanny-api-client-0.99.9/docs/OctoPrinterProfile.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/OctoPrinterProfileRequest.md` & `printnanny-api-client-0.99.9/docs/OctoPrinterProfileRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/OctoprintApi.md` & `printnanny-api-client-0.99.9/docs/OctoprintApi.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PatchedOctoPrintServerRequest.md` & `printnanny-api-client-0.99.9/docs/PatchedOctoPrintServerRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PatchedOctoPrintSettingsRequest.md` & `printnanny-api-client-0.99.9/docs/PatchedOctoPrintSettingsRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PatchedOctoPrinterProfileRequest.md` & `printnanny-api-client-0.99.9/docs/PatchedOctoPrinterProfileRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PatchedPiRequest.md` & `printnanny-api-client-0.99.9/docs/PatchedPiRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PatchedPiSettingsRequest.md` & `printnanny-api-client-0.99.9/docs/PatchedPiSettingsRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PatchedSystemInfoRequest.md` & `printnanny-api-client-0.99.9/docs/PatchedSystemInfoRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PatchedWebrtcStreamRequest.md` & `printnanny-api-client-0.99.9/docs/PatchedWebrtcStreamRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/Pi.md` & `printnanny-api-client-0.99.9/docs/Pi.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PiBootCommand.md` & `printnanny-api-client-0.99.9/docs/PiBootCommand.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PiBootEvent.md` & `printnanny-api-client-0.99.9/docs/PiBootEvent.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PiGstreamerCommand.md` & `printnanny-api-client-0.99.9/docs/PiGstreamerCommand.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PiRequest.md` & `printnanny-api-client-0.99.9/docs/PiRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PiSettings.md` & `printnanny-api-client-0.99.9/docs/PiSettings.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PiSettingsRequest.md` & `printnanny-api-client-0.99.9/docs/PiSettingsRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PiSoftwareUpdateEvent.md` & `printnanny-api-client-0.99.9/docs/PiSoftwareUpdateEvent.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PiSoftwareUpdateEventRequest.md` & `printnanny-api-client-0.99.9/docs/PiSoftwareUpdateEventRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PisApi.md` & `printnanny-api-client-0.99.9/docs/PisApi.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PolymorphicPiEvent.md` & `printnanny-api-client-0.99.9/docs/PolymorphicPiEvent.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/PublicKey.md` & `printnanny-api-client-0.99.9/docs/PublicKey.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/SchemaApi.md` & `printnanny-api-client-0.99.9/docs/SchemaApi.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/SettingsApi.md` & `printnanny-api-client-0.99.9/docs/SettingsApi.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/StripeCustomer.md` & `printnanny-api-client-0.99.9/docs/StripeCustomer.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/StripePaymentMethod.md` & `printnanny-api-client-0.99.9/docs/StripePaymentMethod.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/StripePlan.md` & `printnanny-api-client-0.99.9/docs/StripePlan.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/StripeSubscription.md` & `printnanny-api-client-0.99.9/docs/StripeSubscription.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/StripeSubscriptionSchedule.md` & `printnanny-api-client-0.99.9/docs/StripeSubscriptionSchedule.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/SystemInfo.md` & `printnanny-api-client-0.99.9/docs/SystemInfo.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/SystemInfoRequest.md` & `printnanny-api-client-0.99.9/docs/SystemInfoRequest.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/docs/WebrtcStream.md` & `printnanny-api-client-0.99.9/docs/WebrtcStream.md`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/__init__.py` & `printnanny-api-client-0.99.9/printnanny_api_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.99.8"
+__version__ = "0.99.9"
 
 # import apis into sdk package
 from printnanny_api_client.api.accounts_api import AccountsApi
 from printnanny_api_client.api.alerts_api import AlertsApi
 from printnanny_api_client.api.billing_api import BillingApi
 from printnanny_api_client.api.devices_api import DevicesApi
 from printnanny_api_client.api.events_api import EventsApi
@@ -53,14 +53,15 @@
 from printnanny_api_client.models.end_behavior_enum import EndBehaviorEnum
 from printnanny_api_client.models.error_detail import ErrorDetail
 from printnanny_api_client.models.event_types_enum import EventTypesEnum
 from printnanny_api_client.models.gcode_file import GcodeFile
 from printnanny_api_client.models.interval_enum import IntervalEnum
 from printnanny_api_client.models.janus_config_type import JanusConfigType
 from printnanny_api_client.models.login_request import LoginRequest
+from printnanny_api_client.models.nats_app import NatsApp
 from printnanny_api_client.models.octo_print_backup import OctoPrintBackup
 from printnanny_api_client.models.octo_print_server import OctoPrintServer
 from printnanny_api_client.models.octo_print_server_request import OctoPrintServerRequest
 from printnanny_api_client.models.octo_print_settings import OctoPrintSettings
 from printnanny_api_client.models.octo_print_settings_request import OctoPrintSettingsRequest
 from printnanny_api_client.models.octo_printer_profile import OctoPrinterProfile
 from printnanny_api_client.models.octo_printer_profile_request import OctoPrinterProfileRequest
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api/__init__.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api/accounts_api.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api/accounts_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api/alerts_api.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api/alerts_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api/billing_api.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api/billing_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api/devices_api.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api/devices_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api/events_api.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api/events_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api/janus_api.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api/janus_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api/octoprint_api.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api/octoprint_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api/pis_api.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api/pis_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api/schema_api.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api/schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api/settings_api.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api/settings_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/api_client.py` & `printnanny-api-client-0.99.9/printnanny_api_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -76,15 +76,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.99.8/python'
+        self.user_agent = 'OpenAPI-Generator/0.99.9/python'
         self.client_side_validation = configuration.client_side_validation
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.close()
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/configuration.py` & `printnanny-api-client-0.99.9/printnanny_api_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -409,16 +409,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.99.8\n"\
-               "SDK Package Version: 0.99.8".\
+               "Version of the API: 0.99.9\n"\
+               "SDK Package Version: 0.99.9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/exceptions.py` & `printnanny-api-client-0.99.9/printnanny_api_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/__init__.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -29,14 +29,15 @@
 from printnanny_api_client.models.end_behavior_enum import EndBehaviorEnum
 from printnanny_api_client.models.error_detail import ErrorDetail
 from printnanny_api_client.models.event_types_enum import EventTypesEnum
 from printnanny_api_client.models.gcode_file import GcodeFile
 from printnanny_api_client.models.interval_enum import IntervalEnum
 from printnanny_api_client.models.janus_config_type import JanusConfigType
 from printnanny_api_client.models.login_request import LoginRequest
+from printnanny_api_client.models.nats_app import NatsApp
 from printnanny_api_client.models.octo_print_backup import OctoPrintBackup
 from printnanny_api_client.models.octo_print_server import OctoPrintServer
 from printnanny_api_client.models.octo_print_server_request import OctoPrintServerRequest
 from printnanny_api_client.models.octo_print_settings import OctoPrintSettings
 from printnanny_api_client.models.octo_print_settings_request import OctoPrintSettingsRequest
 from printnanny_api_client.models.octo_printer_profile import OctoPrinterProfile
 from printnanny_api_client.models.octo_printer_profile_request import OctoPrinterProfileRequest
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/billing_summary.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/billing_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/callback_token_auth_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/callback_token_auth_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/cloudiot_device.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/cloudiot_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/cloudiot_device_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/cloudiot_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/collection_method_enum.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/collection_method_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/detail_response.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/detail_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/email_alert_settings.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/email_alert_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/email_alert_settings_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/email_alert_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/email_auth_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/email_auth_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/email_waitlist.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/email_waitlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/email_waitlist_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/email_waitlist_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/end_behavior_enum.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/end_behavior_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/error_detail.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/error_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/event_types_enum.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/event_types_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/gcode_file.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/gcode_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/interval_enum.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/interval_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/janus_config_type.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/janus_config_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/login_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/login_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/octo_print_backup.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/octo_print_backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/octo_print_server.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/octo_print_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/octo_print_server_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/octo_print_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/octo_print_settings.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/octo_print_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/octo_print_settings_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/octo_print_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/octo_printer_profile.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/octo_printer_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/octo_printer_profile_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/octo_printer_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/os_edition.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/os_edition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_cloudiot_device_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_cloudiot_device_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_email_alert_settings_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_email_alert_settings_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_gcode_file_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_gcode_file_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_octo_print_backup_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_octo_print_backup_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_octo_print_server_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_octo_print_server_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_octo_print_settings_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_octo_print_settings_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_octo_printer_profile_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_octo_printer_profile_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_pi_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_pi_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_pi_settings_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_pi_settings_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_polymorphic_pi_event_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_polymorphic_pi_event_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_public_key_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_public_key_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_system_info_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_system_info_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/paginated_webrtc_stream_list.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/paginated_webrtc_stream_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/password_change_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/password_change_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/password_reset_confirm_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/password_reset_confirm_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/password_reset_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/password_reset_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/patched_cloudiot_device_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/patched_cloudiot_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/patched_email_alert_settings_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/patched_email_alert_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/patched_octo_print_server_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/patched_octo_print_server_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/patched_octo_print_settings_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/patched_octo_print_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/patched_octo_printer_profile_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/patched_octo_printer_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/patched_pi_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/patched_pi_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/patched_pi_settings_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/patched_pi_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/patched_public_key_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/patched_public_key_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/patched_system_info_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/patched_system_info_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/patched_user_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/patched_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/patched_webrtc_stream_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/patched_webrtc_stream_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_command.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_command_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_command_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_command_type.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_command_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_event.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_event_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_boot_event_type.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_boot_event_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_gstreamer_command.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_gstreamer_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_gstreamer_command_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_gstreamer_command_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_gstreamer_command_type.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_software_update_event_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,28 +18,29 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from printnanny_api_client.configuration import Configuration
 
 
-class PiGstreamerCommandType(object):
+class PiSoftwareUpdateEventType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    START = "Start"
-    STOP = "Stop"
+    STARTED = "Started"
+    SUCCESS = "Success"
+    ERROR = "Error"
 
-    allowable_values = [START, STOP]  # noqa: E501
+    allowable_values = [STARTED, SUCCESS, ERROR]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -47,15 +48,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """PiGstreamerCommandType - a model defined in OpenAPI"""  # noqa: E501
+        """PiSoftwareUpdateEventType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
@@ -95,18 +96,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PiGstreamerCommandType):
+        if not isinstance(other, PiSoftwareUpdateEventType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, PiGstreamerCommandType):
+        if not isinstance(other, PiSoftwareUpdateEventType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_settings.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_settings_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_software_update_event.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_software_update_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_software_update_event_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_software_update_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_software_update_event_type.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_gstreamer_command_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,29 +18,28 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from printnanny_api_client.configuration import Configuration
 
 
-class PiSoftwareUpdateEventType(object):
+class PiGstreamerCommandType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    STARTED = "Started"
-    SUCCESS = "Success"
-    ERROR = "Error"
+    START = "Start"
+    STOP = "Stop"
 
-    allowable_values = [STARTED, SUCCESS, ERROR]  # noqa: E501
+    allowable_values = [START, STOP]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -48,15 +47,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """PiSoftwareUpdateEventType - a model defined in OpenAPI"""  # noqa: E501
+        """PiGstreamerCommandType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
@@ -96,18 +95,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PiSoftwareUpdateEventType):
+        if not isinstance(other, PiGstreamerCommandType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, PiSoftwareUpdateEventType):
+        if not isinstance(other, PiGstreamerCommandType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/pi_urls.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/pi_urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/polymorphic_pi_event.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/polymorphic_pi_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/polymorphic_pi_event_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/polymorphic_pi_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/print_nanny_api_config.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/print_nanny_api_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/print_nanny_license.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/print_nanny_license.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -33,37 +33,62 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'nats_app': 'NatsApp',
         'api': 'PrintNannyApiConfig',
         'pi': 'Pi'
     }
 
     attribute_map = {
+        'nats_app': 'nats_app',
         'api': 'api',
         'pi': 'pi'
     }
 
-    def __init__(self, api=None, pi=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, nats_app=None, api=None, pi=None, local_vars_configuration=None):  # noqa: E501
         """PrintNannyLicense - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._nats_app = None
         self._api = None
         self._pi = None
         self.discriminator = None
 
+        self.nats_app = nats_app
         self.api = api
         self.pi = pi
 
     @property
+    def nats_app(self):
+        """Gets the nats_app of this PrintNannyLicense.  # noqa: E501
+
+
+        :return: The nats_app of this PrintNannyLicense.  # noqa: E501
+        :rtype: NatsApp
+        """
+        return self._nats_app
+
+    @nats_app.setter
+    def nats_app(self, nats_app):
+        """Sets the nats_app of this PrintNannyLicense.
+
+
+        :param nats_app: The nats_app of this PrintNannyLicense.  # noqa: E501
+        :type nats_app: NatsApp
+        """
+
+        self._nats_app = nats_app
+
+    @property
     def api(self):
         """Gets the api of this PrintNannyLicense.  # noqa: E501
 
 
         :return: The api of this PrintNannyLicense.  # noqa: E501
         :rtype: PrintNannyApiConfig
         """
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/public_key.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/public_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/public_key_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/public_key_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/register_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/register_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/resend_email_verification_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/resend_email_verification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/rest_auth_detail.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/rest_auth_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/sbc_enum.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/sbc_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_customer.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_customer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_payment_method.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_payment_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_plan.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_subscription.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_subscription_schedule.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_subscription_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_subscription_schedule_status_enum.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_subscription_schedule_status_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/stripe_subscription_status_enum.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/stripe_subscription_status_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/system_info.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/system_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/system_info_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/system_info_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/tax_exempt_enum.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/tax_exempt_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/token.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/token_response.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/token_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/type_enum.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/type_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/usage_type_enum.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/usage_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/user.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/user_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/verify_email_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/verify_email_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/webrtc_stream.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/webrtc_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/models/webrtc_stream_request.py` & `printnanny-api-client-0.99.9/printnanny_api_client/models/webrtc_stream_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client/rest.py` & `printnanny-api-client-0.99.9/printnanny_api_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

### Comparing `printnanny-api-client-0.99.8/printnanny_api_client.egg-info/SOURCES.txt` & `printnanny-api-client-0.99.9/printnanny_api_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 docs/EventTypesEnum.md
 docs/EventsApi.md
 docs/GcodeFile.md
 docs/IntervalEnum.md
 docs/JanusApi.md
 docs/JanusConfigType.md
 docs/LoginRequest.md
+docs/NatsApp.md
 docs/OctoPrintBackup.md
 docs/OctoPrintServer.md
 docs/OctoPrintServerRequest.md
 docs/OctoPrintSettings.md
 docs/OctoPrintSettingsRequest.md
 docs/OctoPrinterProfile.md
 docs/OctoPrinterProfileRequest.md
@@ -148,14 +149,15 @@
 printnanny_api_client/models/end_behavior_enum.py
 printnanny_api_client/models/error_detail.py
 printnanny_api_client/models/event_types_enum.py
 printnanny_api_client/models/gcode_file.py
 printnanny_api_client/models/interval_enum.py
 printnanny_api_client/models/janus_config_type.py
 printnanny_api_client/models/login_request.py
+printnanny_api_client/models/nats_app.py
 printnanny_api_client/models/octo_print_backup.py
 printnanny_api_client/models/octo_print_server.py
 printnanny_api_client/models/octo_print_server_request.py
 printnanny_api_client/models/octo_print_settings.py
 printnanny_api_client/models/octo_print_settings_request.py
 printnanny_api_client/models/octo_printer_profile.py
 printnanny_api_client/models/octo_printer_profile_request.py
@@ -253,14 +255,15 @@
 test/test_event_types_enum.py
 test/test_events_api.py
 test/test_gcode_file.py
 test/test_interval_enum.py
 test/test_janus_api.py
 test/test_janus_config_type.py
 test/test_login_request.py
+test/test_nats_app.py
 test/test_octo_print_backup.py
 test/test_octo_print_server.py
 test/test_octo_print_server_request.py
 test/test_octo_print_settings.py
 test/test_octo_print_settings_request.py
 test/test_octo_printer_profile.py
 test/test_octo_printer_profile_request.py
```

### Comparing `printnanny-api-client-0.99.8/setup.py` & `printnanny-api-client-0.99.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_namespace_packages  # noqa: H301
 
 NAME = "printnanny-api-client"
-VERSION = "0.99.8"
+VERSION = "0.99.9"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `printnanny-api-client-0.99.8/test/test_accounts_api.py` & `printnanny-api-client-0.99.9/test/test_accounts_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_alerts_api.py` & `printnanny-api-client-0.99.9/test/test_alerts_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_billing_api.py` & `printnanny-api-client-0.99.9/test/test_billing_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_billing_summary.py` & `printnanny-api-client-0.99.9/test/test_billing_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_callback_token_auth_request.py` & `printnanny-api-client-0.99.9/test/test_callback_token_auth_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_cloudiot_device.py` & `printnanny-api-client-0.99.9/test/test_cloudiot_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_cloudiot_device_request.py` & `printnanny-api-client-0.99.9/test/test_cloudiot_device_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_collection_method_enum.py` & `printnanny-api-client-0.99.9/test/test_collection_method_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_detail_response.py` & `printnanny-api-client-0.99.9/test/test_error_detail.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import printnanny_api_client
-from printnanny_api_client.models.detail_response import DetailResponse  # noqa: E501
+from printnanny_api_client.models.error_detail import ErrorDetail  # noqa: E501
 from printnanny_api_client.rest import ApiException
 
-class TestDetailResponse(unittest.TestCase):
-    """DetailResponse unit test stubs"""
+class TestErrorDetail(unittest.TestCase):
+    """ErrorDetail unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test DetailResponse
+        """Test ErrorDetail
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = printnanny_api_client.models.detail_response.DetailResponse()  # noqa: E501
+        # model = printnanny_api_client.models.error_detail.ErrorDetail()  # noqa: E501
         if include_optional :
-            return DetailResponse(
-                detail = ''
+            return ErrorDetail(
+                detail = '', 
+                code = ''
             )
         else :
-            return DetailResponse(
+            return ErrorDetail(
                 detail = '',
+                code = '',
         )
 
-    def testDetailResponse(self):
-        """Test DetailResponse"""
+    def testErrorDetail(self):
+        """Test ErrorDetail"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `printnanny-api-client-0.99.8/test/test_devices_api.py` & `printnanny-api-client-0.99.9/test/test_devices_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_email_alert_settings.py` & `printnanny-api-client-0.99.9/test/test_email_alert_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_email_alert_settings_request.py` & `printnanny-api-client-0.99.9/test/test_email_alert_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_email_auth_request.py` & `printnanny-api-client-0.99.9/test/test_email_auth_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_email_waitlist.py` & `printnanny-api-client-0.99.9/test/test_email_waitlist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_email_waitlist_request.py` & `printnanny-api-client-0.99.9/test/test_email_waitlist_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_end_behavior_enum.py` & `printnanny-api-client-0.99.9/test/test_end_behavior_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_error_detail.py` & `printnanny-api-client-0.99.9/test/test_detail_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import printnanny_api_client
-from printnanny_api_client.models.error_detail import ErrorDetail  # noqa: E501
+from printnanny_api_client.models.detail_response import DetailResponse  # noqa: E501
 from printnanny_api_client.rest import ApiException
 
-class TestErrorDetail(unittest.TestCase):
-    """ErrorDetail unit test stubs"""
+class TestDetailResponse(unittest.TestCase):
+    """DetailResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ErrorDetail
+        """Test DetailResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = printnanny_api_client.models.error_detail.ErrorDetail()  # noqa: E501
+        # model = printnanny_api_client.models.detail_response.DetailResponse()  # noqa: E501
         if include_optional :
-            return ErrorDetail(
-                detail = '', 
-                code = ''
+            return DetailResponse(
+                detail = ''
             )
         else :
-            return ErrorDetail(
+            return DetailResponse(
                 detail = '',
-                code = '',
         )
 
-    def testErrorDetail(self):
-        """Test ErrorDetail"""
+    def testDetailResponse(self):
+        """Test DetailResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `printnanny-api-client-0.99.8/test/test_event_types_enum.py` & `printnanny-api-client-0.99.9/test/test_event_types_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_events_api.py` & `printnanny-api-client-0.99.9/test/test_events_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_gcode_file.py` & `printnanny-api-client-0.99.9/test/test_gcode_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_interval_enum.py` & `printnanny-api-client-0.99.9/test/test_interval_enum.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_janus_api.py` & `printnanny-api-client-0.99.9/test/test_janus_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_janus_config_type.py` & `printnanny-api-client-0.99.9/test/test_janus_config_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_login_request.py` & `printnanny-api-client-0.99.9/test/test_login_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_octo_print_backup.py` & `printnanny-api-client-0.99.9/test/test_octo_print_backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_octo_print_server.py` & `printnanny-api-client-0.99.9/test/test_octo_print_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_octo_print_server_request.py` & `printnanny-api-client-0.99.9/test/test_octo_print_server_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_octo_print_settings.py` & `printnanny-api-client-0.99.9/test/test_octo_print_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_octo_print_settings_request.py` & `printnanny-api-client-0.99.9/test/test_octo_print_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_octo_printer_profile.py` & `printnanny-api-client-0.99.9/test/test_octo_printer_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_octo_printer_profile_request.py` & `printnanny-api-client-0.99.9/test/test_octo_printer_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_octoprint_api.py` & `printnanny-api-client-0.99.9/test/test_octoprint_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_os_edition.py` & `printnanny-api-client-0.99.9/test/test_os_edition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_cloudiot_device_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_cloudiot_device_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_email_alert_settings_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_email_alert_settings_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_gcode_file_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_gcode_file_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_octo_print_backup_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_octo_print_backup_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_octo_print_server_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_octo_print_server_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_octo_print_settings_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_octo_print_settings_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_octo_printer_profile_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_octo_printer_profile_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_pi_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_pi_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_pi_settings_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_pi_settings_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_polymorphic_pi_event_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_polymorphic_pi_event_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_public_key_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_public_key_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_system_info_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_system_info_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_paginated_webrtc_stream_list.py` & `printnanny-api-client-0.99.9/test/test_paginated_webrtc_stream_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_password_change_request.py` & `printnanny-api-client-0.99.9/test/test_password_change_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_password_reset_confirm_request.py` & `printnanny-api-client-0.99.9/test/test_password_reset_confirm_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_password_reset_request.py` & `printnanny-api-client-0.99.9/test/test_password_reset_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_patched_cloudiot_device_request.py` & `printnanny-api-client-0.99.9/test/test_patched_cloudiot_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_patched_email_alert_settings_request.py` & `printnanny-api-client-0.99.9/test/test_patched_email_alert_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_patched_octo_print_server_request.py` & `printnanny-api-client-0.99.9/test/test_patched_octo_print_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_patched_octo_print_settings_request.py` & `printnanny-api-client-0.99.9/test/test_patched_octo_print_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_patched_octo_printer_profile_request.py` & `printnanny-api-client-0.99.9/test/test_patched_octo_printer_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_patched_pi_request.py` & `printnanny-api-client-0.99.9/test/test_patched_pi_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_patched_pi_settings_request.py` & `printnanny-api-client-0.99.9/test/test_patched_pi_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_patched_public_key_request.py` & `printnanny-api-client-0.99.9/test/test_patched_public_key_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_patched_system_info_request.py` & `printnanny-api-client-0.99.9/test/test_patched_system_info_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_patched_user_request.py` & `printnanny-api-client-0.99.9/test/test_patched_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_patched_webrtc_stream_request.py` & `printnanny-api-client-0.99.9/test/test_patched_webrtc_stream_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi.py` & `printnanny-api-client-0.99.9/test/test_pi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_boot_command.py` & `printnanny-api-client-0.99.9/test/test_pi_boot_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_boot_command_request.py` & `printnanny-api-client-0.99.9/test/test_pi_boot_command_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_boot_command_type.py` & `printnanny-api-client-0.99.9/test/test_pi_boot_command_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_boot_event.py` & `printnanny-api-client-0.99.9/test/test_pi_boot_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_boot_event_request.py` & `printnanny-api-client-0.99.9/test/test_pi_boot_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_boot_event_type.py` & `printnanny-api-client-0.99.9/test/test_pi_boot_event_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_gstreamer_command.py` & `printnanny-api-client-0.99.9/test/test_pi_gstreamer_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_gstreamer_command_request.py` & `printnanny-api-client-0.99.9/test/test_pi_gstreamer_command_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_gstreamer_command_type.py` & `printnanny-api-client-0.99.9/test/test_pi_gstreamer_command_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_request.py` & `printnanny-api-client-0.99.9/test/test_pi_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_settings.py` & `printnanny-api-client-0.99.9/test/test_pi_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_settings_request.py` & `printnanny-api-client-0.99.9/test/test_pi_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_software_update_event.py` & `printnanny-api-client-0.99.9/test/test_pi_software_update_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_software_update_event_request.py` & `printnanny-api-client-0.99.9/test/test_pi_software_update_event_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_software_update_event_type.py` & `printnanny-api-client-0.99.9/test/test_pi_software_update_event_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pi_urls.py` & `printnanny-api-client-0.99.9/test/test_pi_urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_pis_api.py` & `printnanny-api-client-0.99.9/test/test_pis_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_polymorphic_pi_event.py` & `printnanny-api-client-0.99.9/test/test_polymorphic_pi_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_polymorphic_pi_event_request.py` & `printnanny-api-client-0.99.9/test/test_polymorphic_pi_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_print_nanny_api_config.py` & `printnanny-api-client-0.99.9/test/test_print_nanny_api_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_print_nanny_license.py` & `printnanny-api-client-0.99.9/test/test_print_nanny_license.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -33,19 +33,21 @@
         """Test PrintNannyLicense
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = printnanny_api_client.models.print_nanny_license.PrintNannyLicense()  # noqa: E501
         if include_optional :
             return PrintNannyLicense(
+                nats_app = None, 
                 api = None, 
                 pi = None
             )
         else :
             return PrintNannyLicense(
+                nats_app = None,
                 api = None,
                 pi = None,
         )
 
     def testPrintNannyLicense(self):
         """Test PrintNannyLicense"""
         inst_req_only = self.make_instance(include_optional=False)
```

### Comparing `printnanny-api-client-0.99.8/test/test_public_key.py` & `printnanny-api-client-0.99.9/test/test_public_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_public_key_request.py` & `printnanny-api-client-0.99.9/test/test_public_key_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_register_request.py` & `printnanny-api-client-0.99.9/test/test_register_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_resend_email_verification_request.py` & `printnanny-api-client-0.99.9/test/test_resend_email_verification_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_rest_auth_detail.py` & `printnanny-api-client-0.99.9/test/test_rest_auth_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_sbc_enum.py` & `printnanny-api-client-0.99.9/test/test_sbc_enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_schema_api.py` & `printnanny-api-client-0.99.9/test/test_schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_settings_api.py` & `printnanny-api-client-0.99.9/test/test_settings_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_stripe_customer.py` & `printnanny-api-client-0.99.9/test/test_stripe_customer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_stripe_payment_method.py` & `printnanny-api-client-0.99.9/test/test_stripe_payment_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_stripe_plan.py` & `printnanny-api-client-0.99.9/test/test_stripe_plan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_stripe_subscription.py` & `printnanny-api-client-0.99.9/test/test_stripe_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_stripe_subscription_schedule.py` & `printnanny-api-client-0.99.9/test/test_stripe_subscription_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_stripe_subscription_schedule_status_enum.py` & `printnanny-api-client-0.99.9/test/test_stripe_subscription_schedule_status_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_stripe_subscription_status_enum.py` & `printnanny-api-client-0.99.9/test/test_stripe_subscription_status_enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_system_info.py` & `printnanny-api-client-0.99.9/test/test_system_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_system_info_request.py` & `printnanny-api-client-0.99.9/test/test_system_info_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_tax_exempt_enum.py` & `printnanny-api-client-0.99.9/test/test_tax_exempt_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_token.py` & `printnanny-api-client-0.99.9/test/test_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_token_response.py` & `printnanny-api-client-0.99.9/test/test_token_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_type_enum.py` & `printnanny-api-client-0.99.9/test/test_type_enum.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_usage_type_enum.py` & `printnanny-api-client-0.99.9/test/test_usage_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_user.py` & `printnanny-api-client-0.99.9/test/test_user.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_user_request.py` & `printnanny-api-client-0.99.9/test/test_user_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_verify_email_request.py` & `printnanny-api-client-0.99.9/test/test_verify_email_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_webrtc_stream.py` & `printnanny-api-client-0.99.9/test/test_webrtc_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `printnanny-api-client-0.99.8/test/test_webrtc_stream_request.py` & `printnanny-api-client-0.99.9/test/test_webrtc_stream_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     printnanny-api-client
 
     Official API client library for printnanny.ai  # noqa: E501
 
-    The version of the OpenAPI document: 0.99.8
+    The version of the OpenAPI document: 0.99.9
     Contact: leigh@printnanny.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

