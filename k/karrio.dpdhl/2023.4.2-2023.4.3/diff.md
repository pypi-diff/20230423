# Comparing `tmp/karrio.dpdhl-2023.4.2-py3-none-any.whl.zip` & `tmp/karrio.dpdhl-2023.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 14429 bytes, number of entries: 16
--rw-rw-r--  2.0 unx      558 b- defN 23-Apr-20 21:26 karrio/mappers/dpdhl/__init__.py
--rw-rw-r--  2.0 unx     2030 b- defN 23-Apr-20 21:26 karrio/mappers/dpdhl/mapper.py
--rw-rw-r--  2.0 unx     2431 b- defN 23-Apr-22 03:54 karrio/mappers/dpdhl/proxy.py
--rw-rw-r--  2.0 unx     1021 b- defN 23-Apr-20 21:26 karrio/mappers/dpdhl/settings.py
+Zip file size: 14537 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx      558 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/__init__.py
+-rw-rw-r--  2.0 unx     2030 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/mapper.py
+-rw-rw-r--  2.0 unx     2431 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/proxy.py
+-rw-rw-r--  2.0 unx     1021 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/settings.py
 -rw-rw-r--  2.0 unx      313 b- defN 22-Nov-15 19:21 karrio/providers/dpdhl/__init__.py
--rw-rw-r--  2.0 unx     3115 b- defN 23-Mar-29 20:04 karrio/providers/dpdhl/error.py
--rw-rw-r--  2.0 unx     3657 b- defN 23-Apr-20 21:26 karrio/providers/dpdhl/tracking.py
--rw-rw-r--  2.0 unx     7670 b- defN 23-Apr-20 21:26 karrio/providers/dpdhl/units.py
--rw-rw-r--  2.0 unx     1684 b- defN 23-Apr-20 21:26 karrio/providers/dpdhl/utils.py
+-rw-rw-r--  2.0 unx     4884 b- defN 23-Apr-23 05:01 karrio/providers/dpdhl/error.py
+-rw-rw-r--  2.0 unx     3657 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/tracking.py
+-rw-rw-r--  2.0 unx     7670 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/units.py
+-rw-rw-r--  2.0 unx     1684 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/utils.py
 -rw-rw-r--  2.0 unx      226 b- defN 22-Nov-15 19:21 karrio/providers/dpdhl/shipment/__init__.py
--rw-rw-r--  2.0 unx     2425 b- defN 23-Apr-20 21:26 karrio/providers/dpdhl/shipment/cancel.py
--rw-rw-r--  2.0 unx    19559 b- defN 23-Apr-20 21:26 karrio/providers/dpdhl/shipment/create.py
--rw-rw-r--  2.0 unx      994 b- defN 23-Apr-22 03:55 karrio.dpdhl-2023.4.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-22 03:55 karrio.dpdhl-2023.4.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-22 03:55 karrio.dpdhl-2023.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1419 b- defN 23-Apr-22 03:55 karrio.dpdhl-2023.4.2.dist-info/RECORD
-16 files, 47201 bytes uncompressed, 12053 bytes compressed:  74.5%
+-rw-rw-r--  2.0 unx     2425 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/shipment/cancel.py
+-rw-rw-r--  2.0 unx    19559 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/shipment/create.py
+-rw-rw-r--  2.0 unx      994 b- defN 23-Apr-23 05:37 karrio.dpdhl-2023.4.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-23 05:37 karrio.dpdhl-2023.4.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-23 05:37 karrio.dpdhl-2023.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1419 b- defN 23-Apr-23 05:37 karrio.dpdhl-2023.4.3.dist-info/RECORD
+16 files, 48970 bytes uncompressed, 12161 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: karrio/providers/dpdhl/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/dpdhl/shipment/create.py
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.2.dist-info/METADATA
+Filename: karrio.dpdhl-2023.4.3.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.2.dist-info/WHEEL
+Filename: karrio.dpdhl-2023.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.2.dist-info/top_level.txt
+Filename: karrio.dpdhl-2023.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.2.dist-info/RECORD
+Filename: karrio.dpdhl-2023.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/providers/dpdhl/error.py

```diff
@@ -54,34 +54,75 @@
         models.Message(
             carrier_id=settings.carrier_id,
             carrier_name=settings.carrier_name,
             code=error.statusCode,
             message=error.statusText,
             details={
                 **(
-                    {"message": lib.join(*error.statusMessage, join=" ")}
-                    if any(error.statusMessage)
+                    lib.failsafe(
+                        lambda: lib.to_dict(
+                            {
+                                "message": lib.join(
+                                    *[
+                                        _
+                                        for _ in error.statusMessage
+                                        if isinstance(_, str)
+                                    ],
+                                    join=" ",
+                                )
+                            }
+                        )
+                    )
+                    or {}
+                    if any(error.statusMessage or [])
                     else {}
                 ),
                 **(
-                    {
-                        "error": lib.join(
-                            *[
-                                f"{_.statusElement}: {_.statusMessage}"
-                                for _ in error.errorMessage
-                            ],
-                            join=" ",
+                    lib.failsafe(
+                        lambda: lib.to_dict(
+                            {
+                                "error": lib.join(
+                                    *[
+                                        f"{_.statusElement}: {_.statusMessage}"
+                                        for _ in error.errorMessage
+                                    ],
+                                    join=" ",
+                                )
+                            }
                         )
-                    }
-                    if any(error.errorMessage or "")
+                    )
+                    or {}
+                    if any(error.errorMessage or [])
                     else {}
                 ),
                 **(
-                    {"warning": error.warningMessage}
-                    if any(error.warningMessage or "")
+                    lib.failsafe(
+                        lambda: lib.to_dict(
+                            {
+                                "warning": lib.join(
+                                    *(
+                                        [
+                                            _
+                                            for _ in error.warningMessage
+                                            if isinstance(_, str)
+                                        ]
+                                        if isinstance(error.warningMessage, list)
+                                        else (
+                                            [error.warningMessage]
+                                            if isinstance(error.warningMessage, str)
+                                            else []
+                                        )
+                                    ),
+                                    join=" ",
+                                )
+                            }
+                        )
+                    )
+                    or {}
+                    if any(error.warningMessage or [])
                     else {}
                 ),
                 **kwargs,
             },
         )
         for error in errors
     ]
```

## Comparing `karrio.dpdhl-2023.4.2.dist-info/METADATA` & `karrio.dpdhl-2023.4.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dpdhl
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: Karrio - Deutsche Post DHL Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.dpdhl-2023.4.2.dist-info/RECORD` & `karrio.dpdhl-2023.4.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 karrio/mappers/dpdhl/__init__.py,sha256=hI9K0SVajo90niTvmU5BP9iV2QoOFh8tEbtZfVRax_c,558
 karrio/mappers/dpdhl/mapper.py,sha256=PX1mAMSFl8JmtAQ-SaKr8xDrV0eybOXzNLJbrUGKLfM,2030
 karrio/mappers/dpdhl/proxy.py,sha256=29jmjAngUb4FkLHu3bTB4leP7VxDROBb78-s8aAj4nk,2431
 karrio/mappers/dpdhl/settings.py,sha256=nRq7QoFa8Amrg1glJy_UmZ9fQUxuseC8KNKPltbifm0,1021
 karrio/providers/dpdhl/__init__.py,sha256=XtaZQrNssm_oho6v6SAYEH3cViuOZ3VFAPhHgW6f-yw,313
-karrio/providers/dpdhl/error.py,sha256=VoSZ2pyx3nUudmqX3L0nIMQ2yOVlvfr_GJ8DrlczDj4,3115
+karrio/providers/dpdhl/error.py,sha256=IKFlWE1FbfeNf6TjeB3L_lraLX716XpoDKCe87kgcDc,4884
 karrio/providers/dpdhl/tracking.py,sha256=Qn2luGRnyIlJkaa2JSRjlawLVq-jMnAkfFGRcJFugqc,3657
 karrio/providers/dpdhl/units.py,sha256=DDQX6MIFiYqMXl6exNkXfRbolbRD2czyMqeAcvMSk1w,7670
 karrio/providers/dpdhl/utils.py,sha256=Hdf1-fC0uK3SlNJlVb5ZlHshn2nC6hH61wO-EFvvCws,1684
 karrio/providers/dpdhl/shipment/__init__.py,sha256=5tF7dih8kTSVa5pw4UXU8_byCMnuvtsJIz_h7VAOOyY,226
 karrio/providers/dpdhl/shipment/cancel.py,sha256=1Z_h5EUUNLS7LAiLLU04dkEPufmXSJGavvn543FGxQE,2425
 karrio/providers/dpdhl/shipment/create.py,sha256=AKmTE_tcKX3n7wStuyFZGJXU5H8J40WgqZqLVSV96gg,19559
-karrio.dpdhl-2023.4.2.dist-info/METADATA,sha256=RBI_kHxhQ56ZHSH8P7fayBqvFrwKHbyJBbOFv0Q6H-4,994
-karrio.dpdhl-2023.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.dpdhl-2023.4.2.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.dpdhl-2023.4.2.dist-info/RECORD,,
+karrio.dpdhl-2023.4.3.dist-info/METADATA,sha256=5SrdVdSxeyoi-ghiVWx7BuWSTqHNCuo7Kfer8NpDCWI,994
+karrio.dpdhl-2023.4.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.dpdhl-2023.4.3.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.dpdhl-2023.4.3.dist-info/RECORD,,
```

