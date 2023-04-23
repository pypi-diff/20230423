# Comparing `tmp/ok-dmrlib-0.7.tar.gz` & `tmp/ok_dmrlib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ok-dmrlib-0.7.tar", last modified: Sun Nov 13 08:57:15 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `ok-dmrlib-0.7.tar` & `ok_dmrlib-0.8.0.tar`

### file list

```diff
@@ -1,143 +1,131 @@
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.489118 ok-dmrlib-0.7/
--rw-r--r--   0 smarek    (1000) smarek    (1000)    34535 2021-11-21 14:02:25.000000 ok-dmrlib-0.7/LICENSE
--rw-r--r--   0 smarek    (1000) smarek    (1000)    10540 2022-11-13 08:57:15.489118 ok-dmrlib-0.7/PKG-INFO
--rw-r--r--   0 smarek    (1000) smarek    (1000)     9693 2022-11-13 08:52:52.000000 ok-dmrlib-0.7/README.md
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.473117 ok-dmrlib-0.7/ok_dmrlib.egg-info/
--rw-r--r--   0 smarek    (1000) smarek    (1000)    10540 2022-11-13 08:57:15.000000 ok-dmrlib-0.7/ok_dmrlib.egg-info/PKG-INFO
--rw-r--r--   0 smarek    (1000) smarek    (1000)     5131 2022-11-13 08:57:15.000000 ok-dmrlib-0.7/ok_dmrlib.egg-info/SOURCES.txt
--rw-r--r--   0 smarek    (1000) smarek    (1000)        1 2022-11-13 08:57:15.000000 ok-dmrlib-0.7/ok_dmrlib.egg-info/dependency_links.txt
--rw-r--r--   0 smarek    (1000) smarek    (1000)       80 2022-11-13 08:57:15.000000 ok-dmrlib-0.7/ok_dmrlib.egg-info/entry_points.txt
--rw-r--r--   0 smarek    (1000) smarek    (1000)       59 2022-11-13 08:57:15.000000 ok-dmrlib-0.7/ok_dmrlib.egg-info/requires.txt
--rw-r--r--   0 smarek    (1000) smarek    (1000)        6 2022-11-13 08:57:15.000000 ok-dmrlib-0.7/ok_dmrlib.egg-info/top_level.txt
--rw-r--r--   0 smarek    (1000) smarek    (1000)        1 2022-06-28 21:33:59.000000 ok-dmrlib-0.7/ok_dmrlib.egg-info/zip-safe
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.469117 ok-dmrlib-0.7/okdmr/
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.473117 ok-dmrlib-0.7/okdmr/dmrlib/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2021-11-20 09:31:46.000000 ok-dmrlib-0.7/okdmr/dmrlib/__init__.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.473117 ok-dmrlib-0.7/okdmr/dmrlib/etsi/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2021-11-30 21:51:21.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/__init__.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.473117 ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2021-12-03 11:47:48.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    10368 2022-08-16 16:57:14.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/crc.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1348 2022-03-08 19:40:02.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/crc16.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1214 2022-02-02 14:53:13.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/crc32.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1053 2022-02-03 18:12:28.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/crc8.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1701 2022-07-13 20:09:37.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/crc9.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.477118 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2021-11-30 23:31:37.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    16048 2022-03-23 17:11:05.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/bptc_196_96.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      566 2021-12-08 19:18:56.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/fec_utils.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1171 2021-12-03 13:52:30.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/five_bit_checksum.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     2076 2021-12-03 11:28:32.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/golay_20_8_7.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1090 2022-02-02 14:39:48.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_13_9_3.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1264 2022-02-02 14:39:50.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_15_11_3.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1300 2022-02-02 14:39:52.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_16_11_4.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1357 2022-02-02 14:43:50.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_17_12_3.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      705 2022-02-02 14:39:45.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_7_4_3.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     2863 2022-03-08 20:59:23.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_common.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     2088 2021-12-03 13:04:54.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/quadratic_residue_16_7_6.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     7120 2022-02-03 21:44:57.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/reed_solomon_12_9_4.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     8828 2022-03-09 10:43:36.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/trellis.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    14503 2022-03-05 17:36:11.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/vbptc_128_72.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     8025 2022-07-03 16:44:47.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/vbptc_32_11.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    12159 2022-08-16 16:56:18.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/vbptc_68_28.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.477118 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2021-11-30 21:51:32.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    12833 2022-11-07 11:08:09.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/burst.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.481118 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/
--rw-r--r--   0 smarek    (1000) smarek    (1000)       57 2022-02-07 10:08:43.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      335 2022-07-30 12:05:31.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/access_types.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      225 2022-07-30 12:05:31.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/burst_types.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      452 2022-07-30 12:05:31.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/crc_masks.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     3405 2022-07-30 12:06:31.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/csbk_opcodes.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1066 2022-07-30 12:05:31.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/data_packet_formats.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      726 2022-07-30 12:03:15.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/data_types.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1611 2022-07-30 12:05:31.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/defined_data_formats.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     2525 2022-07-30 13:11:28.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/feature_set_ids.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1044 2022-03-03 21:34:01.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/flcos.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1583 2022-08-16 16:55:34.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/fragment_sequence_number.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      365 2022-03-08 08:25:01.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/full_message_flag.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      256 2022-02-02 22:52:29.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/lcss.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      268 2022-02-03 16:18:45.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/preemption_power_indicator.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      372 2022-03-08 08:25:01.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/resynchronize_flag.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      915 2022-03-08 10:44:16.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/sap_identifier.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      323 2022-07-30 12:06:39.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/sarq.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1140 2022-07-30 12:06:47.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/slcos.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      347 2022-03-08 13:12:40.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/supplementary_flag.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1264 2022-03-09 10:43:48.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/sync_patterns.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      907 2022-03-08 13:06:21.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/udt_format.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      556 2022-07-30 13:11:28.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/voice_bursts.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.481118 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/
--rw-r--r--   0 smarek    (1000) smarek    (1000)      121 2022-02-07 10:08:43.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    15956 2022-07-13 11:23:52.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/csbk.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    16601 2022-09-09 08:12:41.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/data_header.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     3335 2022-07-13 07:20:57.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/embedded_signalling.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     8585 2022-04-20 10:11:56.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/full_link_control.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1223 2022-03-12 00:08:56.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/pi_header.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     6656 2022-09-08 20:04:50.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/rate12_data.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     6671 2022-07-13 20:58:34.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/rate1_data.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     7000 2022-07-13 20:58:47.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/rate34_data.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     3429 2022-03-08 20:59:23.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/short_link_control.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     2296 2022-02-28 12:46:09.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/slot_type.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.481118 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2022-02-07 15:58:33.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/__init__.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.485118 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2022-02-07 15:58:48.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1195 2022-07-30 12:05:32.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/activity_id.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      371 2022-07-30 12:07:26.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/additional_information_field.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      727 2022-07-30 12:07:34.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/answer_response.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      897 2022-07-30 12:07:40.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/channel_timing_opcode.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      786 2022-07-30 12:07:46.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/dynamic_identifier.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1166 2022-08-16 15:59:38.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/ip_address_identifier.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      847 2022-07-30 12:07:53.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/position_error.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      670 2022-07-30 12:07:59.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/reason_code.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     2234 2022-03-08 20:49:52.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/service_options.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      313 2022-07-30 12:10:56.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/source_type.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      845 2022-07-30 12:11:13.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/talker_alias_data_format.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1428 2022-09-08 20:27:15.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/udp_port_identifier.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      240 2022-07-30 12:11:31.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/udt_option_flag.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.485118 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/pdu/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2022-02-07 15:58:54.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/pdu/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     6408 2022-11-07 11:32:43.000000 ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/pdu/udp_ipv4_compressed_header.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.485118 ok-dmrlib-0.7/okdmr/dmrlib/hytera/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2022-02-14 09:48:38.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      597 2022-02-25 10:17:52.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/hytera_constants.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1877 2022-08-14 23:43:51.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/hytera_ipsc_sync.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1364 2022-02-18 16:33:06.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/hytera_ipsc_wakeup.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.485118 ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2022-06-25 08:17:13.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     3583 2022-11-13 08:53:05.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/hdap.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     5425 2022-11-06 15:23:13.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/hrnp.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     8758 2022-11-07 11:30:57.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/hstrp.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     8668 2022-11-12 13:58:11.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/location_protocol.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     9948 2022-11-12 13:58:17.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/radio_control_protocol.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1637 2022-11-06 12:02:44.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/radio_ip.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     4463 2022-11-12 13:58:20.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/radio_registration_service.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     7010 2022-11-13 08:53:05.000000 ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/text_message_protocol.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.485118 ok-dmrlib-0.7/okdmr/dmrlib/motorola/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2022-07-07 07:32:03.000000 ok-dmrlib-0.7/okdmr/dmrlib/motorola/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      442 2022-07-13 11:21:35.000000 ok-dmrlib-0.7/okdmr/dmrlib/motorola/arrp.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    15399 2022-11-07 11:30:57.000000 ok-dmrlib-0.7/okdmr/dmrlib/motorola/automatic_registration_service.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     8896 2022-08-16 14:08:27.000000 ok-dmrlib-0.7/okdmr/dmrlib/motorola/lrrp.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    35786 2022-11-07 11:52:10.000000 ok-dmrlib-0.7/okdmr/dmrlib/motorola/mbxml.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    11684 2022-11-12 12:02:10.000000 ok-dmrlib-0.7/okdmr/dmrlib/motorola/text_messaging_service.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.485118 ok-dmrlib-0.7/okdmr/dmrlib/tools/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2022-02-23 11:45:17.000000 ok-dmrlib-0.7/okdmr/dmrlib/tools/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    19393 2022-11-12 12:02:10.000000 ok-dmrlib-0.7/okdmr/dmrlib/tools/pcap_tool.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.489118 ok-dmrlib-0.7/okdmr/dmrlib/transmission/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2021-12-21 10:00:13.000000 ok-dmrlib-0.7/okdmr/dmrlib/transmission/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1578 2022-08-15 08:45:13.000000 ok-dmrlib-0.7/okdmr/dmrlib/transmission/terminal.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     2854 2022-06-28 22:56:20.000000 ok-dmrlib-0.7/okdmr/dmrlib/transmission/timeslot.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)    11685 2022-11-12 12:02:10.000000 ok-dmrlib-0.7/okdmr/dmrlib/transmission/transmission.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1946 2022-07-13 09:01:55.000000 ok-dmrlib-0.7/okdmr/dmrlib/transmission/transmission_generator.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     3800 2022-08-16 15:08:48.000000 ok-dmrlib-0.7/okdmr/dmrlib/transmission/transmission_observer_interface.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      127 2022-01-31 18:31:51.000000 ok-dmrlib-0.7/okdmr/dmrlib/transmission/transmission_types.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     2881 2022-07-13 21:31:41.000000 ok-dmrlib-0.7/okdmr/dmrlib/transmission/transmission_watcher.py
-drwxr-xr-x   0 smarek    (1000) smarek    (1000)        0 2022-11-13 08:57:15.489118 ok-dmrlib-0.7/okdmr/dmrlib/utils/
--rw-r--r--   0 smarek    (1000) smarek    (1000)        0 2021-11-30 22:32:37.000000 ok-dmrlib-0.7/okdmr/dmrlib/utils/__init__.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     2001 2022-03-08 08:25:01.000000 ok-dmrlib-0.7/okdmr/dmrlib/utils/bits_bytes.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      380 2022-02-03 21:13:25.000000 ok-dmrlib-0.7/okdmr/dmrlib/utils/bits_interface.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      726 2022-11-07 11:30:57.000000 ok-dmrlib-0.7/okdmr/dmrlib/utils/bytes_interface.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)      505 2021-12-21 10:36:31.000000 ok-dmrlib-0.7/okdmr/dmrlib/utils/logging_trait.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)     3041 2022-08-28 08:04:59.000000 ok-dmrlib-0.7/okdmr/dmrlib/utils/parsing.py
--rw-r--r--   0 smarek    (1000) smarek    (1000)       38 2022-11-13 08:57:15.489118 ok-dmrlib-0.7/setup.cfg
--rw-r--r--   0 smarek    (1000) smarek    (1000)     1968 2022-11-13 08:56:38.000000 ok-dmrlib-0.7/setup.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/.yamllint
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/Makefile
+-rw-r--r--   0        0        0    10379 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/README.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/crc/__init__.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/crc/crc.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/crc/crc16.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/crc/crc32.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/crc/crc8.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/crc/crc9.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/__init__.py
+-rw-r--r--   0        0        0    16048 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/bptc_196_96.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/fec_utils.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/five_bit_checksum.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/golay_20_8_7.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_13_9_3.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_15_11_3.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_16_11_4.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_17_12_3.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_7_4_3.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_common.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/quadratic_residue_16_7_6.py
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/reed_solomon_12_9_4.py
+-rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/trellis.py
+-rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/vbptc_128_72.py
+-rw-r--r--   0        0        0     8025 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/vbptc_32_11.py
+-rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/vbptc_68_28.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/__init__.py
+-rw-r--r--   0        0        0    13015 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/burst.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/access_types.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/burst_types.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/crc_masks.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/csbk_opcodes.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/data_packet_formats.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/data_types.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/defined_data_formats.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/feature_set_ids.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/flcos.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/fragment_sequence_number.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/full_message_flag.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/lcss.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/preemption_power_indicator.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/resynchronize_flag.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/sap_identifier.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/sarq.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/slcos.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/supplementary_flag.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/sync_patterns.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/udt_format.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/voice_bursts.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/__init__.py
+-rw-r--r--   0        0        0    22652 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/csbk.py
+-rw-r--r--   0        0        0    17071 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/data_header.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/embedded_signalling.py
+-rw-r--r--   0        0        0     9067 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/full_link_control.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/pi_header.py
+-rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/rate12_data.py
+-rw-r--r--   0        0        0     6830 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/rate1_data.py
+-rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/rate34_data.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/short_link_control.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/slot_type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/activity_id.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/additional_information_field.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/announcement_type.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/answer_response.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/channel_timing_opcode.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/dynamic_identifier.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/ip_address_identifier.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/position_error.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/random_access_service_function.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/reason_code.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/service_options.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/source_type.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/talker_alias_data_format.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/udp_port_identifier.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/udt_option_flag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/pdu/__init__.py
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/pdu/udp_ipv4_compressed_header.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/__init__.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/hytera_constants.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/hytera_ipsc_sync.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/hytera_ipsc_wakeup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/__init__.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/hdap.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/hrnp.py
+-rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/hstrp.py
+-rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/location_protocol.py
+-rw-r--r--   0        0        0    27840 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/radio_control_protocol.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/radio_ip.py
+-rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/radio_registration_service.py
+-rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/text_message_protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/motorola/__init__.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/motorola/arrp.py
+-rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/motorola/automatic_registration_service.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/motorola/lrrp.py
+-rw-r--r--   0        0        0    37400 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/motorola/mbxml.py
+-rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/motorola/text_messaging_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/protocols/hytera/__init__.py
+-rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/protocols/hytera/hstrp_datagram_protocol.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/protocols/hytera/rrs_datagram_protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/protocols/motorola/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/tools/__init__.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/tools/dmrlib_tool.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/tools/hrnp_client.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/tools/hytera_tool.py
+-rw-r--r--   0        0        0    19480 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/tools/pcap_tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/terminal.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/timeslot.py
+-rw-r--r--   0        0        0    11696 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/transmission.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/transmission_generator.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/transmission_observer_interface.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/transmission_types.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/transmission_watcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/utils/__init__.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/utils/bits_bytes.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/utils/bits_interface.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/utils/bytes_interface.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/utils/logging_trait.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/utils/parsing.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/okdmr/dmrlib/utils/protocol_tool.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/.gitignore
+-rw-r--r--   0        0        0    34535 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 ok_dmrlib-0.8.0/PKG-INFO
```

### Comparing `ok-dmrlib-0.7/LICENSE` & `ok_dmrlib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/PKG-INFO` & `ok_dmrlib-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 Metadata-Version: 2.1
 Name: ok-dmrlib
-Version: 0.7
-Summary: Parse, assemble and handle DMR data
-Home-page: https://github.com/OK-DMR/ok-dmrlib
-Author: Marek Sebera
-Author-email: marek.sebera@gmail.com
+Version: 0.8.0
+Summary: DMR PDUs, elements, FEC and CRC library, including proprietary DMR protocols of Hytera and Motorola
+Project-URL: repository, https://github.com/OK-DMR/ok-dmrlib
+Author-email: Marek Sebera <marek.sebera@gmail.com>
 License: AGPL-3.0
-Keywords: dmr etsi ham mmdvm homebrew radio hytera motorola
+License-File: LICENSE
+Keywords: dmr,etsi,ham,homebrew,hytera,mmdvm,motorola,radio
 Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Environment :: Console
-Classifier: Topic :: Communications :: Ham Radio
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Typing :: Typed
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Telecommunications Industry
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Communications :: Ham Radio
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
+Requires-Dist: asyncio>=3.4.0
+Requires-Dist: bitarray>=2.7
+Requires-Dist: dmr-kaitai>=1.0
+Requires-Dist: numpy>=1.24.0
+Requires-Dist: scapy>=2.4.0
+Provides-Extra: pre-commit
+Requires-Dist: pre-commit>=3.0.0; extra == 'pre-commit'
+Provides-Extra: test
+Requires-Dist: crc>=4.0.0; extra == 'test'
+Requires-Dist: pytest-asyncio>=0.20.0; extra == 'test'
+Requires-Dist: pytest-cov>=4.0.0; extra == 'test'
+Requires-Dist: pytest>=7.0.0; extra == 'test'
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # OK-DMR Lib
 
-[![.github/workflows/sanity.yml](https://img.shields.io/github/workflow/status/OK-DMR/ok-dmrlib/Sanity?style=flat-square)](https://github.com/OK-DMR/ok-dmrlib/actions)
+[![.github/workflows/sanity.yml](https://img.shields.io/github/actions/workflow/status/OK-DMR/ok-dmrlib/sanity.yml?style=flat-square&branch=master)](https://github.com/OK-DMR/ok-dmrlib/actions)
 [![Code Style: Python Black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![License](https://img.shields.io/github/license/OK-DMR/ok-dmrlib?style=flat-square)](https://github.com/OK-DMR/ok-dmrlib/blob/master/LICENSE)
 [![Last released version](https://img.shields.io/pypi/v/ok-dmrlib?style=flat-square)](https://pypi.org/project/ok-dmrlib/)
 [![PyPI downloads](https://img.shields.io/pypi/dd/ok-dmrlib?style=flat-square)](https://libraries.io/pypi/ok-dmrlib)
 [![Python versions](https://img.shields.io/pypi/pyversions/ok-dmrlib?style=flat-square)](https://pypi.org/project/ok-dmrlib/)
 [![Wheel](https://img.shields.io/pypi/wheel/ok-dmrlib?style=flat-square)](https://pypi.org/project/ok-dmrlib/#files)
 [![Codecov](https://img.shields.io/codecov/c/github/ok-dmr/ok-dmrlib?style=flat-square)](https://app.codecov.io/gh/OK-DMR/ok-dmrlib)
@@ -121,14 +132,28 @@
 - Motorola has MBXML (Motorola Binary XML) which is used to represent LRRP/ARRP documents, ok-dmrlib contains abstract
   MBXML implementation with various tools, LRRP implementation tested with both examples and real-world data
 - LRRP is supported as `[bytes] <-> [mbxml document(s)] -> [xml representation]`, currently serialization of xml
   document to bytes is not supported
 - There are some catches, when you want to serialize MBXML token with common name, look through the test_mbxml and
   test_lrrp modules, to see how to select specific (correct) token programatically
 
+### Available CLI tools
+
+- dmrlib-pcap-tool - PCAP/PCAPNG traffic description and data extraction
+- dmrlib-dmr-burst - Describe full Tier-II burst (33 bytes)
+- dmrlib-dmr-header - Describe DMR Data Header
+- dmrlib-dmr-ipudp - Describe DMR UDP/IPv4 Compressed data (header + user payload)
+- dmrlib-hytera-hstrp - Hytera Simple Transport Protocol
+- dmrlib-hytera-hdap - Hytera DMR Application Protocol
+- dmrlib-hytera-hrnp - Hytera Radio Network Protocol
+- dmrlib-hytera-lp - Hytera Location Protocol
+- dmrlib-hytera-rcp - Hytera Radio Control Protocol
+- dmrlib-hytera-rrs - Hytera Radio Registration Service
+- dmrlib-hytera-tmp - Hytera Text Message Protocol
+
 ### Additional notes
 
 - Almost every class/enum supports BitsInterface (de-serialization from on-air bits, serialization to transmission bits)
   , or for byte-aligned protocols (Hytera, Motorola) BytesInterface (with explicit endianness support)
 - Every FEC/CRC implemented supports both calculation, verification and (if possible) also self-correction
 - Working with Vocoder and Data/Control Bursts is supported, along with handling rates 1, 1/2 and 3/4
 - CRCs interface classes may require appropriate CRC Mask to be provided when generating or verifying
```

### Comparing `ok-dmrlib-0.7/README.md` & `ok_dmrlib-0.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # OK-DMR Lib
 
-[![.github/workflows/sanity.yml](https://img.shields.io/github/workflow/status/OK-DMR/ok-dmrlib/Sanity?style=flat-square)](https://github.com/OK-DMR/ok-dmrlib/actions)
+[![.github/workflows/sanity.yml](https://img.shields.io/github/actions/workflow/status/OK-DMR/ok-dmrlib/sanity.yml?style=flat-square&branch=master)](https://github.com/OK-DMR/ok-dmrlib/actions)
 [![Code Style: Python Black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![License](https://img.shields.io/github/license/OK-DMR/ok-dmrlib?style=flat-square)](https://github.com/OK-DMR/ok-dmrlib/blob/master/LICENSE)
 [![Last released version](https://img.shields.io/pypi/v/ok-dmrlib?style=flat-square)](https://pypi.org/project/ok-dmrlib/)
 [![PyPI downloads](https://img.shields.io/pypi/dd/ok-dmrlib?style=flat-square)](https://libraries.io/pypi/ok-dmrlib)
 [![Python versions](https://img.shields.io/pypi/pyversions/ok-dmrlib?style=flat-square)](https://pypi.org/project/ok-dmrlib/)
 [![Wheel](https://img.shields.io/pypi/wheel/ok-dmrlib?style=flat-square)](https://pypi.org/project/ok-dmrlib/#files)
 [![Codecov](https://img.shields.io/codecov/c/github/ok-dmr/ok-dmrlib?style=flat-square)](https://app.codecov.io/gh/OK-DMR/ok-dmrlib)
@@ -98,21 +98,35 @@
 - Motorola has MBXML (Motorola Binary XML) which is used to represent LRRP/ARRP documents, ok-dmrlib contains abstract
   MBXML implementation with various tools, LRRP implementation tested with both examples and real-world data
 - LRRP is supported as `[bytes] <-> [mbxml document(s)] -> [xml representation]`, currently serialization of xml
   document to bytes is not supported
 - There are some catches, when you want to serialize MBXML token with common name, look through the test_mbxml and
   test_lrrp modules, to see how to select specific (correct) token programatically
 
+### Available CLI tools
+
+- dmrlib-pcap-tool - PCAP/PCAPNG traffic description and data extraction
+- dmrlib-dmr-burst - Describe full Tier-II burst (33 bytes)
+- dmrlib-dmr-header - Describe DMR Data Header
+- dmrlib-dmr-ipudp - Describe DMR UDP/IPv4 Compressed data (header + user payload)
+- dmrlib-hytera-hstrp - Hytera Simple Transport Protocol
+- dmrlib-hytera-hdap - Hytera DMR Application Protocol
+- dmrlib-hytera-hrnp - Hytera Radio Network Protocol
+- dmrlib-hytera-lp - Hytera Location Protocol
+- dmrlib-hytera-rcp - Hytera Radio Control Protocol
+- dmrlib-hytera-rrs - Hytera Radio Registration Service
+- dmrlib-hytera-tmp - Hytera Text Message Protocol
+
 ### Additional notes
 
 - Almost every class/enum supports BitsInterface (de-serialization from on-air bits, serialization to transmission bits)
   , or for byte-aligned protocols (Hytera, Motorola) BytesInterface (with explicit endianness support)
 - Every FEC/CRC implemented supports both calculation, verification and (if possible) also self-correction
 - Working with Vocoder and Data/Control Bursts is supported, along with handling rates 1, 1/2 and 3/4
 - CRCs interface classes may require appropriate CRC Mask to be provided when generating or verifying
 - Through [dmr-kaitai](https://github.com/ok-dmr/dmr-kaitai) handling of ETSI, Hytera and MMDVM/Homebrew UDP data is
   supported
 - To inspect on-wire traffic PcapTool (provided in cli as `dmrlib-pcap-tool` script) supports PCAP/PCAPNG files with
   various functions on describing bursts, port/data filtering, data extraction, ...
 - Everything is tested, specifically now we have 95% pytest coverage for whole ok-dmrlib codebase
 - Not everything is probably documented as it should be, but the usage should always be very clear, when you look at
-  tests of particular component
+  tests of particular component
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/crc.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/crc/crc.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/crc16.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/crc/crc16.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/crc32.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/crc/crc32.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,9 +32,9 @@
     def calculate(data: bytes) -> int:
         """
         Will perform bytes-swap of payload and returns CRC32 as int
         :param data: bytes object of data to be checksumed
         :return: int crc32
         """
         return ba2int(
-            CRC32.CALC.calculate_checksum(bytes_to_bits(byteswap_bytes(data)))
+            CRC32.CALC.calculate_checksum(bytes_to_bits(byteswap_bytes(data), "little"))
         )
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/crc8.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/crc/crc8.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/crc/crc9.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/crc/crc9.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/bptc_196_96.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/bptc_196_96.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/fec_utils.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/fec_utils.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/five_bit_checksum.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/five_bit_checksum.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/golay_20_8_7.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/golay_20_8_7.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_13_9_3.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_13_9_3.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_15_11_3.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_15_11_3.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_16_11_4.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_16_11_4.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_17_12_3.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_17_12_3.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_7_4_3.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_7_4_3.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/hamming_common.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/hamming_common.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/quadratic_residue_16_7_6.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/quadratic_residue_16_7_6.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/reed_solomon_12_9_4.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/reed_solomon_12_9_4.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/trellis.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/trellis.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/vbptc_128_72.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/vbptc_128_72.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/vbptc_32_11.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/vbptc_32_11.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/fec/vbptc_68_28.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/fec/vbptc_68_28.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/burst.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/burst.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from typing import Optional
+from typing import Optional, Literal
 
 from bitarray import bitarray
+from okdmr.kaitai.homebrew.mmdvm2020 import Mmdvm2020
+from okdmr.kaitai.hytera.ip_site_connect_protocol import IpSiteConnectProtocol
+
 from okdmr.dmrlib.etsi.fec.bptc_196_96 import BPTC19696
 from okdmr.dmrlib.etsi.fec.trellis import Trellis34
 from okdmr.dmrlib.etsi.layer2.elements.burst_types import BurstTypes
 from okdmr.dmrlib.etsi.layer2.elements.data_types import DataTypes
 from okdmr.dmrlib.etsi.layer2.elements.sync_patterns import SyncPatterns
 from okdmr.dmrlib.etsi.layer2.elements.voice_bursts import VoiceBursts
 from okdmr.dmrlib.etsi.layer2.pdu.csbk import CSBK
@@ -16,26 +19,25 @@
 from okdmr.dmrlib.etsi.layer2.pdu.rate1_data import Rate1Data
 from okdmr.dmrlib.etsi.layer2.pdu.rate34_data import Rate34Data
 from okdmr.dmrlib.etsi.layer2.pdu.slot_type import SlotType
 from okdmr.dmrlib.hytera.hytera_constants import IPSC_KAITAI_VOICE_SLOTS
 from okdmr.dmrlib.transmission.transmission_types import TransmissionTypes
 from okdmr.dmrlib.utils.bits_bytes import bits_to_bytes, bytes_to_bits, byteswap_bytes
 from okdmr.dmrlib.utils.bits_interface import BitsInterface
-from okdmr.kaitai.homebrew.mmdvm2020 import Mmdvm2020
-from okdmr.kaitai.hytera.ip_site_connect_protocol import IpSiteConnectProtocol
+from okdmr.dmrlib.utils.bytes_interface import BytesInterface
 
 
-class Burst:
+class Burst(BytesInterface):
     """
     ETSI TS 102 361-1 V2.5.1 (2017-10) - 4.2.2   Burst and frame structure
     """
 
     def __init__(
         self,
-        full_bits: bitarray = bitarray(264),
+        full_bits: bitarray = bitarray([0] * 264),
         burst_type: BurstTypes = BurstTypes.Undefined,
     ):
         assert (
             len(full_bits) == 264
         ), f"DMR Layer 2 burst must be 264 bits, got {len(full_bits)}"
         self.full_bits: bitarray = full_bits
         self.embedded_signalling_bits: bitarray = self.full_bits[116:148]
@@ -121,15 +123,14 @@
     def guess_target_radio_id(self) -> int:
         """
         Will return 0 if target cannot be guessed from contents of burst
         """
         if isinstance(self.data, CSBK):
             return int(self.data.target_address or 0)
         elif isinstance(self.data, DataHeader):
-            print(f"header llid destination {self.data.llid_destination}")
             return int(self.data.llid_destination or 0)
 
         return 0
 
     def extract_data(self) -> Optional[BitsInterface]:
         if self.data_type == DataTypes.CSBK:
             return CSBK.from_bits(self.info_bits_deinterleaved)
@@ -218,20 +219,25 @@
         center_bits = (
             (emb_bits[:8] + self.embedded_signalling_bits + emb_bits[8:])
             if self.has_emb
             else self.sync_or_embedded_signalling.as_bits()
         )
         return self.voice_bits[:108] + center_bits + self.voice_bits[108:]
 
+    def as_bytes(self, endian: Literal["big", "little"] = "big") -> bytes:
+        return bits_to_bytes(self.as_bits())
+
     @staticmethod
     def from_bits(bits: bitarray, burst_type: BurstTypes) -> "Burst":
         return Burst(full_bits=bits, burst_type=burst_type)
 
     @staticmethod
-    def from_bytes(data: bytes, burst_type: BurstTypes) -> "Burst":
+    def from_bytes(
+        data: bytes, burst_type: BurstTypes = BurstTypes.DataAndControl
+    ) -> "Burst":
         return Burst(full_bits=bytes_to_bits(data), burst_type=burst_type)
 
     @staticmethod
     def from_mmdvm(mmdvm: Mmdvm2020.TypeDmrData) -> "Burst":
         b = Burst(
             full_bits=bytes_to_bits(mmdvm.dmr_data),
             burst_type=(
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/csbk_opcodes.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/csbk_opcodes.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/data_packet_formats.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/data_packet_formats.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/data_types.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/data_types.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/defined_data_formats.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/defined_data_formats.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/feature_set_ids.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/feature_set_ids.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/flcos.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/flcos.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/fragment_sequence_number.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/fragment_sequence_number.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/sap_identifier.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/sap_identifier.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/slcos.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/slcos.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/sync_patterns.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/sync_patterns.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/udt_format.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/udt_format.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/elements/voice_bursts.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/elements/voice_bursts.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/csbk.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/data_header.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,346 +1,349 @@
-from typing import Union, Optional
+from typing import Union, Optional, Literal
 
 from bitarray import bitarray
 from bitarray.util import ba2int, int2ba
 
 from okdmr.dmrlib.etsi.crc.crc16 import CRC16
 from okdmr.dmrlib.etsi.layer2.elements.crc_masks import CrcMasks
 from okdmr.dmrlib.etsi.layer2.elements.csbk_opcodes import CsbkOpcodes
-from okdmr.dmrlib.etsi.layer2.elements.feature_set_ids import FeatureSetIDs
-from okdmr.dmrlib.etsi.layer3.elements.additional_information_field import (
-    AdditionalInformationField,
+from okdmr.dmrlib.etsi.layer2.elements.data_packet_formats import DataPacketFormats
+from okdmr.dmrlib.etsi.layer2.elements.defined_data_formats import DefinedDataFormats
+from okdmr.dmrlib.etsi.layer2.elements.fragment_sequence_number import (
+    FragmentSequenceNumber,
 )
-from okdmr.dmrlib.etsi.layer3.elements.answer_response import AnswerResponse
-from okdmr.dmrlib.etsi.layer3.elements.channel_timing_opcode import ChannelTimingOpcode
-from okdmr.dmrlib.etsi.layer3.elements.dynamic_identifier import DynamicIdentifier
-from okdmr.dmrlib.etsi.layer3.elements.reason_code import ReasonCode
-from okdmr.dmrlib.etsi.layer3.elements.service_options import ServiceOptions
-from okdmr.dmrlib.etsi.layer3.elements.source_type import SourceType
-from okdmr.dmrlib.utils.bits_bytes import bits_to_bytes, bytes_to_bits
+from okdmr.dmrlib.etsi.layer2.elements.full_message_flag import FullMessageFlag
+from okdmr.dmrlib.etsi.layer2.elements.resynchronize_flag import ResynchronizeFlag
+from okdmr.dmrlib.etsi.layer2.elements.sap_identifier import SAPIdentifier
+from okdmr.dmrlib.etsi.layer2.elements.sarq import SARQ
+from okdmr.dmrlib.etsi.layer2.elements.supplementary_flag import SupplementaryFlag
+from okdmr.dmrlib.etsi.layer2.elements.udt_format import UDTFormat
+from okdmr.dmrlib.etsi.layer3.elements.udt_option_flag import UDTOptionFlag
+from okdmr.dmrlib.utils.bits_bytes import bytes_to_bits, bits_to_bytes
 from okdmr.dmrlib.utils.bits_interface import BitsInterface
+from okdmr.dmrlib.utils.bytes_interface import BytesInterface
 
 
-class CSBK(BitsInterface):
+class DataHeader(BitsInterface, BytesInterface):
     """
-    ETSI TS 102 361-2 V2.4.1 (2017-10) - 7.1.2  Control Signalling BlocK (CSBK) PDUs
+    ETSI TS 102 361-1 V2.5.1 (2017-10) - 8.2.1 Header block structure
     """
 
     def __init__(
         self,
-        csbko: CsbkOpcodes,
-        last_block: Union[bool, int] = True,
-        protect_flag: Union[bool, int] = False,
-        manufacturers_feature_set_id: FeatureSetIDs = FeatureSetIDs.StandardizedFID,
-        # default value for crc indicates, it must be recalculated on construct
-        crc: int = 0,
-        # bs outbound activation fields
-        bs_address: int = 0,
-        source_address: int = 0,
-        # unit to unit voice service request fields
-        service_options: Optional[ServiceOptions] = None,
-        target_address: int = 0,
-        # unit to unit voice service response fields
-        answer_response: Optional[AnswerResponse] = None,
-        # negative acknowledge response fields
-        additional_information_field: Optional[AdditionalInformationField] = None,
-        source_type: Optional[SourceType] = None,
-        service_type: Optional[CsbkOpcodes] = None,
-        reason_code: Optional[ReasonCode] = None,
-        # preamble fields
-        csbk_content_follows_preambles: Union[int, bool] = False,
-        target_address_is_individual: Union[int, bool] = False,
+        dpf: DataPacketFormats,
+        crc: Optional[bitarray] = None,
+        # some common fields
+        is_group: Union[int, bool] = False,
+        is_response_requested: Union[int, bool] = False,
+        pad_octet_count: int = 0,
+        sap_identifier: Optional[SAPIdentifier] = None,
+        llid_destination: int = 0,
+        llid_source: int = 0,
+        full_message_flag: Optional[FullMessageFlag] = None,
         blocks_to_follow: int = 0,
-        # channel timing fields
-        sync_age: int = 0,
-        generation: int = 0,
-        leader_identifier: int = 0,
-        new_leader: Union[int, bool] = 0,
-        leader_dynamic_identifier: Union[DynamicIdentifier, int] = 0,
-        channel_timing_opcode: Union[ChannelTimingOpcode, int] = 0,
-        source_identifier: int = 0,
-        source_dynamic_identifier: Union[DynamicIdentifier, int] = 0,
-        # for unknown / manufacturer-specific data
-        raw_data: Union[bytes, bitarray] = b"",
+        resynchronize_flag: Optional[ResynchronizeFlag] = None,
+        send_sequence_number: int = 0,
+        fragment_sequence_number: Union[FragmentSequenceNumber, int] = 0,
+        # Confirmed Response packet Header (C_RHEAD) PDU
+        response_class: int = 0,
+        response_type: int = 0,
+        response_status: int = 0,
+        # Defined Data short data packet Header (DD_HEAD) PDU
+        appended_blocks: int = 0,
+        defined_data_format: Optional[DefinedDataFormats] = None,
+        sarq: Optional[SARQ] = None,
+        bit_padding: Optional[bitarray] = bitarray(),
+        # Unified Data Transport Header (UDT_HEAD) PDU
+        is_emergency: Union[int, bool] = False,
+        udt_option_flag: Optional[UDTOptionFlag] = None,
+        pad_nibbles_count: int = 0,
+        udt_format: Optional[UDTFormat] = None,
+        udt_opcode: Optional[CsbkOpcodes] = None,
+        supplementary_flag: Optional[SupplementaryFlag] = None,
     ):
-        """
-        Params that are optional, are specific for particular CSBKO
-
-        :param last_block: value 0/1
-        :param protect_flag: value 0/1
-        :param csbko: CsbkOpcodes enum
-        :param manufacturers_feature_set_id: FeatureSetIDs enum
-        :param crc: crc-ccit (crc16-ccit) value
-        :param bs_address: optional value 0-16777215
-        :param source_address: optional value 0-16777215
-        :param service_options: optional ServiceOptions element instance
-        :param target_address: optional value 0-16777215
-        :param answer_response: optional AnswerResponse enum
-        :param additional_information_field: optional AdditionalInformationField enum
-        :param source_type: optional SourceType enum
-        :param service_type: optional CsbkOpcodes enum
-        :param reason_code: optional ReasonCode enum
-        :param csbk_content_follows_preambles: value 0/1
-        :param target_address_is_individual: value 0/1
-        :param blocks_to_follow: value 0-255
-        :param sync_age: value 0-2047, amount of SAIncr (500ms) since last beacon
-        :param generation: value 0-31, number of timing hops from leader
-        :param leader_identifier: value 0-1048575, ms derived identifier
-        :param new_leader: 0 => ms accepts current leader, 1 => new leader is appointed
-        :param leader_dynamic_identifier: DynamicIdentifier or value 0-3
-        :param channel_timing_opcode: ChannelTimingOpcode or value 0-3
-        :param source_identifier: value 0-1048575, ms derived identifier
-        :param source_dynamic_identifier: DynamicIdentifier or value 0-3
-        """
-        self.last_block: bool = last_block in (True, 1)
-        self.protect_flag: bool = protect_flag in (True, 1)
-        self.csbko: CsbkOpcodes = csbko
-        self.feature_set: FeatureSetIDs = manufacturers_feature_set_id
-        self.crc: int = crc
-
-        self.bs_address: int = bs_address
-        self.source_address: int = source_address
-        self.service_options: Optional[ServiceOptions] = service_options
-        self.target_address: int = target_address
-        self.answer_response: Optional[AnswerResponse] = answer_response
-        self.additional_information_field: Optional[
-            AdditionalInformationField
-        ] = additional_information_field
-        self.source_type: Optional[SourceType] = source_type
-        self.service_type: Optional[CsbkOpcodes] = service_type
-        self.reason_code: Optional[ReasonCode] = reason_code
-        self.csbk_content_follows_preambles: bool = csbk_content_follows_preambles in (
-            True,
-            1,
-        )
-        self.target_address_is_individual: bool = target_address_is_individual in (
-            True,
-            1,
-        )
+        self.data_packet_format: DataPacketFormats = dpf
+        self.crc: bitarray = crc or bitarray([0] * 16)
+        self.is_group: bool = is_group in (True, 1)
+        self.is_response_requested: bool = is_response_requested in (True, 1)
+        self.pad_octet_count: int = pad_octet_count
+        self.sap_identifier: Optional[SAPIdentifier] = sap_identifier
+        self.llid_destination: int = llid_destination
+        self.llid_source: int = llid_source
+        self.full_message_flag: Optional[FullMessageFlag] = full_message_flag
         self.blocks_to_follow: int = blocks_to_follow
-        self.sync_age: int = sync_age
-        self.generation: int = generation
-        self.leader_identifier: int = leader_identifier
-        self.new_leader: int = int(new_leader)
-        self.leader_dynamic_identifier: DynamicIdentifier = (
-            leader_dynamic_identifier
-            if isinstance(leader_dynamic_identifier, DynamicIdentifier)
-            else DynamicIdentifier(leader_dynamic_identifier)
-        )
-        self.channel_timing_opcode: ChannelTimingOpcode = (
-            channel_timing_opcode
-            if isinstance(channel_timing_opcode, ChannelTimingOpcode)
-            else ChannelTimingOpcode(channel_timing_opcode)
-        )
-        self.source_identifier: int = source_identifier
-        self.source_dynamic_identifier = (
-            source_dynamic_identifier
-            if isinstance(source_dynamic_identifier, DynamicIdentifier)
-            else DynamicIdentifier(source_dynamic_identifier)
-        )
-        self.raw_data: bytes = (
-            bits_to_bytes(raw_data) if isinstance(raw_data, bitarray) else raw_data
+        self.resynchronize_flag: Optional[ResynchronizeFlag] = resynchronize_flag
+        self.send_sequence_number: int = send_sequence_number
+        self.fragment_sequence_number: FragmentSequenceNumber = (
+            FragmentSequenceNumber(fragment_sequence_number)
+            if isinstance(fragment_sequence_number, int)
+            else fragment_sequence_number
         )
+        # Confirmed Response packet Header (C_RHEAD) PDU
+        self.response_class: int = response_class
+        self.response_type: int = response_type
+        self.response_status: int = response_status
+        # Defined Data short data packet Header (DD_HEAD) PDU
+        self.appended_blocks: int = appended_blocks
+        self.defined_data_format: Optional[DefinedDataFormats] = defined_data_format
+        self.sarq: Optional[SARQ] = sarq
+        self.bit_padding: bitarray = bit_padding
+        # Unified Data Transport Header (UDT_HEAD) PDU
+        self.is_emergency: bool = is_emergency in (True, 1)
+        self.udt_option_flag: Optional[UDTOptionFlag] = udt_option_flag
+        self.pad_nibbles_count: int = pad_nibbles_count
+        self.udt_format: Optional[UDTFormat] = udt_format
+        self.udt_opcode: Optional[CsbkOpcodes] = udt_opcode
+        self.supplementary_flag: Optional[SupplementaryFlag] = supplementary_flag
+
+        if len(self.crc) != 16 or ba2int(self.crc) <= 0:
+            self.crc_ok: bool = True
+            self.crc = int2ba(
+                CRC16.calculate(self.as_bits()[:-16].tobytes(), CrcMasks.DataHeader),
+                length=16,
+            )
+        else:
+            self.crc_ok: bool = CRC16.check(
+                self.as_bits()[:-16].tobytes(), ba2int(self.crc), CrcMasks.DataHeader
+            )
+
+    def get_blocks_to_follow(self) -> Optional[int]:
+        if self.data_packet_format == DataPacketFormats.UnifiedDataTransport:
+            return None
+        elif self.data_packet_format == DataPacketFormats.ShortDataDefined:
+            return self.appended_blocks
+        else:
+            return self.blocks_to_follow
+
+    def __repr__(self):
+        descr: str = f"[{self.data_packet_format}] "
+
+        if self.data_packet_format == DataPacketFormats.DataPacketConfirmed:
+            descr += (
+                f"{'[CRC INVALID] ' if not self.crc_ok else ''}"
+                + f"[{self.sap_identifier}] "
+                + ("[TARGET IS GROUP] " if self.is_group else "[TARGET IS INDIVIDUAL] ")
+                + ("[RESPONSE REQUESTED] " if self.is_response_requested else "")
+                + f"[PAD OCTETS: {self.pad_octet_count}] "
+                + f"[SOURCE: {self.llid_source}] [DESTINATION: {self.llid_destination}] [{self.full_message_flag}] "
+                + f"[BTF: {self.blocks_to_follow}] [{self.resynchronize_flag}] [N(S): {self.send_sequence_number}] "
+                + f"{repr(self.fragment_sequence_number)}"
+            )
+        elif self.data_packet_format == DataPacketFormats.DataPacketUnconfirmed:
+            descr += (
+                f"{'[CRC INVALID] ' if not self.crc_ok else ''}"
+                + f"[{self.sap_identifier}] "
+                + ("[TARGET IS GROUP] " if self.is_group else "[TARGET IS INDIVIDUAL] ")
+                + ("[RESPONSE REQUESTED] " if self.is_response_requested else "")
+                + f"[PAD OCTETS: {self.pad_octet_count}] "
+                + f"[SOURCE: {self.llid_source}] [DESTINATION: {self.llid_destination}] [{self.full_message_flag}] "
+                + f"[BTF: {self.blocks_to_follow}] "
+                + f"{repr(self.fragment_sequence_number)}"
+            )
+        elif self.data_packet_format == DataPacketFormats.ResponsePacket:
+            descr += (
+                f"{'[CRC INVALID] ' if not self.crc_ok else ''}"
+                + f"[{self.sap_identifier}] "
+                + ("[RESPONSE REQUESTED] " if self.is_response_requested else "")
+                + f"[RESPONSE TYPE: {self.response_type} CLASS: {self.response_class} STATUS: {self.response_status}] "
+                + f"[SOURCE: {self.llid_source}] [DESTINATION: {self.llid_destination}] [{self.full_message_flag}] "
+                + f"[BTF: {self.blocks_to_follow}] "
+            )
+        elif self.data_packet_format == DataPacketFormats.ShortDataDefined:
+            descr += (
+                f"{'[CRC INVALID] ' if not self.crc_ok else ''}"
+                + f"[{self.sap_identifier}] [{self.defined_data_format}] [{self.sarq}] "
+                + ("[TARGET IS GROUP] " if self.is_group else "[TARGET IS INDIVIDUAL] ")
+                + ("[RESPONSE REQUESTED] " if self.is_response_requested else "")
+                + f"[SOURCE: {self.llid_source}] [DESTINATION: {self.llid_destination}] [{self.full_message_flag}] "
+                + f"[APPENDED BLOCKS: {self.appended_blocks}] "
+            )
+        elif self.data_packet_format == DataPacketFormats.UnifiedDataTransport:
+            descr += (
+                f"{'[CRC INVALID] ' if not self.crc_ok else ''}"
+                + f"[{self.sap_identifier}] [{self.udt_format}] [UDT Opcode: {self.udt_opcode}] "
+                + ("[TARGET IS GROUP] " if self.is_group else "[TARGET IS INDIVIDUAL] ")
+                + ("[RESPONSE REQUESTED] " if self.is_response_requested else "")
+                + f"[SOURCE: {self.llid_source}] [DESTINATION: {self.llid_destination}] [{self.supplementary_flag}] "
+            )
+        else:
+            raise KeyError(f"__repr__ not implemented for {self.data_packet_format}")
 
-        if self.crc <= 0:
-            self.calculate_crc_ccit()
+        return descr
 
-    def calculate_crc_ccit(self) -> "CSBK":
-        self.crc = CRC16.calculate(self.as_bits()[0:80].tobytes(), CrcMasks.CSBK)
-        return self
+    def as_bytes(self, endian: Literal["big", "little"] = "big") -> bytes:
+        return bits_to_bytes(self.as_bits())
 
     def as_bits(self) -> bitarray:
-        pdu: bitarray = (
-            bitarray([self.last_block, self.protect_flag])
-            + self.csbko.as_bits()
-            + self.feature_set.as_bits()
-        )
-        if self.csbko == CsbkOpcodes.BSOutboundActivation:
-            pdu += (
-                int2ba(0, length=16)
-                + int2ba(self.bs_address, length=24)
-                + int2ba(self.source_address, length=24)
-            )
-        elif self.csbko == CsbkOpcodes.UnitToUnitVoiceServiceRequest:
-            pdu += (
-                self.service_options.as_bits()
-                + int2ba(0, length=8)
-                + int2ba(self.target_address, length=24)
-                + int2ba(self.source_address, length=24)
-            )
-        elif self.csbko == CsbkOpcodes.UnitToUnitVoiceServiceAnswerResponse:
-            pdu += (
-                self.service_options.as_bits()
-                + self.answer_response.as_bits()
-                + int2ba(self.target_address, length=24)
-                + int2ba(self.source_address, length=24)
-            )
-        elif self.csbko == CsbkOpcodes.NegativeAcknowledgementResponse:
-            pdu += (
-                bitarray([1, self.source_type == SourceType.MSSourced])
-                + self.service_type.as_bits()
-                + self.reason_code.as_bits()
-                + int2ba(self.source_address, length=24)
-                + int2ba(self.target_address, length=24)
+        if self.data_packet_format == DataPacketFormats.DataPacketConfirmed:
+            poc = int2ba(self.pad_octet_count, length=5)
+            return (
+                bitarray([self.is_group, self.is_response_requested, 0, poc[0]])
+                + self.data_packet_format.as_bits()
+                + self.sap_identifier.as_bits()
+                + poc[1:]
+                + int2ba(self.llid_destination, length=24)
+                + int2ba(self.llid_source, length=24)
+                + bitarray([self.full_message_flag.value])
+                + int2ba(self.blocks_to_follow, length=7)
+                + bitarray([self.resynchronize_flag.value])
+                + int2ba(self.send_sequence_number, length=3)
+                + self.fragment_sequence_number.as_bits()
+                + self.crc
+            )
+        elif self.data_packet_format == DataPacketFormats.DataPacketUnconfirmed:
+            poc = int2ba(self.pad_octet_count, length=5)
+            return (
+                bitarray([self.is_group, self.is_response_requested, 0, poc[0]])
+                + self.data_packet_format.as_bits()
+                + self.sap_identifier.as_bits()
+                + poc[1:]
+                + int2ba(self.llid_destination, length=24)
+                + int2ba(self.llid_source, length=24)
+                + bitarray([self.full_message_flag.value])
+                + int2ba(self.blocks_to_follow, length=7)
+                + bitarray([0] * 4)
+                + self.fragment_sequence_number.as_bits()
+                + self.crc
+            )
+        elif self.data_packet_format == DataPacketFormats.ResponsePacket:
+            return (
+                bitarray([0] * 4)
+                + self.data_packet_format.as_bits()
+                + self.sap_identifier.as_bits()
+                + bitarray([0] * 4)
+                + int2ba(self.llid_destination, length=24)
+                + int2ba(self.llid_source, length=24)
+                + bitarray([self.full_message_flag.value])
+                + int2ba(self.blocks_to_follow, length=7)
+                + int2ba(self.response_class, length=2)
+                + int2ba(self.response_type, length=3)
+                + int2ba(self.response_status, length=3)
+                + self.crc
+            )
+        elif self.data_packet_format == DataPacketFormats.ShortDataDefined:
+            ab = int2ba(self.appended_blocks, length=6)
+            return (
+                bitarray([self.is_group, self.is_response_requested, ab[0], ab[1]])
+                + self.data_packet_format.as_bits()
+                + self.sap_identifier.as_bits()
+                + ab[2:]
+                + int2ba(self.llid_destination, length=24)
+                + int2ba(self.llid_source, length=24)
+                + self.defined_data_format.as_bits()
+                + bitarray([self.sarq.value, self.full_message_flag.value])
+                + self.bit_padding
+                + self.crc
             )
-        elif self.csbko == CsbkOpcodes.PreambleCSBK:
-            pdu += (
+        elif self.data_packet_format == DataPacketFormats.UnifiedDataTransport:
+            return (
                 bitarray(
                     [
-                        not self.csbk_content_follows_preambles,
-                        not self.target_address_is_individual,
+                        self.is_group,
+                        self.is_response_requested,
+                        self.is_emergency,
+                        self.udt_option_flag.value,
                     ]
                 )
-                + int2ba(0, length=6)
-                + int2ba(self.blocks_to_follow, length=8)
-                + int2ba(self.target_address, length=24)
-                + int2ba(self.source_address, length=24)
-            )
-        elif self.csbko == CsbkOpcodes.ChannelTimingCSBK:
-            cto = self.channel_timing_opcode.as_bits()
-            pdu += (
-                int2ba(self.sync_age, length=11)
-                + int2ba(self.generation, length=5)
-                + int2ba(self.leader_identifier, length=20)
-                + int2ba(self.new_leader, length=1)
-                + self.leader_dynamic_identifier.as_bits()
-                + bitarray([cto[0]])
-                + int2ba(self.source_identifier, length=20)
+                + self.data_packet_format.as_bits()
+                + self.sap_identifier.as_bits()
+                + self.udt_format.as_bits()
+                + int2ba(self.llid_destination, length=24)
+                + int2ba(self.llid_source, length=24)
+                + int2ba(self.pad_nibbles_count, length=5)
                 + bitarray([0])
-                + self.source_dynamic_identifier.as_bits()
-                + bitarray([cto[1]])
+                + int2ba(self.appended_blocks, length=2)
+                + bitarray([self.supplementary_flag.value, 0])
+                + self.udt_opcode.as_bits()
+                + self.crc
             )
-        elif self.csbko == CsbkOpcodes.HyteraIPSCSync:
-            pdu += bytes_to_bits(self.raw_data)
+        raise NotImplementedError(
+            f"as_bits not implemented for {self.data_packet_format}"
+        )
 
-        return pdu + int2ba(self.crc, length=16)
+    @staticmethod
+    def from_bytes(
+        data: bytes, endian: Literal["big", "little"] = "big"
+    ) -> Optional["DataHeader"]:
+        return DataHeader.from_bits(bytes_to_bits(data))
 
     @staticmethod
-    def from_bits(bits: bitarray) -> "CSBK":
-        assert (
-            len(bits) >= 96
-        ), f"A single CSBK PDU has a length of 96 bits, got only {len(bits)}"
-        lb: int = bits[0]
-        pf: int = bits[1]
-        csbko: CsbkOpcodes = CsbkOpcodes(ba2int(bits[2:8]))
-        fid: FeatureSetIDs = FeatureSetIDs(ba2int(bits[8:16]))
-        crc_ccit: int = ba2int(bits[80:96])
-        if csbko == CsbkOpcodes.BSOutboundActivation:
-            return CSBK(
-                last_block=lb,
-                protect_flag=pf,
-                manufacturers_feature_set_id=fid,
-                crc=crc_ccit,
-                csbko=csbko,
-                bs_address=ba2int(bits[32:56]),
-                source_address=ba2int(bits[56:80]),
-            )
-        elif csbko == CsbkOpcodes.UnitToUnitVoiceServiceRequest:
-            return CSBK(
-                last_block=lb,
-                protect_flag=pf,
-                manufacturers_feature_set_id=fid,
-                crc=crc_ccit,
-                csbko=csbko,
-                service_options=ServiceOptions.from_bits(bits[16:24]),
-                target_address=ba2int(bits[32:56]),
-                source_address=ba2int(bits[56:80]),
-            )
-        elif csbko == CsbkOpcodes.UnitToUnitVoiceServiceAnswerResponse:
-            return CSBK(
-                last_block=lb,
-                protect_flag=pf,
-                manufacturers_feature_set_id=fid,
-                crc=crc_ccit,
-                csbko=csbko,
-                service_options=ServiceOptions.from_bits(bits[16:24]),
-                answer_response=AnswerResponse(ba2int(bits[24:32])),
-                target_address=ba2int(bits[32:56]),
-                source_address=ba2int(bits[56:80]),
-            )
-        elif csbko == CsbkOpcodes.NegativeAcknowledgementResponse:
-            return CSBK(
-                last_block=lb,
-                protect_flag=pf,
-                manufacturers_feature_set_id=fid,
-                crc=crc_ccit,
-                csbko=csbko,
-                additional_information_field=AdditionalInformationField(bits[16]),
-                source_type=SourceType(bits[17]),
-                service_type=CsbkOpcodes.from_bits(bits[18:24]),
-                reason_code=ReasonCode(ba2int(bits[24:32])),
-                source_address=ba2int(bits[32:56]),
-                target_address=ba2int(bits[56:80]),
-            )
-        elif csbko == CsbkOpcodes.PreambleCSBK:
-            return CSBK(
-                last_block=lb,
-                protect_flag=pf,
-                manufacturers_feature_set_id=fid,
-                crc=crc_ccit,
-                csbko=csbko,
-                csbk_content_follows_preambles=not bits[16],
-                target_address_is_individual=not bits[17],
-                blocks_to_follow=ba2int(bits[24:32]),
-                target_address=ba2int(bits[32:56]),
-                source_address=ba2int(bits[56:80]),
-            )
-        elif csbko == CsbkOpcodes.ChannelTimingCSBK:
-            return CSBK(
-                last_block=lb,
-                protect_flag=pf,
-                manufacturers_feature_set_id=fid,
-                crc=crc_ccit,
-                csbko=csbko,
-                sync_age=ba2int(bits[16:27]),
-                generation=ba2int(bits[27:32]),
-                leader_identifier=ba2int(bits[32:52]),
-                new_leader=bits[52],
-                leader_dynamic_identifier=DynamicIdentifier.from_bits(bits[53:55]),
-                channel_timing_opcode=ba2int(bitarray([bits[55], bits[79]])),
-                source_identifier=ba2int(bits[56:76]),
-                source_dynamic_identifier=DynamicIdentifier.from_bits(bits[77:79]),
-            )
-        elif csbko == CsbkOpcodes.HyteraIPSCSync:
-            return CSBK(
-                last_block=lb,
-                protect_flag=pf,
-                manufacturers_feature_set_id=fid,
-                crc=crc_ccit,
-                csbko=csbko,
-                raw_data=bits[16:80],
+    def from_bits(bits: bitarray) -> "DataHeader":
+        dpf: DataPacketFormats = DataPacketFormats.from_bits(bits[4:8])
+        if dpf == DataPacketFormats.DataPacketConfirmed:
+            return DataHeader(
+                dpf=dpf,
+                crc=bits[80:96],
+                is_group=bits[0],
+                is_response_requested=bits[1],
+                pad_octet_count=(bits[3] << 4) + ba2int(bits[12:16]),
+                sap_identifier=SAPIdentifier.from_bits(bits[8:12]),
+                llid_destination=ba2int(bits[16:40]),
+                llid_source=ba2int(bits[40:64]),
+                full_message_flag=FullMessageFlag(bits[64]),
+                blocks_to_follow=ba2int(bits[65:72]),
+                resynchronize_flag=ResynchronizeFlag(bits[72]),
+                send_sequence_number=ba2int(bits[73:76]),
+                fragment_sequence_number=ba2int(bits[76:80]),
+            )
+        elif dpf == DataPacketFormats.ResponsePacket:
+            return DataHeader(
+                dpf=dpf,
+                crc=bits[80:96],
+                is_response_requested=bits[1],
+                sap_identifier=SAPIdentifier.from_bits(bits[8:12]),
+                llid_destination=ba2int(bits[16:40]),
+                llid_source=ba2int(bits[40:64]),
+                full_message_flag=FullMessageFlag(bits[64]),
+                blocks_to_follow=ba2int(bits[65:72]),
+                response_class=ba2int(bits[72:74]),
+                response_type=ba2int(bits[74:77]),
+                response_status=ba2int(bits[77:80]),
+            )
+        elif dpf == DataPacketFormats.ShortDataDefined:
+            return DataHeader(
+                dpf=dpf,
+                crc=bits[80:96],
+                is_group=bits[0],
+                is_response_requested=bits[1],
+                appended_blocks=ba2int(bits[2:4] + bits[12:16]),
+                sap_identifier=SAPIdentifier.from_bits(bits[8:12]),
+                llid_destination=ba2int(bits[16:40]),
+                llid_source=ba2int(bits[40:64]),
+                defined_data_format=DefinedDataFormats.from_bits(bits[64:70]),
+                sarq=SARQ(bits[70]),
+                full_message_flag=FullMessageFlag(bits[71]),
+                bit_padding=bits[72:80],
+            )
+        elif dpf == DataPacketFormats.DataPacketUnconfirmed:
+            return DataHeader(
+                dpf=dpf,
+                crc=bits[80:96],
+                is_group=bits[0],
+                is_response_requested=bits[1],
+                pad_octet_count=(bits[3] << 4) + ba2int(bits[12:16]),
+                sap_identifier=SAPIdentifier.from_bits(bits[8:12]),
+                llid_destination=ba2int(bits[16:40]),
+                llid_source=ba2int(bits[40:64]),
+                full_message_flag=FullMessageFlag(bits[64]),
+                blocks_to_follow=ba2int(bits[65:72]),
+                fragment_sequence_number=ba2int(bits[76:80]),
+            )
+        elif dpf == DataPacketFormats.UnifiedDataTransport:
+            return DataHeader(
+                dpf=dpf,
+                crc=bits[80:96],
+                is_group=bits[0],
+                is_response_requested=bits[1],
+                is_emergency=bits[2],
+                udt_option_flag=UDTOptionFlag(bits[3]),
+                sap_identifier=SAPIdentifier.from_bits(bits[8:12]),
+                udt_format=UDTFormat.from_bits(bits[12:16]),
+                llid_destination=ba2int(bits[16:40]),
+                llid_source=ba2int(bits[40:64]),
+                pad_nibbles_count=ba2int(bits[64:69]),
+                appended_blocks=ba2int(bits[70:72]),
+                supplementary_flag=SupplementaryFlag(bits[72]),
+                udt_opcode=CsbkOpcodes.from_bits(bits[74:80]),
             )
-
-        raise NotImplementedError(
-            f"Not-implemented CSBKO {csbko} PDU {bits_to_bytes(bits).hex()}"
-        )
-
-    def __repr__(self) -> str:
-        description = f"[{self.csbko}] [LB: {int(self.last_block)}] [PF: {int(self.protect_flag)}] [{self.feature_set}] "
-        if self.csbko == CsbkOpcodes.BSOutboundActivation:
-            description += (
-                f"[BS ADDR: {self.bs_address}] [SRC ADDR: {self.source_address}]"
-            )
-        elif self.csbko == CsbkOpcodes.UnitToUnitVoiceServiceRequest:
-            description += f"[{self.service_options}] [DST ADDR: {self.target_address}] [SRC ADDR: {self.source_address}]"
-        elif self.csbko == CsbkOpcodes.UnitToUnitVoiceServiceAnswerResponse:
-            description += f"[{self.service_options}] [{self.answer_response}] [DST ADDR: {self.target_address}] [SRC ADDR: {self.source_address}]"
-        elif self.csbko == CsbkOpcodes.NegativeAcknowledgementResponse:
-            description += f"[{self.source_type}] [{self.service_type}] [{self.reason_code}] [SRC ADDR: {self.source_address}] [DST ADDR: {self.target_address}]"
-        elif self.csbko == CsbkOpcodes.PreambleCSBK:
-            description += (
-                f"[TARGET IS {'INDIVIDUAL' if self.target_address_is_individual else 'GROUP'}] "
-                f"[FOLLOWED BY {'CSBK' if self.csbk_content_follows_preambles else 'DATA'}] "
-                f"[BTF: {self.blocks_to_follow}] [DST ADDR: {self.target_address}] [SRC ADDR: {self.source_address}]"
-            )
-        elif self.csbko == CsbkOpcodes.ChannelTimingCSBK:
-            description += (
-                f"[AGE: {500 * self.sync_age}ms] [GENERATION: {self.generation}] "
-                f"[LEADER IDENTIFIER: {self.leader_identifier}] [NEW LEADER: {self.new_leader}] "
-                f"[LEADER DYN IDENTIFIER: {self.leader_dynamic_identifier}] "
-                f"[SOURCE IDENTIFIER: {self.source_identifier}] "
-                f"[SOURCE DYN IDENTIFIER: {self.source_dynamic_identifier}] "
-                f"[CTO: {self.channel_timing_opcode}]"
-            )
-        elif self.csbko == CsbkOpcodes.HyteraIPSCSync:
-            description += f"[MFID DATA HEX({self.raw_data.hex()})]"
-        return description
+        else:
+            raise NotImplementedError(f"from_bits not implemented for {dpf}")
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/embedded_signalling.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/embedded_signalling.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/full_link_control.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/full_link_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from typing import Union, Optional
+from typing import Union, Optional, Literal
 
 from bitarray import bitarray
 from bitarray.util import ba2int, int2ba
 
 from okdmr.dmrlib.etsi.layer2.elements.feature_set_ids import FeatureSetIDs
 from okdmr.dmrlib.etsi.layer2.elements.flcos import FLCOs
 from okdmr.dmrlib.etsi.layer3.elements.position_error import PositionError
 from okdmr.dmrlib.etsi.layer3.elements.service_options import ServiceOptions
 from okdmr.dmrlib.etsi.layer3.elements.talker_alias_data_format import (
     TalkerAliasDataFormat,
 )
-from okdmr.dmrlib.utils.bits_bytes import bytes_to_bits
+from okdmr.dmrlib.utils.bits_bytes import bytes_to_bits, bits_to_bytes
 from okdmr.dmrlib.utils.bits_interface import BitsInterface
+from okdmr.dmrlib.utils.bytes_interface import BytesInterface
 
 
-class FullLinkControl(BitsInterface):
+class FullLinkControl(BytesInterface, BitsInterface):
     """
     ETSI TS 102 361-1 V2.5.1 (2017-10) - 9.1.6  Full Link Control (FULL LC) PDU
     ETSI TS 102 361-2 V2.4.1 (2017-10) - 7.1.1  Full Link Control PDUs
     """
 
     def __init__(
         self,
@@ -90,14 +91,24 @@
             return descr + (
                 f"[{self.talker_alias_data.hex()}] [utf16le: {self.talker_alias_data.decode('ascii')}]"
             )
 
         raise KeyError(f"FullLinkControl.__repr__ does not support " + descr)
 
     @staticmethod
+    def from_bytes(
+        data: bytes, endian: Literal["big", "little"] = "big"
+    ) -> Optional["FullLinkControl"]:
+        _bits = bytes_to_bits(data)
+        return FullLinkControl.from_bits(_bits[:-3] if len(_bits) == 80 else _bits)
+
+    def as_bytes(self, endian: Literal["big", "little"] = "big") -> bytes:
+        return bits_to_bytes(self.as_bits())
+
+    @staticmethod
     def from_bits(bits: bitarray) -> "FullLinkControl":
         assert len(bits) in (
             96,
             77,
         ), f"Unexpected Full LC bits length, expected 96 (reed-solomon) or 77 (5-bit checksum), got {len(bits)}"
         flco: FLCOs = FLCOs.from_bits(bits[2:8])
         pf: int = bits[0]
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/pi_header.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/pi_header.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/rate12_data.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/rate12_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Union
 
 from bitarray import bitarray
 from bitarray.util import int2ba, ba2int
 
 from okdmr.dmrlib.etsi.crc.crc9 import CRC9
 from okdmr.dmrlib.etsi.layer2.elements.crc_masks import CrcMasks
+from okdmr.dmrlib.etsi.layer2.elements.data_types import DataTypes
 from okdmr.dmrlib.utils.bits_bytes import bits_to_bytes, bytes_to_bits
 from okdmr.dmrlib.utils.bits_interface import BitsInterface
 
 
 @enum.unique
 class Rate12DataTypes(enum.Enum):
     Unconfirmed = 12
@@ -68,14 +69,18 @@
         self.crc9: int = crc9 if isinstance(crc9, int) else ba2int(crc9[::-1])
         calculated_crc9 = self.calculate_crc9()
         if self.crc9 <= 0:
             self.crc9 = calculated_crc9
         self.crc9_ok: bool = self.crc9 == calculated_crc9
 
     @staticmethod
+    def get_data_type() -> DataTypes:
+        return DataTypes.Rate12Data
+
+    @staticmethod
     def validate_packet_type(packet_type: Rate12DataTypes, data_length: int) -> bool:
         if data_length == 0 or packet_type == Rate12DataTypes.Undefined:
             return True
         else:
             assert (
                 data_length == packet_type.value
             ), f"{packet_type} data must be {packet_type.value} bytes, got {data_length} bytes"
@@ -106,15 +111,15 @@
             f"[DATA({self.packet_type.value}) {self.data.hex()}] "
         )
         if self.is_confirmed():
             label += f"[DBSN: {self.dbsn}] " f"[CRC9: {self.crc9}] " + (
                 " [CRC9 INVALID]" if not self.crc9_ok else ""
             )
         if self.is_last_block():
-            label += f" [CRC32 int({self.crc32}) hex({self.crc32.to_bytes(4, byteorder='big').hex()})]"
+            label += f" [CRC32 int({self.crc32}) hex({self.crc32.to_bytes(4, byteorder='little').hex()})]"
         return label
 
     @staticmethod
     def from_bits(bits: bitarray) -> "Rate12Data":
         return Rate12Data.from_bits_typed(bits, Rate12DataTypes.Undefined)
 
     @staticmethod
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/rate1_data.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/rate1_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Union
 
 from bitarray import bitarray
 from bitarray.util import int2ba, ba2int
 
 from okdmr.dmrlib.etsi.crc.crc9 import CRC9
 from okdmr.dmrlib.etsi.layer2.elements.crc_masks import CrcMasks
+from okdmr.dmrlib.etsi.layer2.elements.data_types import DataTypes
 from okdmr.dmrlib.utils.bits_bytes import bits_to_bytes, bytes_to_bits
 from okdmr.dmrlib.utils.bits_interface import BitsInterface
 
 
 @enum.unique
 class Rate1DataTypes(enum.Enum):
     Unconfirmed = 24
@@ -68,14 +69,18 @@
         self.crc9: int = crc9 if isinstance(crc9, int) else ba2int(crc9[::-1])
         calculated_crc9 = self.calculate_crc9()
         if self.crc9 <= 0:
             self.crc9 = calculated_crc9
         self.crc9_ok: bool = self.crc9 == calculated_crc9
 
     @staticmethod
+    def get_data_type() -> DataTypes:
+        return DataTypes.Rate1Data
+
+    @staticmethod
     def validate_packet_type(packet_type: Rate1DataTypes, data_length: int) -> bool:
         if data_length == 0 or packet_type == Rate1DataTypes.Undefined:
             return True
         else:
             assert (
                 data_length == packet_type.value
             ), f"{packet_type} data must be {packet_type.value} bytes, got {data_length} bytes"
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/rate34_data.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/rate34_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import enum
 from typing import Union
 
 from bitarray import bitarray
 from bitarray.util import int2ba, ba2int
 from okdmr.dmrlib.etsi.crc.crc9 import CRC9
 from okdmr.dmrlib.etsi.layer2.elements.crc_masks import CrcMasks
+from okdmr.dmrlib.etsi.layer2.elements.data_types import DataTypes
 from okdmr.dmrlib.utils.bits_bytes import bits_to_bytes, bytes_to_bits
 from okdmr.dmrlib.utils.bits_interface import BitsInterface
 
 
 @enum.unique
 class Rate34DataTypes(enum.Enum):
     Undefined = 0
@@ -56,14 +57,18 @@
 
         self.crc9: int = crc9 if isinstance(crc9, int) else ba2int(crc9[::-1])
         calculated_crc9 = self.calculate_crc9()
         if self.crc9 <= 0:
             self.crc9 = calculated_crc9
         self.crc9_ok: bool = self.crc9 == calculated_crc9
 
+    @staticmethod
+    def get_data_type() -> DataTypes:
+        return DataTypes.Rate34Data
+
     def calculate_crc9(self) -> int:
         return CRC9.calculate_from_parts(
             data=self.data,
             serial_number=self.dbsn,
             crc32=self.crc32,
             mask=CrcMasks.Rate34DataContinuation,
         )
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/short_link_control.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/short_link_control.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer2/pdu/slot_type.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer2/pdu/slot_type.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/activity_id.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/activity_id.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/answer_response.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/answer_response.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/channel_timing_opcode.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/channel_timing_opcode.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/dynamic_identifier.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/dynamic_identifier.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/ip_address_identifier.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/ip_address_identifier.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/position_error.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/position_error.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/reason_code.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/reason_code.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/service_options.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/service_options.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/elements/udp_port_identifier.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/elements/udp_port_identifier.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/etsi/layer3/pdu/udp_ipv4_compressed_header.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/etsi/layer3/pdu/udp_ipv4_compressed_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Union, Optional
+from typing import Union, Optional, Literal
 
 from bitarray import bitarray
 from bitarray.util import ba2int, int2ba
-from okdmr.dmrlib.utils.bytes_interface import BytesInterface
 
 from okdmr.dmrlib.etsi.layer3.elements.ip_address_identifier import IPAddressIdentifier
 from okdmr.dmrlib.etsi.layer3.elements.udp_port_identifier import UDPPortIdentifier
 from okdmr.dmrlib.utils.bits_bytes import bits_to_bytes, bytes_to_bits
 from okdmr.dmrlib.utils.bits_interface import BitsInterface
+from okdmr.dmrlib.utils.bytes_interface import BytesInterface
 
 
 class UDPIPv4CompressedHeader(BitsInterface, BytesInterface):
     def __init__(
         self,
         ipv4_identification: int,
         source_ip_address_id: Union[IPAddressIdentifier, int],
@@ -154,7 +154,10 @@
     @staticmethod
     def from_bytes(
         data: bytes, endian: str = "big"
     ) -> Optional["UDPIPv4CompressedHeader"]:
         return UDPIPv4CompressedHeader.from_bits(
             bytes_to_bits(payload=data, endian=endian)
         )
+
+    def as_bytes(self, endian: Literal["big", "little"] = "big") -> bytes:
+        return bits_to_bytes(self.as_bits())
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/hytera/hytera_constants.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/hytera_constants.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/hytera/hytera_ipsc_sync.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/hytera_ipsc_sync.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/hytera/hytera_ipsc_wakeup.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/hytera_ipsc_wakeup.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/hdap.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/hdap.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/hrnp.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/hrnp.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,25 +21,28 @@
     Hytera Radio Network Protocol - big-endian, transport wrapper for Hytera PDUs over IP or USB interface
 
     | Header (0x7E) | HRNP Version (0x00 - 0x04) | Fragment number (0x00 - 0xFF) | Opcode (0x00 - 0xFF) |
     | Source (0x00 - 0xFF) | Destination (0x00 - 0xFF) | Packet Number (0x0000 - 0xFFFF) | Data Length (0x0000 - 0xFFFF) |
     | HRNP Header Checksum (0x0000 - 0xFFFF) | Data (Payload, HDAP in case Opcode == DATA)
     """
 
+    DEFAULT_HEADER: bytes = b"\x7E"
+    DEFAULT_VERSION: bytes = b"\x04"
+
     def __init__(
         self,
         data: Optional[Union[bytes, HDAP]] = None,
         opcode: HRNPOpcodes = HRNPOpcodes.CONNECT,
         source: int = 0x20,
         destination: int = 0x10,
         block_number: int = 0x00,
         packet_number: int = 0x00,
         checksum: Union[int, bytes] = b"\x00\x00",
-        header: Union[int, bytes] = b"\x7E",
-        version: Union[int, bytes] = b"\x04",
+        header: Union[int, bytes] = DEFAULT_HEADER,
+        version: Union[int, bytes] = DEFAULT_VERSION,
     ):
         """
 
         :param data: inner (wrapped) data, can be HDAP
         :param checksum: if non-zero checksum provided, it will be checked
         :param header: constant 0x7E
         :param version: current (last) version is 0x04
@@ -73,14 +76,15 @@
 
     @staticmethod
     def from_bytes(data: bytes, endian: Literal["big", "little"] = "big") -> "HRNP":
         assert (
             len(data) >= 12
         ), f"At least 12-bytes for HRNP required, got {len(data)} bytes instead"
         hrnp_packet_len = int.from_bytes(data[8:10], byteorder="big")
+        assert len(data) >= hrnp_packet_len, f"packet seems incomplete"
         return HRNP(
             header=data[0:1],
             version=data[1:2],
             block_number=data[2],
             opcode=HRNPOpcodes(data[3]),
             source=data[4],
             destination=data[5],
@@ -94,58 +98,65 @@
             self.header
             + self.version
             + bytes(
                 [self.block_number, self.opcode.value, self.source, self.destination]
             )
             + self.packet_number.to_bytes(length=2, byteorder="big")
             + len(self).to_bytes(2, byteorder="big")
-            + self.checksum
+            # checksum must be calculated from data assembled here, not data passed to constructor
+            + self.verify_checksum(self.checksum)[1]
             + (self.data.as_bytes() if self.has_data() else b"")
         )
 
     def has_data(self):
         return self.opcode == HRNPOpcodes.DATA
 
     def __len__(self):
         return 12 + (len(self.data) if self.has_data() else 0)
 
     def __repr__(self):
-        return (
-            f"[HRNP v{self.version.hex()}] [SOURCE: {self.source}] [DESTINATION: {self.destination}] "
-            f"[PN: {self.packet_number}] [BLOCK: {self.block_number}] [{self.opcode}] "
-            + (repr(self.data) if self.opcode == HRNPOpcodes.DATA else "")
+        return f"[HRNP v{self.version.hex()}] [SOURCE: {self.source}] [DESTINATION: {self.destination}] " f"[PN: {self.packet_number}] [BLOCK: {self.block_number}] [{self.opcode}] " + (
+            f"[CHECKSUM: {self.checksum.hex()}] " if hasattr(self, "checksum") else f""
+        ) + (
+            repr(self.data) if self.opcode == HRNPOpcodes.DATA else ""
         )
 
     def verify_checksum(
         self, checksum: Union[bytes, int] = b"\x00\x00"
     ) -> Tuple[bool, bytes]:
+        # checksumed data
         checked_data: bytes = (
             self.header
             + self.version
             + bytes(
                 [self.block_number, self.opcode.value, self.source, self.destination]
             )
             + self.packet_number.to_bytes(length=2, byteorder="big")
             + len(self).to_bytes(2, byteorder="big")
         )
+
         if self.has_data():
             checked_data += self.data.as_bytes()
+
         if len(checked_data) % 2 == 1:
-            # pad with single zero byte, to allow for crc16 checksum
+            # add padding byte
             checked_data += b"\x00"
 
+        # calc checksum
+        check: int = 0
+
+        for i in range(0, len(checked_data), 2):
+            check += int.from_bytes(checked_data[i : i + 2], byteorder="big")
+
+        while check >> 16:
+            check = (check & 0xFFFF) + (check >> 16)
+
+        check = ~check & 0xFFFF
+
+        # make check and checksum comparable
         checksum: int = (
             checksum
             if isinstance(checksum, int)
             else int.from_bytes(checksum, byteorder="big")
         )
 
-        # weird quirk, checksum is always off-by-one when opcode is HRNPOpcodes.DATA
-        check: int = 1 if self.has_data() else 0
-
-        for i in range(0, len(checked_data), 2):
-            check = (
-                check + int.from_bytes(checked_data[i : i + 2], byteorder="big")
-            ) & 0xFFFF
-        check = (check ^ 0xFFFF) & 0xFFFF
-
         return check == checksum, check.to_bytes(length=2, byteorder="big")
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/hstrp.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/hstrp.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,68 +12,68 @@
 class HSTRPPacketType(BytesInterface):
     """
     Represents single byte that indicate contents of HSTRP PDU
     """
 
     def __init__(
         self,
-        is_option: bool = False,
+        have_options: bool = False,
         is_reject: bool = False,
         is_close: bool = False,
         is_connect: bool = False,
         is_heartbeat: bool = False,
         is_ack: bool = False,
     ):
-        self.is_option: bool = is_option
+        self.have_options: bool = have_options
         self.is_reject: bool = is_reject
         self.is_close: bool = is_close
         self.is_connect: bool = is_connect
         self.is_heartbeat: bool = is_heartbeat
         self.is_ack: bool = is_ack
 
     @staticmethod
     def from_bytes(
         data: bytes, endian: Literal["big", "little"] = "big"
     ) -> Optional["HSTRPPacketType"]:
         assert len(data) > 0, f"HSTRP Option Byte needs at least one byte"
         bits = bytes_to_bits(data[0:1])
         return HSTRPPacketType(
-            is_option=bits[2] == 1,
+            have_options=bits[2] == 1,
             is_reject=bits[3] == 1,
             is_close=bits[4] == 1,
             is_connect=bits[5] == 1,
             is_heartbeat=bits[6] == 1,
             is_ack=bits[7] == 1,
         )
 
     def __repr__(self) -> str:
         return (
             "HSTRPPacketType "
-            + ("IS_OPTION " if self.is_option else "")
+            + ("HAVE_OPTIONS " if self.have_options else "")
             + ("IS_REJECT " if self.is_reject else "")
             + ("IS_CLOSE " if self.is_close else "")
             + ("IS_CONNECT " if self.is_connect else "")
             + ("IS_HEARTBEAT " if self.is_heartbeat else "")
             + ("IS_ACK " if self.is_ack else "")
         ).strip()
 
     @property
     def has_options(self):
-        return not self.is_heartbeat and self.is_option
+        return not self.is_heartbeat and self.have_options
 
     @property
     def has_data(self):
-        return self.is_option or self.is_ack
+        return self.have_options or self.is_ack
 
     def as_bytes(self, endian: Literal["big", "little"] = "big") -> bytes:
         return bitarray(
             [
                 False,
                 False,
-                self.is_option,
+                self.have_options,
                 self.is_reject,
                 self.is_close,
                 self.is_connect,
                 self.is_heartbeat,
                 self.is_ack,
             ]
         ).tobytes()
@@ -109,34 +109,34 @@
         self.options.append((command, data))
         return self
 
     def as_bytes(self, endian: Literal["big", "little"] = "big") -> bytes:
         options_count: int = len(self.options)
         current_option: int = 0
         rtn = b""
-        for (command, data) in self.options:
+        for command, data in self.options:
             is_last: bool = current_option == (options_count - 1)
             current_option += 1
 
             rtn += (
                 bytes([command.value | (0x80 if not is_last else 0x00), len(data)])
                 + data
             )
         return rtn
 
     def __len__(self) -> int:
         length: int = 0
-        for (command, data) in self.options:
+        for command, data in self.options:
             length += 2 + len(data)
         return length
 
     def __repr__(self) -> str:
         r: str = ""
-        for (command, data) in self.options:
-            r += f"[{command}: {int.from_bytes(data, byteorder='little') if command != HSTRPOptionType.RTP else ''}] "
+        for command, data in self.options:
+            r += f"[{command}: {int.from_bytes(data, byteorder='big') if command != HSTRPOptionType.RTP else ''}] "
         return r
 
     @staticmethod
     def from_bytes(
         data: bytes, endian: Literal["big", "little"] = "big"
     ) -> "HSTRPOptions":
         options = HSTRPOptions()
@@ -216,14 +216,15 @@
 
         pkt_type: HSTRPPacketType = HSTRPPacketType.from_bytes(data[3:4])
         options = (
             HSTRPOptions.from_bytes(data[6:])
             if pkt_type.has_options
             else HSTRPOptions()
         )
+
         # payload might be there even if the options is_option=False
         payload = (
             HDAP.from_bytes(data[6 + len(options) :])
             if pkt_type.has_data or len(data) > 6 + len(options)
             else None
         )
 
@@ -251,12 +252,12 @@
                 if isinstance(self.payload, BytesInterface)
                 else b""
             )
         )
 
     def __repr__(self) -> str:
         label = f"[{self.pkt_type}] [S/N: {self.sn}]"
-        if isinstance(self.options, HSTRPOptions):
+        if isinstance(self.options, HSTRPOptions) and len(self.options.options) > 0:
             label += "\n\tOPTIONS: " + repr(self.options)
         if isinstance(self.payload, BytesInterface):
             label += "\n\tPAYLOAD: " + repr(self.payload)
         return label
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/location_protocol.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/location_protocol.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,48 +71,66 @@
         latitude: Union[bytes, float],
         east_west: Literal["E", "W"],
         longitude: Union[bytes, float],
         speed_knots: Union[bytes, float],
         direction: Union[bytes, int],
     ):
         self.data_valid: Literal["A", "V"] = data_valid
-        self.greenwich_time: time = (
+        self.greenwich_time: Optional[time] = (
             greenwich_time
             if isinstance(greenwich_time, time)
-            else time(
-                hour=int(greenwich_time[0:2]),
-                minute=int(greenwich_time[2:4]),
-                second=int(greenwich_time[4:6]),
+            else (
+                time(
+                    hour=int(greenwich_time[0:2]),
+                    minute=int(greenwich_time[2:4]),
+                    second=int(greenwich_time[4:6]),
+                )
+                if len(greenwich_time.replace(b"\x00", b""))
+                else None
             )
         )
-        self.greenwich_date: date = (
+        self.greenwich_date: Optional[date] = (
             greenwich_date
             if isinstance(greenwich_date, date)
-            else date(
-                day=int(greenwich_date[0:2]),
-                month=int(greenwich_date[2:4]),
-                year=2000 + int(greenwich_date[4:6]),
+            else (
+                date(
+                    day=int(greenwich_date[0:2]),
+                    month=int(greenwich_date[2:4]),
+                    year=2000 + int(greenwich_date[4:6]),
+                )
+                if len(greenwich_date.replace(b"\x00", b""))
+                else None
             )
         )
         self.north_south: Literal["N", "S"] = north_south
         self.east_west: Literal["E", "W"] = east_west
         self.latitude: float = (
-            latitude if isinstance(latitude, float) else float(latitude.decode("ascii"))
+            float(latitude.decode("ascii"))
+            if isinstance(latitude, bytes)
+            else float(latitude)
         )
         self.longitude: float = (
-            longitude
-            if isinstance(longitude, float)
-            else float(longitude.decode("ascii"))
+            float(longitude.decode("ascii"))
+            if isinstance(longitude, bytes)
+            else longitude
         )
         self.speed_knots: float = (
             speed_knots
             if isinstance(speed_knots, float)
-            else float(speed_knots.decode("ascii"))
+            else (
+                float(speed_knots.decode("ascii"))
+                if len(speed_knots.replace(b"\x00", b""))
+                else 0
+            )
+        )
+        self.direction: int = (
+            direction
+            if isinstance(direction, int)
+            else (int(direction) if len(direction.replace(b"\x00", b"")) else 0)
         )
-        self.direction: int = int(direction)
 
     @staticmethod
     def from_bytes(
         data: bytes, endian: Literal["big", "little"] = "big"
     ) -> Optional["GPSData"]:
         assert (
             len(data) == 40
@@ -125,39 +143,69 @@
             latitude=data[14:23],
             east_west="E" if data[23:24] == b"E" else "W",
             longitude=data[24:34],
             speed_knots=data[34:37],
             direction=data[37:40],
         )
 
+    @staticmethod
+    def zero() -> "GPSData":
+        return GPSData(
+            data_valid="V",
+            greenwich_time=time(),
+            greenwich_date=date.today(),
+            latitude=0,
+            longitude=0,
+            east_west="E",
+            north_south="N",
+            speed_knots=0.0,
+            direction=0,
+        )
+
     def as_bytes(self, endian: Literal["big", "little"] = "big") -> bytes:
         return (
             self.data_valid
-            + self.greenwich_time.strftime("%H%M%S")
-            + self.greenwich_date.strftime("%d%m%y")
+            + (
+                "\0" * 6
+                if self.greenwich_time is None
+                else self.greenwich_time.strftime("%H%M%S")
+            )
+            + (
+                "\0" * 6
+                if self.greenwich_date is None
+                else self.greenwich_date.strftime("%d%m%y")
+            )
             + self.north_south
             + f"{self.latitude:09.4f}"
             + self.east_west
             + f"{self.longitude:010.4f}"
-            + f"{self.speed_knots:03}"
-            + f"{self.direction:03}"
+            + ("\0" * 3 if self.speed_knots <= 0 else f"{self.speed_knots:03}")
+            + ("\0" * 3 if not self.direction else f"{self.direction:03}")
         ).encode("ascii")
 
     def __repr__(self) -> str:
         _lat: str = f"{self.latitude:09.4f}"
         _lon: str = f"{self.longitude:010.4f}"
 
         return (
             ("VALID " if self.data_valid else "INVALID ")
-            + self.greenwich_date.strftime("%H:%M:%S ")
-            + self.greenwich_time.strftime("%d.%m.%Y ")
+            + (
+                ""
+                if not self.greenwich_date
+                else self.greenwich_date.strftime("%H:%M:%S ")
+            )
+            + (
+                ""
+                if not self.greenwich_time
+                else self.greenwich_time.strftime("%d.%m.%Y ")
+            )
             + self.north_south
-            + f"{round(float(_lat[:2]) + float(_lat[2:])/60.0, 8)} "
+            + f"{round(float(_lat[:2]) + float(_lat[2:]) / 60.0, 8)} "
             + self.east_west
-            + f"{round(float(_lon[:3]) + float(_lon[3:])/60.0, 8)} "
+            + f"{round(float(_lon[:3]) + float(_lon[3:]) / 60.0, 8)} "
             + f"speed:{round(self.speed_knots * 1.852, 5)} km/h "
             + f"direction:{self.direction}°"
         )
 
 
 class LocationProtocol(HDAP):
     """
@@ -165,16 +213,16 @@
     """
 
     def __init__(
         self,
         opcode: Union[bytes, LocationProtocolSpecificService],
         request_id: Union[int, bytes],
         radio_ip: Union[bytes, RadioIP],
-        result: Union[int, bytes],
-        gpsdata: Union[bytes, GPSData],
+        result: Union[int, bytes] = 0,  # 0 = OK, SUCCESS RESULT
+        gpsdata: Union[bytes, GPSData] = GPSData.zero(),
         is_reliable: bool = False,
     ):
         super().__init__(is_reliable=is_reliable)
         self.specific_service = (
             opcode
             if isinstance(opcode, LocationProtocolSpecificService)
             else LocationProtocolSpecificService(
@@ -211,14 +259,19 @@
         if self.specific_service == LocationProtocolSpecificService.StandardReport:
             return (
                 self.request_id.to_bytes(length=4, byteorder="big")
                 + self.radio_ip.as_bytes()
                 + self.result.value.to_bytes(length=2, byteorder="big")
                 + self.gpsdata.as_bytes()
             )
+        elif self.specific_service == LocationProtocolSpecificService.StandardRequest:
+            return (
+                self.request_id.to_bytes(length=4, byteorder="big")
+                + self.radio_ip.as_bytes()
+            )
         raise ValueError(f"LP get_payload not implemented for {self.specific_service}")
 
     @staticmethod
     def from_bytes(
         data: bytes, endian: Literal["big", "little"] = "big"
     ) -> "LocationProtocol":
         (is_reliable, service_type) = HDAP.get_reliable_and_service(data[0:1])
@@ -232,18 +285,24 @@
                 opcode=opcode,
                 request_id=data[5:9],
                 radio_ip=data[9:13],
                 result=data[13:15],
                 gpsdata=data[15:55],
                 is_reliable=is_reliable,
             )
+        elif opcode == LocationProtocolSpecificService.StandardRequest:
+            return LocationProtocol(
+                opcode=opcode, request_id=data[5:9], radio_ip=data[9:13]
+            )
 
         raise ValueError(f"LP {opcode} not yet implemented")
 
     def __repr__(self):
         repre: str = f"[LP {self.general_service} {self.specific_service}] "
         if self.specific_service == LocationProtocolSpecificService.StandardReport:
             repre += (
                 f"[Request ID {self.request_id}] [Radio IP {self.radio_ip}] "
                 f"[Result {self.result}] [GpsData {self.gpsdata}]"
             )
+        elif self.specific_service == LocationProtocolSpecificService.StandardRequest:
+            repre += f"[Request ID {self.request_id}] [Radio IP {self.radio_ip}] "
         return repre
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/radio_ip.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/radio_ip.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,26 +7,33 @@
 class RadioIP(BytesInterface):
     """
     Simple wrapper around RadioID/RadioIP fields, Hytera uses similar to Motorola Subnet and ID,
     Hytera limits subnet to single byte (first IP octet)
     """
 
     def __init__(self, radio_id: Union[int, bytes], subnet: int = 0x0A):
+        """
+
+        @param radio_id:
+        @param subnet: 0x0A is "10" as in IP "10.0.0.1"
+        """
         self.subnet: int = subnet
         self.radio_id: int = (
             radio_id
             if isinstance(radio_id, int)
             else int.from_bytes(radio_id, byteorder="big")
         )
 
     @staticmethod
     def from_bytes(
         data: bytes, endian: Literal["big", "little"] = "big"
     ) -> Optional["RadioIP"]:
-        assert len(data) >= 4, f"4 bytes required to construct RadioIP"
+        assert (
+            len(data) == 4
+        ), f"4 bytes required to construct RadioIP, got {len(data)} :: {data.hex()}"
         if endian == "little":
             data = data[::-1]
         return RadioIP(subnet=data[0], radio_id=data[1:4])
 
     def as_bytes(self, endian: Literal["big", "little"] = "big") -> bytes:
         raw: bytes = bytes([self.subnet]) + self.radio_id.to_bytes(
             length=3, byteorder="big"
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/hytera/pdu/radio_registration_service.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/hytera/pdu/radio_registration_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -121,9 +121,21 @@
                 opcode=opcode,
                 radio_ip=data[5:9],
                 radio_state=data[9],
             )
 
     def __repr__(self) -> str:
         r: str = f"[{self.opcode}]"
-        # TODO add more descriptive fields
+        # radio ip is in all messages
+        if self.radio_ip:
+            r += f" {repr(self.radio_ip)}"
+        # answer contains result and renew period
+        if self.opcode == RRSTypes.RadioRegistrationAnswer:
+            if self.result:
+                r += f" [RESULT: {self.result}]"
+            if self.renew_time_seconds:
+                r += f" [RENEW PERIOD: {self.renew_time_seconds}s]"
+        # status check answer contains status
+        if self.opcode == RRSTypes.RegistrationStatusCheckAnswer:
+            if self.radio_state:
+                r += f" [STATUS: {self.radio_state}]"
         return r
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/motorola/automatic_registration_service.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/motorola/automatic_registration_service.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/motorola/lrrp.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/motorola/lrrp.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/motorola/mbxml.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/motorola/mbxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+import logging
 import math
 from copy import copy
 from datetime import datetime
 from typing import List, Optional, Tuple, Dict, Type, Union
 from xml.dom import minidom
 
 from bitarray.util import ba2int
@@ -162,15 +163,14 @@
     ARRP_InformationProtocolRequest_NCDT = (0x26, True, "")
     ARRP_InformationProtocolReport_NCDT = (0x27, True, "")
 
     # fmt:on
 
     @classmethod
     def resolve(cls, docid: int) -> Optional["MBXMLDocumentIdentifier"]:
-
         for _doc in cls:
             (_docid, _is_ncdt, _) = _doc.value
             if _docid == docid:
                 return _doc
 
         return None
 
@@ -203,14 +203,15 @@
         self.length: Optional[int] = length
         self.path: Optional[str] = path
         self.value: Optional[MBXMLToken_Value] = value
         self.constant_position: Optional[int] = constant_position
 
     def get_value(self, doc: "MBXMLDocument") -> MBXMLToken_Value:
         if self.token_type in (GlobalToken.STR8_ST, GlobalToken.OPAQUE_T):
+            print(f"get_value for {self.token_type} from {self.value} ->read_opaque")
             (val, idx) = MBXML.read_opaque(doc.constants_table, self.value)
             return val.decode("ascii")
         elif isinstance(self.value, bytes):
             return self.value.hex().upper()
         elif self.token_type in (GlobalToken.SFLOATVAR, GlobalToken.UFLOATVAR):
             return round(self.value, 5)
         return self.value
@@ -362,25 +363,28 @@
         elements_config: Optional[Dict[int, MBXMLToken]] = None,
         attributes_config: Optional[Dict[int, MBXMLToken]] = None,
         constants_table: bytes = b"",
         default_constants_table: Optional[Dict[int, MBXMLToken]] = None,
     ) -> None:
         self.id: MBXMLDocumentIdentifier = document_id
         self.constants_table: bytes = constants_table
+        self.is_constant_table_default: bool = True
+        """Indicates whether the table is expected per document id or custom (that needs to be encoded into bytes)"""
         self.default_constants_table: Dict[int, MBXMLToken] = (
             default_constants_table or {}
         )
         self.parts: List[MBXMLToken] = []
         self.elements_config: Dict[int, MBXMLToken] = elements_config or {}
         self.attributes_config: Dict[int, MBXMLToken] = attributes_config or {}
 
     def set_default_constants_table(
         self, constants: Dict[int, MBXMLToken]
     ) -> "MBXMLDocument":
         self.default_constants_table = constants
+        self.is_constant_table_default = True
         self.constants_table = MBXML.build_constants_table(self.id)
         return self
 
     def __str__(self) -> str:
         return f"[MBXMLDocument {self.id.name} (+ {len(self.parts)} elements)"
 
     def __repr__(self) -> str:
@@ -440,26 +444,25 @@
         is_request: bool = True,
     ) -> MBXMLToken:
         """
         attributes can be specified as name=>value or id=>value
         """
         tokens = cls.get_known_tokens(is_request=is_request)
         for tokenset in tokens:
-            for (tokendef_id, tokendef_setting) in tokenset.items():
-
+            for tokendef_id, tokendef_setting in tokenset.items():
                 valid_candidate: bool = (
                     tokendef_setting.name == name
                     if isinstance(name, str)
                     else tokendef_id == name
                 )
                 attributes_to_set: List[MBXMLToken] = list()
 
                 if valid_candidate:
                     # verify found token has required attributes
-                    for (attr_key, attr_val) in attributes.items():
+                    for attr_key, attr_val in attributes.items():
                         (attr_copy, value_changed) = cls.get_attribute(
                             name=attr_key, value=attr_val
                         )
                         if attr_copy.token_id not in tokendef_setting.attributes:
                             valid_candidate = False
                             break
                         elif value_changed:
@@ -490,15 +493,15 @@
         is_request: bool = True,
     ) -> (MBXMLToken, bool):
         """
         Returns token (if found, otherwise raises ModuleNotFoundError) and bool indication, whether the value is different from default (implied) one
         """
         attrs = cls.get_known_attributes(is_request=is_request)
         for attrset in attrs:
-            for (attrdef_id, attrdef_setting) in attrset.items():
+            for attrdef_id, attrdef_setting in attrset.items():
                 if (
                     attrdef_setting.name == name
                     if isinstance(name, str)
                     else attrdef_id == name
                 ):
                     if (
                         attrdef_setting.value is not None
@@ -721,32 +724,53 @@
             + value.hour * 2**12
             + value.minute * 2**6
             + value.second
         ).to_bytes(byteorder="big", length=5)
 
     @classmethod
     def read_document(
-        cls, doctype: MBXMLDocumentIdentifier, data: bytes, idx: int
+        cls,
+        doctype: MBXMLDocumentIdentifier,
+        data: bytes,
+        idx: int,
+        previous_doc: Optional[MBXMLDocument] = None,
     ) -> MBXMLDocument:
         doctype_configuration = cls.get_implementation(doctype).get_configuration(
             doctype
         )
         (document_id, has_no_constants_table, _) = doctype.value
         doc = MBXMLDocument(
             document_id=doctype,
             elements_config=doctype_configuration[MBXMLTokenType.ELEMENT_TOKEN],
             attributes_config=doctype_configuration[MBXMLTokenType.ATTRIBUTE_TOKEN],
         )
         if cls.DEBUG:
             print(repr(doc))
 
         if not has_no_constants_table:
-            # fill in constants, if indicated
-            (constants, idx) = cls.read_opaque(data, idx)
-            doc.constants_table = constants
+            (cdt_length, idx) = cls.read_uintvar(data, idx)
+            assert idx >= 1, f"MBXML CDT_LEN value is invalid"
+            if idx == 1:
+                # 2.11 Representation of Multiple Documents
+                # special cdt len value (1) means to CDT from previous document
+                if previous_doc:
+                    doc.constants_table = previous_doc.constants_table
+                    doc.is_constant_table_default = (
+                        previous_doc.is_constant_table_default
+                    )
+                else:
+                    logging.getLogger().error(
+                        f"CDT_LEN(1) requires previous_doc be available, CDT will not correspond to tokens"
+                    )
+            else:
+                # cdt_length does not include itself
+                (doc.constants_table, idx) = cls.read_opaque_defined_size(
+                    data, idx, cdt_length
+                )
+                doc.is_constant_table_default = False
         elif MBXMLTokenType.CONSTANT_TOKEN in doctype_configuration:
             doc.set_default_constants_table(
                 doctype_configuration[MBXMLTokenType.CONSTANT_TOKEN]
             )
 
         _lastidx = 0
         while idx != len(data):
@@ -885,15 +909,17 @@
 
             return LRRP
         elif prefix == "ARRP":
             from okdmr.dmrlib.motorola.arrp import ARRP
 
             return ARRP
 
-        print(f"get_implementation returns default for {doc_type}")
+        logging.getLogger().warning(
+            f"get_implementation returns default for {doc_type}"
+        )
         return MBXMLDocument
 
     @classmethod
     def build_constants_table(cls, document_type: MBXMLDocumentIdentifier):
         impl = cls.get_implementation(doc_type=document_type)
         values: Dict[int, MBXMLToken] = impl.get_configuration(doc_type=document_type)[
             MBXMLTokenType.CONSTANT_TOKEN
@@ -913,28 +939,37 @@
         data_len = len(data)
         rtn: List[MBXMLDocument] = []
 
         if cls.DEBUG:
             print(f"MBXML.from_bytes {data.hex()}")
 
         idx: int = 0
+        last_doc: Optional[MBXMLDocument] = None
         while True:
             (doc_id, idx) = cls.read_uintvar(data, idx)
-            doctype = MBXMLDocumentIdentifier.resolve(doc_id)
+            doctype = MBXMLDocumentIdentifier.resolve(docid=doc_id)
             (doc_len_bytes, idx) = cls.read_uintvar(data, idx)
-            rtn.append(cls.read_document(doctype, data, idx))
+            rtn.append(
+                cls.read_document(
+                    doctype=doctype, data=data, idx=idx, previous_doc=last_doc
+                )
+            )
             idx += doc_len_bytes
             if idx == data_len:
+                # no more documents in data
                 break
 
         cls.DEBUG = False
         return rtn
 
     @classmethod
     def as_bytes(cls, doc: MBXMLDocument) -> bytes:
         rtn = cls.write_uintvar(doc.id.value[0])
 
         body = b""
+        if not doc.is_constant_table_default:
+            body += cls.write_uintvar(len(doc.constants_table)) + doc.constants_table
+
         for part in doc.parts:
             body += cls.write_part(part)
 
         return rtn + cls.write_uintvar(len(body)) + body
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/motorola/text_messaging_service.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/motorola/text_messaging_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,20 +53,20 @@
         is_reserved: Union[int, bool] = False,
         is_control_message: Union[int, bool] = False,
         pdu_type: Union[int, TMSPDUType] = 0,
     ):
         self.has_more_headers: bool = bool(has_more_headers)
         self.is_acknowledged: bool = bool(is_acknowledged)
         self.is_reserved: bool = bool(is_reserved)
-        self.is_control_message: bool = bool(is_control_message)
         self.pdu_type: TMSPDUType = (
             TMSPDUType((is_control_message, pdu_type))
             if isinstance(pdu_type, int)
             else pdu_type
         )
+        self.is_control_message: bool = bool(self.pdu_type.value[0])
 
     def set_has_more_headers(self, has: bool) -> "FirstHeader":
         self.has_more_headers = has
         return self
 
     @staticmethod
     def from_bytes(
@@ -101,14 +101,15 @@
     def __repr__(self) -> str:
         return (
             f"[{self.pdu_type.name}("
             + (
                 ("HAS-EXT " if self.has_more_headers else "")
                 + ("IS-ACK " if self.is_acknowledged else "")
                 + ("IS-CONTROL-MSG " if self.is_control_message else "IS-USER-DATA ")
+                + ("IS-RESERVED " if self.is_reserved else "")
             ).strip()
             + ")]"
         )
 
 
 class AvailabilitySecondHeader(BytesInterface):
     def __init__(self, capability: TMSDeviceCapability):
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/tools/pcap_tool.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/tools/pcap_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 import logging
 import sys
 import traceback
-from argparse import ArgumentParser
+from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from typing import Callable, List, Dict, Optional, Tuple
 
 from bitarray import bitarray
 from kaitaistruct import KaitaiStruct
 from okdmr.dmrlib.etsi.fec.vbptc_128_72 import VBPTC12873
 from okdmr.dmrlib.etsi.layer2.burst import Burst
 from okdmr.dmrlib.etsi.layer2.elements.lcss import LCSS
@@ -89,17 +89,17 @@
                 # prettyprint(kaitai_pkt)
                 row = self.map.get(rowkey, dict())
                 subrowkey = f"voice" if burst.is_vocoder else data.__class__.__name__
                 row[data.__class__.__name__] = row.get(data.__class__.__name__, 0) + 1
                 self.map[rowkey] = row
 
     def print_stats(self):
-        for ((slot, frame), dt_stats) in self.map.items():
+        for (slot, frame), dt_stats in self.map.items():
             print(f"SLOT: {slot} FRAME: {frame}")
-            for (dt, dt_count) in dt_stats.items():
+            for dt, dt_count in dt_stats.items():
                 print(f"\tCOUNT: {dt_count}\tDT: {dt}")
 
 
 # noinspection PyDefaultArgument
 class PcapTool:
     """
     Various static methods for working with PCAP/PCAPNG files containing DMR protocols
@@ -344,15 +344,16 @@
                             print("=" * 30, file=sys.stderr)
 
         return statistics
 
     @staticmethod
     def _arguments() -> ArgumentParser:
         parser = ArgumentParser(
-            description="Read and debug UDP packets in PCAP/PCAPNG file"
+            description="Read and debug UDP packets in PCAP/PCAPNG file",
+            formatter_class=ArgumentDefaultsHelpFormatter,
         )
         parser.add_argument(
             "files", type=str, nargs="+", help="PCAP or PCAPNG file to be read"
         )
         parser.add_argument(
             "--ports",
             "-p",
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/transmission/terminal.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/terminal.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/transmission/timeslot.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/timeslot.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ):
         super().__init__(observers=observers)
         self.timeslot = timeslot
         self.last_packet_received: float = 0
         self.rx_sequence: int = 0
         self.reset_rx_sequence: bool = False
         self.transmission: Transmission = Transmission(self)
-        self.color_code: int = 0
+        self.colour_code: int = 0
 
     def voice_transmission_ended(
         self, voice_header: FullLinkControl, blocks: List[BitsInterface]
     ):
         super().voice_transmission_ended(voice_header=voice_header, blocks=blocks)
         self.reset_rx_sequence = True
 
@@ -48,15 +48,15 @@
     def process_burst(self, dmrdata: Burst) -> Burst:
         self.last_packet_received = time()
         if (
             not dmrdata.is_voice_superframe_start
             or dmrdata.sync_or_embedded_signalling == SyncPatterns.Reserved
         ):
             # Voice burst with SYNC (MS/BS Sourced, TDMA TS1/2, Reserved) do not carry CC information
-            self.color_code = dmrdata.colour_code
+            self.colour_code = dmrdata.colour_code
 
         out: Burst = (
             self.transmission.process_packet(dmrdata)
             .set_sequence_no(self.get_rx_sequence())
             .set_stream_no(self.transmission.stream_no)
         )
 
@@ -67,12 +67,12 @@
         return out
 
     def debug(self, printout: bool = True) -> str:
         status: str = (
             f"[TS {self.timeslot}] "
             f"[STATUS {self.transmission.type.name}] "
             f"[LAST PACKET {datetime.fromtimestamp(self.last_packet_received)} {self.transmission.last_burst_data_type.name}] "
-            f"[COLOR CODE {self.color_code}]"
+            f"[COLOUR CODE {self.colour_code}]"
         )
         if printout:
             print(status)
         return status
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/transmission/transmission.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/transmission.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,17 +77,17 @@
         self.blocks_received += 1
 
     def process_data_header(self, data_header: DataHeader):
         self.ensure_transmission(TransmissionTypes.DataTransmission)
 
         if data_header.get_blocks_to_follow():
             if self.blocks_expected == 0:
-                self.blocks_expected = data_header.blocks_to_follow + 1
+                self.blocks_expected = data_header.get_blocks_to_follow() + 1
             elif self.blocks_expected != (
-                self.blocks_received + data_header.blocks_to_follow + 1
+                self.blocks_received + data_header.get_blocks_to_follow() + 1
             ):
                 pass
                 # self.log_warning(
                 #    f"[Blocks To Follow / Appended Blocks] DMR Data Header block count mismatch [{self.blocks_expected} - {self.blocks_received} != {data_header.blocks_to_follow}]"
                 # )
 
         self.header = data_header
@@ -132,15 +132,14 @@
         )
 
     def end_voice_transmission(self):
         if self.finished or self.type == TransmissionTypes.Idle:
             return
         self.log_info(f"[VOICE CALL END]")
         if isinstance(self.header, FullLinkControl):
-
             self.voice_transmission_ended(self.header, self.blocks)
 
             if self.header.full_link_control_opcode == FLCOs.GroupVoiceChannelUser:
                 self.log_info(
                     f"[GROUP] [{self.header.source_address} -> "
                     f"{self.header.group_address}]"
                 )
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/transmission/transmission_observer_interface.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/transmission_observer_interface.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/transmission/transmission_watcher.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/transmission/transmission_watcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,32 +34,38 @@
 
         burst: Optional[Burst] = PcapTool.debug_packet(
             data=data, packet=packet, silent=True
         )
         if burst:
             self.process_burst(burst)
             if self.debug_voice_bytes and burst.is_vocoder:
+                import logging
+
+                if self.get_logger().getEffectiveLevel() < logging.DEBUG:
+                    self.log_error(f"Cannot print Vocoder with logger not being DEBUG")
                 voice_bytes = burst.voice_bits.tobytes()
                 if burst.stream_no != self.last_stream_no:
                     self.last_stream_no = burst.stream_no
-                    print(
-                        f"[STREAM {burst.stream_no}] [FROM {burst.source_radio_id}] [TO {burst.target_radio_id}]"
+                    self.log_debug(
+                        f"[STREAM {burst.stream_no.hex().upper()}] [FROM {burst.source_radio_id}] [TO {burst.target_radio_id}]"
                     )
-                print(f"{[x for x in voice_bytes[:9]]},")
-                print(f"{[x for x in voice_bytes[9:18]]},")
-                print(f"{[x for x in voice_bytes[18:]]},")
+                self.log_debug(f"{[x for x in voice_bytes[:9]]},")
+                self.log_debug(f"{[x for x in voice_bytes[9:18]]},")
+                self.log_debug(f"{[x for x in voice_bytes[18:]]},")
 
     def process_burst(self, burst: Burst) -> Optional[Burst]:
+        if not burst:
+            return
         if not burst.target_radio_id:
             if type(burst) not in (HyteraIPSCSync, HyteraIPSCWakeup):
-                print(
+                self.log_warning(
                     f"TransmissionWatcher.process_burst ignoring {burst.__class__.__name__} with target radio id {burst.target_radio_id}"
                 )
-                print(repr(burst))
-            return None
+                self.log_warning(repr(burst))
+                return None
         self.ensure_terminal(burst.target_radio_id)
         return self.terminals[burst.target_radio_id].process_incoming_burst(
             burst=burst, timeslot=burst.timeslot
         )
 
     def end_all_transmissions(self) -> None:
         for terminal in self.terminals.values():
```

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/utils/bits_bytes.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/utils/bits_bytes.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/utils/bytes_interface.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/utils/bytes_interface.py`

 * *Files identical despite different names*

### Comparing `ok-dmrlib-0.7/okdmr/dmrlib/utils/parsing.py` & `ok_dmrlib-0.8.0/okdmr/dmrlib/utils/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,27 +31,26 @@
         rtsp = RealTimeTransportProtocol.from_bytes(bytedata)
         return rtsp
     elif (
         int.from_bytes(bytedata[0:8], byteorder="little") == 0
         or bytedata[0:4] == b"ZZZZ"
         or (
             len(bytedata) >= 21 and bytedata[20] == bytedata[21]
-        )  # color code shall be same in both bytes
+        )  # colour code shall be same in both bytes
     ):
         if bytedata[5:9] == bytes([0x00, 0x00, 0x00, 0x14]):
             return IpSiteConnectHeartbeat.from_bytes(bytedata)
         else:
             return IpSiteConnectProtocol.from_bytes(bytedata)
     else:
         # HDAP
         return HyteraDmrApplicationProtocol.from_bytes(bytedata)
 
 
 def try_parse_packet(udpdata: bytes) -> Optional[KaitaiStruct]:
-
     try:
         # known unsupported, that incidentally gets decoded as Hytera IPSC packet
         if udpdata[:4] == b"USRP":
             return None
     finally:
         pass
```

