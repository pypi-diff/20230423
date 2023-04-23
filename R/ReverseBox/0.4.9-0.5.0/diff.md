# Comparing `tmp/ReverseBox-0.4.9.tar.gz` & `tmp/ReverseBox-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseBox-0.4.9.tar", last modified: Sat Apr 15 13:32:07 2023, max compression
+gzip compressed data, was "ReverseBox-0.5.0.tar", last modified: Sun Apr 23 18:25:16 2023, max compression
```

## Comparing `ReverseBox-0.4.9.tar` & `ReverseBox-0.5.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.544533 ReverseBox-0.4.9/
--rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:47.000000 ReverseBox-0.4.9/LICENSE
--rw-rw-rw-   0        0        0     5157 2023-04-15 13:32:07.544533 ReverseBox-0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     3895 2023-04-15 13:25:24.000000 ReverseBox-0.4.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.494599 ReverseBox-0.4.9/ReverseBox.egg-info/
--rw-rw-rw-   0        0        0     5157 2023-04-15 13:32:07.000000 ReverseBox-0.4.9/ReverseBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1757 2023-04-15 13:32:07.000000 ReverseBox-0.4.9/ReverseBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 13:32:07.000000 ReverseBox-0.4.9/ReverseBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 13:32:07.000000 ReverseBox-0.4.9/ReverseBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-15 13:32:07.000000 ReverseBox-0.4.9/ReverseBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.495600 ReverseBox-0.4.9/reversebox/
--rw-rw-rw-   0        0        0        0 2022-06-25 12:19:26.000000 ReverseBox-0.4.9/reversebox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.499601 ReverseBox-0.4.9/reversebox/checksum/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.9/reversebox/checksum/__init__.py
--rw-rw-rw-   0        0        0      404 2023-01-08 20:51:07.000000 ReverseBox-0.4.9/reversebox/checksum/checksum_adler32.py
--rw-rw-rw-   0        0        0      403 2023-01-09 21:19:57.000000 ReverseBox-0.4.9/reversebox/checksum/checksum_fletcher16.py
--rw-rw-rw-   0        0        0      510 2023-01-09 22:41:53.000000 ReverseBox-0.4.9/reversebox/checksum/checksum_fletcher32.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.502601 ReverseBox-0.4.9/reversebox/common/
--rw-rw-rw-   0        0        0        0 2022-06-25 16:29:13.000000 ReverseBox-0.4.9/reversebox/common/__init__.py
--rw-rw-rw-   0        0        0      418 2023-04-12 20:41:34.000000 ReverseBox-0.4.9/reversebox/common/common.py
--rw-rw-rw-   0        0        0      730 2022-09-07 19:55:27.000000 ReverseBox-0.4.9/reversebox/common/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.507308 ReverseBox-0.4.9/reversebox/compression/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.9/reversebox/compression/__init__.py
--rw-rw-rw-   0        0        0      484 2022-10-16 11:14:45.000000 ReverseBox-0.4.9/reversebox/compression/compression_jcalg1.py
--rw-rw-rw-   0        0        0      335 2022-12-27 14:56:59.000000 ReverseBox-0.4.9/reversebox/compression/compression_lzo.py
--rw-rw-rw-   0        0        0      330 2022-10-15 10:41:38.000000 ReverseBox-0.4.9/reversebox/compression/compression_zlib.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.515450 ReverseBox-0.4.9/reversebox/crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:26:29.000000 ReverseBox-0.4.9/reversebox/crc/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:19.000000 ReverseBox-0.4.9/reversebox/crc/crc16_arc.py
--rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:31.000000 ReverseBox-0.4.9/reversebox/crc/crc16_ccitt.py
--rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:06.000000 ReverseBox-0.4.9/reversebox/crc/crc16_dnp.py
--rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:19.000000 ReverseBox-0.4.9/reversebox/crc/crc16_kermit.py
--rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:37.000000 ReverseBox-0.4.9/reversebox/crc/crc16_modbus.py
--rw-rw-rw-   0        0        0      735 2022-07-21 21:35:31.000000 ReverseBox-0.4.9/reversebox/crc/crc16_sick.py
--rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:19.000000 ReverseBox-0.4.9/reversebox/crc/crc32_iso_hdlc.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.519451 ReverseBox-0.4.9/reversebox/encryption/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.9/reversebox/encryption/__init__.py
--rw-rw-rw-   0        0        0      579 2022-07-17 23:25:19.000000 ReverseBox-0.4.9/reversebox/encryption/encryption_xor_basic.py
--rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:01.000000 ReverseBox-0.4.9/reversebox/encryption/encryption_xor_gianas_return_zda.py
--rw-rw-rw-   0        0        0      574 2022-07-17 23:25:19.000000 ReverseBox-0.4.9/reversebox/encryption/encryption_xor_retro64_eco.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.523451 ReverseBox-0.4.9/reversebox/hash/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.9/reversebox/hash/__init__.py
--rw-rw-rw-   0        0        0      280 2022-09-11 18:48:36.000000 ReverseBox-0.4.9/reversebox/hash/hash_md5.py
--rw-rw-rw-   0        0        0      283 2023-01-08 14:05:01.000000 ReverseBox-0.4.9/reversebox/hash/hash_sha1.py
--rw-rw-rw-   0        0        0      289 2023-01-08 14:07:31.000000 ReverseBox-0.4.9/reversebox/hash/hash_sha2.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.528357 ReverseBox-0.4.9/reversebox/image/
--rw-rw-rw-   0        0        0        0 2022-12-27 21:18:24.000000 ReverseBox-0.4.9/reversebox/image/__init__.py
--rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:19.000000 ReverseBox-0.4.9/reversebox/image/image_finder_gui.py
--rw-rw-rw-   0        0        0      715 2022-12-31 14:42:11.000000 ReverseBox-0.4.9/reversebox/image/image_finder_main.py
--rw-rw-rw-   0        0        0     1507 2023-04-15 13:20:43.000000 ReverseBox-0.4.9/reversebox/image/psp_swizzle.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.532530 ReverseBox-0.4.9/reversebox/io_files/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.4.9/reversebox/io_files/__init__.py
--rw-rw-rw-   0        0        0      306 2023-01-02 21:01:57.000000 ReverseBox-0.4.9/reversebox/io_files/bytes_handler.py
--rw-rw-rw-   0        0        0      951 2022-09-03 13:15:52.000000 ReverseBox-0.4.9/reversebox/io_files/check_file.py
--rw-rw-rw-   0        0        0     6621 2023-04-12 20:36:37.000000 ReverseBox-0.4.9/reversebox/io_files/file_handler.py
--rw-rw-rw-   0        0        0       42 2023-04-15 13:32:07.544533 ReverseBox-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0     1816 2023-04-15 09:57:04.000000 ReverseBox-0.4.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.534531 ReverseBox-0.4.9/tests/
--rw-rw-rw-   0        0        0        0 2022-07-19 22:27:10.000000 ReverseBox-0.4.9/tests/__init__.py
--rw-rw-rw-   0        0        0      626 2023-04-12 20:56:38.000000 ReverseBox-0.4.9/tests/common.py
-drwxrwxrwx   0        0        0        0 2023-04-15 13:32:07.543533 ReverseBox-0.4.9/tests/tests_crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:28:33.000000 ReverseBox-0.4.9/tests/tests_crc/__init__.py
--rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:08.000000 ReverseBox-0.4.9/tests/tests_crc/test_crc16_arc.py
--rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:08.000000 ReverseBox-0.4.9/tests/tests_crc/test_crc16_ccitt.py
--rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:08.000000 ReverseBox-0.4.9/tests/tests_crc/test_crc16_dnp.py
--rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:08.000000 ReverseBox-0.4.9/tests/tests_crc/test_crc16_kermit.py
--rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:08.000000 ReverseBox-0.4.9/tests/tests_crc/test_crc16_modbus.py
--rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:08.000000 ReverseBox-0.4.9/tests/tests_crc/test_crc16_sick.py
--rw-rw-rw-   0        0        0     2657 2023-01-09 18:34:08.000000 ReverseBox-0.4.9/tests/tests_crc/test_crc32_iso_hdlc.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.080831 ReverseBox-0.5.0/
+-rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:47.000000 ReverseBox-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     5602 2023-04-23 18:25:16.080246 ReverseBox-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4340 2023-04-22 15:45:22.000000 ReverseBox-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.028616 ReverseBox-0.5.0/ReverseBox.egg-info/
+-rw-rw-rw-   0        0        0     5602 2023-04-23 18:25:15.000000 ReverseBox-0.5.0/ReverseBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1805 2023-04-23 18:25:15.000000 ReverseBox-0.5.0/ReverseBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 18:25:15.000000 ReverseBox-0.5.0/ReverseBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-23 18:25:15.000000 ReverseBox-0.5.0/ReverseBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-23 18:25:15.000000 ReverseBox-0.5.0/ReverseBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.029616 ReverseBox-0.5.0/reversebox/
+-rw-rw-rw-   0        0        0        0 2022-06-25 12:19:26.000000 ReverseBox-0.5.0/reversebox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.033805 ReverseBox-0.5.0/reversebox/checksum/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.0/reversebox/checksum/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-01-08 20:51:07.000000 ReverseBox-0.5.0/reversebox/checksum/checksum_adler32.py
+-rw-rw-rw-   0        0        0      403 2023-01-09 21:19:57.000000 ReverseBox-0.5.0/reversebox/checksum/checksum_fletcher16.py
+-rw-rw-rw-   0        0        0      510 2023-01-09 22:41:53.000000 ReverseBox-0.5.0/reversebox/checksum/checksum_fletcher32.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.036806 ReverseBox-0.5.0/reversebox/common/
+-rw-rw-rw-   0        0        0        0 2022-06-25 16:29:13.000000 ReverseBox-0.5.0/reversebox/common/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-04-15 13:54:42.000000 ReverseBox-0.5.0/reversebox/common/common.py
+-rw-rw-rw-   0        0        0      730 2022-09-07 19:55:27.000000 ReverseBox-0.5.0/reversebox/common/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.041002 ReverseBox-0.5.0/reversebox/compression/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.0/reversebox/compression/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-04-23 00:00:01.000000 ReverseBox-0.5.0/reversebox/compression/compression_jcalg1.py
+-rw-rw-rw-   0        0        0      335 2022-12-27 14:56:59.000000 ReverseBox-0.5.0/reversebox/compression/compression_lzo.py
+-rw-rw-rw-   0        0        0      330 2022-10-15 10:41:38.000000 ReverseBox-0.5.0/reversebox/compression/compression_zlib.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.049185 ReverseBox-0.5.0/reversebox/crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:26:29.000000 ReverseBox-0.5.0/reversebox/crc/__init__.py
+-rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:19.000000 ReverseBox-0.5.0/reversebox/crc/crc16_arc.py
+-rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:31.000000 ReverseBox-0.5.0/reversebox/crc/crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:06.000000 ReverseBox-0.5.0/reversebox/crc/crc16_dnp.py
+-rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:19.000000 ReverseBox-0.5.0/reversebox/crc/crc16_kermit.py
+-rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:37.000000 ReverseBox-0.5.0/reversebox/crc/crc16_modbus.py
+-rw-rw-rw-   0        0        0      735 2022-07-21 21:35:31.000000 ReverseBox-0.5.0/reversebox/crc/crc16_sick.py
+-rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:19.000000 ReverseBox-0.5.0/reversebox/crc/crc32_iso_hdlc.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.053602 ReverseBox-0.5.0/reversebox/encryption/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.0/reversebox/encryption/__init__.py
+-rw-rw-rw-   0        0        0      579 2022-07-17 23:25:19.000000 ReverseBox-0.5.0/reversebox/encryption/encryption_xor_basic.py
+-rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:01.000000 ReverseBox-0.5.0/reversebox/encryption/encryption_xor_gianas_return_zda.py
+-rw-rw-rw-   0        0        0      574 2022-07-17 23:25:19.000000 ReverseBox-0.5.0/reversebox/encryption/encryption_xor_retro64_eco.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.057602 ReverseBox-0.5.0/reversebox/hash/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.0/reversebox/hash/__init__.py
+-rw-rw-rw-   0        0        0      280 2022-09-11 18:48:36.000000 ReverseBox-0.5.0/reversebox/hash/hash_md5.py
+-rw-rw-rw-   0        0        0      283 2023-01-08 14:05:01.000000 ReverseBox-0.5.0/reversebox/hash/hash_sha1.py
+-rw-rw-rw-   0        0        0      289 2023-01-08 14:07:31.000000 ReverseBox-0.5.0/reversebox/hash/hash_sha2.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.062076 ReverseBox-0.5.0/reversebox/image/
+-rw-rw-rw-   0        0        0        0 2022-12-27 21:18:24.000000 ReverseBox-0.5.0/reversebox/image/__init__.py
+-rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:19.000000 ReverseBox-0.5.0/reversebox/image/image_finder_gui.py
+-rw-rw-rw-   0        0        0      713 2023-04-23 00:00:01.000000 ReverseBox-0.5.0/reversebox/image/image_finder_main.py
+-rw-rw-rw-   0        0        0     1507 2023-04-15 13:20:43.000000 ReverseBox-0.5.0/reversebox/image/psp_swizzle.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.064621 ReverseBox-0.5.0/reversebox/io_files/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.5.0/reversebox/io_files/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-04-23 15:32:28.000000 ReverseBox-0.5.0/reversebox/io_files/bytes_handler.py
+-rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:49.000000 ReverseBox-0.5.0/reversebox/io_files/check_file.py
+-rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:41.000000 ReverseBox-0.5.0/reversebox/io_files/file_handler.py
+-rw-rw-rw-   0        0        0     5345 2023-04-23 18:16:41.000000 ReverseBox-0.5.0/reversebox/io_files/translation_text_handler.py
+-rw-rw-rw-   0        0        0       42 2023-04-23 18:25:16.080831 ReverseBox-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2023-04-23 18:15:14.000000 ReverseBox-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.064621 ReverseBox-0.5.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-19 22:27:10.000000 ReverseBox-0.5.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-04-12 20:56:38.000000 ReverseBox-0.5.0/tests/common.py
+drwxrwxrwx   0        0        0        0 2023-04-23 18:25:16.064621 ReverseBox-0.5.0/tests/tests_crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:28:33.000000 ReverseBox-0.5.0/tests/tests_crc/__init__.py
+-rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:08.000000 ReverseBox-0.5.0/tests/tests_crc/test_crc16_arc.py
+-rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:08.000000 ReverseBox-0.5.0/tests/tests_crc/test_crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:08.000000 ReverseBox-0.5.0/tests/tests_crc/test_crc16_dnp.py
+-rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:08.000000 ReverseBox-0.5.0/tests/tests_crc/test_crc16_kermit.py
+-rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:08.000000 ReverseBox-0.5.0/tests/tests_crc/test_crc16_modbus.py
+-rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:08.000000 ReverseBox-0.5.0/tests/tests_crc/test_crc16_sick.py
+-rw-rw-rw-   0        0        0     2655 2023-04-23 00:00:01.000000 ReverseBox-0.5.0/tests/tests_crc/test_crc32_iso_hdlc.py
```

### Comparing `ReverseBox-0.4.9/LICENSE` & `ReverseBox-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/PKG-INFO` & `ReverseBox-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.4.9
+Version: 0.5.0
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -104,14 +104,15 @@
   - PSP Swizzling/Twiddling ✔️
   - [SourceSDK Swizzling](https://forum.xentax.com/viewtopic.php?p=139510#p139510) (TODO) ❌
 
 * IO
   - File Reader ✔️
   - File Writer ✔️
   - Bytes Handler ✔️
+  - Translation Text Handler ✔️
   - File extension checking ✔️
   - Padding calculation ✔️
   - File size checking ✔️
 
 # Checksum calculation - example
 
 // CRC32 calculation
@@ -184,7 +185,15 @@
 print("SHA-1 hash: ", sha1)
 ```
 
 // SHA-1 Output
 ```
 SHA-1 hash:  b'\x81\xfe\x8b\xfe\x87Wl>\xcb"Bo\x8eW\x84s\x82\x91z\xcf'
 ```
+
+# More Examples
+
+Need more examples? <br>
+Check out list of tools written using ReverseBox:
+- [Giana's Return ZDA Tool](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/Gianas%20Return/Gianas_Return_ZDA_Tool.py)
+- [ObsCure 2 HVP Extractor](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/ObsCure%202/ObsCure%202%20HVP%20Tools/Obscure_2_hvp_extractor.py)
+- and more...
```

### Comparing `ReverseBox-0.4.9/README.md` & `ReverseBox-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -75,14 +75,15 @@
   - PSP Swizzling/Twiddling ✔️
   - [SourceSDK Swizzling](https://forum.xentax.com/viewtopic.php?p=139510#p139510) (TODO) ❌
 
 * IO
   - File Reader ✔️
   - File Writer ✔️
   - Bytes Handler ✔️
+  - Translation Text Handler ✔️
   - File extension checking ✔️
   - Padding calculation ✔️
   - File size checking ✔️
 
 # Checksum calculation - example
 
 // CRC32 calculation
@@ -155,7 +156,15 @@
 print("SHA-1 hash: ", sha1)
 ```
 
 // SHA-1 Output
 ```
 SHA-1 hash:  b'\x81\xfe\x8b\xfe\x87Wl>\xcb"Bo\x8eW\x84s\x82\x91z\xcf'
 ```
+
+# More Examples
+
+Need more examples? <br>
+Check out list of tools written using ReverseBox:
+- [Giana's Return ZDA Tool](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/Gianas%20Return/Gianas_Return_ZDA_Tool.py)
+- [ObsCure 2 HVP Extractor](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/ObsCure%202/ObsCure%202%20HVP%20Tools/Obscure_2_hvp_extractor.py)
+- and more...
```

### Comparing `ReverseBox-0.4.9/ReverseBox.egg-info/PKG-INFO` & `ReverseBox-0.5.0/ReverseBox.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.4.9
+Version: 0.5.0
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -104,14 +104,15 @@
   - PSP Swizzling/Twiddling ✔️
   - [SourceSDK Swizzling](https://forum.xentax.com/viewtopic.php?p=139510#p139510) (TODO) ❌
 
 * IO
   - File Reader ✔️
   - File Writer ✔️
   - Bytes Handler ✔️
+  - Translation Text Handler ✔️
   - File extension checking ✔️
   - Padding calculation ✔️
   - File size checking ✔️
 
 # Checksum calculation - example
 
 // CRC32 calculation
@@ -184,7 +185,15 @@
 print("SHA-1 hash: ", sha1)
 ```
 
 // SHA-1 Output
 ```
 SHA-1 hash:  b'\x81\xfe\x8b\xfe\x87Wl>\xcb"Bo\x8eW\x84s\x82\x91z\xcf'
 ```
+
+# More Examples
+
+Need more examples? <br>
+Check out list of tools written using ReverseBox:
+- [Giana's Return ZDA Tool](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/Gianas%20Return/Gianas_Return_ZDA_Tool.py)
+- [ObsCure 2 HVP Extractor](https://github.com/bartlomiejduda/Tools/blob/master/NEW%20Tools/ObsCure%202/ObsCure%202%20HVP%20Tools/Obscure_2_hvp_extractor.py)
+- and more...
```

### Comparing `ReverseBox-0.4.9/ReverseBox.egg-info/SOURCES.txt` & `ReverseBox-0.5.0/ReverseBox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 reversebox/image/image_finder_gui.py
 reversebox/image/image_finder_main.py
 reversebox/image/psp_swizzle.py
 reversebox/io_files/__init__.py
 reversebox/io_files/bytes_handler.py
 reversebox/io_files/check_file.py
 reversebox/io_files/file_handler.py
+reversebox/io_files/translation_text_handler.py
 tests/__init__.py
 tests/common.py
 tests/tests_crc/__init__.py
 tests/tests_crc/test_crc16_arc.py
 tests/tests_crc/test_crc16_ccitt.py
 tests/tests_crc/test_crc16_dnp.py
 tests/tests_crc/test_crc16_kermit.py
```

### Comparing `ReverseBox-0.4.9/reversebox/common/logger.py` & `ReverseBox-0.5.0/reversebox/common/logger.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/crc/crc16_arc.py` & `ReverseBox-0.5.0/reversebox/crc/crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/crc/crc16_ccitt.py` & `ReverseBox-0.5.0/reversebox/crc/crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/crc/crc16_dnp.py` & `ReverseBox-0.5.0/reversebox/crc/crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/crc/crc16_kermit.py` & `ReverseBox-0.5.0/reversebox/crc/crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/crc/crc16_modbus.py` & `ReverseBox-0.5.0/reversebox/crc/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/crc/crc16_sick.py` & `ReverseBox-0.5.0/reversebox/crc/crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/crc/crc32_iso_hdlc.py` & `ReverseBox-0.5.0/reversebox/crc/crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/encryption/encryption_xor_basic.py` & `ReverseBox-0.5.0/reversebox/encryption/encryption_xor_basic.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/encryption/encryption_xor_gianas_return_zda.py` & `ReverseBox-0.5.0/reversebox/encryption/encryption_xor_gianas_return_zda.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/encryption/encryption_xor_retro64_eco.py` & `ReverseBox-0.5.0/reversebox/encryption/encryption_xor_retro64_eco.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/image/image_finder_gui.py` & `ReverseBox-0.5.0/reversebox/image/image_finder_gui.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/image/image_finder_main.py` & `ReverseBox-0.5.0/reversebox/image/image_finder_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 logger = get_logger(__name__)
 
 MAIN_DIRECTORY = os.path.dirname(os.path.abspath(__file__))
 
 
 def run_image_finder() -> int:
-
     logger.info("Starting image finder...")
 
     root = tk.Tk()
     ImageFinderGUI(root, "v0.1", MAIN_DIRECTORY)  # start GUI
     root.lift()
     center_tk_window.center_on_screen(root)
     root.mainloop()
```

### Comparing `ReverseBox-0.4.9/reversebox/image/psp_swizzle.py` & `ReverseBox-0.5.0/reversebox/image/psp_swizzle.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/reversebox/io_files/check_file.py` & `ReverseBox-0.5.0/reversebox/io_files/check_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Copyright © 2023  Bartłomiej Duda
+License: GPL-3.0 License
+"""
+
 import os
 from typing import Tuple
 
 
 def check_file(
     in_file_path: str,
     expected_extension: str,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ReverseBox-0.4.9/reversebox/io_files/file_handler.py` & `ReverseBox-0.5.0/reversebox/io_files/file_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Copyright © 2023  Bartłomiej Duda
+License: GPL-3.0 License
+"""
+import os
 import struct
 from io import BufferedReader
 from typing import Optional
 
 # mypy: ignore-errors
 from reversebox.common.logger import get_logger
 
@@ -13,17 +18,30 @@
         self.file_path = file_path
         self.open_mode = open_mode
         self.endianess = self._get_endianess(endianess_str)
 
         self.file: Optional[BufferedReader] = None
 
     def open(self) -> bool:
-        self.file = open(self.file_path, self.open_mode)
+        error_message = "File can't be opened!"
+        if "r" in self.open_mode:
+            if not self.check_if_file_is_readable():
+                raise Exception(error_message)
+        if "w" in self.open_mode:
+            if not self.check_if_file_is_writable():
+                raise Exception(error_message)
+
+        try:
+            self.file = open(self.file_path, self.open_mode)
+        except OSError as error:
+            error_message += " Error: " + str(error)
+            logger.error(error_message)
+            raise Exception(error_message)
+
         if not self.file:
-            error_message = "File can't be opened!"
             logger.error(error_message)
             raise Exception(error_message)
         return True
 
     def close(self) -> bool:
         self.file.close()
         return True
@@ -61,51 +79,78 @@
     def _check_read_mode(self) -> bool:
         if "r" not in self.open_mode:
             error_message = 'Wrong file open mode! You need to specify one of the "read" open modes!'
             logger.error(error_message)
             raise Exception(error_message)
         return True
 
+    def check_if_file_is_readable(self) -> bool:
+        if not os.access(self.file_path, os.R_OK):
+            error_message = "Can't read from this file!"
+            logger.error(error_message)
+            raise Exception(error_message)
+        return True
+
     def _check_write_mode(self) -> bool:
-        if "w" not in self.open_mode:
+        if "w" not in self.open_mode and "a" not in self.open_mode:
             error_message = 'Wrong file open mode! You need to specify one of the "write" open modes!'
             logger.error(error_message)
             raise Exception(error_message)
         return True
 
+    def check_if_file_is_writable(self) -> bool:
+        if os.path.exists(self.file_path):
+            if os.path.isfile(self.file_path):
+                return os.access(self.file_path, os.W_OK)
+            else:
+                return False
+        pdir = os.path.dirname(self.file_path)
+        if not pdir:
+            pdir = "."
+        return os.access(pdir, os.W_OK)
+
     def seek(self, seek_value, seek_type: int = 0):
         # 0 = SEEK_SET (from file start)
         # 1 = SEEK_CUR (from current offset)
         # 2 = SEEK_END (from file end)
         self._check_file()
         self.file.seek(seek_value, seek_type)
 
     def get_position(self) -> int:
         self._check_file()
         return self.file.tell()
 
     def get_file_size(self) -> int:
         current_position = self.get_position()
         self.seek(0, 2)
-        end_of_file__position = self.get_position()
+        end_of_file_position = self.get_position()
         self.seek(current_position, 0)
-        return end_of_file__position
+        return end_of_file_position
 
     def read_str(self, str_length: int, encoding: str = "utf8") -> str:
         self._check_file()
         self._check_read_mode()
         data = self.file.read(str_length)
         return data.decode(encoding)
 
     def read_bytes(self, number_of_bytes: int) -> bytes:
         self._check_file()
         self._check_read_mode()
         data = self.file.read(number_of_bytes)
         return data
 
+    def read_whole_file_content(self) -> bytes:
+        self._check_file()
+        self._check_read_mode()
+        current_position = self.get_position()
+        self.seek(0)
+        data = self.file.read()
+        self.seek(current_position)
+        return data
+
     def read_uint32(self) -> int:
         self._check_file()
         self._check_read_mode()
         data = self.file.read(4)
         return struct.unpack(self.endianess + "L", data)[0]
 
     def read_int32(self) -> int:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ReverseBox-0.4.9/setup.py` & `ReverseBox-0.5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
-Copyright © 2022  Bartłomiej Duda
+Copyright © 2023  Bartłomiej Duda
 License: GPL-3.0 License
 """
 
 import os
 
 import setuptools
 
-VERSION_NUM = "0.4.9"
+VERSION_NUM = "0.5.0"
 
 
 def get_long_description() -> str:
     with open(
         os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf8"
     ) as readme:
         readme_text = readme.read()
@@ -45,10 +45,10 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Natural Language :: English",
     ],
     test_suite="tests",
     keywords="ReverseBox, reverse engineering, RE, CRC, Hash, Encryption, Compression, Checksum, Python",
     python_requires=">=3.6",
-    install_requires=["lzokay"],
+    install_requires=["lzokay", "polib"],
     packages=setuptools.find_packages(),
 )
```

### Comparing `ReverseBox-0.4.9/tests/common.py` & `ReverseBox-0.5.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/tests/tests_crc/test_crc16_arc.py` & `ReverseBox-0.5.0/tests/tests_crc/test_crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/tests/tests_crc/test_crc16_ccitt.py` & `ReverseBox-0.5.0/tests/tests_crc/test_crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/tests/tests_crc/test_crc16_dnp.py` & `ReverseBox-0.5.0/tests/tests_crc/test_crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/tests/tests_crc/test_crc16_kermit.py` & `ReverseBox-0.5.0/tests/tests_crc/test_crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/tests/tests_crc/test_crc16_modbus.py` & `ReverseBox-0.5.0/tests/tests_crc/test_crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/tests/tests_crc/test_crc16_sick.py` & `ReverseBox-0.5.0/tests/tests_crc/test_crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.4.9/tests/tests_crc/test_crc32_iso_hdlc.py` & `ReverseBox-0.5.0/tests/tests_crc/test_crc32_iso_hdlc.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         test_result_str = convert_int_to_hex_string(test_result)
         assert test_result == crc_entry.expected_int
         assert test_result_str == crc_entry.expected_str
 
 
 @pytest.mark.unittest
 def test_crc_calculate_crc32_iso_hdlc_to_match_zlib_result():
-
     test_data_array = [
         b"",
         b" ",
         b"123456789",
         b"123",
         b"Hello Python",
         b"Secret123@123#!",
```

