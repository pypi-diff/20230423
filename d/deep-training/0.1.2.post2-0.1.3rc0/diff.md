# Comparing `tmp/deep_training-0.1.2.post2-py3-none-any.whl.zip` & `tmp/deep_training-0.1.3rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 244738 bytes, number of entries: 145
+Zip file size: 267297 bytes, number of entries: 155
 -rw-rw-rw-  2.0 fat       47 b- defN 23-Mar-22 07:43 deep_training/__init__.py
--rw-rw-rw-  2.0 fat      903 b- defN 23-Apr-20 02:26 deep_training/setup.py
+-rw-rw-rw-  2.0 fat      900 b- defN 23-Apr-23 01:18 deep_training/setup.py
 -rw-rw-rw-  2.0 fat       55 b- defN 22-Dec-09 05:30 deep_training/cv/__init__.py
 -rw-rw-rw-  2.0 fat      195 b- defN 23-Jan-29 01:07 deep_training/data_helper/__init__.py
 -rw-rw-rw-  2.0 fat    29088 b- defN 23-Apr-06 04:11 deep_training/data_helper/data_helper.py
 -rw-rw-rw-  2.0 fat     4926 b- defN 23-Feb-17 02:41 deep_training/data_helper/data_module.py
 -rw-rw-rw-  2.0 fat     1383 b- defN 23-Jan-29 01:07 deep_training/data_helper/data_writer.py
 -rw-rw-rw-  2.0 fat    12557 b- defN 23-Apr-19 09:13 deep_training/data_helper/training_args.py
 -rw-rw-rw-  2.0 fat       70 b- defN 22-Dec-13 03:17 deep_training/nlp/__init__.py
@@ -109,14 +109,24 @@
 -rw-rw-rw-  2.0 fat    13576 b- defN 23-Apr-12 08:35 deep_training/nlp/models/lora/v1/lora_wrapper.py
 -rw-rw-rw-  2.0 fat      206 b- defN 23-Apr-11 01:58 deep_training/nlp/models/lora/v2/__init__.py
 -rw-rw-rw-  2.0 fat    13112 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/v2/adalora_model.py
 -rw-rw-rw-  2.0 fat    11281 b- defN 23-Apr-11 06:27 deep_training/nlp/models/lora/v2/configuration.py
 -rw-rw-rw-  2.0 fat    11745 b- defN 23-Apr-18 01:24 deep_training/nlp/models/lora/v2/lora_model.py
 -rw-rw-rw-  2.0 fat    10265 b- defN 23-Apr-11 01:58 deep_training/nlp/models/lora/v2/lora_wrapper.py
 -rw-rw-rw-  2.0 fat     4889 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/v2/save_and_load.py
+-rw-rw-rw-  2.0 fat      467 b- defN 23-Apr-21 04:29 deep_training/nlp/models/moss/__init__.py
+-rw-rw-rw-  2.0 fat     5097 b- defN 23-Apr-23 01:11 deep_training/nlp/models/moss/configuration_moss.py
+-rw-rw-rw-  2.0 fat     6735 b- defN 23-Apr-23 01:05 deep_training/nlp/models/moss/custom_autotune.py
+-rw-rw-rw-  2.0 fat    30926 b- defN 23-Apr-23 01:04 deep_training/nlp/models/moss/modeling_moss.py
+-rw-rw-rw-  2.0 fat    18866 b- defN 23-Apr-23 01:02 deep_training/nlp/models/moss/quantization.py
+-rw-rw-rw-  2.0 fat    14782 b- defN 23-Apr-21 04:15 deep_training/nlp/models/moss/tokenization_moss.py
+-rw-rw-rw-  2.0 fat       55 b- defN 23-Apr-20 03:02 deep_training/nlp/models/rlhf/__init__.py
+-rw-rw-rw-  2.0 fat       55 b- defN 23-Apr-20 03:02 deep_training/nlp/models/rlhf/ppo/__init__.py
+-rw-rw-rw-  2.0 fat      212 b- defN 23-Apr-20 09:24 deep_training/nlp/models/rlhf/ppo/configuration.py
+-rw-rw-rw-  2.0 fat       55 b- defN 23-Apr-20 03:05 deep_training/nlp/models/rlhf/ppo/ppo.py
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Nov-22 08:00 deep_training/nlp/models/splinker/__init__.py
 -rw-rw-rw-  2.0 fat     2851 b- defN 22-Dec-22 08:14 deep_training/nlp/models/splinker/splinker.py
 -rw-rw-rw-  2.0 fat    14478 b- defN 23-Feb-11 09:07 deep_training/nlp/models/t5decoder/__init__.py
 -rw-rw-rw-  2.0 fat     6646 b- defN 23-Feb-09 00:28 deep_training/nlp/models/t5encoder/__init__.py
 -rw-rw-rw-  2.0 fat       56 b- defN 22-Dec-14 08:02 deep_training/nlp/optimizer/__init__.py
 -rw-rw-rw-  2.0 fat     5225 b- defN 23-Mar-08 00:14 deep_training/nlp/optimizer/lamb.py
 -rw-rw-rw-  2.0 fat       99 b- defN 23-Mar-02 05:27 deep_training/nlp/optimizer/lion/__init__.py
@@ -136,12 +146,12 @@
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:25 deep_training/tfnlp/scheduler/__init__.py
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:26 deep_training/tfnlp/utils/__init__.py
 -rw-rw-rw-  2.0 fat       55 b- defN 23-Mar-07 01:20 deep_training/utils/__init__.py
 -rw-rw-rw-  2.0 fat     1941 b- defN 23-Mar-07 01:20 deep_training/utils/distributed.py
 -rw-rw-rw-  2.0 fat     1724 b- defN 23-Mar-07 01:22 deep_training/utils/func.py
 -rw-rw-rw-  2.0 fat     5117 b- defN 23-Feb-21 09:01 deep_training/utils/maskedlm.py
 -rw-rw-rw-  2.0 fat     7469 b- defN 23-Mar-20 00:27 deep_training/utils/trainer.py
--rw-rw-rw-  2.0 fat      629 b- defN 23-Apr-20 02:27 deep_training-0.1.2.post2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 02:27 deep_training-0.1.2.post2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-20 02:27 deep_training-0.1.2.post2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    14010 b- defN 23-Apr-20 02:27 deep_training-0.1.2.post2.dist-info/RECORD
-145 files, 834705 bytes uncompressed, 222026 bytes compressed:  73.4%
+-rw-rw-rw-  2.0 fat      626 b- defN 23-Apr-23 01:18 deep_training-0.1.3rc0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-23 01:18 deep_training-0.1.3rc0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-23 01:18 deep_training-0.1.3rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    15020 b- defN 23-Apr-23 01:18 deep_training-0.1.3rc0.dist-info/RECORD
+155 files, 912959 bytes uncompressed, 242935 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -336,14 +336,44 @@
 
 Filename: deep_training/nlp/models/lora/v2/lora_wrapper.py
 Comment: 
 
 Filename: deep_training/nlp/models/lora/v2/save_and_load.py
 Comment: 
 
+Filename: deep_training/nlp/models/moss/__init__.py
+Comment: 
+
+Filename: deep_training/nlp/models/moss/configuration_moss.py
+Comment: 
+
+Filename: deep_training/nlp/models/moss/custom_autotune.py
+Comment: 
+
+Filename: deep_training/nlp/models/moss/modeling_moss.py
+Comment: 
+
+Filename: deep_training/nlp/models/moss/quantization.py
+Comment: 
+
+Filename: deep_training/nlp/models/moss/tokenization_moss.py
+Comment: 
+
+Filename: deep_training/nlp/models/rlhf/__init__.py
+Comment: 
+
+Filename: deep_training/nlp/models/rlhf/ppo/__init__.py
+Comment: 
+
+Filename: deep_training/nlp/models/rlhf/ppo/configuration.py
+Comment: 
+
+Filename: deep_training/nlp/models/rlhf/ppo/ppo.py
+Comment: 
+
 Filename: deep_training/nlp/models/splinker/__init__.py
 Comment: 
 
 Filename: deep_training/nlp/models/splinker/splinker.py
 Comment: 
 
 Filename: deep_training/nlp/models/t5decoder/__init__.py
@@ -417,20 +447,20 @@
 
 Filename: deep_training/utils/maskedlm.py
 Comment: 
 
 Filename: deep_training/utils/trainer.py
 Comment: 
 
-Filename: deep_training-0.1.2.post2.dist-info/METADATA
+Filename: deep_training-0.1.3rc0.dist-info/METADATA
 Comment: 
 
-Filename: deep_training-0.1.2.post2.dist-info/WHEEL
+Filename: deep_training-0.1.3rc0.dist-info/WHEEL
 Comment: 
 
-Filename: deep_training-0.1.2.post2.dist-info/top_level.txt
+Filename: deep_training-0.1.3rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: deep_training-0.1.2.post2.dist-info/RECORD
+Filename: deep_training-0.1.3rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deep_training/setup.py

```diff
@@ -1,15 +1,15 @@
 #! -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 ignore = ['test','tests']
 setup(
     name='deep_training',
-    version='0.1.2@post2',
+    version='0.1.3rc0',
     description='an easy training architecture',
     long_description='torch_training: https://github.com/ssbuild/deep_training.git',
     license='Apache License 2.0',
     url='https://github.com/ssbuild/deep_training',
     author='ssbuild',
     author_email='9727464@qq.com',
     install_requires=['pytorch-lightning>=2',
```

## Comparing `deep_training-0.1.2.post2.dist-info/METADATA` & `deep_training-0.1.3rc0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-training
-Version: 0.1.2-post2
+Version: 0.1.3rc0
 Summary: an easy training architecture
 Home-page: https://github.com/ssbuild/deep_training
 Author: ssbuild
 Author-email: 9727464@qq.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Dist: pytorch-lightning (>=2)
```

## Comparing `deep_training-0.1.2.post2.dist-info/RECORD` & `deep_training-0.1.3rc0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 deep_training/__init__.py,sha256=bhATnUT4VEzwvA8_8IwxspnDRKf32ZgEeHYCN2E5Dd4,47
-deep_training/setup.py,sha256=uLO1dDML4prp6R2XGy5XlYXPfe-I7vgxToq8ekav7Tw,903
+deep_training/setup.py,sha256=46TsaKTiTi81hV6hEosREfIgocgVQ3BI2m-oNRY5yaQ,900
 deep_training/cv/__init__.py,sha256=J-zlKxMsAfAgoO0vSAzgYJXSuMSJcJ7NKAPKeaeC3TM,55
 deep_training/data_helper/__init__.py,sha256=P8rAMalR6xNepAf-9ldGoOSsEiUtur8Px6gUpTXQhd8,195
 deep_training/data_helper/data_helper.py,sha256=wamHVXHpCIcG-COkVLRmwIjmcQ0MQy99xjago0ulkkY,29088
 deep_training/data_helper/data_module.py,sha256=cRqwzcKMpFaE2HhdbAEwrIC9KxOE0rLkeQ25VCJh2W8,4926
 deep_training/data_helper/data_writer.py,sha256=BnxUmMuR60Wawd1SH9TTEBsQuDLozxWJdmLozuO-Wv4,1383
 deep_training/data_helper/training_args.py,sha256=xAjTMEaNvXXzgdV9oNvSCaR1lKX4wdeIJoqus1VTN7w,12557
 deep_training/nlp/__init__.py,sha256=L4_ltrwpG8mrgN1hZRKimefLHgjhRYyXVtLMFzr1grw,70
@@ -108,14 +108,24 @@
 deep_training/nlp/models/lora/v1/lora_wrapper.py,sha256=449xBRufJ8Tt4p_OLsp7TZ3v8Y3iIBdpccgReGDzUng,13576
 deep_training/nlp/models/lora/v2/__init__.py,sha256=2XorjeFlyNuH6xTXiyNO1A8A3P5acBApOjxVv3YEon0,206
 deep_training/nlp/models/lora/v2/adalora_model.py,sha256=iKfKWnW--iY2gmXkMcBv6QWJr9vu-uSll57r1UNvRrY,13112
 deep_training/nlp/models/lora/v2/configuration.py,sha256=RXTsOjRKUHGFKpSrrFywjV41kT2liEPj1C6Li-ogJpI,11281
 deep_training/nlp/models/lora/v2/lora_model.py,sha256=5k09kzj8bSvU-CQm5GJWtg5isXUEUYPmvKuxdLPc_V4,11745
 deep_training/nlp/models/lora/v2/lora_wrapper.py,sha256=tzDCWUiGYC81cbfNiu4ZKo3VZsftM_SF8NwH8r56BO0,10265
 deep_training/nlp/models/lora/v2/save_and_load.py,sha256=U7_ZaPm8gpg8gQhZei6UG5KvsJXDtSNZfZk1gWo6nWc,4889
+deep_training/nlp/models/moss/__init__.py,sha256=_dQslDggRX8ZsR6RPTUuBzAHotQt8MPAqZ1-nGULPns,467
+deep_training/nlp/models/moss/configuration_moss.py,sha256=Qqp7anpWGnsotkqd5UOfc9e5zhxgx7j5xetSQUOmhaQ,5097
+deep_training/nlp/models/moss/custom_autotune.py,sha256=O-C9w-hZkcrUgDfK4B1iPtKjHQAZwELNefYhlLABHyc,6735
+deep_training/nlp/models/moss/modeling_moss.py,sha256=smkAESJv2rw-npBasohtoz1ztxtrCo479RGbkw_nUIk,30926
+deep_training/nlp/models/moss/quantization.py,sha256=z43YME9DW_yER96uUoyWdE0GwyZaZX4psA40LRHLhP0,18866
+deep_training/nlp/models/moss/tokenization_moss.py,sha256=nqDlylb3w1FOpOTwHySh9WMxmPo9IXdZrYkkHgjdCbw,14782
+deep_training/nlp/models/rlhf/__init__.py,sha256=c1W6T8PhNnCVnEIKtr7qu-jHY2IliW9HcMOv5TZ92b0,55
+deep_training/nlp/models/rlhf/ppo/__init__.py,sha256=IqNQicmSmtZVbJIdNZdaQxpx0EbqvTJSUb2Bx1pRdys,55
+deep_training/nlp/models/rlhf/ppo/configuration.py,sha256=XDkcqvL5IVHYQe5Yew7hoxeWK3BQW7pTreg4VCF5G_s,212
+deep_training/nlp/models/rlhf/ppo/ppo.py,sha256=kMqYK4UyKiqavDLCExOYUiKNSBsc2axgtshOHczVSn4,55
 deep_training/nlp/models/splinker/__init__.py,sha256=QtgnpJa78vAq9bzfjN67NmHU3dXU6WH84jeyZoD1sBs,102
 deep_training/nlp/models/splinker/splinker.py,sha256=cAXQoPucM3ULYUhBw9z-OxPK_b9hHKEZPgMb4vFfQwc,2851
 deep_training/nlp/models/t5decoder/__init__.py,sha256=R9Op4Ysli9isootQQ2FcjhpbG13fNESlmUROu6cfGH0,14478
 deep_training/nlp/models/t5encoder/__init__.py,sha256=692ChfLf2sZWgzhBM37g1PdpmEmsU1R9RRl_uTHRET0,6646
 deep_training/nlp/optimizer/__init__.py,sha256=c4cmx9ebIdqwXBu3N9QbcNNHb32t2MV6fTK9aC2VBGQ,56
 deep_training/nlp/optimizer/lamb.py,sha256=htvZQHPWHG5GCDgo9xCaZikWwRyaD2PjDioIQvX7qXw,5225
 deep_training/nlp/optimizer/lion/__init__.py,sha256=AvYkLp7sOpRIC3a5ejuniUUKyQmmBA1TPJdt2RA7Nqg,99
@@ -135,11 +145,11 @@
 deep_training/tfnlp/scheduler/__init__.py,sha256=69flKnae4cQQyWUDwuYE0w0iaPonvH0P_WjBd_t-IqU,53
 deep_training/tfnlp/utils/__init__.py,sha256=kAmlOWNSpQCHbtT-mAsKGQzQFoWKp2jQf3neCJ0cCRY,53
 deep_training/utils/__init__.py,sha256=JFm7m_LPsS9Oavyxn9rbWqllCmV_zBho19rISlHNX4c,55
 deep_training/utils/distributed.py,sha256=-dhvJ6YHpRxvtZ1_on50IE33fUFW3zKXBKqqK-L1HGM,1941
 deep_training/utils/func.py,sha256=1p8hiQDCyk_gQGKrF7y6Dt66k3jLXSAt2IQeJuHQEl8,1724
 deep_training/utils/maskedlm.py,sha256=o8EB2BbDdh7wdgqz9Oi6SsVr1uBWxV15qfTk2VPjWsU,5117
 deep_training/utils/trainer.py,sha256=Rit5xEC2r9MvQdDR4A5A6E4_gzNCVNmW9m55kC83O50,7469
-deep_training-0.1.2.post2.dist-info/METADATA,sha256=7DPlXexw6vD32Bc_gEcsvA0I3Su07O4FHL29vH6dJ2g,629
-deep_training-0.1.2.post2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-deep_training-0.1.2.post2.dist-info/top_level.txt,sha256=P4qengiW56PZRm1VvlGcseSUCmAaBCsalCviUABZtO0,14
-deep_training-0.1.2.post2.dist-info/RECORD,,
+deep_training-0.1.3rc0.dist-info/METADATA,sha256=Jl4kZax1kYebJvVKjPOty8QymGDMpFNXgdwSbwY0VAw,626
+deep_training-0.1.3rc0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+deep_training-0.1.3rc0.dist-info/top_level.txt,sha256=P4qengiW56PZRm1VvlGcseSUCmAaBCsalCviUABZtO0,14
+deep_training-0.1.3rc0.dist-info/RECORD,,
```

