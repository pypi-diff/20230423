# Comparing `tmp/payme-pkg-2.1.tar.gz` & `tmp/payme-pkg-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payme-pkg-2.1.tar", last modified: Sun Oct 30 17:52:40 2022, max compression
+gzip compressed data, was "dist/payme-pkg-2.2.tar", last modified: Sun Apr 23 09:45:13 2023, max compression
```

## Comparing `payme-pkg-2.1.tar` & `payme-pkg-2.2.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2022-10-30 17:52:40.584771 payme-pkg-2.1/
--rw-r--r--   0 thenight   (501) staff       (20)     1062 2022-10-22 20:03:01.000000 payme-pkg-2.1/LICENSE.txt
--rw-r--r--   0 thenight   (501) staff       (20)      338 2022-10-30 17:52:40.585046 payme-pkg-2.1/PKG-INFO
--rw-r--r--   0 thenight   (501) staff       (20)    18991 2022-10-30 17:44:46.000000 payme-pkg-2.1/README.md
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2022-10-30 17:52:40.543503 payme-pkg-2.1/lib/
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2022-10-30 17:52:40.556169 payme-pkg-2.1/lib/payme/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2022-10-22 19:57:48.000000 payme-pkg-2.1/lib/payme/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)      189 2022-10-22 20:23:00.000000 payme-pkg-2.1/lib/payme/admin.py
--rw-r--r--   0 thenight   (501) staff       (20)      142 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/apps.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2022-10-30 17:52:40.560523 payme-pkg-2.1/lib/payme/cards/
--rw-r--r--   0 thenight   (501) staff       (20)       28 2022-10-22 19:57:48.000000 payme-pkg-2.1/lib/payme/cards/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     4454 2022-10-22 19:57:48.000000 payme-pkg-2.1/lib/payme/cards/subscribe_cards.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2022-10-30 17:52:40.564717 payme-pkg-2.1/lib/payme/errors/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/errors/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     1437 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/errors/exceptions.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2022-10-30 17:52:40.572154 payme-pkg-2.1/lib/payme/methods/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/methods/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     1649 2022-10-30 05:30:37.000000 payme-pkg-2.1/lib/payme/methods/cancel_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)      478 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/methods/check_perform_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)     1666 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/methods/check_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)     1954 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/methods/create_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)     1484 2022-10-30 17:22:15.000000 payme-pkg-2.1/lib/payme/methods/generate_link.py
--rw-r--r--   0 thenight   (501) staff       (20)     1606 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/methods/perform_transaction.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2022-10-30 17:52:40.574469 payme-pkg-2.1/lib/payme/migrations/
--rw-r--r--   0 thenight   (501) staff       (20)     1803 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/migrations/0001_initial.py
--rw-r--r--   0 thenight   (501) staff       (20)        0 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/migrations/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     1187 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/models.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2022-10-30 17:52:40.575929 payme-pkg-2.1/lib/payme/receipts/
--rw-r--r--   0 thenight   (501) staff       (20)       31 2022-10-22 19:57:48.000000 payme-pkg-2.1/lib/payme/receipts/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     6058 2022-10-22 20:17:31.000000 payme-pkg-2.1/lib/payme/receipts/subscribe_receipts.py
--rw-r--r--   0 thenight   (501) staff       (20)     1625 2022-10-30 15:19:57.000000 payme-pkg-2.1/lib/payme/serializers.py
--rw-r--r--   0 thenight   (501) staff       (20)      139 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/urls.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2022-10-30 17:52:40.580065 payme-pkg-2.1/lib/payme/utils/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/utils/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)      680 2022-10-30 15:20:58.000000 payme-pkg-2.1/lib/payme/utils/get_params.py
--rw-r--r--   0 thenight   (501) staff       (20)      784 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/utils/logger.py
--rw-r--r--   0 thenight   (501) staff       (20)      209 2022-10-22 20:17:18.000000 payme-pkg-2.1/lib/payme/utils/support.py
--rw-r--r--   0 thenight   (501) staff       (20)     4270 2022-10-30 16:45:00.000000 payme-pkg-2.1/lib/payme/views.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2022-10-30 17:52:40.584194 payme-pkg-2.1/lib/payme_pkg.egg-info/
--rw-r--r--   0 thenight   (501) staff       (20)      338 2022-10-30 17:52:40.000000 payme-pkg-2.1/lib/payme_pkg.egg-info/PKG-INFO
--rw-r--r--   0 thenight   (501) staff       (20)     1013 2022-10-30 17:52:40.000000 payme-pkg-2.1/lib/payme_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 thenight   (501) staff       (20)        1 2022-10-30 17:52:40.000000 payme-pkg-2.1/lib/payme_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 thenight   (501) staff       (20)       45 2022-10-30 17:52:40.000000 payme-pkg-2.1/lib/payme_pkg.egg-info/requires.txt
--rw-r--r--   0 thenight   (501) staff       (20)        6 2022-10-30 17:52:40.000000 payme-pkg-2.1/lib/payme_pkg.egg-info/top_level.txt
--rw-r--r--   0 thenight   (501) staff       (20)      107 2022-10-30 17:52:40.586445 payme-pkg-2.1/setup.cfg
--rw-r--r--   0 thenight   (501) staff       (20)      513 2022-10-30 17:52:24.000000 payme-pkg-2.1/setup.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/
+-rw-r--r--   0 thenight   (501) staff       (20)      338 2023-04-23 09:45:13.000000 payme-pkg-2.2/PKG-INFO
+-rw-r--r--   0 thenight   (501) staff       (20)    19593 2023-04-23 09:08:57.000000 payme-pkg-2.2/README.md
+-rw-r--r--   0 thenight   (501) staff       (20)      538 2023-04-23 09:44:11.000000 payme-pkg-2.2/setup.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/
+-rw-r--r--   0 thenight   (501) staff       (20)      338 2023-04-23 09:45:12.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 thenight   (501) staff       (20)     1097 2023-04-23 09:45:12.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 thenight   (501) staff       (20)       59 2023-04-23 09:45:12.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/requires.txt
+-rw-r--r--   0 thenight   (501) staff       (20)        6 2023-04-23 09:45:12.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/top_level.txt
+-rw-r--r--   0 thenight   (501) staff       (20)        1 2023-04-23 09:45:12.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/dependency_links.txt
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/receipts/
+-rw-r--r--   0 thenight   (501) staff       (20)     6616 2023-04-19 14:50:57.000000 payme-pkg-2.2/lib/payme/receipts/subscribe_receipts.py
+-rw-r--r--   0 thenight   (501) staff       (20)       32 2023-04-19 09:04:54.000000 payme-pkg-2.2/lib/payme/receipts/__init__.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/migrations/
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-19 08:59:40.000000 payme-pkg-2.2/lib/payme/migrations/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2061 2023-04-19 08:59:33.000000 payme-pkg-2.2/lib/payme/migrations/0001_initial.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/methods/
+-rw-r--r--   0 thenight   (501) staff       (20)      708 2023-04-19 05:54:29.000000 payme-pkg-2.2/lib/payme/methods/check_perform_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1847 2023-04-19 15:06:51.000000 payme-pkg-2.2/lib/payme/methods/cancel_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2302 2023-04-19 06:34:08.000000 payme-pkg-2.2/lib/payme/methods/create_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1538 2023-04-19 07:34:08.000000 payme-pkg-2.2/lib/payme/methods/perform_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/methods/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1954 2023-04-19 07:14:23.000000 payme-pkg-2.2/lib/payme/methods/generate_link.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1424 2023-04-19 15:07:40.000000 payme-pkg-2.2/lib/payme/methods/check_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1974 2023-04-23 09:30:02.000000 payme-pkg-2.2/lib/payme/models.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/decorators/
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-19 13:55:21.000000 payme-pkg-2.2/lib/payme/decorators/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)      908 2023-04-19 16:14:02.000000 payme-pkg-2.2/lib/payme/decorators/decorators.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/cards/
+-rw-r--r--   0 thenight   (501) staff       (20)     5071 2023-04-19 16:17:49.000000 payme-pkg-2.2/lib/payme/cards/subscribe_cards.py
+-rw-r--r--   0 thenight   (501) staff       (20)       29 2023-04-18 16:06:59.000000 payme-pkg-2.2/lib/payme/cards/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2588 2023-04-19 16:07:41.000000 payme-pkg-2.2/lib/payme/serializers.py
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-19 11:31:50.000000 payme-pkg-2.2/lib/payme/__init__.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/utils/
+-rw-r--r--   0 thenight   (501) staff       (20)      186 2023-04-19 17:04:27.000000 payme-pkg-2.2/lib/payme/utils/logging.py
+-rw-r--r--   0 thenight   (501) staff       (20)      209 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/utils/support.py
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/utils/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)      236 2023-04-19 13:45:21.000000 payme-pkg-2.2/lib/payme/utils/to_json.py
+-rw-r--r--   0 thenight   (501) staff       (20)      680 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/utils/get_params.py
+-rw-r--r--   0 thenight   (501) staff       (20)      264 2023-04-18 19:19:38.000000 payme-pkg-2.2/lib/payme/apps.py
+-rw-r--r--   0 thenight   (501) staff       (20)      287 2023-04-23 08:58:58.000000 payme-pkg-2.2/lib/payme/admin.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/errors/
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/errors/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2241 2023-04-19 05:45:54.000000 payme-pkg-2.2/lib/payme/errors/exceptions.py
+-rw-r--r--   0 thenight   (501) staff       (20)      139 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/urls.py
+-rw-r--r--   0 thenight   (501) staff       (20)     4370 2023-04-19 13:41:19.000000 payme-pkg-2.2/lib/payme/views.py
+-rw-r--r--   0 thenight   (501) staff       (20)      107 2023-04-23 09:45:13.000000 payme-pkg-2.2/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `payme-pkg-2.1/README.md` & `payme-pkg-2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # Payme Uzbekistan Integration Uzcard and Humo
 <p align="center">
     <img style="width: 70%;" src="https://www.gazeta.uz/media/img/2019/07/GDpmEM15631750293941_b.jpg"></img>
 </p>
 
+Support Group - https://t.me/+Ng1axYLNyBAyYTRi <br/>
+Implementation Sample - https://github.com/Muhammadali-Akbarov/payme-sample
 
 ## Installation
 
 ```
 $ pip install payme-pkg
 ```
 ### Test-Credentials
 ```
 Card Numer: 8600 4954 7331 6478 Expire Date: 03/99 SMS Code: 666666 
 Card Numer: 8600 0691 9540 6311 Expire Date: 03/99 SMS Code: 666666 
 ```
 
 ## Documentation
   * [Merchant API](#merchant-api)
+  * [Generate Pay Link](#generate-pay-link)
   * Subscribe Cards
     * [Cards Create](#cards-create)
     * [Cards Get Verify Code](#cards-get-verify-code)
     * [Cards Verify](#cards-verify)
     * [Cards Check](#cards-check)
     * [Cards Remove](#cards-remove)
    
@@ -51,14 +54,16 @@
     'PAYME_ID': 'payme-id',
     'PAYME_KEY': 'payme-key',
     'PAYME_URL': 'payme-checkout-url',
     'PAYME_CALL_BACK_URL': 'your-callback-url', # merchant api callback url
     'PAYME_MIN_AMOUNT': 'payme-min-amount', # integer field
     'PAYME_ACCOUNT': 'order-id',
 }
+
+ORDER_MODEL = 'your_app.models.Your_Order_Model'
 ```
 Add a `payme` path to core of urlpatterns:
 ```python
 from django.urls import path
 from django.urls import include
 
 urlpatterns = [
@@ -69,14 +74,36 @@
 ```
 Run migrations
 ```
 $ python manage.py migrate
 ```
 🎉 Congratulations you have been integrated merchant api methods with django, keep reading docs.After successfull migrations check your admin panel and see results what happened.
 
+## Generate Pay Link
+Example to generate link:
+
+* Input
+
+```python
+from pprint import pprint
+
+from payme.methods.generate_link import GeneratePayLink
+
+pay_link = GeneratePayLink(
+  order_id=999,
+  amount=9999
+).generate_link()
+
+pprint(pay_link)
+```
+* Output
+
+```
+Link: https://checkout.paycom.uz/bT01ZTczMGU4ZTBiODUyYTQxN2FhNDljZWI7YWMub3JkZXItaWQ9OTk5O2E9OTk5OTtjPXlvdXItY2FsbGJhY2stdXJs
+```
 ## Cards Create
 Example for cards create method for to generate token from card:
 
 * Request
 
 ```
 from pprint import pprint
@@ -85,15 +112,15 @@
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb"
 )
 
-resp = client._cards_create(
+resp = client.cards_create(
     number="8600069195406311",
     expire="0399",
     save=True,
 )
 
 pprint(resp)
 ```
@@ -125,15 +152,15 @@
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb"
 )
 
-resp = client._card_get_verify_code(
+resp = client.card_get_verify_code(
     token="630e5ffdd15d8d8d093b379b_2fsaoABWafecn20kofV4PFafFZjeGDWS9adM1PmboQaEZbbaxMcnaskctMbU9Iv8qgrOuKGz8SnjvZvYXDK64m1eS9gA5jZ7BBRaQybMXrDPtFPJ1fwek5B1KoIv5cMiCWYXj7ezpYEdJAKTIQw0Np9HsTXjqco4gQG3m8MOfeH9ovkdm66O6yj45oKXRmJyAK5i0SchXNNomACH3Oq80KyoRE1VoBRxvoKyMkOx0xcepXovxK9d3v26a8z7UtyokwY33N8MupviM3A5WHB5Xh35WZJJyFnxTSi1vvnYnG7uVd6Bb1GjV2yAHnimss8aEZGW5V7ZiPrhf8r6WJAeHciYDGK3msRKZJBQTfjgOdE9tGrEnMezVkxr1JXX0xSn5qqec2"
 )
 
 pprint(resp)
 ```
 * Response
 ```
@@ -157,15 +184,15 @@
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb"
 )
 
-resp = client._cards_verify(
+resp = client.cards_verify(
     verify_code="666666",
     token="630e691fd15d8d8d093b379c_70mKyzqS8d1wTWzovIGjt9dKmjpn1KI8Y9XakPrfpbUASTBaZYbC1DjDcjYRmuNJep9gZrTRtHyEGBQYmBaPufuozF51bv4qEPsQnodq1VcD7tYyREwUXjMXXZUeu7Ek0REQCekCvVHX6rtNBpb4vtViJoNVjp94XpTqu0Bn3yYYb0CHu951wFydzRsieGxjGNrvx1oKyBcq0CdOUwoffRIt2VPvx5R2aVmc6ahwyhn387FEEcpO1PnjIJkWKTBWdI35ZPQnb1u1oss5aPg06E279THXRkoTThixbeqiD2JkWSXweNVGGDhTS30V4j61G3NWEPO2H3k4uFmCjjIQSzx4TxKzUgHg1i2q953PRUGjT4JZBRHMDxaN5tWuctEMNmY06p"
 )
 
 pprint(resp)
 ```
 * Response
@@ -195,15 +222,15 @@
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb"
 )
 
-resp = client._cards_check(
+resp = client.cards_check(
     token="630e691fd15d8d8d093b379c_70mKyzqS8d1wTWzovIGjt9dKmjpn1KI8Y9XakPrfpbUASTBaZYbC1DjDcjYRmuNJep9gZrTRtHyEGBQYmBaPufuozF51bv4qEPsQnodq1VcD7tYyREwUXjMXXZUeu7Ek0REQCekCvVHX6rtNBpb4vtViJoNVjp94XpTqu0Bn3yYYb0CHu951wFydzRsieGxjGNrvx1oKyBcq0CdOUwoffRIt2VPvx5R2aVmc6ahwyhn387FEEcpO1PnjIJkWKTBWdI35ZPQnb1u1oss5aPg06E279THXRkoTThixbeqiD2JkWSXweNVGGDhTS30V4j61G3NWEPO2H3k4uFmCjjIQSzx4TxKzUgHg1i2q953PRUGjT4JZBRHMDxaN5tWuctEMNmY06p"
 )
 
 pprint(resp)
 ```
 * Response
 ```
@@ -231,15 +258,15 @@
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb"
 )
 
-resp = client._cards_check(
+resp = client.cards_remove(
     token="630e691fd15d8d8d093b379c_70mKyzqS8d1wTWzovIGjt9dKmjpn1KI8Y9XakPrfpbUASTBaZYbC1DjDcjYRmuNJep9gZrTRtHyEGBQYmBaPufuozF51bv4qEPsQnodq1VcD7tYyREwUXjMXXZUeu7Ek0REQCekCvVHX6rtNBpb4vtViJoNVjp94XpTqu0Bn3yYYb0CHu951wFydzRsieGxjGNrvx1oKyBcq0CdOUwoffRIt2VPvx5R2aVmc6ahwyhn387FEEcpO1PnjIJkWKTBWdI35ZPQnb1u1oss5aPg06E279THXRkoTThixbeqiD2JkWSXweNVGGDhTS30V4j61G3NWEPO2H3k4uFmCjjIQSzx4TxKzUgHg1i2q953PRUGjT4JZBRHMDxaN5tWuctEMNmY06p"
 )
 
 pprint(resp)
 ```
 * Response
 ```
@@ -261,15 +288,15 @@
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb",
     paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
 )
 
-resp = rclient._receipts_create(
+resp = rclient.receipts_create(
     amount=10000,
     order_id="1"
 )
 
 pprint(resp)
 ```
 * Response
@@ -337,15 +364,15 @@
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb",
     paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
 )
 
-resp = rclient._receipts_pay(
+resp = rclient.receipts_pay(
     invoice_id="631186b6c4420cbf2712a243",
     token="63118a5dd15d8d8d093b37b7_X2j34OIJPnROfsgzYZCZ0w7OcC50zzwiowTsotEVO1uUbxkzaDrvdOno6jicQTrcRmxvibxrye4vUS3AynTNPaPCTGpfk3RCKmT9NaOAyyTmctAjWsjwvqGR5XUzAP1Xcx12GkhuQi6VJ4BeaIXOokSRu06rRjaivmJQ8HTiJiR9b3OmZtrhkIRNcNXnnp9zYm1mFP4BuqGpS8BMnY0ASIE6ffxWykjgBcDTAfWBFt4mg7O9Dsvx0aj3IB8z3RIbZYtDZJnUVhCZrwW7ONVI9uEAdxNthorjO6PbV7TQ8XCjrztgGf6uCtOwwxasiIUVZN6tCVDk8A8NvVSUzUHXQHVkaPn5heJNa3K4WsffIckq7SwMbiw3UbawipeZKyD3iwk1Km",
     phone="998901304527"
 )
 
 pprint(resp)
 ```
@@ -418,15 +445,15 @@
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb",
     paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
 )
 
-resp = rclient._receipts_send(
+resp = rclient.receipts_send(
     invoice_id="631186b6c4420cbf2712a243",
     phone="998901304527"
 )
 
 pprint(resp)
 ```
 * Response
@@ -450,15 +477,15 @@
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb",
     paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
 )
 
-resp = rclient._receipts_cancel(
+resp = rclient.receipts_cancel(
     invoice_id="63119303c4420cbf2712a245"
 )
 
 pprint(resp)
 ```
 * Response
 ```
@@ -530,15 +557,15 @@
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb",
     paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
 )
 
-resp = rclient._receipts_check(
+resp = rclient.receipts_check(
     invoice_id="63119303c4420cbf2712a245"
 )
 
 pprint(resp)
 ```
 * Response
 ```
@@ -561,15 +588,15 @@
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb",
     paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
 )
 
-resp = rclient._reciepts_get(
+resp = rclient.reciepts_get(
     invoice_id="6311946bc4420cbf2712a247"
 )
 
 pprint(resp)
 ```
 * Response
 ```
@@ -637,15 +664,15 @@
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb",
     paycom_key="#MWnwHNYATJo%W@XvO5nISiY&mG7PEuzDX18"
 )
 
-resp = rclient._reciepts_get_all(
+resp = rclient.reciepts_get_all(
     count=2,
     _from=1636398000000,
     to=1636398000000,
     offset=0
 )
 
 pprint(resp)
@@ -759,8 +786,8 @@
         "owner": "5e730e8e0b852a417aa49ceb",
         "source_cancel": "subscribe"
       },
       "processing_id": null
     }
   ]
 }
-```
+
```

### Comparing `payme-pkg-2.1/lib/payme/cards/subscribe_cards.py` & `payme-pkg-2.2/lib/payme/cards/subscribe_cards.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,139 +1,166 @@
-import json
-import requests
+from payme.utils.to_json import to_json
+from payme.decorators.decorators import payme_request
 
 
 class PaymeSubscribeCards:
-    """The PaymeSubscribeCards class inclues
+    """
+    The PaymeSubscribeCards class inclues
     all paycom methods which are belongs to cards.
 
-    :param base_url string: The base url of the paycom api
-    :param paycom_id string: The paycom_id uses to identify
+    Parameters
+    ----------
+    base_url: str — The base url of the paycom api
+    paycom_id: str — The paycom_id uses to identify
+    timeout: int — How many seconds to wait for the server to send data
+
+    Full method documentation
+    -------------------------
+    https://developer.help.paycom.uz/metody-subscribe-api/
     """
-    def __init__(self, base_url: str, paycom_id: str) -> None:
-        self.__base_url: str = base_url
-        self.__paycom_id: str = paycom_id
-
-        self.__headers: dict = {
-            "X-Auth": self.__paycom_id,
+    def __init__(
+        self,
+        base_url: str,
+        paycom_id: str,
+        timeout=5
+    ) -> "PaymeSubscribeCards":
+        self.base_url: str = base_url
+        self.timeout: int = timeout
+        self.headers: dict = {
+            "X-Auth": paycom_id,
         }
         self.__methods: dict = {
             "cards_check": "cards.check",
             "cards_create": "cards.create",
             "cards_remove": "cards.remove",
             "cards_verify": "cards.verify",
             "cards_get_verify_code": "cards.get_verify_code",
         }
 
-    def __request(self, card_info: dict) -> dict:
-        """Use this private method to request.On success,
-        response will be OK with format JSON.
-
-        :param card_info dict: Includes card data information.
+    @payme_request
+    def __request(self, data) -> dict:
         """
-        req_data: dict = {
-            "data": card_info,
-            "url": self.__base_url,
-            "headers": self.__headers,
-        }
+        Use this private method to request.
+        On success,response will be OK with format JSON.
 
-        return requests.post(**req_data).json()
-
-    def _cards_create(self, number: str, expire: str, save: bool) -> dict:
-        """Use this method to create a new card's token.
-
-        :param number string: The card number maximum length 18 char
-        :param expire string: The card expiration string maximum length 5 char
-        :param save bool: Type of token
-
-        Full method documentation:
-        https://developer.help.paycom.uz/uz/metody-subscribe-api/cards.create
+        Parameters
+        ----------
+        data: dict — Includes request data.
+
+        Returns dictionary Payme Response
+        ---------------------------------
+        """
+        return data
+
+    def cards_create(self, number: str, expire: str, save: bool = True) -> dict:
+        """
+        Use this method to create a new card's token.
+
+        Parameters
+        ----------
+        number: str — The card number maximum length 18 char
+        expire: str — The card expiration string maximum length 5 char
+        save: bool \
+            Type of token. Optional parameter
+            The option is enabled or disabled depending on the application's business logic
+            If the flag is true, the token can be used for further payments
+            if the flag is false the token can only be used once
+            The one-time token is deleted after payment
+
+        Full method documentation
+        -------------------------
+        https://developer.help.paycom.uz/metody-subscribe-api/cards.create
         """
         data: dict = {
             "method": self.__methods.get("cards_create"),
             "params": {
                 "card": {
                     "number": number,
                     "expire": expire,
                 },
                 "save": save,
             }
         }
-        return self.__request(self._parse_to_json(**data))
+        return self.__request(to_json(**data))
 
-    def _card_get_verify_code(self, token: str) -> dict:
-        """Use this method to get the verification code.
+    def card_get_verify_code(self, token: str) -> dict:
+        """
+        Use this method to get the verification code.
 
-        :param token string: The card's non-active token
+        Parameters
+        ----------
+        token: str — The card's non-active token
 
-        Full method documentation:
-        https://developer.help.paycom.uz/uz/metody-subscribe-api/cards.get_verify_code
+        Full method documentation
+        -------------------------
+        https://developer.help.paycom.uz/metody-subscribe-api/cards.get_verify_code
         """
         data: dict = {
             "method": self.__methods.get('cards_get_verify_code'),
             "params": {
                 "token": token,
             }
         }
-        return self.__request(self._parse_to_json(**data))
+        return self.__request(to_json(**data))
 
-    def _cards_verify(self, verify_code: int, token: str) -> dict:
-        """Verification of the card using the code sent via SMS.
+    def cards_verify(self, verify_code: int, token: str) -> dict:
+        """
+        Verification of the card using the code sent via SMS.
 
-        :param verify_code string: Code for verification
-        :param token string: The card's non-active token
+        Parameters
+        ----------
+        verify_code: int — Code for verification
+        token: str — The card's non-active token
 
-        Full method documentation:
-        https://developer.help.paycom.uz/uz/metody-subscribe-api/cards.verify
+        Full method documentation
+        -------------------------
+        https://developer.help.paycom.uz/metody-subscribe-api/cards.verify
         """
         data: dict = {
             "method": self.__methods.get("cards_verify"),
             "params": {
                 "token": token,
                 "code": verify_code
             }
         }
-        return self.__request(self._parse_to_json(**data))
+        return self.__request(to_json(**data))
 
-    def _cards_check(self, token: str) -> dict:
-        """Checking the card token active or non-active.
+    def cards_check(self, token: str) -> dict:
+        """
+        Checking the card token active or non-active.
 
-        :param token: The card's token for checking
+        Parameters
+        ----------
+        token: str — The card's non-active token
 
-        Full method documentation:
-        https://developer.help.paycom.uz/uz/metody-subscribe-api/cards.check
+        Full method documentation
+        -------------------------
+        https://developer.help.paycom.uz/metody-subscribe-api/cards.check
         """
         data: dict = {
             "method": self.__methods.get("cards_check"),
             "params": {
                 "token": token,
             }
         }
 
-        return self.__request(self._parse_to_json(**data))
+        return self.__request(to_json(**data))
 
-    def _cards_remove(self, token: str) -> dict:
-        """Delete card's token on success returns success.
+    def cards_remove(self, token: str) -> dict:
+        """
+        Delete card's token on success returns success.
 
-        :param token: The card's token for deleting
+        Parameters
+        ----------
+        token: str — The card's non-active token
 
-        Full method documentation:
-        https://developer.help.paycom.uz/uz/metody-subscribe-api/cards.remove
+        Full method documentation
+        -------------------------
+        https://developer.help.paycom.uz/metody-subscribe-api/cards.remove
         """
         data: dict = {
             "method": self.__methods.get("cards_remove"),
             "params": {
                 "token": token,
             }
         }
-        return self.__request(self._parse_to_json(**data))
-
-    @staticmethod
-    def _parse_to_json(**kwargs) -> dict:
-        """Use this static method to data dumps.
-        """
-        data: dict = {
-            "method": kwargs.pop("method"),
-            "params": kwargs.pop("params"),
-        }
-
-        return json.dumps(data)
+        return self.__request(to_json(**data))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `payme-pkg-2.1/lib/payme/methods/check_transaction.py` & `payme-pkg-2.2/lib/payme/methods/create_transaction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,68 @@
-from payme.utils.logger import logged
-from payme.utils.get_params import get_params
+import uuid
+import time
+import datetime
 
+from payme.utils.logging import logger
+from payme.utils.get_params import get_params
 from payme.models import MerchatTransactionsModel
+from payme.errors.exceptions import TooManyRequests
 from payme.serializers import MerchatTransactionsModelSerializer
 
 
-class CheckTransaction:
-    def __call__(self, params: dict) -> None:
-        response: dict = None
+class CreateTransaction:
+    """
+    CreateTransaction class
+    That's used to create transaction
+
+    Full method documentation
+    -------------------------
+    https://developer.help.paycom.uz/metody-merchant-api/createtransaction
+    """
+    def __call__(self, params: dict) -> dict:
         serializer = MerchatTransactionsModelSerializer(
             data=get_params(params)
         )
         serializer.is_valid(raise_exception=True)
-        clean_data: dict = serializer.validated_data
+        order_id = serializer.validated_data.get("order_id")
 
         try:
-            logged_message = "started check transaction in db"
-            transaction = \
-                MerchatTransactionsModel.objects.get(
-                    _id=clean_data.get("_id"),
+            transaction = MerchatTransactionsModel.objects.filter(
+                order_id=order_id
+            ).last()
+
+            if transaction is not None:
+                if transaction._id != serializer.validated_data.get("_id"):
+                    raise TooManyRequests()
+
+        except TooManyRequests as error:
+            logger.error("Too many requests for transaction %s", error)
+            raise TooManyRequests() from error
+
+        if transaction is None:
+            transaction, _ = \
+                MerchatTransactionsModel.objects.get_or_create(
+                    _id=serializer.validated_data.get('_id'),
+                    order_id=serializer.validated_data.get('order_id'),
+                    transaction_id=uuid.uuid4(),
+                    amount=serializer.validated_data.get('amount'),
+                    created_at_ms=int(time.time() * 1000),
                 )
-            logged(
-                logged_message=logged_message,
-                logged_type="info",
-            )
-            response = {
+
+        if transaction:
+            response: dict = {
                 "result": {
                     "create_time": int(transaction.created_at_ms),
-                    "perform_time": transaction.perform_time,
-                    "cancel_time": transaction.cancel_time,
                     "transaction": transaction.transaction_id,
-                    "state": transaction.state,
-                    "reason": None,
+                    "state": int(transaction.state),
                 }
             }
-            if transaction.reason is not None:
-                response["result"]["reason"] = int(transaction.reason)
-
-        except Exception as e:
-            logged_message = "error during get transaction in db {}{}"
-            logged(
-                logged_message=logged_message.format(e, clean_data.get("id")),
-                logged_type="error",
-            )
 
         return response
+
+    @staticmethod
+    def _convert_ms_to_datetime(time_ms: str) -> int:
+        """Use this format to convert from time ms to datetime format.
+        """
+        readable_datetime = datetime.datetime.fromtimestamp(time_ms / 1000)
+
+        return readable_datetime
```

### Comparing `payme-pkg-2.1/lib/payme/methods/create_transaction.py` & `payme-pkg-2.2/lib/payme/serializers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,84 @@
-import uuid
-import time
-import datetime
+from django.conf import settings
 
-from payme.utils.get_params import get_params
+from rest_framework import serializers
 
+from payme.models import Order
+from payme.utils.logging import logger
+from payme.utils.get_params import get_params
 from payme.models import MerchatTransactionsModel
-from payme.errors.exceptions import TooManyRequests
-from payme.serializers import MerchatTransactionsModelSerializer
+from payme.errors.exceptions import IncorrectAmount
+from payme.errors.exceptions import PerformTransactionDoesNotExist
 
 
-class CreateTransaction:
-    def __call__(self, params: dict) -> dict:
-        serializer = MerchatTransactionsModelSerializer(
-            data=get_params(params)
-        )
-        serializer.is_valid(raise_exception=True)
-        order_id = serializer.validated_data.get("order_id")
+class MerchatTransactionsModelSerializer(serializers.ModelSerializer):
+    """
+    MerchatTransactionsModelSerializer class \
+        That's used to serialize merchat transactions data.
+    """
+    class Meta:
+        # pylint: disable=missing-class-docstring
+        model: MerchatTransactionsModel = MerchatTransactionsModel
+        fields: str = "__all__"
 
-        try:
-            transaction = MerchatTransactionsModel.objects.filter(
-                order_id=order_id
-            ).last()
-
-            if transaction is not None:
-                if transaction._id != serializer.validated_data.get("_id"):
-                    raise TooManyRequests()
-
-        except TooManyRequests:
-            raise TooManyRequests()
-
-        if transaction is None:
-            transaction, _ = \
-                MerchatTransactionsModel.objects.get_or_create(
-                    _id=serializer.validated_data.get('_id'),
-                    order_id=serializer.validated_data.get('order_id'),
-                    transaction_id=uuid.uuid4(),
-                    amount=serializer.validated_data.get('amount'),
-                    created_at_ms=int(time.time() * 1000),
+    def validate(self, attrs) -> dict:
+        """
+        Validate the data given to the MerchatTransactionsModel.
+        """
+        if attrs.get("order_id") is not None:
+            try:
+                order = Order.objects.get(
+                    id=attrs['order_id']
                 )
+                if order.amount != int(attrs['amount']):
+                    raise IncorrectAmount()
+
+            except IncorrectAmount as error:
+                logger.error("Invalid amount for order: %s", attrs['order_id'])
+                raise IncorrectAmount() from error
 
-        if transaction:
-            response: dict = {
-                "result": {
-                    "create_time": int(transaction.created_at_ms),
-                    "transaction": transaction.transaction_id,
-                    "state": int(transaction.state),
-                }
-            }
+        return attrs
+
+    def validate_amount(self, amount) -> int:
+        """
+        Validator for Transactions Amount.
+        """
+        if amount is not None:
+            if int(amount) <= settings.PAYME.get("PAYME_MIN_AMOUNT"):
+                raise IncorrectAmount()
 
-        return response
+        return amount
+
+    def validate_order_id(self, order_id) -> int:
+        """
+        Use this method to check if a transaction is allowed to be executed.
+
+        Parameters
+        ----------
+        order_id: str -> Order Indentation.
+        """
+        try:
+            Order.objects.get(
+                id=order_id,
+            )
+        except Order.DoesNotExist as error:
+            logger.error("Order does not exist order_id: %s", order_id)
+            raise PerformTransactionDoesNotExist() from error
+
+        return order_id
 
     @staticmethod
-    def _convert_ms_to_datetime(time_ms: str) -> int:
-        """Use this format to convert from time ms to datetime format.
+    def get_validated_data(params: dict) -> dict:
         """
-        readable_datetime = datetime.datetime.fromtimestamp(time_ms / 1000)
+        This static method helps to get validated data.
+
+        Parameters
+        ----------
+        params: dict — Includes request params.
+        """
+        serializer = MerchatTransactionsModelSerializer(
+            data=get_params(params)
+        )
+        serializer.is_valid(raise_exception=True)
+        clean_data: dict = serializer.validated_data
 
-        return readable_datetime
+        return clean_data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `payme-pkg-2.1/lib/payme/methods/perform_transaction.py` & `payme-pkg-2.2/lib/payme/methods/check_transaction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,44 @@
-import time
 
-from payme.utils.get_params import get_params
+from django.db import DatabaseError
 
-from payme.utils.logger import logged
+from payme.utils.logging import logger
 from payme.models import MerchatTransactionsModel
-from payme.serializers import MerchatTransactionsModelSerializer
+from payme.serializers import MerchatTransactionsModelSerializer as MTMS
 
 
-class PerformTransaction:
-    def __call__(self, params: dict) -> dict:
-        serializer = MerchatTransactionsModelSerializer(
-            data=get_params(params)
+class CheckTransaction:
+    """
+    CheckTransaction class
+    That's used to check transaction
+
+    Full method documentation
+    -------------------------
+    https://developer.help.paycom.uz/metody-merchant-api/checkperformtransaction
+    """
+    def __call__(self, params: dict) -> None:
+        clean_data: dict = MTMS.get_validated_data(
+            params=params
         )
-        serializer.is_valid(raise_exception=True)
-        clean_data: dict = serializer.validated_data
-        response: dict = None
+
         try:
-            logged_message = "started check trx in db(perform_transaction)"
             transaction = \
                 MerchatTransactionsModel.objects.get(
                     _id=clean_data.get("_id"),
                 )
-            logged(
-                logged_message=logged_message,
-                logged_type="info",
-            )
-            transaction.state = 2
-            if transaction.perform_time == 0:
-                transaction.perform_time = int(time.time() * 1000)
-
-            transaction.save()
-            response: dict = {
+            response = {
                 "result": {
-                    "perform_time": int(transaction.perform_time),
+                    "create_time": int(transaction.created_at_ms),
+                    "perform_time": transaction.perform_time,
+                    "cancel_time": transaction.cancel_time,
                     "transaction": transaction.transaction_id,
-                    "state": int(transaction.state),
+                    "state": transaction.state,
+                    "reason": None,
                 }
             }
-        except Exception as e:
-            logged_message = "error during get transaction in db {}{}"
-            logged(
-                logged_message=logged_message.format(e, clean_data.get("id")),
-                logged_type="error",
-            )
+            if transaction.reason is not None:
+                response["result"]["reason"] = int(transaction.reason)
+
+        except DatabaseError as error:
+            logger.error("Error getting transaction in database: %s", error)
 
         return response
```

### Comparing `payme-pkg-2.1/lib/payme/migrations/0001_initial.py` & `payme-pkg-2.2/lib/payme/migrations/0001_initial.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-# Generated by Django 4.1.2 on 2022-10-22 18:15
-
-from django.db import migrations, models
+# pylint: disable=invalid-name
+from django.db import models
+from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
+    """
+    Migration class for Django Migrations.
+    """
     initial = True
 
     dependencies = [
     ]
 
     operations = [
         migrations.CreateModel(
             name='MerchatTransactionsModel',
             fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('id', models.BigAutoField(
+                    auto_created=True,
+                    primary_key=True,
+                    serialize=False,
+                    verbose_name='ID')
+                ),
                 ('_id', models.CharField(max_length=255, null=True)),
                 ('transaction_id', models.CharField(max_length=255, null=True)),
                 ('order_id', models.BigIntegerField(blank=True, null=True)),
                 ('amount', models.FloatField(blank=True, null=True)),
                 ('time', models.BigIntegerField(blank=True, null=True)),
                 ('perform_time', models.BigIntegerField(default=0, null=True)),
                 ('cancel_time', models.BigIntegerField(default=0, null=True)),
@@ -28,14 +35,19 @@
                 ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('updated_at', models.DateTimeField(auto_now=True)),
             ],
         ),
         migrations.CreateModel(
             name='Order',
             fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('id', models.BigAutoField(
+                    auto_created=True,
+                    primary_key=True,
+                    serialize=False,
+                    verbose_name='ID')
+                 ),
                 ('amount', models.IntegerField(blank=True, null=True)),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('updated_at', models.DateTimeField(auto_now=True)),
             ],
         ),
     ]
```

### Comparing `payme-pkg-2.1/lib/payme/serializers.py` & `payme-pkg-2.2/lib/payme/methods/cancel_transaction.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,54 @@
-from django.conf import settings
+import time
 
-from rest_framework import serializers
+from django.db import transaction
 
-from payme.models import Order
+from payme.utils.logging import logger
 from payme.models import MerchatTransactionsModel
-from payme.errors.exceptions import IncorrectAmount
 from payme.errors.exceptions import PerformTransactionDoesNotExist
+from payme.serializers import MerchatTransactionsModelSerializer as MTMS
 
 
-class MerchatTransactionsModelSerializer(serializers.ModelSerializer):
-
-    class Meta:
-        model: MerchatTransactionsModel = MerchatTransactionsModel
-        fields: str = "__all__"
-
-    def validate(self, data):
-        """
-        Validate the data given to the MerchatTransactionsModel.
-        """
-        if data.get("order_id") is not None:
-            try:
-                order = Order.objects.get(
-                    id=data['order_id']
-                )
-                if order.amount != int(data['amount']):
-                    raise IncorrectAmount()
-
-            except IncorrectAmount:
-                raise IncorrectAmount()
-
-        return data
-
-    def validate_amount(self, amount) -> int:
-        """
-        Validator for Transactions Amount
-        """
-        if amount is not None:
-            if int(amount) <= settings.PAYME.get("PAYME_MIN_AMOUNT"):
-                raise IncorrectAmount()
-
-        return amount
-
-    def validate_order_id(self, order_id) -> int:
-        """
-        Use this method to check if a transaction is allowed to be executed.
-        :param order_id: string -> Order Indentation.
-        """
+class CancelTransaction:
+    """
+    CancelTransaction class
+    That is used to cancel a transaction.
+
+    Full method documentation
+    -------------------------
+    https://developer.help.paycom.uz/metody-merchant-api/canceltransaction
+    """
+
+    @transaction.atomic
+    def __call__(self, params: dict):
+        clean_data: dict = MTMS.get_validated_data(
+            params=params
+        )
         try:
-            Order.objects.get(
-                id=order_id,
-            )
-        except Order.DoesNotExist:
-            raise PerformTransactionDoesNotExist()
+            with transaction.atomic():
+                transactions: MerchatTransactionsModel = \
+                    MerchatTransactionsModel.objects.filter(
+                        _id=clean_data.get('_id'),
+                    ).first()
+                if transactions.cancel_time == 0:
+                    transactions.cancel_time = int(time.time() * 1000)
+                if transactions.perform_time == 0:
+                    transactions.state = -1
+                if transactions.perform_time != 0:
+                    transactions.state = -2
+                transactions.reason = clean_data.get("reason")
+                transactions.save()
+
+        except PerformTransactionDoesNotExist as error:
+            logger.error("Paycom transaction does not exist: %s", error)
+            raise PerformTransactionDoesNotExist() from error
+
+        response: dict = {
+            "result": {
+                "state": transactions.state,
+                "cancel_time": transactions.cancel_time,
+                "transaction": transactions.transaction_id,
+                "reason": int(transactions.reason),
+            }
+        }
 
-        return order_id
+        return response
```

### Comparing `payme-pkg-2.1/lib/payme/utils/get_params.py` & `payme-pkg-2.2/lib/payme/utils/get_params.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.1/lib/payme/views.py` & `payme-pkg-2.2/lib/payme/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,53 +3,62 @@
 
 from django.conf import settings
 
 from rest_framework.views import APIView
 from rest_framework.response import Response
 from rest_framework.exceptions import ValidationError
 
-from payme.utils.logger import logged
+from payme.utils.logging import logger
 
 from payme.errors.exceptions import MethodNotFound
 from payme.errors.exceptions import PermissionDenied
 from payme.errors.exceptions import PerformTransactionDoesNotExist
 
 from payme.methods.check_transaction import CheckTransaction
 from payme.methods.cancel_transaction import CancelTransaction
 from payme.methods.create_transaction import CreateTransaction
 from payme.methods.perform_transaction import PerformTransaction
 from payme.methods.check_perform_transaction import CheckPerformTransaction
 
 
 class MerchantAPIView(APIView):
+    """
+    MerchantAPIView class provides payme call back functionality.
+    """
     permission_classes = ()
     authentication_classes = ()
 
-    def post(self, request, *args, **kwargs):
+    def post(self, request) -> Response:
+        """
+        Payme sends post request to our call back url.
+        That methods are includes 5 methods
+            - CheckTransaction
+            - CreateTransaction
+            - CancelTransaction
+            - PerformTransaction
+            - CheckPerformTransaction
+        """
         password = request.META.get('HTTP_AUTHORIZATION')
         if self.authorize(password):
             incoming_data: dict = request.data
             incoming_method: str = incoming_data.get("method")
-            logged_message: str = "Incoming {data}"
 
-            logged(
-                logged_message=logged_message.format(
-                    method=incoming_method,
-                    data=incoming_data
-                ),
-                logged_type="info"
-            )
+            logger.info("Call back data is incoming %s", incoming_data)
+
             try:
                 paycom_method = self.get_paycom_method_by_name(
                     incoming_method=incoming_method
                 )
-            except ValidationError:
-                raise MethodNotFound()
-            except PerformTransactionDoesNotExist:
-                raise PerformTransactionDoesNotExist()
+            except ValidationError as error:
+                logger.error("Validation Error occurred: %s", error)
+                raise MethodNotFound() from error
+
+            except PerformTransactionDoesNotExist as error:
+                logger.error("PerformTransactionDoesNotExist Error occurred: %s", error)
+                raise PerformTransactionDoesNotExist() from error
 
             paycom_method = paycom_method(incoming_data.get("params"))
 
         return Response(data=paycom_method)
 
     @staticmethod
     def get_paycom_method_by_name(incoming_method: str) -> object:
@@ -62,66 +71,55 @@
             "CreateTransaction": CreateTransaction,
             "CancelTransaction": CancelTransaction,
             "PerformTransaction": PerformTransaction,
             "CheckPerformTransaction": CheckPerformTransaction
         }
 
         try:
-            MerchantMethod = available_methods[incoming_method]
-        except Exception:
-            error_message = "Unavailable method: %s" % incoming_method
-            logged(
-                logged_message=error_message,
-                logged_type="error"
-            )
-            raise MethodNotFound(error_message=error_message)
+            merchant_method = available_methods[incoming_method]
+        except Exception as error:
+            error_message = "Unavailable method: %s", incoming_method
+            logger.error(error_message)
+            raise MethodNotFound(error_message=error_message) from error
 
-        merchant_method = MerchantMethod()
+        merchant_method = merchant_method()
 
         return merchant_method
 
     @staticmethod
     def authorize(password: str) -> None:
         """
         Authorize the Merchant.
         :param password: string -> Merchant authorization password
         """
         is_payme: bool = False
         error_message: str = ""
 
         if not isinstance(password, str):
             error_message = "Request from an unauthorized source!"
-            logged(
-                logged_message=error_message,
-                logged_type="error"
-            )
+            logger.error(error_message)
             raise PermissionDenied(error_message=error_message)
 
         password = password.split()[-1]
 
         try:
             password = base64.b64decode(password).decode('utf-8')
-        except (binascii.Error, UnicodeDecodeError):
+        except (binascii.Error, UnicodeDecodeError) as error:
             error_message = "Error when authorize request to merchant!"
-            logged(
-                logged_message=error_message,
-                logged_type="error"
-            )
-            raise PermissionDenied(error_message=error_message)
+            logger.error(error_message)
+
+            raise PermissionDenied(error_message=error_message) from error
 
         merchant_key = password.split(':')[-1]
 
         if merchant_key == settings.PAYME.get('PAYME_KEY'):
             is_payme = True
 
         if merchant_key != settings.PAYME.get('PAYME_KEY'):
-            logged(
-                logged_message="Invalid key in request!",
-                logged_type="error"
-            )
+            logger.error("Invalid key in request!")
 
         if is_payme is False:
             raise PermissionDenied(
                 error_message="Unavailable data for unauthorized users!"
             )
 
         return is_payme
```

### Comparing `payme-pkg-2.1/lib/payme_pkg.egg-info/SOURCES.txt` & `payme-pkg-2.2/lib/payme_pkg.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-LICENSE.txt
 README.md
 setup.cfg
 setup.py
 lib/payme/__init__.py
 lib/payme/admin.py
 lib/payme/apps.py
 lib/payme/models.py
 lib/payme/serializers.py
 lib/payme/urls.py
 lib/payme/views.py
 lib/payme/cards/__init__.py
 lib/payme/cards/subscribe_cards.py
+lib/payme/decorators/__init__.py
+lib/payme/decorators/decorators.py
 lib/payme/errors/__init__.py
 lib/payme/errors/exceptions.py
 lib/payme/methods/__init__.py
 lib/payme/methods/cancel_transaction.py
 lib/payme/methods/check_perform_transaction.py
 lib/payme/methods/check_transaction.py
 lib/payme/methods/create_transaction.py
@@ -22,14 +23,15 @@
 lib/payme/methods/perform_transaction.py
 lib/payme/migrations/0001_initial.py
 lib/payme/migrations/__init__.py
 lib/payme/receipts/__init__.py
 lib/payme/receipts/subscribe_receipts.py
 lib/payme/utils/__init__.py
 lib/payme/utils/get_params.py
-lib/payme/utils/logger.py
+lib/payme/utils/logging.py
 lib/payme/utils/support.py
+lib/payme/utils/to_json.py
 lib/payme_pkg.egg-info/PKG-INFO
 lib/payme_pkg.egg-info/SOURCES.txt
 lib/payme_pkg.egg-info/dependency_links.txt
 lib/payme_pkg.egg-info/requires.txt
 lib/payme_pkg.egg-info/top_level.txt
```

### Comparing `payme-pkg-2.1/setup.py` & `payme-pkg-2.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='payme-pkg',
-    version='2.1',
+    version='2.2',
     license='MIT',
     author="Muhammadali Akbarov",
     author_email='muhammadali17abc@gmail.com',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     url='https://github.com/Muhammadali-Akbarov/payme-pkg',
     keywords='paymeuz paycomuz payme-merchant merchant-api subscribe-api payme-pkg payme-api',
     install_requires=[
-        'requests==2.28.1',
+        'requests==2.*',
+        'dataclasses==0.*',
         'djangorestframework==3.14.0'
       ],
 )
```

