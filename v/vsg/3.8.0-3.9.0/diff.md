# Comparing `tmp/vsg-3.8.0.tar.gz` & `tmp/vsg-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vsg-3.8.0.tar", last modified: Sun Feb 13 15:07:36 2022, max compression
+gzip compressed data, was "dist/vsg-3.9.0.tar", last modified: Sun Feb 20 15:31:39 2022, max compression
```

## Comparing `vsg-3.8.0.tar` & `vsg-3.9.0.tar`

### file list

```diff
@@ -1,1381 +1,1430 @@
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.810000 vsg-3.8.0/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       96 2021-03-06 15:16:58.000000 vsg-3.8.0/MANIFEST.in
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9674 2022-02-13 15:07:36.810000 vsg-3.8.0/PKG-INFO
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     7116 2022-02-05 12:05:24.000000 vsg-3.8.0/README.rst
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      147 2022-02-13 15:07:36.810000 vsg-3.8.0/setup.cfg
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2195 2021-03-20 15:05:16.000000 vsg-3.8.0/setup.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.580000 vsg-3.8.0/vsg/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      497 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/CustomArgumentParser.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     6025 2022-01-31 12:23:48.000000 vsg-3.8.0/vsg/__main__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1186 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/__parser__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4973 2022-02-05 19:36:49.000000 vsg-3.8.0/vsg/__rule_doc_gen__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4127 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/apply_rules.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      715 2022-02-12 14:46:58.000000 vsg-3.8.0/vsg/block_rule.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4873 2022-01-31 12:42:04.000000 vsg-3.8.0/vsg/cmd_line_args.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     7623 2021-10-31 12:21:33.000000 vsg-3.8.0/vsg/config.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      539 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/deprecated_rule.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      227 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/exceptions.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4285 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/junit.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9261 2022-02-12 14:46:58.000000 vsg-3.8.0/vsg/parser.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      627 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/proposed_rule.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.580000 vsg-3.8.0/vsg/report/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       85 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/report/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      876 2021-03-06 15:16:58.000000 vsg-3.8.0/vsg/report/summary_stdout.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      862 2021-03-06 15:16:58.000000 vsg-3.8.0/vsg/report/syntastic_stdout.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3140 2021-03-06 15:16:58.000000 vsg-3.8.0/vsg/report/vsg_stdout.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8438 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rule.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.590000 vsg-3.8.0/vsg/rule_group/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rule_group/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      458 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rule_group/alignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      460 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rule_group/blank_line.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      448 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rule_group/case.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      452 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rule_group/indent.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      602 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rule_group/length.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      452 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rule_group/naming.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      458 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rule_group/structure.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      456 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rule_group/whitespace.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    12965 2022-02-05 12:32:32.000000 vsg-3.8.0/vsg/rule_list.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.610000 vsg-3.8.0/vsg/rules/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9864 2022-02-13 14:52:39.000000 vsg-3.8.0/vsg/rules/__init__.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.610000 vsg-3.8.0/vsg/rules/after/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       94 2021-12-26 15:41:52.000000 vsg-3.8.0/vsg/rules/after/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5843 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/after/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9681 2022-02-05 19:38:07.000000 vsg-3.8.0/vsg/rules/after/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5934 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/after/rule_003.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.610000 vsg-3.8.0/vsg/rules/alias_declaration/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      345 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/rules/alias_declaration/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      628 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/alias_declaration/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      710 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/alias_declaration/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      733 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/alias_declaration/rule_101.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      507 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/alias_declaration/rule_102.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      517 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/alias_declaration/rule_300.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      589 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/alias_declaration/rule_500.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      583 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/alias_declaration/rule_501.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      645 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/alias_declaration/rule_502.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2050 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/alias_declaration/rule_503.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      689 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/alias_declaration/rule_600.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      689 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/alias_declaration/rule_601.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3036 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/align_consecutive_lines_after_line_starting_with_token_and_stopping_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4528 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/align_consecutive_lines_starting_with_a_comment_above_line_starting_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2610 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/align_left_token_with_right_token_if_right_token_starts_a_line.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8616 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/align_tokens_in_region_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9818 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/align_tokens_in_region_between_tokens_skipping_lines_starting_with_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    13077 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/align_tokens_in_region_between_tokens_unless_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    10748 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/align_tokens_in_region_between_tokens_when_between_tokens_unless_between_tokens.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.620000 vsg-3.8.0/vsg/rules/architecture/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1087 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/architecture/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      507 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      657 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      627 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      585 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      678 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      728 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      487 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      545 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      577 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      846 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      694 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      676 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      664 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      659 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      681 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      685 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      584 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      646 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_018.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      578 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_019.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      578 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_020.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      578 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_021.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      694 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_022.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1010 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_024.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1139 2022-02-10 23:52:45.000000 vsg-3.8.0/vsg/rules/architecture/rule_025.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1472 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_026.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1293 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_027.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      627 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_028.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1580 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_029.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_030.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      633 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_031.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      642 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_032.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      650 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_033.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      636 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_200.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1878 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_600.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9489 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/architecture/rule_601.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.620000 vsg-3.8.0/vsg/rules/assert_statement/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      188 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/assert_statement/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      812 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/assert_statement/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1176 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/assert_statement/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1298 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/assert_statement/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1182 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/assert_statement/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1260 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/assert_statement/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4252 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/assert_statement/rule_400.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.620000 vsg-3.8.0/vsg/rules/attribute/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       62 2021-12-26 15:41:52.000000 vsg-3.8.0/vsg/rules/attribute/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      558 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/attribute/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      558 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/attribute/rule_002.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.620000 vsg-3.8.0/vsg/rules/attribute_declaration/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      189 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/attribute_declaration/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      634 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_declaration/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      527 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_declaration/rule_101.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      570 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_declaration/rule_300.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      597 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_declaration/rule_500.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      635 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_declaration/rule_501.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      764 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_declaration/rule_502.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.620000 vsg-3.8.0/vsg/rules/attribute_specification/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      220 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/attribute_specification/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1047 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_specification/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      674 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_specification/rule_101.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      636 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_specification/rule_300.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      663 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_specification/rule_500.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      721 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_specification/rule_501.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      649 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_specification/rule_502.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      649 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/attribute_specification/rule_503.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3246 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/blank_line_above_line_starting_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1054 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/blank_line_above_line_starting_with_token_when_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3256 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/blank_line_below_line_ending_with_several_possible_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3449 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/blank_line_below_line_ending_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1570 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/blank_lines_between_token_pairs.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.620000 vsg-3.8.0/vsg/rules/block/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      906 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/block/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1171 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1040 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      999 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      563 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      703 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      997 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1305 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      700 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_101.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      553 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_200.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      927 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_201.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      867 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_202.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      590 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_203.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      665 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_204.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      608 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_205.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      490 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_300.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      493 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_301.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      551 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_302.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1379 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_400.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1404 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_401.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      598 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_500.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      557 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_501.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      551 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_502.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      583 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_503.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      553 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_504.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      582 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_505.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      631 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_506.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      633 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_600.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      671 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/block/rule_601.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.620000 vsg-3.8.0/vsg/rules/block_comment/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       94 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/block_comment/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4635 2022-02-12 14:46:58.000000 vsg-3.8.0/vsg/rules/block_comment/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2876 2022-02-12 14:46:58.000000 vsg-3.8.0/vsg/rules/block_comment/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4903 2022-02-12 14:46:58.000000 vsg-3.8.0/vsg/rules/block_comment/rule_003.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.620000 vsg-3.8.0/vsg/rules/case/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      715 2022-02-09 14:33:33.000000 vsg-3.8.0/vsg/rules/case/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      728 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      585 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      587 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      650 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      630 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      688 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      349 2022-02-09 14:33:33.000000 vsg-3.8.0/vsg/rules/case/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      630 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      569 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      821 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      719 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      597 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      647 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      643 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      611 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      631 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      637 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_018.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      859 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_019.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      649 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_020.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      919 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_021.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      611 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/case/rule_200.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      754 2022-02-09 14:33:33.000000 vsg-3.8.0/vsg/rules/case/rule_201.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9591 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/case_utils.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.630000 vsg-3.8.0/vsg/rules/comment/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      127 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/comment/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      632 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/comment/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1098 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/comment/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2556 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/comment/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3251 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/comment/rule_100.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.630000 vsg-3.8.0/vsg/rules/component/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      652 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/component/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      633 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      602 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      642 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      617 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      683 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      603 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      589 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      634 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      557 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      605 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      653 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      654 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      603 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      352 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      693 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1423 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      635 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_018.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1014 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_019.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1762 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_020.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      826 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/component/rule_021.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.630000 vsg-3.8.0/vsg/rules/concurrent/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      342 2021-12-26 15:41:52.000000 vsg-3.8.0/vsg/rules/concurrent/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      907 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/concurrent/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      704 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/concurrent/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1314 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/concurrent/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      946 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/concurrent/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      820 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/concurrent/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      953 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/concurrent/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3667 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/concurrent/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8172 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/concurrent/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    24195 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/concurrent/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1192 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/concurrent/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4092 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/concurrent/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3101 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/consistent_case_of_tokens_from_between_tokens_applied_to_region.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2623 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/consistent_token_case.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.630000 vsg-3.8.0/vsg/rules/constant/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      501 2022-02-07 23:25:33.000000 vsg-3.8.0/vsg/rules/constant/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      645 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      585 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      520 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      632 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      595 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      669 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1579 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      772 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      533 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/rules/constant/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    12445 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2231 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1295 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      610 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    22223 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      674 2022-02-07 23:25:33.000000 vsg-3.8.0/vsg/rules/constant/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      610 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/constant/rule_600.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.630000 vsg-3.8.0/vsg/rules/context/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      868 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/context/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      505 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      612 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      700 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      549 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      655 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      632 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      713 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      711 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      807 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1023 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1124 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      624 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      566 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      578 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      641 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      616 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      659 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_018.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      699 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_019.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      496 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_020.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      810 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_021.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      872 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_022.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      585 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_023.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      689 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_024.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      583 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_025.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      619 2022-02-13 13:33:04.000000 vsg-3.8.0/vsg/rules/context/rule_026.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-13 13:33:04.000000 vsg-3.8.0/vsg/rules/context/rule_027.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      874 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/context/rule_028.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.630000 vsg-3.8.0/vsg/rules/context_ref/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      279 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/context_ref/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      489 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/context_ref/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      611 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/context_ref/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      539 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/context_ref/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      684 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/context_ref/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      729 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/context_ref/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      508 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/context_ref/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      575 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/context_ref/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      472 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/context_ref/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      587 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/context_ref/rule_009.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.640000 vsg-3.8.0/vsg/rules/entity/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      685 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/entity/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      499 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      532 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      547 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      667 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      588 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      616 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      613 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      545 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      608 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      630 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      668 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      596 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      755 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      760 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1232 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1386 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_018.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      899 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_019.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1562 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_020.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      738 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_200.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1761 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/entity/rule_600.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.640000 vsg-3.8.0/vsg/rules/entity_specification/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      188 2021-12-26 15:41:52.000000 vsg-3.8.0/vsg/rules/entity_specification/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      715 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/entity_specification/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      729 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/entity_specification/rule_101.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      647 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/entity_specification/rule_500.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      635 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/entity_specification/rule_501.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      715 2022-02-12 15:03:40.000000 vsg-3.8.0/vsg/rules/entity_specification/rule_502.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      642 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/entity_specification/rule_503.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      957 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/existence_of_tokens_which_should_not_occur.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.640000 vsg-3.8.0/vsg/rules/exit_statement/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/exit_statement/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      512 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/exit_statement/rule_300.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      859 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/file_length.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.640000 vsg-3.8.0/vsg/rules/file_statement/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       94 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/file_statement/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      942 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/file_statement/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      751 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/file_statement/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      754 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/file_statement/rule_003.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.640000 vsg-3.8.0/vsg/rules/for_loop/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      156 2022-01-28 13:20:44.000000 vsg-3.8.0/vsg/rules/for_loop/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      334 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/for_loop/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      330 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/for_loop/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      331 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/for_loop/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      331 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/for_loop/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      331 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/for_loop/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1404 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/formal_part_in_association_element_between_tokens.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.640000 vsg-3.8.0/vsg/rules/function/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      782 2021-12-26 15:41:52.000000 vsg-3.8.0/vsg/rules/function/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      879 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      848 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      625 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      755 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1566 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1216 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1068 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1232 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      782 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      624 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1454 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      646 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      615 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1614 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1006 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_101.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_201.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_202.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_203.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_204.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      804 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_300.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      816 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_502.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      855 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/function/rule_506.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.640000 vsg-3.8.0/vsg/rules/generate/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      778 2022-02-12 19:26:16.000000 vsg-3.8.0/vsg/rules/generate/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      823 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      895 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      758 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      734 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      766 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      531 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      710 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      916 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      679 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      744 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5021 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      762 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      993 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      996 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1053 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      642 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      936 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      623 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_018.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1682 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_400.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1709 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_401.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1677 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_402.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1704 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_403.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1683 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_404.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1710 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_405.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      880 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generate/rule_600.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.650000 vsg-3.8.0/vsg/rules/generic/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      593 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/rules/generic/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      386 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      575 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      684 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1314 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1169 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/rules/generic/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1127 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1117 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      496 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      536 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      612 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      782 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1117 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      937 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1145 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      597 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_018.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      782 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_019.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      934 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_020.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      616 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_021.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      934 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic/rule_600.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.650000 vsg-3.8.0/vsg/rules/generic_map/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      249 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/generic_map/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      825 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic_map/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1035 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic_map/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      759 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic_map/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      734 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic_map/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      858 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic_map/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      790 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic_map/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      934 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic_map/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      935 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/generic_map/rule_008.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.650000 vsg-3.8.0/vsg/rules/ieee/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/rules/ieee/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1162 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/rules/ieee/rule_500.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.650000 vsg-3.8.0/vsg/rules/if_statement/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1113 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/if_statement/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8401 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      714 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      722 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      735 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      775 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      812 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      788 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      777 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      778 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      824 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      657 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      655 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      656 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      636 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      614 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_020.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      610 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_021.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      776 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_022.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      675 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_023.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      730 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_024.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      535 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_025.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      547 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_026.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      513 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_027.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      549 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_028.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      539 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_029.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      798 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_030.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      988 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_031.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      959 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_032.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      934 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_033.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      569 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_034.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      770 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_035.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      538 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/if_statement/rule_036.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1572 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1791 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment_and_not_on_same_line_as_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1899 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment_when_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2825 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/insert_token_left_of_token_if_it_does_not_exist_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3712 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/insert_token_left_of_token_if_it_does_not_exist_between_tokens_using_value_from_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3652 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/insert_token_right_of_possible_tokens_if_it_does_not_exist_before_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2658 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/insert_token_right_of_token_if_it_does_not_exist_before_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3312 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/insert_tokens_right_of_token_if_it_does_not_exist_before_token.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.650000 vsg-3.8.0/vsg/rules/instantiation/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1119 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/rules/instantiation/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1295 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      969 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      652 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      773 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      788 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      361 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      361 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      623 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      602 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1371 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      361 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      843 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_018.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      899 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_019.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      365 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_020.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      365 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_021.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      360 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_022.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1013 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_023.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      526 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_024.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      360 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_025.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      372 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_026.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      634 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_027.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2644 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_028.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1343 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_029.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      372 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_030.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      664 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_031.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      919 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_032.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1033 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_033.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1685 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_034.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      639 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_035.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      614 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_600.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      660 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/instantiation/rule_601.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      903 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/is_token_value_one_of.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.650000 vsg-3.8.0/vsg/rules/iteration_scheme/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      189 2022-02-05 12:32:32.000000 vsg-3.8.0/vsg/rules/iteration_scheme/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      613 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/iteration_scheme/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      584 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/iteration_scheme/rule_101.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      697 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/iteration_scheme/rule_300.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      708 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/iteration_scheme/rule_301.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/iteration_scheme/rule_500.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      573 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/iteration_scheme/rule_501.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.650000 vsg-3.8.0/vsg/rules/length/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       94 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/length/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      241 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/length/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      239 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/length/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      481 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/length/rule_003.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.660000 vsg-3.8.0/vsg/rules/library/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      374 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/rules/library/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      543 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/library/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      657 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/library/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1326 2022-02-05 21:27:04.000000 vsg-3.8.0/vsg/rules/library/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      588 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/library/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      688 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/library/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      802 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/library/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      753 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/library/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      595 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/library/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      855 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/library/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      656 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/library/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      646 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/library/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      606 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/library/rule_600.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      898 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/line_length.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.660000 vsg-3.8.0/vsg/rules/logical_operator/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2022-02-13 14:52:39.000000 vsg-3.8.0/vsg/rules/logical_operator/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      808 2022-02-13 14:52:39.000000 vsg-3.8.0/vsg/rules/logical_operator/rule_500.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.660000 vsg-3.8.0/vsg/rules/loop_statement/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      748 2022-02-05 12:32:32.000000 vsg-3.8.0/vsg/rules/loop_statement/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      708 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      582 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      628 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      877 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      808 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      786 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      940 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      636 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      642 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_101.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      586 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_102.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      728 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_103.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      691 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_104.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      874 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_200.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_201.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      575 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_202.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      574 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_203.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      620 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_300.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_301.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      661 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_302.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      559 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_500.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      593 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_501.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_502.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      742 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_503.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      676 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/loop_statement/rule_504.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5049 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/rules/move_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2486 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/rules/move_token_left_to_next_non_whitespace_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2010 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/move_token_next_to_another_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2515 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/move_token_next_to_another_token_if_it_exists_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3097 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/move_token_sequences_left_of_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3412 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/move_token_to_the_right_of_several_possible_tokens_if_it_exists_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    16070 2022-02-01 11:57:55.000000 vsg-3.8.0/vsg/rules/multiline_alignment_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2948 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/n_spaces_after_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4584 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/n_spaces_before_and_after_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2055 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/n_spaces_between_token_pairs_when_bounded_by_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1091 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/number_of_lines_between_tokens.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.660000 vsg-3.8.0/vsg/rules/package/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      653 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/package/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      513 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      795 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      557 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      638 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      557 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      736 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      838 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      630 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      671 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      699 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      608 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      845 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      530 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      649 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      694 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      592 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_018.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1448 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_019.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1503 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_400.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1328 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package/rule_401.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.660000 vsg-3.8.0/vsg/rules/package_body/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      720 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/rules/package_body/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      655 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      946 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      994 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      914 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      961 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_101.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      585 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_200.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      679 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_201.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      699 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_202.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      646 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_203.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      522 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_300.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      548 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_301.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1331 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_400.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1398 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_401.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      569 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_500.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      563 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_501.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      647 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_502.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      549 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_503.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      555 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_504.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      605 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_505.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_506.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      654 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_507.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      664 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_600.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      709 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/package_body/rule_601.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.670000 vsg-3.8.0/vsg/rules/port/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      838 2022-02-10 23:52:42.000000 vsg-3.8.0/vsg/rules/port/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      614 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      470 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      647 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1380 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      416 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      354 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      906 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      905 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      914 2022-02-10 14:33:45.000000 vsg-3.8.0/vsg/rules/port/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1302 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1224 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2974 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1062 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      859 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      762 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1004 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      518 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1326 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_018.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1169 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_019.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1226 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_020.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      578 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_021.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      971 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_022.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1526 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_023.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      970 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_024.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1219 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_025.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2853 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_026.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      613 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port/rule_027.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.670000 vsg-3.8.0/vsg/rules/port_map/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      250 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/port_map/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      804 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port_map/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1262 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port_map/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      839 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port_map/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      594 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port_map/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      922 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port_map/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1053 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port_map/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      910 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port_map/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1043 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/port_map/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     7140 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/previous_line.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.670000 vsg-3.8.0/vsg/rules/procedure/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      966 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/procedure/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      921 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      905 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      901 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1629 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1234 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      680 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1231 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      789 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      634 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1454 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1065 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1400 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1043 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_101.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      618 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_200.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      359 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_201.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      359 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_202.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      359 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_203.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      359 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_204.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      359 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_205.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1316 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_401.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1145 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_410.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1198 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_411.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1250 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_412.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      589 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_500.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      635 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_501.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      779 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_502.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      811 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_503.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      785 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_504.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      610 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_505.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      876 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_506.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1203 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure/rule_507.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.670000 vsg-3.8.0/vsg/rules/procedure_call/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      318 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/procedure_call/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      747 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure_call/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      818 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure_call/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1416 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure_call/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      605 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure_call/rule_300.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      558 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure_call/rule_301.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      495 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure_call/rule_302.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      658 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure_call/rule_500.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      602 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/procedure_call/rule_501.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.670000 vsg-3.8.0/vsg/rules/process/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1181 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/process/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      741 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1029 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      693 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      785 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      621 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      754 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      750 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      551 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      591 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      786 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      636 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1332 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      779 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      972 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      981 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      801 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      836 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_017.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1054 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_018.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      618 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_019.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      916 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_020.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5706 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_021.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      864 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_022.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      644 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_023.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      877 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_024.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      911 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_025.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5465 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_026.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5257 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_027.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      962 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_028.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     6524 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_029.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2848 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_030.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1684 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_031.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1117 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_032.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1315 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_033.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1639 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_034.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1405 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_035.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      684 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_036.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1704 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_400.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      684 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/process/rule_600.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/ranges/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       63 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/ranges/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      687 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/ranges/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      663 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/ranges/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1948 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/remove_blank_lines_above_line_starting_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1816 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/remove_carriage_return_after_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1897 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/remove_carriage_returns_between_token_pairs.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2044 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/remove_comments_from_end_of_lines_bounded_by_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2668 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/remove_excessive_blank_lines_above_line_starting_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2568 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/remove_excessive_blank_lines_below_line_ending_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2076 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/remove_lines_starting_with_token_between_token_pairs.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1120 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/remove_spaces_before_token_rule.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1121 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/remove_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1144 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/remove_tokens_bounded_by_tokens_and_remove_trailing_whitespace.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/report_statement/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      253 2021-12-26 15:41:52.000000 vsg-3.8.0/vsg/rules/report_statement/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      723 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/report_statement/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      829 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/report_statement/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      571 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/report_statement/rule_100.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      628 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/report_statement/rule_101.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      638 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/report_statement/rule_300.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4016 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/report_statement/rule_400.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      656 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/report_statement/rule_500.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      660 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/report_statement/rule_501.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3131 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/separate_multiple_signal_identifiers_into_individual_statements.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/sequential/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      218 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/sequential/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      641 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/sequential/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      982 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/sequential/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      759 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/sequential/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1040 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/sequential/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      351 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/sequential/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1113 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/sequential/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      883 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/sequential/rule_007.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/signal/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      467 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/signal/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      647 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      569 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      760 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      612 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      637 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      652 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      718 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      705 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      334 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/rules/signal/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      531 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/rules/signal/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     6099 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1859 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      890 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      767 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      705 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/signal/rule_600.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2034 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/rules/single_space_after_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2646 2022-02-05 12:32:32.000000 vsg-3.8.0/vsg/rules/single_space_before_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1192 2022-02-05 12:32:32.000000 vsg-3.8.0/vsg/rules/single_space_before_token_if_on_same_line_as_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2233 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/single_space_between_token_pairs.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1978 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/single_space_between_token_pairs_bounded_by_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1841 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/single_space_between_tokens.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/source_file/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/source_file/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1106 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/source_file/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     6145 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/rules/spaces_before_and_after_tokens_when_bounded_by_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1453 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/split_line_at_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2621 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/split_line_at_token_if_on_same_line_as_token_if_token_pair_are_not_on_the_same_line.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1742 2022-01-30 20:22:29.000000 vsg-3.8.0/vsg/rules/split_line_at_token_when_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1832 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/split_line_at_token_when_between_tokens_unless_token_is_found.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/subprogram_body/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      188 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/subprogram_body/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1010 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/subprogram_body/rule_201.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1017 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/subprogram_body/rule_202.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      712 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/subprogram_body/rule_203.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      663 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/subprogram_body/rule_204.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      752 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/subprogram_body/rule_205.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1698 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/subprogram_body/rule_400.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/subtype/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      158 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/subtype/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      698 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/subtype/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1387 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/subtype/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      761 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/subtype/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      627 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/subtype/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      627 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/subtype/rule_600.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1453 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_case.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2815 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_case_formal_part_of_association_element_in_map_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      750 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_case_in_range_bounded_by_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      807 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_case_in_range_bounded_by_tokens_with_prefix_suffix.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2094 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_case_n_token_after_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2453 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_case_n_token_after_tokens_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      816 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_case_subtype_indication.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      628 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_case_with_prefix_suffix.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1389 2022-02-05 12:32:32.000000 vsg-3.8.0/vsg/rules/token_does_not_exist_before_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3272 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_indent.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2757 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_indent_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2576 2022-02-12 02:42:55.000000 vsg-3.8.0/vsg/rules/token_indent_unless_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2179 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_prefix.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2305 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_prefix_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1529 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_suffix.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1663 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/token_suffix_between_tokens.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/type_definition/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      561 2021-12-26 15:41:52.000000 vsg-3.8.0/vsg/rules/type_definition/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      691 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      675 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      758 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      834 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      661 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      708 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1328 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1103 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1105 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_009.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      719 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      774 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      901 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      708 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1143 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_014.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      726 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_015.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      701 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_016.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1039 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_400.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      726 2022-02-05 19:34:26.000000 vsg-3.8.0/vsg/rules/type_definition/rule_600.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     6467 2022-02-10 23:52:42.000000 vsg-3.8.0/vsg/rules/utils.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/variable/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      344 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/variable/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      704 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      577 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      762 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      618 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      655 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      656 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      645 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      533 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/rules/variable/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1943 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      653 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable/rule_600.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/variable_assignment/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      187 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/variable_assignment/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      800 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable_assignment/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      860 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable_assignment/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      794 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable_assignment/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      858 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable_assignment/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      360 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable_assignment/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      939 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/variable_assignment/rule_006.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/wait/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/wait/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      678 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/wait/rule_001.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/when/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/when/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3602 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/when/rule_001.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.680000 vsg-3.8.0/vsg/rules/while_loop/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       63 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/while_loop/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      336 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/while_loop/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      332 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/while_loop/rule_002.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.690000 vsg-3.8.0/vsg/rules/whitespace/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      373 2022-02-13 13:33:04.000000 vsg-3.8.0/vsg/rules/whitespace/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2241 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      350 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_002.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      531 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_003.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      545 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_004.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1822 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_005.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      877 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_006.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      572 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_007.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1583 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_008.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_010.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1050 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_011.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2423 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_012.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      729 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/whitespace/rule_013.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1350 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/whitespace_before_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1618 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/rules/whitespace_before_tokens_in_between_tokens.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.690000 vsg-3.8.0/vsg/rules/with_statement/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2021-12-26 15:41:51.000000 vsg-3.8.0/vsg/rules/with_statement/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      789 2022-02-05 19:34:25.000000 vsg-3.8.0/vsg/rules/with_statement/rule_001.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2214 2021-03-06 15:16:58.000000 vsg-3.8.0/vsg/severity.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.690000 vsg-3.8.0/vsg/styles/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/styles/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      164 2020-12-06 16:00:11.000000 vsg-3.8.0/vsg/styles/indent_only.yaml
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2121 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/styles/jcl.yaml
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.730000 vsg-3.8.0/vsg/token/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      217 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/access_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      666 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/adding_operator.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1088 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/alias_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1915 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/architecture_body.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1116 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/assertion.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      545 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/assertion_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      556 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/association_element.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      184 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/association_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      758 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/attribute_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      991 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/attribute_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      207 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/token/binding_indication.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      196 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/block_header.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2270 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/block_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      822 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/case_generate_alternative.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1555 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/case_generate_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1637 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/case_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      609 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/case_statement_alternative.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      201 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/choice.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      167 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/choices.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1255 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/component.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1383 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/component_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      616 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/component_instantiation_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      384 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/token/component_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      817 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/concurrent_assertion_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      839 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/concurrent_conditional_signal_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      815 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/concurrent_procedure_call_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1452 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/concurrent_selected_signal_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      637 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/concurrent_signal_assignment_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      819 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/concurrent_simple_signal_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      209 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/condition_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      404 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/conditional_expressions.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      787 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/conditional_force_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/conditional_variable_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/conditional_waveform_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      750 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/conditional_waveforms.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1744 2021-03-19 12:49:30.000000 vsg-3.8.0/vsg/token/configuration_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1170 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/constant_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      412 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/constrained_array_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1357 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/context_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      734 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/context_reference.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      592 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/delay_mechanism.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      344 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/direction.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      366 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/element_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1394 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/entity.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1566 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/token/entity_aspect.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1527 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/entity_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      210 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/entity_designator.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      552 2022-01-20 15:37:21.000000 vsg-3.8.0/vsg/token/entity_name_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      375 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/entity_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      832 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/enumeration_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1065 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/exit_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2025 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/file_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      820 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/file_open_information.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      394 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/file_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1545 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/for_generate_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      372 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/force_mode.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      767 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/full_type_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1610 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/function_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      783 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/generate_statement_body.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      793 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/generic_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      814 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/generic_map_aspect.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      384 2021-03-19 13:20:19.000000 vsg-3.8.0/vsg/token/group_constituent_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1344 2021-03-19 13:35:22.000000 vsg-3.8.0/vsg/token/group_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      370 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/identifier.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      367 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/identifier_list.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.730000 vsg-3.8.0/vsg/token/ieee/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/ieee/__init__.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.730000 vsg-3.8.0/vsg/token/ieee/std_logic_1164/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/ieee/std_logic_1164/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      416 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/ieee/std_logic_1164/function.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1480 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/token/ieee/std_logic_1164/types.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2503 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/if_generate_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1778 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/if_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      601 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/incomplete_type_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      596 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/index_constraint.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      425 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/index_subtype_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1783 2022-01-20 15:39:34.000000 vsg-3.8.0/vsg/token/instantiated_unit.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      747 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/token/instantiation_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1031 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_constant_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      808 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_file_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1702 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_function_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      228 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_incomplete_type_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      383 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      832 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_package_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1316 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_package_generic_map_aspect.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1097 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_procedure_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1978 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_signal_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      220 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_subprogram_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      431 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_subprogram_default.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1016 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_unknown_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1031 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/interface_variable_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      390 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/iteration_scheme.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      369 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/library_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      379 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/logical_name_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1339 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/logical_operator.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1270 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/loop_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      848 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/miscellaneous_operator.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      940 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/mode.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      993 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/multiplying_operator.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1065 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/next_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      711 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/null_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1698 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/package_body.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1553 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/package_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      194 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/package_header.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1037 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/package_instantiation_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      402 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/parameter_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      807 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/token/physical_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      775 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/port_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      798 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/port_map_aspect.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      180 2021-01-09 19:00:33.000000 vsg-3.8.0/vsg/token/pragma.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      388 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/token/primary_unit_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      611 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/procedure_call.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      560 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/procedure_call_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1042 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/procedure_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      213 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/process_sensitivity_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2491 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/process_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1210 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/protected_type_body.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      858 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/protected_type_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      209 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/range_constraint.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      824 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/record_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2717 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/relational_operator.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      914 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/report_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      723 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/return_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      757 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/token/secondary_unit_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      384 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/selected_expressions.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1364 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/selected_force_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1188 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/selected_variable_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1188 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/selected_waveform_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      380 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/selected_waveforms.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      205 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/sensitivity_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      184 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/sensitivity_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1734 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/shared_variable_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1187 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/shift_operator.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      451 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/sign.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      392 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/signal_assignment_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1687 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/signal_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      386 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/signal_kind.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      733 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/signature.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      823 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/token/simple_configuration_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      767 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/simple_force_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      779 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/simple_release_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      584 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/simple_variable_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      584 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/simple_waveform_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      924 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/subprogram_body.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      206 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/subprogram_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      628 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/subprogram_header.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1057 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/subprogram_instantiation_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      405 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/subprogram_kind.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      765 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/subtype_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      203 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/timeout_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      722 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/type_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      177 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/type_mark.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1465 2021-04-07 19:53:22.000000 vsg-3.8.0/vsg/token/unary_logical_operator.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1010 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/unbounded_array_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      706 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/use_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      396 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/variable_assignment_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1891 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/variable_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      191 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/vhdl_range.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      711 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/wait_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      363 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/waveform.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      392 2020-12-18 15:01:20.000000 vsg-3.8.0/vsg/token/waveform_element.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     7189 2022-02-13 03:57:59.000000 vsg-3.8.0/vsg/token_map.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     7328 2022-02-06 14:42:23.000000 vsg-3.8.0/vsg/tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1942 2022-02-05 12:32:32.000000 vsg-3.8.0/vsg/utils.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1511 2022-02-13 14:54:16.000000 vsg-3.8.0/vsg/version.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       39 2022-02-13 15:07:18.000000 vsg-3.8.0/vsg/version_info.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.730000 vsg-3.8.0/vsg/vhdlFile/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       31 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/__init__.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.800000 vsg-3.8.0/vsg/vhdlFile/classify/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      603 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/access_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      227 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/actual_parameter_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1256 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/alias_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2007 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/architecture_body.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      288 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/architecture_declarative_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      316 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/architecture_statement_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      534 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/array_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1107 2022-01-21 13:26:52.000000 vsg-3.8.0/vsg/vhdlFile/classify/assertion.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      641 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/assertion_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1756 2021-03-24 22:10:00.000000 vsg-3.8.0/vsg/vhdlFile/classify/association_element.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      559 2021-03-24 22:10:06.000000 vsg-3.8.0/vsg/vhdlFile/classify/association_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      867 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/attribute_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1153 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/attribute_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      785 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/binding_indication.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      123 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/blank.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3763 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/block_declarative_item.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      281 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/block_declarative_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      994 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/block_header.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2029 2022-01-21 13:27:00.000000 vsg-3.8.0/vsg/vhdlFile/classify/block_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      273 2021-02-13 15:21:05.000000 vsg-3.8.0/vsg/vhdlFile/classify/block_statement_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      849 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/case_generate_alternative.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1813 2021-03-13 13:52:43.000000 vsg-3.8.0/vsg/vhdlFile/classify/case_generate_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1610 2021-01-06 14:50:59.000000 vsg-3.8.0/vsg/vhdlFile/classify/case_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      823 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/case_statement_alternative.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      765 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/choice.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      539 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/choices.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      196 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/comment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1665 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/component_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1324 2022-01-20 12:14:56.000000 vsg-3.8.0/vsg/vhdlFile/classify/component_instantiation_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      542 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/component_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      506 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/composite_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      910 2022-01-21 13:27:24.000000 vsg-3.8.0/vsg/vhdlFile/classify/concurrent_assertion_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2070 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/concurrent_conditional_signal_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      725 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/concurrent_procedure_call_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1617 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/concurrent_selected_signal_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1714 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/concurrent_signal_assignment_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1285 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/concurrent_simple_signal_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1640 2022-01-21 13:27:29.000000 vsg-3.8.0/vsg/vhdlFile/classify/concurrent_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      212 2022-01-02 20:24:13.000000 vsg-3.8.0/vsg/vhdlFile/classify/condition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      553 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/condition_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1285 2021-01-06 14:56:06.000000 vsg-3.8.0/vsg/vhdlFile/classify/conditional_expressions.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1193 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/conditional_force_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      895 2021-12-04 13:56:28.000000 vsg-3.8.0/vsg/vhdlFile/classify/conditional_signal_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1031 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/conditional_variable_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1106 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/conditional_waveform_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1267 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/conditional_waveforms.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2000 2021-03-19 12:56:46.000000 vsg-3.8.0/vsg/vhdlFile/classify/configuration_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      659 2021-03-19 13:33:03.000000 vsg-3.8.0/vsg/vhdlFile/classify/configuration_declarative_item.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      384 2021-03-19 12:56:15.000000 vsg-3.8.0/vsg/vhdlFile/classify/configuration_declarative_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      384 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/configuration_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1275 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/constant_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      975 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/constrained_array_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      266 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/context_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1329 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/context_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      623 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/context_item.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      954 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/context_reference.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1036 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/delay_mechanism.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      401 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/design_file.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      431 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/design_unit.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1065 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/discrete_range.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      685 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/element_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      254 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/element_subtype_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1364 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/entity_aspect.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1973 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/entity_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3572 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/entity_declarative_item.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      285 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/entity_declarative_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      386 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/entity_designator.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      364 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/entity_header.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      900 2020-12-18 19:12:03.000000 vsg-3.8.0/vsg/vhdlFile/classify/entity_name_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      504 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/entity_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      798 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/entity_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      262 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/entity_statement_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      829 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/enumeration_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1160 2022-01-02 20:24:04.000000 vsg-3.8.0/vsg/vhdlFile/classify/exit_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2605 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/vhdlFile/classify/expression.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1087 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/file_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      230 2021-03-12 02:10:05.000000 vsg-3.8.0/vsg/vhdlFile/classify/file_logical_name.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      900 2021-01-09 01:19:19.000000 vsg-3.8.0/vsg/vhdlFile/classify/file_open_information.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      644 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/file_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1767 2021-01-06 14:56:26.000000 vsg-3.8.0/vsg/vhdlFile/classify/for_generate_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      353 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/force_mode.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      219 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/formal_parameter_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      915 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/full_type_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1747 2021-12-04 13:56:28.000000 vsg-3.8.0/vsg/vhdlFile/classify/function_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      706 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/generate_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1513 2020-12-19 16:06:52.000000 vsg-3.8.0/vsg/vhdlFile/classify/generate_statement_body.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      871 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/generic_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      208 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/generic_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      862 2022-01-21 01:09:08.000000 vsg-3.8.0/vsg/vhdlFile/classify/generic_map_aspect.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      552 2021-03-19 13:42:17.000000 vsg-3.8.0/vsg/vhdlFile/classify/group_constituent_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1159 2021-03-19 13:35:58.000000 vsg-3.8.0/vsg/vhdlFile/classify/group_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      276 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/identifier.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      598 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/identifier_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2742 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/if_generate_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2152 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/if_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      704 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/incomplete_type_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      690 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/index_constraint.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      518 2021-03-12 02:10:05.000000 vsg-3.8.0/vsg/vhdlFile/classify/index_subtype_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2068 2022-01-21 01:20:04.000000 vsg-3.8.0/vsg/vhdlFile/classify/instantiated_unit.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      889 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/instantiation_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      211 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/integer_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1305 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_constant_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      991 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      222 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_element.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      880 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_file_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1720 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_function_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      579 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_incomplete_type_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      554 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1326 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_object_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1100 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_package_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1317 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_package_generic_map_aspect.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1113 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_procedure_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1402 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_signal_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      975 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_subprogram_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      436 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_subprogram_default.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      592 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_subprogram_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      277 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_type_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1597 2021-03-13 14:15:53.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_unknown_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1296 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/interface_variable_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1245 2021-01-11 14:53:18.000000 vsg-3.8.0/vsg/vhdlFile/classify/iteration_scheme.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      697 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/library_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      441 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/library_unit.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      593 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/logical_name_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1623 2021-01-08 23:25:47.000000 vsg-3.8.0/vsg/vhdlFile/classify/loop_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      649 2022-02-10 23:52:42.000000 vsg-3.8.0/vsg/vhdlFile/classify/mode.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1117 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/vhdlFile/classify/name.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1245 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/next_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      742 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/null_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1855 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/package_body.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3199 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/package_body_declarative_item.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      380 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/package_body_declarative_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1900 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/package_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3208 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/package_declarative_item.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      360 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/package_declarative_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      587 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/package_header.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1187 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/package_instantiation_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      536 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/parameter_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1503 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/physical_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      845 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/port_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      202 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/port_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      894 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/port_map_aspect.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      496 2021-01-09 19:31:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/pragma.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      382 2020-12-21 21:26:06.000000 vsg-3.8.0/vsg/vhdlFile/classify/preprocessor.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1161 2021-03-19 12:47:20.000000 vsg-3.8.0/vsg/vhdlFile/classify/primary_unit.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      510 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/primary_unit_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1478 2022-01-02 21:59:03.000000 vsg-3.8.0/vsg/vhdlFile/classify/procedure_call.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1538 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/procedure_call_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1313 2021-01-04 23:49:22.000000 vsg-3.8.0/vsg/vhdlFile/classify/procedure_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3025 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/process_declarative_item.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      361 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/process_declarative_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      470 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/process_sensitivity_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2564 2022-01-21 14:00:04.000000 vsg-3.8.0/vsg/vhdlFile/classify/process_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      346 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/process_statement_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1260 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/protected_type_body.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3036 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/protected_type_body_declarative_item.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      337 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/protected_type_body_declarative_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1120 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/protected_type_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1027 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/protected_type_declarative_item.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      315 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/protected_type_declarative_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      505 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/protected_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      686 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/range_constraint.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1022 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/record_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1064 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/report_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1001 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/return_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      904 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/scalar_type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      457 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/secondary_unit.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      771 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/secondary_unit_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1068 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/selected_expressions.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1626 2021-01-06 14:53:15.000000 vsg-3.8.0/vsg/vhdlFile/classify/selected_force_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      811 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/selected_signal_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1400 2021-01-06 14:59:24.000000 vsg-3.8.0/vsg/vhdlFile/classify/selected_variable_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1527 2021-01-06 14:52:38.000000 vsg-3.8.0/vsg/vhdlFile/classify/selected_waveform_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2084 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/selected_waveforms.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      566 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/sensitivity_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1451 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/sensitivity_list.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      346 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/sequence_of_statements.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3197 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/sequential_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1237 2021-12-04 13:56:28.000000 vsg-3.8.0/vsg/vhdlFile/classify/signal_assignment_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1368 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/signal_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      623 2022-02-06 14:42:23.000000 vsg-3.8.0/vsg/vhdlFile/classify/signal_kind.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1490 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/signature.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1251 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/simple_configuration_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1142 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/simple_force_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      858 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/simple_release_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1128 2022-01-06 14:38:32.000000 vsg-3.8.0/vsg/vhdlFile/classify/simple_signal_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1016 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/simple_variable_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1461 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/classify/simple_waveform_assignment.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1391 2021-12-04 13:56:28.000000 vsg-3.8.0/vsg/vhdlFile/classify/subprogram_body.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      525 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/subprogram_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3030 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/subprogram_declarative_item.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      372 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/subprogram_declarative_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      991 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/subprogram_header.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1444 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/subprogram_instantiation_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      606 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/subprogram_kind.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      516 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/subprogram_specification.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      349 2021-12-04 13:56:28.000000 vsg-3.8.0/vsg/vhdlFile/classify/subprogram_statement_part.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      920 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/subtype_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1612 2022-02-10 02:28:44.000000 vsg-3.8.0/vsg/vhdlFile/classify/subtype_indication.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      552 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/timeout_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      506 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/type_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1104 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/type_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      251 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/type_mark.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1450 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/unbounded_array_definition.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      838 2021-10-03 15:24:26.000000 vsg-3.8.0/vsg/vhdlFile/classify/use_clause.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1263 2021-12-04 13:56:28.000000 vsg-3.8.0/vsg/vhdlFile/classify/variable_assignment_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1452 2021-01-06 14:52:06.000000 vsg-3.8.0/vsg/vhdlFile/classify/variable_declaration.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1253 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/wait_statement.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      948 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/waveform.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      867 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/classify/waveform_element.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      742 2021-10-31 12:21:34.000000 vsg-3.8.0/vsg/vhdlFile/classify/whitespace.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1835 2021-01-12 00:26:21.000000 vsg-3.8.0/vsg/vhdlFile/code_tags.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.810000 vsg-3.8.0/vsg/vhdlFile/extract/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4866 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/vhdlFile/extract/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      116 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_all_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1404 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_association_elements_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_blank_lines_above_line_starting_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      431 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_blank_lines_above_line_starting_with_token_when_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1092 2021-02-22 23:22:47.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_blank_lines_below_line_ending_with_several_possible_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1530 2021-02-22 23:22:47.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_blank_lines_below_line_ending_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      423 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_column_of_token_index.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1775 2022-02-13 04:02:24.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_consecutive_lines_starting_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1496 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_consecutive_lines_starting_with_token_and_stopping_when_token_starting_line_is_found.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      984 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_if_statement_conditions.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1794 2021-03-13 13:39:55.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_interface_elements_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      690 2021-01-13 02:11:45.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_line_above_line_starting_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      786 2021-01-13 23:21:55.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_line_above_line_starting_with_token_with_hierarchy.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      735 2021-02-22 23:22:47.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_several_possible_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      696 2021-01-30 01:28:59.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      740 2021-01-30 01:28:15.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_token_with_hierarchy.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      710 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_line_count_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2262 2021-03-12 02:10:05.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_line_preceeding_line.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      460 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_line_succeeding_line.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      767 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_line_which_includes_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      720 2021-03-13 14:16:38.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_lines_with_length_that_exceed_column.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      936 2021-12-18 14:17:44.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_m_tokens_before_and_n_tokens_after_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      688 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_n_token_after_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      886 2021-03-13 13:40:45.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_n_token_after_tokens_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      486 2021-03-12 02:10:05.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_n_tokens_before_and_after_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      540 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_n_tokens_before_and_after_tokens_bounded_by_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      716 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_sequence_of_tokens_matching.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      792 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_sequence_of_tokens_matching_bounded_by_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      528 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_sequence_of_tokens_not_matching.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      464 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_token_and_n_tokens_after_it.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      515 2022-02-08 13:13:08.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_token_and_n_tokens_after_it_when_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      496 2020-12-18 16:52:06.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_token_and_n_tokens_before_it.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      550 2021-03-31 12:37:49.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_token_and_n_tokens_before_it_in_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      619 2021-12-18 14:17:44.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_token_and_n_tokens_before_it_in_between_tokens_unless_token_is_found.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      831 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1051 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1439 2021-12-18 14:17:44.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching_unless_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      936 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_between_non_whitespace_token_and_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1055 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_between_tokens_inclusive_while_storing_value_from_token.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3447 2021-10-31 12:21:34.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_bounded_by.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1045 2020-12-22 15:09:26.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_bounded_by_token_when_between_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      709 2021-03-12 02:10:05.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_bounded_by_tokens_if_token_is_between_them.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1623 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_bounded_by_unless_between.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      381 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_from_line.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      426 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_matching.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      658 2020-12-18 15:01:21.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_matching_in_range_bounded_by_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3792 2021-03-13 13:43:39.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_starting_with_token_and_ending_with_one_of_possible_tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)      702 2022-01-26 13:54:48.000000 vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_where_line_starts_with_token_until_ending_token_is_found.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1456 2022-02-12 14:46:58.000000 vsg-3.8.0/vsg/vhdlFile/extract/tokens.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5099 2022-02-13 04:04:46.000000 vsg-3.8.0/vsg/vhdlFile/extract/utils.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.810000 vsg-3.8.0/vsg/vhdlFile/indent/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-21 00:10:23.000000 vsg-3.8.0/vsg/vhdlFile/indent/__init__.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    13941 2022-02-05 12:05:24.000000 vsg-3.8.0/vsg/vhdlFile/indent/indent_config.yaml
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4716 2022-02-12 14:46:58.000000 vsg-3.8.0/vsg/vhdlFile/indent/set_token_indent.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    23595 2022-02-12 16:04:12.000000 vsg-3.8.0/vsg/vhdlFile/utils.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    27809 2022-02-12 02:32:32.000000 vsg-3.8.0/vsg/vhdlFile/vhdlFile.py
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1343 2021-10-31 12:21:34.000000 vsg-3.8.0/vsg/violation.py
-drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-13 15:07:36.580000 vsg-3.8.0/vsg.egg-info/
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9674 2022-02-13 15:07:36.000000 vsg-3.8.0/vsg.egg-info/PKG-INFO
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)    49182 2022-02-13 15:07:36.000000 vsg-3.8.0/vsg.egg-info/SOURCES.txt
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        1 2022-02-13 15:07:36.000000 vsg-3.8.0/vsg.egg-info/dependency_links.txt
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       43 2022-02-13 15:07:36.000000 vsg-3.8.0/vsg.egg-info/entry_points.txt
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        1 2020-06-21 15:29:54.000000 vsg-3.8.0/vsg.egg-info/not-zip-safe
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)       12 2022-02-13 15:07:36.000000 vsg-3.8.0/vsg.egg-info/requires.txt
--rw-r--r--   0 jcleary   (1000) jcleary   (1000)        4 2022-02-13 15:07:36.000000 vsg-3.8.0/vsg.egg-info/top_level.txt
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.400000 vsg-3.9.0/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       96 2021-03-06 15:16:58.000000 vsg-3.9.0/MANIFEST.in
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9674 2022-02-20 15:31:39.400000 vsg-3.9.0/PKG-INFO
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     7116 2022-02-05 12:05:24.000000 vsg-3.9.0/README.rst
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      147 2022-02-20 15:31:39.400000 vsg-3.9.0/setup.cfg
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2195 2021-03-20 15:05:16.000000 vsg-3.9.0/setup.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:38.990000 vsg-3.9.0/vsg/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      497 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/CustomArgumentParser.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     6025 2022-01-31 12:23:48.000000 vsg-3.9.0/vsg/__main__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1186 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/__parser__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4973 2022-02-05 19:36:49.000000 vsg-3.9.0/vsg/__rule_doc_gen__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4127 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/apply_rules.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5349 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/block_rule.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4873 2022-01-31 12:42:04.000000 vsg-3.9.0/vsg/cmd_line_args.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     7623 2021-10-31 12:21:33.000000 vsg-3.9.0/vsg/config.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      539 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/deprecated_rule.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      227 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/exceptions.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4285 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/junit.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9340 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/parser.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      627 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/proposed_rule.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:38.990000 vsg-3.9.0/vsg/report/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       85 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/report/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      876 2021-03-06 15:16:58.000000 vsg-3.9.0/vsg/report/summary_stdout.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      862 2021-03-06 15:16:58.000000 vsg-3.9.0/vsg/report/syntastic_stdout.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3140 2021-03-06 15:16:58.000000 vsg-3.9.0/vsg/report/vsg_stdout.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8438 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rule.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.000000 vsg-3.9.0/vsg/rule_group/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rule_group/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      458 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rule_group/alignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      460 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rule_group/blank_line.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      448 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rule_group/case.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      452 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rule_group/indent.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      602 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rule_group/length.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      452 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rule_group/naming.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      458 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rule_group/structure.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      456 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rule_group/whitespace.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    12965 2022-02-05 12:32:32.000000 vsg-3.9.0/vsg/rule_list.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.020000 vsg-3.9.0/vsg/rules/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    10047 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/__init__.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.030000 vsg-3.9.0/vsg/rules/after/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       94 2021-12-26 15:41:52.000000 vsg-3.9.0/vsg/rules/after/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5843 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/after/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9681 2022-02-05 19:38:07.000000 vsg-3.9.0/vsg/rules/after/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5934 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/after/rule_003.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.030000 vsg-3.9.0/vsg/rules/alias_declaration/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      345 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/rules/alias_declaration/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      628 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/alias_declaration/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      710 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/alias_declaration/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      733 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/alias_declaration/rule_101.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      507 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/alias_declaration/rule_102.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      517 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/alias_declaration/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      589 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/alias_declaration/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      583 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/alias_declaration/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      645 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/alias_declaration/rule_502.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2050 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/alias_declaration/rule_503.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      689 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/alias_declaration/rule_600.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      689 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/alias_declaration/rule_601.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3036 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/align_consecutive_lines_after_line_starting_with_token_and_stopping_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4528 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/align_consecutive_lines_starting_with_a_comment_above_line_starting_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2610 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/align_left_token_with_right_token_if_right_token_starts_a_line.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8616 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/align_tokens_in_region_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9818 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/align_tokens_in_region_between_tokens_skipping_lines_starting_with_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    13077 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/align_tokens_in_region_between_tokens_unless_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    10748 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/align_tokens_in_region_between_tokens_when_between_tokens_unless_between_tokens.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.040000 vsg-3.9.0/vsg/rules/architecture/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1087 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/architecture/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      507 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      657 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      627 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      585 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      678 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      728 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      487 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      545 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      577 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      846 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      694 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      676 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      664 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      659 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      681 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      685 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      584 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      646 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_018.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      578 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_019.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      578 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_020.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      578 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_021.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      694 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_022.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1010 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_024.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1139 2022-02-10 23:52:45.000000 vsg-3.9.0/vsg/rules/architecture/rule_025.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1472 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_026.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1293 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_027.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      627 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_028.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1580 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_029.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_030.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      633 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_031.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      642 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_032.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      650 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_033.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      636 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_200.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1878 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_600.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9489 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/architecture/rule_601.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.040000 vsg-3.9.0/vsg/rules/assert_statement/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      188 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/assert_statement/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      812 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/assert_statement/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1176 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/assert_statement/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1298 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/assert_statement/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1182 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/assert_statement/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1260 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/assert_statement/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4252 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/assert_statement/rule_400.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.040000 vsg-3.9.0/vsg/rules/attribute/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       62 2021-12-26 15:41:52.000000 vsg-3.9.0/vsg/rules/attribute/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      558 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/attribute/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      558 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/attribute/rule_002.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.050000 vsg-3.9.0/vsg/rules/attribute_declaration/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      189 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/attribute_declaration/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      634 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_declaration/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      527 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_declaration/rule_101.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      570 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_declaration/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      597 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_declaration/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      635 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_declaration/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      764 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_declaration/rule_502.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.050000 vsg-3.9.0/vsg/rules/attribute_specification/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      220 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/attribute_specification/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1047 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_specification/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      674 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_specification/rule_101.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      636 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_specification/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      663 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_specification/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      721 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_specification/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      649 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_specification/rule_502.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      649 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/attribute_specification/rule_503.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3246 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/blank_line_above_line_starting_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1054 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/blank_line_above_line_starting_with_token_when_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3256 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/blank_line_below_line_ending_with_several_possible_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3449 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/blank_line_below_line_ending_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1570 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/blank_lines_between_token_pairs.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.060000 vsg-3.9.0/vsg/rules/block/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      906 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/block/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1171 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1040 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      999 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      563 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      703 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      997 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1305 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      700 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_101.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      553 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_200.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      927 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_201.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      867 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_202.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      590 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_203.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      665 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_204.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      608 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_205.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      490 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      493 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_301.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      551 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_302.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1379 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_400.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1404 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_401.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      598 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      557 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      551 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_502.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      583 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_503.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      553 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_504.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      582 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_505.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      631 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_506.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      633 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_600.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      671 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/block/rule_601.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.060000 vsg-3.9.0/vsg/rules/block_comment/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       94 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/block_comment/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3956 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/block_comment/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1907 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/block_comment/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2078 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/block_comment/rule_003.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.070000 vsg-3.9.0/vsg/rules/case/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      715 2022-02-09 14:33:33.000000 vsg-3.9.0/vsg/rules/case/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      728 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      585 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      587 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      650 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      630 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      688 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      349 2022-02-09 14:33:33.000000 vsg-3.9.0/vsg/rules/case/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      630 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      569 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      821 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      719 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      597 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      647 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      643 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      611 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      631 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      637 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_018.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      859 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_019.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      649 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_020.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      919 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_021.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      611 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/case/rule_200.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      754 2022-02-09 14:33:33.000000 vsg-3.9.0/vsg/rules/case/rule_201.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.070000 vsg-3.9.0/vsg/rules/case_generate_alternative/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/case_generate_alternative/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/case_generate_alternative/rule_500.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.070000 vsg-3.9.0/vsg/rules/case_generate_statement/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       63 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/case_generate_statement/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      579 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/case_generate_statement/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      587 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/case_generate_statement/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9591 2022-02-20 13:54:12.000000 vsg-3.9.0/vsg/rules/case_utils.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.070000 vsg-3.9.0/vsg/rules/comment/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      127 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/comment/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      632 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/comment/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1098 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/comment/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2556 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/comment/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3251 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/comment/rule_100.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.080000 vsg-3.9.0/vsg/rules/component/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      652 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/component/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      633 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      602 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      642 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      617 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      683 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      603 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      589 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      634 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      557 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      605 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      653 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      654 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      603 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      352 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      693 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1423 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      635 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_018.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1014 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_019.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1762 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_020.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      826 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/component/rule_021.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.080000 vsg-3.9.0/vsg/rules/concurrent/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      342 2021-12-26 15:41:52.000000 vsg-3.9.0/vsg/rules/concurrent/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      907 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/concurrent/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      704 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/concurrent/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1314 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/concurrent/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      946 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/concurrent/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      820 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/concurrent/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      953 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/concurrent/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3667 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/concurrent/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8172 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/concurrent/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    24195 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/concurrent/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1192 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/concurrent/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4092 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/concurrent/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3101 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/consistent_case_of_tokens_from_between_tokens_applied_to_region.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2623 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/consistent_token_case.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.090000 vsg-3.9.0/vsg/rules/constant/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      501 2022-02-07 23:25:33.000000 vsg-3.9.0/vsg/rules/constant/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      645 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      585 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      520 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      632 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      595 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      669 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1579 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      772 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      533 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/rules/constant/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    12445 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2231 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1295 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      610 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    22223 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      674 2022-02-07 23:25:33.000000 vsg-3.9.0/vsg/rules/constant/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      610 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/constant/rule_600.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.100000 vsg-3.9.0/vsg/rules/context/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      868 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/context/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      505 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      612 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      700 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      549 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      655 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      632 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      713 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      711 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      807 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1023 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1124 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      624 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      566 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      578 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      641 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      616 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      659 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_018.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      699 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_019.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      496 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_020.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      810 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_021.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      872 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_022.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      585 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_023.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      689 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_024.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      583 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_025.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      333 2022-02-20 15:06:44.000000 vsg-3.9.0/vsg/rules/context/rule_026.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      333 2022-02-20 15:06:44.000000 vsg-3.9.0/vsg/rules/context/rule_027.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      874 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/context/rule_028.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.100000 vsg-3.9.0/vsg/rules/context_ref/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      279 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/context_ref/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      489 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/context_ref/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      611 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/context_ref/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      539 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/context_ref/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      684 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/context_ref/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      729 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/context_ref/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      508 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/context_ref/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      575 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/context_ref/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      472 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/context_ref/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      587 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/context_ref/rule_009.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.100000 vsg-3.9.0/vsg/rules/element_association/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       63 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/element_association/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      711 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/element_association/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      528 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/element_association/rule_101.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.110000 vsg-3.9.0/vsg/rules/entity/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1121 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      499 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      532 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      547 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      667 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      588 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      616 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      613 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      545 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      608 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      630 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      668 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      596 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      755 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      760 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1232 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1386 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_018.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      899 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_019.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1562 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_020.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      606 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_021.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      626 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_022.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      628 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_023.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      610 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_024.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      559 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_025.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      606 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_026.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      607 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_027.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_028.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      730 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_029.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      738 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_200.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      506 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_201.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      723 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_202.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      501 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_203.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      476 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      613 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1761 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/entity/rule_600.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.110000 vsg-3.9.0/vsg/rules/entity_specification/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      188 2021-12-26 15:41:52.000000 vsg-3.9.0/vsg/rules/entity_specification/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      715 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/entity_specification/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      729 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/entity_specification/rule_101.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      647 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/entity_specification/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      635 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/entity_specification/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      371 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/entity_specification/rule_502.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      642 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/entity_specification/rule_503.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      957 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/existence_of_tokens_which_should_not_occur.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.110000 vsg-3.9.0/vsg/rules/exit_statement/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/exit_statement/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      512 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/exit_statement/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      859 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/file_length.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.110000 vsg-3.9.0/vsg/rules/file_statement/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       94 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/file_statement/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      942 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/file_statement/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      751 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/file_statement/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      754 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/file_statement/rule_003.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.110000 vsg-3.9.0/vsg/rules/for_generate_statement/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       63 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/for_generate_statement/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/for_generate_statement/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      609 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/for_generate_statement/rule_501.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.120000 vsg-3.9.0/vsg/rules/for_loop/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      156 2022-01-28 13:20:44.000000 vsg-3.9.0/vsg/rules/for_loop/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      334 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/for_loop/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      330 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/for_loop/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      331 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/for_loop/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      331 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/for_loop/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      331 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/for_loop/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1404 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/formal_part_in_association_element_between_tokens.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.130000 vsg-3.9.0/vsg/rules/function/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      782 2021-12-26 15:41:52.000000 vsg-3.9.0/vsg/rules/function/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      879 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      848 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      625 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      755 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1566 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1216 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1068 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1232 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      782 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      624 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1454 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      646 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      615 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1614 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1006 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_101.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_201.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_202.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_203.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      358 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_204.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      804 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      816 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_502.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      855 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/function/rule_506.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.130000 vsg-3.9.0/vsg/rules/generate/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      841 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/generate/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      823 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      895 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      758 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      734 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      766 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      531 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      710 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      916 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      679 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      744 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5021 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      762 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      993 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      996 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1053 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      642 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      936 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      623 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_018.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1682 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_400.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1709 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_401.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1677 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_402.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1704 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_403.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1683 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_404.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1710 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_405.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      602 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/generate/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      666 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/generate/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      880 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generate/rule_600.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.140000 vsg-3.9.0/vsg/rules/generic/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      593 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/rules/generic/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      386 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      575 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      684 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1314 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1169 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/rules/generic/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1127 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1117 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      496 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      536 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      612 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      782 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1117 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      937 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1145 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      597 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_018.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      782 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_019.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      934 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_020.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      616 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_021.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      934 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic/rule_600.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.140000 vsg-3.9.0/vsg/rules/generic_map/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      249 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/generic_map/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      825 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic_map/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1035 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic_map/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      759 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic_map/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      734 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic_map/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      858 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic_map/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      790 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic_map/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      934 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic_map/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      935 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/generic_map/rule_008.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.140000 vsg-3.9.0/vsg/rules/ieee/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/rules/ieee/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1162 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/rules/ieee/rule_500.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.150000 vsg-3.9.0/vsg/rules/if_generate_statement/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      125 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/if_generate_statement/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/if_generate_statement/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      683 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/if_generate_statement/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      577 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/if_generate_statement/rule_502.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      553 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/if_generate_statement/rule_503.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.150000 vsg-3.9.0/vsg/rules/if_statement/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1113 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/if_statement/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     8401 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      714 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      722 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      687 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/if_statement/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      775 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      812 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      788 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      777 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      778 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      824 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      657 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      655 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      656 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      636 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      614 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_020.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      610 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_021.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      776 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_022.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      675 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_023.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      730 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_024.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      535 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_025.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      547 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_026.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      513 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_027.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      549 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_028.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      539 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_029.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      798 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_030.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      988 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_031.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      959 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_032.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      934 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_033.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      569 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_034.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      770 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_035.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      538 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/if_statement/rule_036.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1572 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1791 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment_and_not_on_same_line_as_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1899 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment_when_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2825 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/insert_token_left_of_token_if_it_does_not_exist_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3712 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/insert_token_left_of_token_if_it_does_not_exist_between_tokens_using_value_from_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3652 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/insert_token_right_of_possible_tokens_if_it_does_not_exist_before_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2658 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/insert_token_right_of_token_if_it_does_not_exist_before_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3312 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/insert_tokens_right_of_token_if_it_does_not_exist_before_token.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.170000 vsg-3.9.0/vsg/rules/instantiation/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1119 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/rules/instantiation/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1295 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      969 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      652 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      773 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      788 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      361 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      361 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      623 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      602 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1371 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      361 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      843 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_018.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      899 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_019.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      365 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_020.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      365 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_021.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      360 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_022.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1013 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_023.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      526 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_024.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      360 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_025.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      372 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_026.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      634 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_027.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2644 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_028.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1343 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_029.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      372 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_030.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      664 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_031.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      919 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_032.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1033 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_033.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1685 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_034.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      639 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_035.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      614 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_600.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      660 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/instantiation/rule_601.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      903 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/is_token_value_one_of.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.170000 vsg-3.9.0/vsg/rules/iteration_scheme/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      189 2022-02-05 12:32:32.000000 vsg-3.9.0/vsg/rules/iteration_scheme/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      613 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/iteration_scheme/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      584 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/iteration_scheme/rule_101.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      697 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/iteration_scheme/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      708 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/iteration_scheme/rule_301.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/iteration_scheme/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      573 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/iteration_scheme/rule_501.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.170000 vsg-3.9.0/vsg/rules/length/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       94 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/length/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      241 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/length/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      239 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/length/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      481 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/length/rule_003.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.170000 vsg-3.9.0/vsg/rules/library/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      374 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/rules/library/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      543 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/library/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      657 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/library/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1326 2022-02-05 21:27:04.000000 vsg-3.9.0/vsg/rules/library/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      588 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/library/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      688 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/library/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      802 2022-02-20 13:54:12.000000 vsg-3.9.0/vsg/rules/library/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      753 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/library/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      595 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/library/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      855 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/library/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      656 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/library/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      646 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/library/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      606 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/library/rule_600.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      898 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/line_length.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.180000 vsg-3.9.0/vsg/rules/logical_operator/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/logical_operator/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      808 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/logical_operator/rule_500.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.180000 vsg-3.9.0/vsg/rules/loop_statement/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      748 2022-02-05 12:32:32.000000 vsg-3.9.0/vsg/rules/loop_statement/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      708 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      582 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      628 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      877 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      808 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      786 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      940 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      636 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      642 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_101.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      586 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_102.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      728 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_103.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      691 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_104.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      874 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_200.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      565 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_201.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      575 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_202.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      574 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_203.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      620 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_301.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      661 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_302.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      559 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      593 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_502.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      742 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_503.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      676 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/loop_statement/rule_504.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5049 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/rules/move_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2581 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/move_token_left_to_next_non_whitespace_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2010 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/move_token_next_to_another_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2515 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/move_token_next_to_another_token_if_it_exists_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3097 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/move_token_sequences_left_of_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3412 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/move_token_to_the_right_of_several_possible_tokens_if_it_exists_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    16070 2022-02-01 11:57:55.000000 vsg-3.9.0/vsg/rules/multiline_alignment_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2948 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/n_spaces_after_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4584 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/n_spaces_before_and_after_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2055 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/n_spaces_between_token_pairs_when_bounded_by_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1091 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/number_of_lines_between_tokens.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.190000 vsg-3.9.0/vsg/rules/package/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      653 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/package/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      513 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      795 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      557 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      638 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      557 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      736 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      838 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      630 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      671 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      699 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      608 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      845 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      530 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      649 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      694 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      592 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_018.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1448 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_019.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1503 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_400.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1328 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package/rule_401.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.200000 vsg-3.9.0/vsg/rules/package_body/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      720 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/rules/package_body/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      655 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      946 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      994 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      914 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      961 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_101.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      585 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_200.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      679 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_201.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      699 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_202.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      646 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_203.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      522 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      548 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_301.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1331 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_400.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1398 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_401.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      569 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      563 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      647 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_502.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      549 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_503.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      555 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_504.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      605 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_505.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_506.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      654 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_507.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      664 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_600.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      709 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/package_body/rule_601.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.210000 vsg-3.9.0/vsg/rules/port/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1149 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/port/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      614 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      470 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      647 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1380 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      416 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      354 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      906 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      905 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      914 2022-02-10 14:33:45.000000 vsg-3.9.0/vsg/rules/port/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1302 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1224 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2974 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1062 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      859 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      762 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1004 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      518 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1326 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_018.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1169 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_019.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1226 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_020.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      578 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_021.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      971 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_022.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1526 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_023.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      970 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_024.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1219 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_025.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2853 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_026.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      613 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port/rule_027.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      995 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/port/rule_600.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      998 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/port/rule_601.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1011 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/port/rule_602.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1013 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/port/rule_603.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1019 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/port/rule_604.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      994 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/port/rule_605.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      996 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/port/rule_606.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1009 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/port/rule_607.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1011 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/port/rule_608.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1017 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/port/rule_609.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.210000 vsg-3.9.0/vsg/rules/port_map/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      250 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/port_map/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      804 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port_map/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1262 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port_map/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      839 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port_map/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      594 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port_map/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      922 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port_map/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1053 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port_map/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      910 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port_map/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1043 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/port_map/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     7140 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/previous_line.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.220000 vsg-3.9.0/vsg/rules/procedure/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      966 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/procedure/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      921 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      905 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      901 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1629 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1234 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      680 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1231 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      789 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      634 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1454 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1065 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1400 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1043 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_101.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      618 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_200.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      359 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_201.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      359 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_202.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      359 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_203.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      359 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_204.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      359 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_205.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1316 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_401.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1145 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_410.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1198 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_411.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1250 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_412.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      589 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      635 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      779 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_502.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      811 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_503.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      785 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_504.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      610 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_505.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      876 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_506.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1203 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure/rule_507.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.220000 vsg-3.9.0/vsg/rules/procedure_call/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      318 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/procedure_call/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      747 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure_call/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      818 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure_call/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1416 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure_call/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      605 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure_call/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      558 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure_call/rule_301.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      495 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure_call/rule_302.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      658 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure_call/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      602 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/procedure_call/rule_501.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.240000 vsg-3.9.0/vsg/rules/process/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1181 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/process/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      741 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1029 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      693 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      785 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      621 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      754 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      750 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      551 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      591 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      786 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      636 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1332 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      779 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      972 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      981 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      801 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      836 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_017.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1054 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_018.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      618 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_019.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      916 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_020.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5706 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_021.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      864 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_022.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      644 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_023.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      877 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_024.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      911 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_025.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5465 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_026.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5257 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_027.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      962 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_028.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     6524 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_029.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2848 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_030.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1684 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_031.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1117 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_032.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1315 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_033.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1639 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_034.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1405 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_035.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      684 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_036.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1704 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_400.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      684 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/process/rule_600.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.240000 vsg-3.9.0/vsg/rules/ranges/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       63 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/ranges/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      687 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/ranges/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      663 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/ranges/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1948 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/remove_blank_lines_above_line_starting_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1816 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/remove_carriage_return_after_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1897 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/remove_carriage_returns_between_token_pairs.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2044 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/remove_comments_from_end_of_lines_bounded_by_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2668 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/remove_excessive_blank_lines_above_line_starting_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2568 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/remove_excessive_blank_lines_below_line_ending_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2076 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/remove_lines_starting_with_token_between_token_pairs.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1120 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/remove_spaces_before_token_rule.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1121 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/remove_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1144 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/remove_tokens_bounded_by_tokens_and_remove_trailing_whitespace.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.240000 vsg-3.9.0/vsg/rules/report_statement/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      253 2021-12-26 15:41:52.000000 vsg-3.9.0/vsg/rules/report_statement/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      723 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/report_statement/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      829 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/report_statement/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      571 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/report_statement/rule_100.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      628 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/report_statement/rule_101.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      638 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/report_statement/rule_300.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4016 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/report_statement/rule_400.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      656 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/report_statement/rule_500.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      660 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/report_statement/rule_501.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3131 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/separate_multiple_signal_identifiers_into_individual_statements.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.240000 vsg-3.9.0/vsg/rules/sequential/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      218 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/sequential/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      641 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/sequential/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      982 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/sequential/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      759 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/sequential/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1040 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/sequential/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      351 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/sequential/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1113 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/sequential/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      883 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/sequential/rule_007.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.250000 vsg-3.9.0/vsg/rules/signal/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      467 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/signal/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      647 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      569 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      760 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      612 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      637 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      652 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      718 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      705 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      334 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/rules/signal/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      531 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/rules/signal/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     6099 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1859 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      890 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      767 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      705 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/signal/rule_600.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2034 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/rules/single_space_after_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2646 2022-02-05 12:32:32.000000 vsg-3.9.0/vsg/rules/single_space_before_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1192 2022-02-05 12:32:32.000000 vsg-3.9.0/vsg/rules/single_space_before_token_if_on_same_line_as_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2233 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/single_space_between_token_pairs.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1978 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/single_space_between_token_pairs_bounded_by_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1841 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/single_space_between_tokens.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.250000 vsg-3.9.0/vsg/rules/source_file/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/source_file/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1106 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/source_file/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     6145 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/rules/spaces_before_and_after_tokens_when_bounded_by_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1453 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/split_line_at_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2621 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/split_line_at_token_if_on_same_line_as_token_if_token_pair_are_not_on_the_same_line.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1742 2022-01-30 20:22:29.000000 vsg-3.9.0/vsg/rules/split_line_at_token_when_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1832 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/split_line_at_token_when_between_tokens_unless_token_is_found.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.250000 vsg-3.9.0/vsg/rules/subprogram_body/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      188 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/subprogram_body/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1010 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/subprogram_body/rule_201.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1017 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/subprogram_body/rule_202.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      712 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/subprogram_body/rule_203.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      663 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/subprogram_body/rule_204.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      752 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/subprogram_body/rule_205.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1698 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/subprogram_body/rule_400.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.250000 vsg-3.9.0/vsg/rules/subtype/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      158 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/subtype/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      698 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/subtype/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1387 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/subtype/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      761 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/subtype/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      627 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/subtype/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      627 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/subtype/rule_600.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1453 2022-02-20 13:54:12.000000 vsg-3.9.0/vsg/rules/token_case.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2815 2022-02-20 13:54:12.000000 vsg-3.9.0/vsg/rules/token_case_formal_part_of_association_element_in_map_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      750 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_case_in_range_bounded_by_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      807 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_case_in_range_bounded_by_tokens_with_prefix_suffix.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2094 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_case_n_token_after_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2453 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_case_n_token_after_tokens_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      816 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_case_subtype_indication.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      628 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_case_with_prefix_suffix.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1389 2022-02-05 12:32:32.000000 vsg-3.9.0/vsg/rules/token_does_not_exist_before_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3272 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_indent.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2757 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_indent_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2576 2022-02-17 04:11:54.000000 vsg-3.9.0/vsg/rules/token_indent_unless_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2179 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_prefix.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2305 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_prefix_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1529 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_suffix.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1663 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/token_suffix_between_tokens.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.260000 vsg-3.9.0/vsg/rules/type_definition/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      561 2021-12-26 15:41:52.000000 vsg-3.9.0/vsg/rules/type_definition/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      691 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      675 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      758 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      834 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      661 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      708 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1328 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1103 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1105 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_009.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      719 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      774 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      901 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      708 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1143 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_014.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      726 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_015.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      701 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_016.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1039 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_400.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      726 2022-02-05 19:34:26.000000 vsg-3.9.0/vsg/rules/type_definition/rule_600.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     7327 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/rules/utils.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.260000 vsg-3.9.0/vsg/rules/variable/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      344 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/variable/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      704 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      577 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      762 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      618 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      655 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      656 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      645 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      533 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/rules/variable/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1943 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      653 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      651 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable/rule_600.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.260000 vsg-3.9.0/vsg/rules/variable_assignment/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      187 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/variable_assignment/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      800 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable_assignment/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      860 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable_assignment/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      794 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable_assignment/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      858 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable_assignment/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      360 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable_assignment/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      939 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/variable_assignment/rule_006.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.260000 vsg-3.9.0/vsg/rules/wait/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/wait/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      678 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/wait/rule_001.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.260000 vsg-3.9.0/vsg/rules/when/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/when/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3602 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/when/rule_001.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.260000 vsg-3.9.0/vsg/rules/while_loop/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       63 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/while_loop/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      336 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/while_loop/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      332 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/while_loop/rule_002.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.270000 vsg-3.9.0/vsg/rules/whitespace/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      405 2022-02-20 15:06:44.000000 vsg-3.9.0/vsg/rules/whitespace/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2241 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      350 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_002.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      531 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_003.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      545 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_004.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1822 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_005.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      877 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_006.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      572 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_007.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1583 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_008.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_010.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1050 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_011.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2423 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_012.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      729 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/whitespace/rule_013.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1743 2022-02-20 15:06:44.000000 vsg-3.9.0/vsg/rules/whitespace/rule_200.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1350 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/whitespace_before_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1618 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/rules/whitespace_before_tokens_in_between_tokens.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.270000 vsg-3.9.0/vsg/rules/with_statement/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       32 2021-12-26 15:41:51.000000 vsg-3.9.0/vsg/rules/with_statement/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      789 2022-02-05 19:34:25.000000 vsg-3.9.0/vsg/rules/with_statement/rule_001.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2214 2021-03-06 15:16:58.000000 vsg-3.9.0/vsg/severity.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.270000 vsg-3.9.0/vsg/styles/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/styles/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      164 2020-12-06 16:00:11.000000 vsg-3.9.0/vsg/styles/indent_only.yaml
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2121 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/styles/jcl.yaml
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.320000 vsg-3.9.0/vsg/token/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      217 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/access_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      666 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/adding_operator.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1088 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/alias_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1915 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/architecture_body.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1116 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/assertion.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      545 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/assertion_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      556 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/association_element.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      184 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/association_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      758 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/attribute_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      991 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/attribute_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      207 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/token/binding_indication.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      196 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/block_header.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2270 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/block_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      822 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/case_generate_alternative.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1555 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/case_generate_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1637 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/case_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      609 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/case_statement_alternative.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      201 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/choice.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      167 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/choices.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1255 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/component.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1383 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/component_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      616 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/component_instantiation_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      384 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/token/component_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      817 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/concurrent_assertion_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      839 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/concurrent_conditional_signal_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      815 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/concurrent_procedure_call_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1452 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/concurrent_selected_signal_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      637 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/concurrent_signal_assignment_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      819 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/concurrent_simple_signal_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      209 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/condition_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      404 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/conditional_expressions.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      787 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/conditional_force_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/conditional_variable_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      599 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/conditional_waveform_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      750 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/conditional_waveforms.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1744 2021-03-19 12:49:30.000000 vsg-3.9.0/vsg/token/configuration_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1170 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/constant_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      412 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/constrained_array_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1357 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/context_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      734 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/context_reference.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      592 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/delay_mechanism.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      344 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/direction.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      212 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/token/element_association.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      366 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/element_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1394 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/entity.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1566 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/token/entity_aspect.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1527 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/entity_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      210 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/entity_designator.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      552 2022-01-20 15:37:21.000000 vsg-3.9.0/vsg/token/entity_name_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      375 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/entity_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      832 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/enumeration_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1065 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/exit_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2025 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/file_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      820 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/file_open_information.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      394 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/file_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1545 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/for_generate_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      372 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/force_mode.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      767 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/full_type_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1610 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/function_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      783 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/generate_statement_body.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      793 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/generic_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      814 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/generic_map_aspect.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      384 2021-03-19 13:20:19.000000 vsg-3.9.0/vsg/token/group_constituent_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1344 2021-03-19 13:35:22.000000 vsg-3.9.0/vsg/token/group_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      370 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/identifier.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      367 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/identifier_list.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.320000 vsg-3.9.0/vsg/token/ieee/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/ieee/__init__.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.320000 vsg-3.9.0/vsg/token/ieee/std_logic_1164/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/ieee/std_logic_1164/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      416 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/ieee/std_logic_1164/function.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1480 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/token/ieee/std_logic_1164/types.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2503 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/if_generate_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1778 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/if_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      601 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/incomplete_type_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      596 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/index_constraint.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      425 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/index_subtype_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1783 2022-01-20 15:39:34.000000 vsg-3.9.0/vsg/token/instantiated_unit.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      747 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/token/instantiation_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1031 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_constant_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      808 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_file_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1702 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_function_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      228 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_incomplete_type_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      383 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      832 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_package_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1316 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_package_generic_map_aspect.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1097 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_procedure_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1978 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_signal_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      220 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_subprogram_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      431 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_subprogram_default.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1016 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_unknown_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1031 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/interface_variable_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      390 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/iteration_scheme.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      369 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/library_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      379 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/logical_name_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1339 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/logical_operator.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1270 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/loop_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      848 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/miscellaneous_operator.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      940 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/mode.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      993 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/multiplying_operator.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1065 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/next_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      711 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/null_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1698 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/package_body.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1553 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/package_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      194 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/package_header.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1037 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/package_instantiation_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      402 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/parameter_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      807 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/token/physical_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      775 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/port_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      798 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/port_map_aspect.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      180 2021-01-09 19:00:33.000000 vsg-3.9.0/vsg/token/pragma.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      388 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/token/primary_unit_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      611 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/procedure_call.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      560 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/procedure_call_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1042 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/procedure_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      213 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/process_sensitivity_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2491 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/process_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1210 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/protected_type_body.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      858 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/protected_type_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      209 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/range_constraint.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      824 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/record_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2717 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/relational_operator.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      914 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/report_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      723 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/return_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      757 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/token/secondary_unit_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      384 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/selected_expressions.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1364 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/selected_force_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1188 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/selected_variable_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1188 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/selected_waveform_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      380 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/selected_waveforms.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      205 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/sensitivity_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      184 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/sensitivity_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1734 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/shared_variable_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1187 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/shift_operator.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      451 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/sign.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      392 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/signal_assignment_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1687 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/signal_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      386 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/signal_kind.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      733 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/signature.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      823 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/token/simple_configuration_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      767 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/simple_force_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      779 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/simple_release_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      584 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/simple_variable_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      584 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/simple_waveform_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      924 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/subprogram_body.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      206 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/subprogram_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      628 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/subprogram_header.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1057 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/subprogram_instantiation_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      405 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/subprogram_kind.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      765 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/subtype_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      203 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/timeout_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      722 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/type_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      177 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/type_mark.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1465 2021-04-07 19:53:22.000000 vsg-3.9.0/vsg/token/unary_logical_operator.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1010 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/unbounded_array_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      706 2022-02-20 13:54:12.000000 vsg-3.9.0/vsg/token/use_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      396 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/variable_assignment_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1891 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/variable_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      191 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/vhdl_range.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      711 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/wait_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      363 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/waveform.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      392 2020-12-18 15:01:20.000000 vsg-3.9.0/vsg/token/waveform_element.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     7300 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/token_map.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     7328 2022-02-06 14:42:23.000000 vsg-3.9.0/vsg/tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1942 2022-02-05 12:32:32.000000 vsg-3.9.0/vsg/utils.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1511 2022-02-20 15:13:53.000000 vsg-3.9.0/vsg/version.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       39 2022-02-20 15:31:16.000000 vsg-3.9.0/vsg/version_info.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.320000 vsg-3.9.0/vsg/vhdlFile/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       31 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/__init__.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.390000 vsg-3.9.0/vsg/vhdlFile/classify/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      603 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/access_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      227 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/actual_parameter_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1256 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/alias_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2007 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/architecture_body.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      288 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/architecture_declarative_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      316 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/architecture_statement_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      534 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/array_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1107 2022-01-21 13:26:52.000000 vsg-3.9.0/vsg/vhdlFile/classify/assertion.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      641 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/assertion_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1756 2021-03-24 22:10:00.000000 vsg-3.9.0/vsg/vhdlFile/classify/association_element.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      559 2021-03-24 22:10:06.000000 vsg-3.9.0/vsg/vhdlFile/classify/association_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      867 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/attribute_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1153 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/attribute_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      785 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/binding_indication.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      123 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/blank.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3763 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/block_declarative_item.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      281 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/block_declarative_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      994 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/block_header.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2029 2022-01-21 13:27:00.000000 vsg-3.9.0/vsg/vhdlFile/classify/block_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      273 2021-02-13 15:21:05.000000 vsg-3.9.0/vsg/vhdlFile/classify/block_statement_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      849 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/case_generate_alternative.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1813 2021-03-13 13:52:43.000000 vsg-3.9.0/vsg/vhdlFile/classify/case_generate_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1610 2021-01-06 14:50:59.000000 vsg-3.9.0/vsg/vhdlFile/classify/case_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      823 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/case_statement_alternative.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      765 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/choice.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      539 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/choices.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      196 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/comment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1665 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/component_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1324 2022-01-20 12:14:56.000000 vsg-3.9.0/vsg/vhdlFile/classify/component_instantiation_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      542 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/component_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      506 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/composite_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      910 2022-01-21 13:27:24.000000 vsg-3.9.0/vsg/vhdlFile/classify/concurrent_assertion_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2070 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/concurrent_conditional_signal_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      725 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/concurrent_procedure_call_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1617 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/concurrent_selected_signal_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1714 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/concurrent_signal_assignment_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1285 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/concurrent_simple_signal_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1640 2022-01-21 13:27:29.000000 vsg-3.9.0/vsg/vhdlFile/classify/concurrent_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      212 2022-01-02 20:24:13.000000 vsg-3.9.0/vsg/vhdlFile/classify/condition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      553 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/condition_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1285 2021-01-06 14:56:06.000000 vsg-3.9.0/vsg/vhdlFile/classify/conditional_expressions.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1193 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/conditional_force_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      895 2021-12-04 13:56:28.000000 vsg-3.9.0/vsg/vhdlFile/classify/conditional_signal_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1031 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/conditional_variable_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1106 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/conditional_waveform_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1267 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/conditional_waveforms.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2000 2021-03-19 12:56:46.000000 vsg-3.9.0/vsg/vhdlFile/classify/configuration_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      659 2021-03-19 13:33:03.000000 vsg-3.9.0/vsg/vhdlFile/classify/configuration_declarative_item.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      384 2021-03-19 12:56:15.000000 vsg-3.9.0/vsg/vhdlFile/classify/configuration_declarative_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      384 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/configuration_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1275 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/constant_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      975 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/constrained_array_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      266 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/context_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1329 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/context_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      623 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/context_item.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      954 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/context_reference.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1036 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/delay_mechanism.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      401 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/design_file.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      431 2022-02-14 12:22:00.000000 vsg-3.9.0/vsg/vhdlFile/classify/design_unit.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1065 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/discrete_range.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      685 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/element_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      254 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/element_subtype_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1364 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/entity_aspect.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1973 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/entity_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3572 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/entity_declarative_item.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      285 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/entity_declarative_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      386 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/entity_designator.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      364 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/entity_header.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      900 2020-12-18 19:12:03.000000 vsg-3.9.0/vsg/vhdlFile/classify/entity_name_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      504 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/entity_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      798 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/entity_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      262 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/entity_statement_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      829 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/enumeration_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1160 2022-01-02 20:24:04.000000 vsg-3.9.0/vsg/vhdlFile/classify/exit_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2605 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/vhdlFile/classify/expression.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1087 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/file_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      230 2021-03-12 02:10:05.000000 vsg-3.9.0/vsg/vhdlFile/classify/file_logical_name.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      900 2021-01-09 01:19:19.000000 vsg-3.9.0/vsg/vhdlFile/classify/file_open_information.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      644 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/file_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1767 2021-01-06 14:56:26.000000 vsg-3.9.0/vsg/vhdlFile/classify/for_generate_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      353 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/force_mode.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      219 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/formal_parameter_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      915 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/full_type_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1747 2021-12-04 13:56:28.000000 vsg-3.9.0/vsg/vhdlFile/classify/function_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      706 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/generate_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1513 2020-12-19 16:06:52.000000 vsg-3.9.0/vsg/vhdlFile/classify/generate_statement_body.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      871 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/generic_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      208 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/generic_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      862 2022-01-21 01:09:08.000000 vsg-3.9.0/vsg/vhdlFile/classify/generic_map_aspect.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      552 2021-03-19 13:42:17.000000 vsg-3.9.0/vsg/vhdlFile/classify/group_constituent_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1159 2021-03-19 13:35:58.000000 vsg-3.9.0/vsg/vhdlFile/classify/group_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      276 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/identifier.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      598 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/identifier_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2742 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/if_generate_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2152 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/if_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      704 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/incomplete_type_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      690 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/index_constraint.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      518 2021-03-12 02:10:05.000000 vsg-3.9.0/vsg/vhdlFile/classify/index_subtype_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2068 2022-01-21 01:20:04.000000 vsg-3.9.0/vsg/vhdlFile/classify/instantiated_unit.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      889 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/instantiation_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      211 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/integer_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1305 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_constant_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      991 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      222 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_element.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      880 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_file_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1720 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_function_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      579 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_incomplete_type_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      554 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1326 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_object_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1100 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_package_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1317 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_package_generic_map_aspect.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1113 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_procedure_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1402 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_signal_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      975 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_subprogram_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      436 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_subprogram_default.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      592 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_subprogram_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      277 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_type_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1597 2021-03-13 14:15:53.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_unknown_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1296 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/interface_variable_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1245 2021-01-11 14:53:18.000000 vsg-3.9.0/vsg/vhdlFile/classify/iteration_scheme.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      697 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/library_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      441 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/library_unit.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      593 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/logical_name_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1623 2021-01-08 23:25:47.000000 vsg-3.9.0/vsg/vhdlFile/classify/loop_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      652 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/vhdlFile/classify/mode.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1117 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/vhdlFile/classify/name.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1245 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/next_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      742 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/null_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1855 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/package_body.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3199 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/package_body_declarative_item.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      380 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/package_body_declarative_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1900 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/package_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3208 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/package_declarative_item.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      360 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/package_declarative_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      587 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/package_header.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1187 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/package_instantiation_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      536 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/parameter_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1503 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/physical_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      845 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/port_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      202 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/port_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      894 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/port_map_aspect.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      496 2021-01-09 19:31:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/pragma.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      382 2020-12-21 21:26:06.000000 vsg-3.9.0/vsg/vhdlFile/classify/preprocessor.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1161 2021-03-19 12:47:20.000000 vsg-3.9.0/vsg/vhdlFile/classify/primary_unit.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      510 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/primary_unit_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1478 2022-01-02 21:59:03.000000 vsg-3.9.0/vsg/vhdlFile/classify/procedure_call.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1538 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/procedure_call_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1313 2021-01-04 23:49:22.000000 vsg-3.9.0/vsg/vhdlFile/classify/procedure_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3025 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/process_declarative_item.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      361 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/process_declarative_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      470 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/process_sensitivity_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2564 2022-01-21 14:00:04.000000 vsg-3.9.0/vsg/vhdlFile/classify/process_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      346 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/process_statement_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1260 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/protected_type_body.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3036 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/protected_type_body_declarative_item.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      337 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/protected_type_body_declarative_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1120 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/protected_type_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1027 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/protected_type_declarative_item.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      315 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/protected_type_declarative_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      505 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/protected_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      686 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/range_constraint.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1022 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/record_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1064 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/report_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1001 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/return_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      904 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/scalar_type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      457 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/secondary_unit.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      771 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/secondary_unit_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1068 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/selected_expressions.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1626 2021-01-06 14:53:15.000000 vsg-3.9.0/vsg/vhdlFile/classify/selected_force_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      811 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/selected_signal_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1400 2021-01-06 14:59:24.000000 vsg-3.9.0/vsg/vhdlFile/classify/selected_variable_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1527 2021-01-06 14:52:38.000000 vsg-3.9.0/vsg/vhdlFile/classify/selected_waveform_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2084 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/selected_waveforms.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      566 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/sensitivity_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1451 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/sensitivity_list.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      346 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/sequence_of_statements.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3197 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/sequential_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1237 2021-12-04 13:56:28.000000 vsg-3.9.0/vsg/vhdlFile/classify/signal_assignment_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1368 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/signal_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      623 2022-02-06 14:42:23.000000 vsg-3.9.0/vsg/vhdlFile/classify/signal_kind.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1490 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/signature.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1251 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/simple_configuration_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1142 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/simple_force_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      858 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/simple_release_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1128 2022-01-06 14:38:32.000000 vsg-3.9.0/vsg/vhdlFile/classify/simple_signal_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1016 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/simple_variable_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1461 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/classify/simple_waveform_assignment.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1391 2021-12-04 13:56:28.000000 vsg-3.9.0/vsg/vhdlFile/classify/subprogram_body.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      525 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/subprogram_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3030 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/subprogram_declarative_item.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      372 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/subprogram_declarative_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      991 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/subprogram_header.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1444 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/subprogram_instantiation_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      606 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/subprogram_kind.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      516 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/subprogram_specification.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      349 2021-12-04 13:56:28.000000 vsg-3.9.0/vsg/vhdlFile/classify/subprogram_statement_part.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      920 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/subtype_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1612 2022-02-10 02:28:44.000000 vsg-3.9.0/vsg/vhdlFile/classify/subtype_indication.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      552 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/timeout_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      506 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/type_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1104 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/type_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      251 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/type_mark.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1450 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/unbounded_array_definition.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      838 2022-02-20 13:54:12.000000 vsg-3.9.0/vsg/vhdlFile/classify/use_clause.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1263 2021-12-04 13:56:28.000000 vsg-3.9.0/vsg/vhdlFile/classify/variable_assignment_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1452 2021-01-06 14:52:06.000000 vsg-3.9.0/vsg/vhdlFile/classify/variable_declaration.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1253 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/wait_statement.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      948 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/waveform.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      867 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/classify/waveform_element.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      742 2021-10-31 12:21:34.000000 vsg-3.9.0/vsg/vhdlFile/classify/whitespace.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1880 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/vhdlFile/code_tags.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.400000 vsg-3.9.0/vsg/vhdlFile/extract/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4866 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/vhdlFile/extract/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      116 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_all_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1404 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_association_elements_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      378 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_blank_lines_above_line_starting_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      431 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_blank_lines_above_line_starting_with_token_when_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1092 2021-02-22 23:22:47.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_blank_lines_below_line_ending_with_several_possible_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1530 2021-02-22 23:22:47.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_blank_lines_below_line_ending_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      423 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_column_of_token_index.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1683 2022-02-20 15:06:44.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_consecutive_lines_starting_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1496 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_consecutive_lines_starting_with_token_and_stopping_when_token_starting_line_is_found.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      984 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_if_statement_conditions.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1794 2021-03-13 13:39:55.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_interface_elements_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      690 2021-01-13 02:11:45.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_line_above_line_starting_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      786 2021-01-13 23:21:55.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_line_above_line_starting_with_token_with_hierarchy.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      735 2021-02-22 23:22:47.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_several_possible_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      696 2021-01-30 01:28:59.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      740 2021-01-30 01:28:15.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_token_with_hierarchy.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      710 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_line_count_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     2262 2021-03-12 02:10:05.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_line_preceeding_line.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      460 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_line_succeeding_line.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      767 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_line_which_includes_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      720 2021-03-13 14:16:38.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_lines_with_length_that_exceed_column.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      936 2021-12-18 14:17:44.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_m_tokens_before_and_n_tokens_after_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      688 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_n_token_after_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      886 2021-03-13 13:40:45.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_n_token_after_tokens_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      486 2021-03-12 02:10:05.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_n_tokens_before_and_after_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      540 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_n_tokens_before_and_after_tokens_bounded_by_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      716 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_sequence_of_tokens_matching.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      792 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_sequence_of_tokens_matching_bounded_by_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      528 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_sequence_of_tokens_not_matching.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      464 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_token_and_n_tokens_after_it.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      515 2022-02-08 13:13:08.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_token_and_n_tokens_after_it_when_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      496 2020-12-18 16:52:06.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_token_and_n_tokens_before_it.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      550 2021-03-31 12:37:49.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_token_and_n_tokens_before_it_in_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      619 2021-12-18 14:17:44.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_token_and_n_tokens_before_it_in_between_tokens_unless_token_is_found.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      831 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1051 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1439 2021-12-18 14:17:44.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching_unless_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      936 2022-02-05 12:05:24.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_between_non_whitespace_token_and_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1055 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_between_tokens_inclusive_while_storing_value_from_token.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3447 2021-10-31 12:21:34.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_bounded_by.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1045 2020-12-22 15:09:26.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_bounded_by_token_when_between_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      709 2021-03-12 02:10:05.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_bounded_by_tokens_if_token_is_between_them.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1623 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_bounded_by_unless_between.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      381 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_from_line.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      426 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_matching.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      658 2020-12-18 15:01:21.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_matching_in_range_bounded_by_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     3792 2021-03-13 13:43:39.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_starting_with_token_and_ending_with_one_of_possible_tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)      702 2022-01-26 13:54:48.000000 vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_where_line_starts_with_token_until_ending_token_is_found.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1820 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/vhdlFile/extract/tokens.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     5099 2022-02-13 04:04:46.000000 vsg-3.9.0/vsg/vhdlFile/extract/utils.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:39.400000 vsg-3.9.0/vsg/vhdlFile/indent/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        0 2020-12-21 00:10:23.000000 vsg-3.9.0/vsg/vhdlFile/indent/__init__.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    14020 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/vhdlFile/indent/indent_config.yaml
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     4920 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/vhdlFile/indent/set_token_indent.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    24015 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/vhdlFile/utils.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    27849 2022-02-20 14:36:34.000000 vsg-3.9.0/vsg/vhdlFile/vhdlFile.py
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     1343 2021-10-31 12:21:34.000000 vsg-3.9.0/vsg/violation.py
+drwxr-xr-x   0 jcleary   (1000) jcleary   (1000)        0 2022-02-20 15:31:38.990000 vsg-3.9.0/vsg.egg-info/
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)     9674 2022-02-20 15:31:38.000000 vsg-3.9.0/vsg.egg-info/PKG-INFO
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)    50701 2022-02-20 15:31:38.000000 vsg-3.9.0/vsg.egg-info/SOURCES.txt
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        1 2022-02-20 15:31:38.000000 vsg-3.9.0/vsg.egg-info/dependency_links.txt
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       43 2022-02-20 15:31:38.000000 vsg-3.9.0/vsg.egg-info/entry_points.txt
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        1 2020-06-21 15:29:54.000000 vsg-3.9.0/vsg.egg-info/not-zip-safe
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)       12 2022-02-20 15:31:38.000000 vsg-3.9.0/vsg.egg-info/requires.txt
+-rw-r--r--   0 jcleary   (1000) jcleary   (1000)        4 2022-02-20 15:31:38.000000 vsg-3.9.0/vsg.egg-info/top_level.txt
```

### Comparing `vsg-3.8.0/PKG-INFO` & `vsg-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: vsg
-Version: 3.8.0
+Version: 3.9.0
 Summary: VHDL Style Guide
 Home-page: https://github.com/jeremiah-c-leary/vhdl-style-guide
 Author: Jeremiah C Leary
 Author-email: jeremiah.c.leary@gmail.com
 License: GNU General Public License
 Download-URL: https://github.com/jeremiah-c-leary/vhdl-style-guide
 Description: VHDL Style Guide (VSG)
```

### Comparing `vsg-3.8.0/README.rst` & `vsg-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/setup.py` & `vsg-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/__main__.py` & `vsg-3.9.0/vsg/__main__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/__parser__.py` & `vsg-3.9.0/vsg/__parser__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/__rule_doc_gen__.py` & `vsg-3.9.0/vsg/__rule_doc_gen__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/apply_rules.py` & `vsg-3.9.0/vsg/apply_rules.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/cmd_line_args.py` & `vsg-3.9.0/vsg/cmd_line_args.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/config.py` & `vsg-3.9.0/vsg/config.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/deprecated_rule.py` & `vsg-3.9.0/vsg/deprecated_rule.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/junit.py` & `vsg-3.9.0/vsg/junit.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/parser.py` & `vsg-3.9.0/vsg/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,14 +296,16 @@
 class comment(item):
     '''
     unique_id = parser : comment
     '''
 
     def __init__(self, sString):
         item.__init__(self, sString)
+        self.is_block_comment = False
+        self.block_comment_indent = None
 
 
 class logical_name(item):
     '''
     unique_id = parser : logical_name
     '''
```

### Comparing `vsg-3.8.0/vsg/proposed_rule.py` & `vsg-3.9.0/vsg/proposed_rule.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/report/summary_stdout.py` & `vsg-3.9.0/vsg/report/summary_stdout.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/report/syntastic_stdout.py` & `vsg-3.9.0/vsg/report/syntastic_stdout.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/report/vsg_stdout.py` & `vsg-3.9.0/vsg/report/vsg_stdout.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rule.py` & `vsg-3.9.0/vsg/rule.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rule_group/length.py` & `vsg-3.9.0/vsg/rule_group/length.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rule_list.py` & `vsg-3.9.0/vsg/rule_list.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/__init__.py` & `vsg-3.9.0/vsg/rules/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,31 +86,35 @@
 from vsg.rules import assert_statement
 from vsg.rules import attribute
 from vsg.rules import attribute_declaration
 from vsg.rules import attribute_specification
 from vsg.rules import block
 from vsg.rules import block_comment
 from vsg.rules import case
+from vsg.rules import case_generate_alternative
+from vsg.rules import case_generate_statement
 from vsg.rules import comment
 from vsg.rules import component
 from vsg.rules import concurrent
 from vsg.rules import constant
 from vsg.rules import context
 from vsg.rules import context_ref
 from vsg.rules import entity
 from vsg.rules import entity_specification
 from vsg.rules import exit_statement
 from vsg.rules import file_statement
 from vsg.rules import for_loop
+from vsg.rules import for_generate_statement
 from vsg.rules import function
 from vsg.rules import generate
 from vsg.rules import generic
 from vsg.rules import generic_map
 from vsg.rules import ieee
 from vsg.rules import if_statement
+from vsg.rules import if_generate_statement
 from vsg.rules import instantiation
 from vsg.rules import iteration_scheme
 from vsg.rules import length
 from vsg.rules import library
 from vsg.rules import logical_operator
 from vsg.rules import loop_statement
 from vsg.rules import package
```

### Comparing `vsg-3.8.0/vsg/rules/after/rule_001.py` & `vsg-3.9.0/vsg/rules/after/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/after/rule_002.py` & `vsg-3.9.0/vsg/rules/after/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/after/rule_003.py` & `vsg-3.9.0/vsg/rules/after/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/alias_declaration/rule_001.py` & `vsg-3.9.0/vsg/rules/alias_declaration/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/alias_declaration/rule_100.py` & `vsg-3.9.0/vsg/rules/alias_declaration/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/alias_declaration/rule_101.py` & `vsg-3.9.0/vsg/rules/alias_declaration/rule_101.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/alias_declaration/rule_300.py` & `vsg-3.9.0/vsg/rules/alias_declaration/rule_300.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/alias_declaration/rule_500.py` & `vsg-3.9.0/vsg/rules/alias_declaration/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/alias_declaration/rule_501.py` & `vsg-3.9.0/vsg/rules/alias_declaration/rule_501.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/alias_declaration/rule_502.py` & `vsg-3.9.0/vsg/rules/alias_declaration/rule_502.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/alias_declaration/rule_503.py` & `vsg-3.9.0/vsg/rules/alias_declaration/rule_503.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/alias_declaration/rule_600.py` & `vsg-3.9.0/vsg/rules/alias_declaration/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/alias_declaration/rule_601.py` & `vsg-3.9.0/vsg/rules/alias_declaration/rule_601.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/align_consecutive_lines_after_line_starting_with_token_and_stopping_with_token.py` & `vsg-3.9.0/vsg/rules/align_consecutive_lines_after_line_starting_with_token_and_stopping_with_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/align_consecutive_lines_starting_with_a_comment_above_line_starting_with_token.py` & `vsg-3.9.0/vsg/rules/align_consecutive_lines_starting_with_a_comment_above_line_starting_with_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/align_left_token_with_right_token_if_right_token_starts_a_line.py` & `vsg-3.9.0/vsg/rules/align_left_token_with_right_token_if_right_token_starts_a_line.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/align_tokens_in_region_between_tokens.py` & `vsg-3.9.0/vsg/rules/align_tokens_in_region_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/align_tokens_in_region_between_tokens_skipping_lines_starting_with_tokens.py` & `vsg-3.9.0/vsg/rules/align_tokens_in_region_between_tokens_skipping_lines_starting_with_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/align_tokens_in_region_between_tokens_unless_between_tokens.py` & `vsg-3.9.0/vsg/rules/align_tokens_in_region_between_tokens_unless_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/align_tokens_in_region_between_tokens_when_between_tokens_unless_between_tokens.py` & `vsg-3.9.0/vsg/rules/align_tokens_in_region_between_tokens_when_between_tokens_unless_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/__init__.py` & `vsg-3.9.0/vsg/rules/architecture/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_002.py` & `vsg-3.9.0/vsg/rules/architecture/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_003.py` & `vsg-3.9.0/vsg/rules/architecture/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_004.py` & `vsg-3.9.0/vsg/rules/architecture/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_005.py` & `vsg-3.9.0/vsg/rules/architecture/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_006.py` & `vsg-3.9.0/vsg/rules/architecture/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_008.py` & `vsg-3.9.0/vsg/rules/architecture/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_009.py` & `vsg-3.9.0/vsg/rules/architecture/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_010.py` & `vsg-3.9.0/vsg/rules/architecture/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_011.py` & `vsg-3.9.0/vsg/rules/architecture/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_012.py` & `vsg-3.9.0/vsg/rules/architecture/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_013.py` & `vsg-3.9.0/vsg/rules/architecture/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_014.py` & `vsg-3.9.0/vsg/rules/architecture/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_015.py` & `vsg-3.9.0/vsg/rules/architecture/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_016.py` & `vsg-3.9.0/vsg/rules/architecture/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_017.py` & `vsg-3.9.0/vsg/rules/architecture/rule_017.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_018.py` & `vsg-3.9.0/vsg/rules/architecture/rule_018.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_019.py` & `vsg-3.9.0/vsg/rules/architecture/rule_019.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_020.py` & `vsg-3.9.0/vsg/rules/architecture/rule_020.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_021.py` & `vsg-3.9.0/vsg/rules/architecture/rule_021.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_022.py` & `vsg-3.9.0/vsg/rules/architecture/rule_022.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_024.py` & `vsg-3.9.0/vsg/rules/architecture/rule_024.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_025.py` & `vsg-3.9.0/vsg/rules/architecture/rule_025.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_026.py` & `vsg-3.9.0/vsg/rules/architecture/rule_026.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_027.py` & `vsg-3.9.0/vsg/rules/architecture/rule_027.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_028.py` & `vsg-3.9.0/vsg/rules/architecture/rule_028.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_029.py` & `vsg-3.9.0/vsg/rules/architecture/rule_029.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_030.py` & `vsg-3.9.0/vsg/rules/architecture/rule_030.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_031.py` & `vsg-3.9.0/vsg/rules/architecture/rule_031.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_032.py` & `vsg-3.9.0/vsg/rules/architecture/rule_032.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_033.py` & `vsg-3.9.0/vsg/rules/architecture/rule_033.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_200.py` & `vsg-3.9.0/vsg/rules/architecture/rule_200.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_600.py` & `vsg-3.9.0/vsg/rules/architecture/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/architecture/rule_601.py` & `vsg-3.9.0/vsg/rules/architecture/rule_601.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/assert_statement/rule_001.py` & `vsg-3.9.0/vsg/rules/assert_statement/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/assert_statement/rule_002.py` & `vsg-3.9.0/vsg/rules/assert_statement/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/assert_statement/rule_003.py` & `vsg-3.9.0/vsg/rules/assert_statement/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/assert_statement/rule_004.py` & `vsg-3.9.0/vsg/rules/assert_statement/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/assert_statement/rule_005.py` & `vsg-3.9.0/vsg/rules/assert_statement/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/assert_statement/rule_400.py` & `vsg-3.9.0/vsg/rules/assert_statement/rule_400.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute/rule_001.py` & `vsg-3.9.0/vsg/rules/attribute/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute/rule_002.py` & `vsg-3.9.0/vsg/rules/attribute/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_declaration/rule_100.py` & `vsg-3.9.0/vsg/rules/attribute_declaration/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_declaration/rule_101.py` & `vsg-3.9.0/vsg/rules/attribute_declaration/rule_101.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_declaration/rule_300.py` & `vsg-3.9.0/vsg/rules/attribute_declaration/rule_300.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_declaration/rule_500.py` & `vsg-3.9.0/vsg/rules/attribute_declaration/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_declaration/rule_501.py` & `vsg-3.9.0/vsg/rules/attribute_declaration/rule_501.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_declaration/rule_502.py` & `vsg-3.9.0/vsg/rules/attribute_declaration/rule_502.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_specification/rule_100.py` & `vsg-3.9.0/vsg/rules/attribute_specification/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_specification/rule_101.py` & `vsg-3.9.0/vsg/rules/attribute_specification/rule_101.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_specification/rule_300.py` & `vsg-3.9.0/vsg/rules/attribute_specification/rule_300.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_specification/rule_500.py` & `vsg-3.9.0/vsg/rules/attribute_specification/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_specification/rule_501.py` & `vsg-3.9.0/vsg/rules/attribute_specification/rule_501.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_specification/rule_502.py` & `vsg-3.9.0/vsg/rules/attribute_specification/rule_502.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/attribute_specification/rule_503.py` & `vsg-3.9.0/vsg/rules/attribute_specification/rule_503.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/blank_line_above_line_starting_with_token.py` & `vsg-3.9.0/vsg/rules/blank_line_above_line_starting_with_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/blank_line_above_line_starting_with_token_when_between_tokens.py` & `vsg-3.9.0/vsg/rules/blank_line_above_line_starting_with_token_when_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/blank_line_below_line_ending_with_several_possible_tokens.py` & `vsg-3.9.0/vsg/rules/blank_line_below_line_ending_with_several_possible_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/blank_line_below_line_ending_with_token.py` & `vsg-3.9.0/vsg/rules/blank_line_below_line_ending_with_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/blank_lines_between_token_pairs.py` & `vsg-3.9.0/vsg/rules/blank_lines_between_token_pairs.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/__init__.py` & `vsg-3.9.0/vsg/rules/block/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_001.py` & `vsg-3.9.0/vsg/rules/block/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_002.py` & `vsg-3.9.0/vsg/rules/block/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_003.py` & `vsg-3.9.0/vsg/rules/block/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_004.py` & `vsg-3.9.0/vsg/rules/block/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_005.py` & `vsg-3.9.0/vsg/rules/block/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_006.py` & `vsg-3.9.0/vsg/rules/block/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_007.py` & `vsg-3.9.0/vsg/rules/block/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_100.py` & `vsg-3.9.0/vsg/rules/block/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_101.py` & `vsg-3.9.0/vsg/rules/block/rule_101.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_200.py` & `vsg-3.9.0/vsg/rules/block/rule_200.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_201.py` & `vsg-3.9.0/vsg/rules/block/rule_201.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_202.py` & `vsg-3.9.0/vsg/rules/block/rule_202.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_203.py` & `vsg-3.9.0/vsg/rules/block/rule_203.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_204.py` & `vsg-3.9.0/vsg/rules/block/rule_204.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_205.py` & `vsg-3.9.0/vsg/rules/block/rule_205.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_302.py` & `vsg-3.9.0/vsg/rules/block/rule_302.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_400.py` & `vsg-3.9.0/vsg/rules/block/rule_400.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_401.py` & `vsg-3.9.0/vsg/rules/block/rule_401.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_500.py` & `vsg-3.9.0/vsg/rules/block/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_501.py` & `vsg-3.9.0/vsg/rules/block/rule_501.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_502.py` & `vsg-3.9.0/vsg/rules/block/rule_502.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_503.py` & `vsg-3.9.0/vsg/rules/block/rule_503.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_504.py` & `vsg-3.9.0/vsg/rules/block/rule_504.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_505.py` & `vsg-3.9.0/vsg/rules/block/rule_505.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_506.py` & `vsg-3.9.0/vsg/rules/block/rule_506.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_600.py` & `vsg-3.9.0/vsg/rules/block/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block/rule_601.py` & `vsg-3.9.0/vsg/rules/block/rule_601.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/block_comment/rule_001.py` & `vsg-3.9.0/vsg/rules/block_comment/rule_001.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
 import math
-import string
 
 from vsg import block_rule
 from vsg import parser
 from vsg import violation
 
 
 class rule_001(block_rule.Rule):
@@ -43,16 +42,14 @@
         self.configuration.extend(['header_left', 'header_left_repeat', 'header_string', 'header_right_repeat', 'header_alignment', 'max_header_column'])
 
     def analyze(self, oFile):
 
         self._print_debug_message('Analyzing rule: ' + self.unique_id)
         lToi = self._get_tokens_of_interest(oFile)
 
-        lUpdate = []
-
         for oToi in lToi:
             lTokens = oToi.get_tokens()
 
             if not self.allow_indenting:
                 iWhitespace = 0
             elif isinstance(lTokens[0], parser.comment):
                 iWhitespace = self.indentSize * lTokens[0].get_indent()
@@ -70,15 +67,14 @@
             if self.header_string is None:
                 sHeader += self.header_left_repeat * (self.max_header_column - iWhitespace - len(sHeader))
             elif self.header_alignment == 'center':
                 iLeft = math.floor((self.max_header_column - iWhitespace - len(self.header_string)) / 2) - iHeader_left - 2
                 sLeft = self.header_left_repeat * iLeft
                 iRight = self.max_header_column - iWhitespace - 2 - iHeader_left - len(self.header_string) - iLeft
                 sRight = self.header_right_repeat * iRight
-#                print(f'({self.max_header_column} - {iWhitespace} - {len(self.header_string)}) / 2  - {iHeader_left} = {iLeft}')
                 sHeader += sLeft + self.header_string + sRight
             elif self.header_alignment == 'left':
                 sHeader += self.header_left_repeat
                 sHeader += self.header_string
                 iLength = self.max_header_column - iWhitespace - len(sHeader)
                 sHeader += self.header_right_repeat * iLength
             elif self.header_alignment == 'right':
@@ -87,39 +83,21 @@
                 sHeader += self.header_string
                 sHeader += self.header_right_repeat
 
             for oToken in lTokens:
                 if isinstance(oToken, parser.comment):
                     sComment = oToken.get_value()
                     try:
-                        if is_header(sComment):
-                            if not self.allow_indenting:
-                                oToken.set_indent(0)
+                        if block_rule.is_header(sComment):
+                            self.set_token_indent(oToken)
                             if sComment != sHeader:
                                 sSolution = 'Change block comment header to : ' + sHeader
                                 oViolation = violation.New(oToi.get_line_number(), oToi, sSolution)
                                 self.add_violation(oViolation)
                         break
                     except IndexError:
                         break
-            if not self.allow_indenting:
-                lUpdate.append(violation.New(0, oToi, ''))
-
-        if not self.allow_indenting:
-            oFile.update(lUpdate)
-
 
-def is_header(sComment):
-    try:
-        if sComment[2] not in string.punctuation:
-            return False
-        if sComment[2] == '!':
-            return False
-        if sComment[3] not in string.punctuation:
-            return False
-    except IndexError:
-        return True
-    return True
 
 #         1         2         3         4         5         6         7         8
 #-------------------------------<-    80 chars    ->-----------------------------
 #------------------------------<-    80 chars    ->------------------------------
```

### Comparing `vsg-3.8.0/vsg/rules/block_comment/rule_002.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_001.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,94 @@
 
-import string
-
-from vsg import block_rule
 from vsg import parser
 from vsg import violation
 
-from vsg.vhdlFile import utils
+from vsg.rule_group import whitespace
 
 
-class rule_002(block_rule.Rule):
+class rule_001(whitespace.Rule):
     '''
-    This rule checks the **comment_left** attribute exists for all comments.
-
-    |configuring_block_comments_link|
+    This rule check for trailing spaces.
 
     **Violation**
 
+    Where periods indicate spaces:
+
     .. code-block:: vhdl
 
-       --+-------------[ Header ]==============
-       --   Comment
-       --   Comment
-       ----------------------------------------
+        library ieee;....
 
     **Fix**
 
     .. code-block:: vhdl
 
-       --+-------------[ Header ]==============
-       --|  Comment
-       --|  Comment
-       ----------------------------------------
+        library ieee;
     '''
 
     def __init__(self):
-        block_rule.Rule.__init__(self, 'block_comment', '002')
-        self.comment_left = None
-        self.configuration.append('comment_left')
 
-    def analyze(self, oFile):
+        whitespace.Rule.__init__(self, 'whitespace', '001')
+        self.phase = 1
+        self.subphase = 0
+        self.solution = 'Remove trailing whitespace'
 
-        self._print_debug_message('Analyzing rule: ' + self.unique_id)
-        lToi = self._get_tokens_of_interest(oFile)
-
-        lUpdate = []
+    def _get_tokens_of_interest(self, oFile):
+        return oFile.get_n_tokens_before_token(2, [parser.carriage_return])
 
+    def _analyze(self, lToi):
         for oToi in lToi:
-            iLine, lTokens = utils.get_toi_parameters(oToi)
+            if whitespace_exists(oToi):
+                create_violation(oToi, self)
+
+    def _fix_violation(self, oViolation):
+        dAction = oViolation.get_action()
+        if need_to_remove_whitespace(dAction):
+            remove_whitespace(oViolation)
+        else:
+            remove_whitespace_and_insert_blank_line(oViolation)
+
+
+def create_violation(oToi, self):
+    lTokens = oToi.get_tokens()
+    oViolation = violation.New(oToi.get_line_number(), oToi, self.solution)
+    dAction = define_action(lTokens)
+    oViolation.set_action(dAction)
+    self.add_violation(oViolation)
+
+
+def whitespace_exists(oToi):
+    lTokens = oToi.get_tokens()
+    if isinstance(lTokens[1], parser.whitespace):
+        return True
+    return False
+
+
+def define_action(lTokens):
+    dAction = {}
+    if isinstance(lTokens[0], parser.carriage_return):
+        dAction['action'] = 'insert_blank_line'
+    else:
+        dAction['action'] = 'remove'
+    return dAction
 
-            iComments = utils.count_token_types_in_list_of_tokens(parser.comment, lTokens)
 
-            iComment = 0
-            for iToken, oToken in enumerate(lTokens):
-                iLine = utils.increment_line_number(iLine, oToken)
-
-                if isinstance(oToken, parser.comment):
-                    iComment += 1
-                    if iComment == 1:
-                        if not is_header(oToken.get_value()):
-                            break
-                    elif iComment > 1 and iComment < iComments:
-                        if not self.allow_indenting:
-                            oToken.set_indent(0)
-
-                        if self.comment_left is None:
-                            continue
-
-                        if isinstance(lTokens[iToken - 1], parser.whitespace):
-                            if not self.allow_indenting:
-                                break
-
-                        sHeader = '--'
-                        sHeader += self.comment_left
-                        sComment = oToken.get_value()
-                        if not sComment.startswith(sHeader):
-                            sSolution = 'Comment must start with ' + sHeader
-                            oViolation = violation.New(iLine, oToi, sSolution)
-                            self.add_violation(oViolation)
-
-            if not self.allow_indenting:
-                lUpdate.append(violation.New(0, oToi, ''))
-
-        if not self.allow_indenting:
-            oFile.update(lUpdate)
-
-
-def is_header(sComment):
-    try:
-        if sComment[2] not in string.punctuation:
-            return False
-        if sComment[2] == '!':
-            return False
-        if sComment[3] not in string.punctuation:
-            return False
-    except IndexError:
+def need_to_remove_whitespace(dAction):
+    if dAction['action'] == 'remove':
         return True
-    return True
+    return False
+
+
+def remove_whitespace(oViolation):
+    lTokens = oViolation.get_tokens()
+    myTokens = []
+    myTokens.append(lTokens[0])
+    myTokens.append(lTokens[-1])
+    oViolation.set_tokens(myTokens)
+
+
+def remove_whitespace_and_insert_blank_line(oViolation):
+    lTokens = oViolation.get_tokens()
+    myTokens = []
+    myTokens.append(lTokens[0])
+    myTokens.append(parser.blank_line())
+    myTokens.append(lTokens[-1])
+    oViolation.set_tokens(myTokens)
```

### Comparing `vsg-3.8.0/vsg/rules/block_comment/rule_003.py` & `vsg-3.9.0/vsg/block_rule.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,130 +1,176 @@
 
 import string
 
-from vsg import block_rule
 from vsg import parser
-from vsg import violation
+
+from vsg.rule_group import structure
 
 from vsg.vhdlFile import utils
+from vsg.rules import utils as rules_utils
 
 
-class rule_003(block_rule.Rule):
-    '''
-    This rule checks the block comment footer is correct.
+class Rule(structure.Rule):
 
-    |configuring_block_comments_link|
+    def __init__(self, name, identifier):
+        structure.Rule.__init__(self, name=name, identifier=identifier)
+        self.fixable = False
+        self.disable = True
 
-    **Violation**
+        self.min_height = 3
+        self.configuration.append('min_height')
+        self.allow_indenting = True
+        self.configuration.append('allow_indenting')
 
-    .. code-block:: vhdl
+    def _get_tokens_of_interest(self, oFile):
+        lToi = oFile.get_consecutive_lines_starting_with_token(parser.comment, self.min_height)
+        lReturn = []
+        for oToi in lToi:
+            iLeft, iLines, iRight = adjust_for_code_tags(oToi)
+            if iLines >= self.min_height:
+                lReturn.append(oToi.extract_tokens(iLeft, iRight))
+        return lReturn
 
-       --+-------------[ Header ]==============
-       --|  Comment
-       --|  Comment
-       ----------------------------------------
+    def _analyze(self, lToi):
 
-    **Fix**
+        for oToi in lToi:
 
-    .. code-block:: vhdl
+            if not first_comment_is_a_header(oToi):
+                continue
 
-       --+-------------[ Header ]==============
-       --|  Comment
-       --|  Comment
-       --+--------------------------[ Footer ]=
-    '''
+            self.analyze_comments(oToi)
 
-    def __init__(self):
-        block_rule.Rule.__init__(self, 'block_comment', '003')
-        self.footer_left = None
-        self.footer_left_repeat = '-'
-        self.footer_string = None
-        self.footer_right_repeat = None
-        self.footer_alignment = 'center'
-        self.max_footer_column = 120
-        self.configuration.extend(['footer_left', 'footer_left_repeat', 'footer_string', 'footer_right_repeat', 'footer_alignment', 'max_footer_column'])
+    def fix(self, oFile, dFixOnly=None):
+        '''
+        Applies fixes for any rule violations.
+        '''
+        self.analyze(oFile)
+
+    def set_token_indent(self, oToken):
+        if self.allow_indenting:
+            oToken.is_block_comment = False
+        else:
+            oToken.set_indent(0)
+            oToken.is_block_comment = True
+            oToken.block_comment_indent = 0
+
+    def calculate_leading_whitespace(self, oToken):
+        if self.allow_indenting:
+            iWhitespace = self.indentSize * oToken.get_indent()
+        else:
+            iWhitespace = 0
+        return iWhitespace
+
+    def build_footer(self, oToken):
+        iWhitespace = self.calculate_leading_whitespace(oToken)
+        sFooter = '--'
+        if self.footer_left is not None:
+            sFooter += self.footer_left
+            iFooter_left = len(self.footer_left)
+        else:
+            iFooter_left = 0
+
+        if self.footer_string is None:
+            sFooter += self.footer_left_repeat * (self.max_footer_column - iWhitespace - len(sFooter))
+        elif self.footer_alignment == 'center':
+            iLength = int((self.max_footer_column - iWhitespace - len(self.footer_string)) / 2) - iFooter_left - 2
+            sFooter += self.footer_left_repeat * (iLength)
+            sFooter += self.footer_string
+            sFooter += self.footer_right_repeat * (self.max_footer_column - len(sFooter))
+        elif self.footer_alignment == 'left':
+            sFooter += self.footer_left_repeat
+            sFooter += self.footer_string
+            sFooter += self.footer_right_repeat * (self.max_footer_column - len(sFooter))
+        elif self.footer_alignment == 'right':
+            iLength = self.max_footer_column - iWhitespace - len(sFooter) - len(self.footer_string) - 1
+            sFooter += self.footer_left_repeat * (iLength)
+            sFooter += self.footer_string
+            sFooter += self.footer_right_repeat
+        return sFooter
+
+    def build_comment(self, oToken):
+        sHeader = '--'
+        sHeader += self.comment_left
+        return sHeader
+
+
+def is_header(sComment):
+    if bare_comment(sComment):
+        return False
+    if not third_character_is_alphanumeric(sComment):
+        return False
+    return fourth_character_is_alphanumeric(sComment)
 
-    def analyze(self, oFile):
 
-        self._print_debug_message('Analyzing rule: ' + self.unique_id)
-        lToi = self._get_tokens_of_interest(oFile)
+def fourth_character_is_alphanumeric(sComment):
+    try:
+        if sComment[3] not in string.punctuation:
+            return False
+    except IndexError:
+        return True
+    return True
 
-        lUpdate = []
 
-        for oToi in lToi:
-            iLine, lTokens = utils.get_toi_parameters(oToi)
+def third_character_is_alphanumeric(sComment):
+    if sComment[2] not in string.punctuation:
+        return False
+    if sComment[2] == '!':
+        return False
+    return True
 
-            iComments = utils.count_token_types_in_list_of_tokens(parser.comment, lTokens)
 
-            iComment = 0
-            for iToken, oToken in enumerate(lTokens):
-                iLine = utils.increment_line_number(iLine, oToken)
-
-                if isinstance(oToken, parser.comment):
-                    iComment += 1
-                    if iComment == iComments:
-
-                        if not self.allow_indenting:
-                            if isinstance(lTokens[iToken - 1], parser.whitespace):
-                                break
-                            else:
-                                oToken.set_indent(0)
-
-                        iWhitespace = self.indentSize * oToken.get_indent()
-
-                        sFooter = '--'
-                        if self.footer_left is not None:
-                            sFooter += self.footer_left
-                            iFooter_left = len(self.footer_left)
-                        else:
-                            iFooter_left = 0
-
-                        if self.footer_string is None:
-                            sFooter += self.footer_left_repeat * (self.max_footer_column - iWhitespace - len(sFooter))
-                        elif self.footer_alignment == 'center':
-                            iLength = int((self.max_footer_column - iWhitespace - len(self.footer_string)) / 2) - iFooter_left - 2
-                            sFooter += self.footer_left_repeat * (iLength)
-                            sFooter += self.footer_string
-                            sFooter += self.footer_right_repeat * (self.max_footer_column - len(sFooter))
-                        elif self.footer_alignment == 'left':
-                            sFooter += self.footer_left_repeat
-                            sFooter += self.footer_string
-                            iLength = self.max_footer_column - iWhitespace - len(sFooter)
-                            sFooter += self.footer_right_repeat * (self.max_footer_column - len(sFooter))
-                        elif self.footer_alignment == 'right':
-                            iLength = self.max_footer_column - iWhitespace - len(sFooter) - len(self.footer_string) - 1
-                            sFooter += self.footer_left_repeat * (iLength)
-                            sFooter += self.footer_string
-                            sFooter += self.footer_right_repeat
-
-                        sComment = oToken.get_value()
-                        try:
-                            if is_footer(sComment):
-                                if not self.allow_indenting:
-                                    oToken.set_indent(0)
-                                if sComment != sFooter:
-                                    sSolution = 'Change block comment footer to : ' + sFooter
-                                    oViolation = violation.New(iLine, oToi, sSolution)
-                                    self.add_violation(oViolation)
-                                    break
-                        except IndexError:
-                            break
+def bare_comment(sString):
+    if sString == '--':
+        return True
+    return False
 
-            if not self.allow_indenting:
-                lUpdate.append(violation.New(0, oToi, ''))
 
-        if not self.allow_indenting:
-            oFile.update(lUpdate)
+def is_footer(sComment):
+    return is_header(sComment)
 
 
-def is_footer(sComment):
-    try:
-        if sComment[2] not in string.punctuation:
-            return False
-        if sComment[2] == '!':
-            return False
-        if sComment[3] not in string.punctuation:
-            return False
+def first_comment_is_a_header(oToi):
+    oToken = oToi.get_first_token_matching(parser.comment)
+    if is_header(oToken.get_value()):
         return True
-    except IndexError:
+    return False
+
+
+def adjust_for_code_tags(oToi):
+    lTokens = oToi.get_tokens()
+    iLeft, iLines, iRight = extract_initial_indexes_from_token_list(lTokens)
+    iLeft, iLines = adjust_indexes_for_code_tags_at_beginning_of_block_comment(lTokens, iLeft, iLines)
+    iRight, iLines = adjust_indexes_for_code_tags_at_end_of_block_comment(lTokens, iRight, iLines)
+    return iLeft, iLines, iRight
+
+
+def extract_initial_indexes_from_token_list(lTokens):
+    iLines = utils.count_carriage_returns(lTokens) + 1
+    iLeft = 0
+    iRight = len(lTokens)
+    return iLeft, iLines, iRight
+
+
+def adjust_indexes_for_code_tags_at_beginning_of_block_comment(lTokens, iLeft, iLines):
+    if code_tag_detected(lTokens[0]):
+        iLeft = 2
+        iLines -= 1
+    if code_tag_detected(lTokens[1]):
+        iLeft = 3
+        iLines -= 1
+    return iLeft, iLines
+
+
+def adjust_indexes_for_code_tags_at_end_of_block_comment(lTokens, iRight, iLines):
+    if code_tag_detected(lTokens[-1]):
+        if rules_utils.token_is_whitespace(lTokens[-2]):
+            iRight = len(lTokens) - 4
+        else:
+            iRight = len(lTokens) - 3
+        iLines -= 1
+    return iRight, iLines
+
+
+def code_tag_detected(oToken):
+    if 'vsg_on' in oToken.get_value() or 'vsg_off' in oToken.get_value():
         return True
-    return True
+    return False
```

### Comparing `vsg-3.8.0/vsg/rules/case/__init__.py` & `vsg-3.9.0/vsg/rules/case/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_001.py` & `vsg-3.9.0/vsg/rules/case/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_002.py` & `vsg-3.9.0/vsg/rules/case/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_003.py` & `vsg-3.9.0/vsg/rules/case/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_004.py` & `vsg-3.9.0/vsg/rules/case/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_005.py` & `vsg-3.9.0/vsg/rules/case/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_006.py` & `vsg-3.9.0/vsg/rules/case/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_007.py` & `vsg-3.9.0/vsg/rules/case/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_009.py` & `vsg-3.9.0/vsg/rules/case/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_010.py` & `vsg-3.9.0/vsg/rules/case/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_011.py` & `vsg-3.9.0/vsg/rules/case/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_012.py` & `vsg-3.9.0/vsg/rules/case/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_013.py` & `vsg-3.9.0/vsg/rules/case/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_014.py` & `vsg-3.9.0/vsg/rules/case/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_015.py` & `vsg-3.9.0/vsg/rules/case/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_016.py` & `vsg-3.9.0/vsg/rules/case/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_017.py` & `vsg-3.9.0/vsg/rules/case/rule_017.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_018.py` & `vsg-3.9.0/vsg/rules/case/rule_018.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_019.py` & `vsg-3.9.0/vsg/rules/case/rule_019.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_020.py` & `vsg-3.9.0/vsg/rules/case/rule_020.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_021.py` & `vsg-3.9.0/vsg/rules/case/rule_021.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_200.py` & `vsg-3.9.0/vsg/rules/case/rule_200.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case/rule_201.py` & `vsg-3.9.0/vsg/rules/case/rule_201.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/case_utils.py` & `vsg-3.9.0/vsg/rules/case_utils.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/comment/rule_004.py` & `vsg-3.9.0/vsg/rules/comment/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/comment/rule_010.py` & `vsg-3.9.0/vsg/rules/comment/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/comment/rule_011.py` & `vsg-3.9.0/vsg/rules/comment/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/comment/rule_100.py` & `vsg-3.9.0/vsg/rules/comment/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/__init__.py` & `vsg-3.9.0/vsg/rules/component/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_001.py` & `vsg-3.9.0/vsg/rules/component/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_002.py` & `vsg-3.9.0/vsg/rules/component/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_003.py` & `vsg-3.9.0/vsg/rules/component/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_004.py` & `vsg-3.9.0/vsg/rules/component/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_005.py` & `vsg-3.9.0/vsg/rules/component/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_006.py` & `vsg-3.9.0/vsg/rules/component/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_007.py` & `vsg-3.9.0/vsg/rules/component/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_008.py` & `vsg-3.9.0/vsg/rules/component/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_009.py` & `vsg-3.9.0/vsg/rules/component/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_010.py` & `vsg-3.9.0/vsg/rules/component/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_011.py` & `vsg-3.9.0/vsg/rules/component/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_012.py` & `vsg-3.9.0/vsg/rules/component/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_013.py` & `vsg-3.9.0/vsg/rules/component/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_014.py` & `vsg-3.9.0/vsg/rules/component/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_016.py` & `vsg-3.9.0/vsg/rules/component/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_017.py` & `vsg-3.9.0/vsg/rules/component/rule_017.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_018.py` & `vsg-3.9.0/vsg/rules/component/rule_018.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_019.py` & `vsg-3.9.0/vsg/rules/component/rule_019.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_020.py` & `vsg-3.9.0/vsg/rules/component/rule_020.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/component/rule_021.py` & `vsg-3.9.0/vsg/rules/component/rule_021.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/concurrent/rule_001.py` & `vsg-3.9.0/vsg/rules/concurrent/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/concurrent/rule_002.py` & `vsg-3.9.0/vsg/rules/concurrent/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/concurrent/rule_003.py` & `vsg-3.9.0/vsg/rules/concurrent/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/concurrent/rule_004.py` & `vsg-3.9.0/vsg/rules/concurrent/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/concurrent/rule_005.py` & `vsg-3.9.0/vsg/rules/concurrent/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/concurrent/rule_006.py` & `vsg-3.9.0/vsg/rules/concurrent/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/concurrent/rule_007.py` & `vsg-3.9.0/vsg/rules/concurrent/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/concurrent/rule_008.py` & `vsg-3.9.0/vsg/rules/concurrent/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/concurrent/rule_009.py` & `vsg-3.9.0/vsg/rules/concurrent/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/concurrent/rule_010.py` & `vsg-3.9.0/vsg/rules/concurrent/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/concurrent/rule_011.py` & `vsg-3.9.0/vsg/rules/concurrent/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/consistent_case_of_tokens_from_between_tokens_applied_to_region.py` & `vsg-3.9.0/vsg/rules/consistent_case_of_tokens_from_between_tokens_applied_to_region.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/consistent_token_case.py` & `vsg-3.9.0/vsg/rules/consistent_token_case.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_001.py` & `vsg-3.9.0/vsg/rules/constant/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_002.py` & `vsg-3.9.0/vsg/rules/constant/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_003.py` & `vsg-3.9.0/vsg/rules/constant/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_004.py` & `vsg-3.9.0/vsg/rules/constant/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_005.py` & `vsg-3.9.0/vsg/rules/constant/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_006.py` & `vsg-3.9.0/vsg/rules/constant/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_007.py` & `vsg-3.9.0/vsg/rules/constant/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_010.py` & `vsg-3.9.0/vsg/rules/constant/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_011.py` & `vsg-3.9.0/vsg/rules/constant/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_012.py` & `vsg-3.9.0/vsg/rules/constant/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_013.py` & `vsg-3.9.0/vsg/rules/constant/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_014.py` & `vsg-3.9.0/vsg/rules/constant/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_015.py` & `vsg-3.9.0/vsg/rules/constant/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_016.py` & `vsg-3.9.0/vsg/rules/constant/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_100.py` & `vsg-3.9.0/vsg/rules/constant/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/constant/rule_600.py` & `vsg-3.9.0/vsg/rules/constant/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/__init__.py` & `vsg-3.9.0/vsg/rules/context/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_002.py` & `vsg-3.9.0/vsg/rules/context/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_003.py` & `vsg-3.9.0/vsg/rules/context/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_004.py` & `vsg-3.9.0/vsg/rules/context/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_005.py` & `vsg-3.9.0/vsg/rules/context/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_006.py` & `vsg-3.9.0/vsg/rules/context/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_007.py` & `vsg-3.9.0/vsg/rules/context/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_008.py` & `vsg-3.9.0/vsg/rules/context/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_009.py` & `vsg-3.9.0/vsg/rules/context/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_010.py` & `vsg-3.9.0/vsg/rules/context/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_011.py` & `vsg-3.9.0/vsg/rules/context/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_012.py` & `vsg-3.9.0/vsg/rules/context/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_013.py` & `vsg-3.9.0/vsg/rules/context/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_014.py` & `vsg-3.9.0/vsg/rules/context/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_015.py` & `vsg-3.9.0/vsg/rules/context/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_016.py` & `vsg-3.9.0/vsg/rules/context/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_017.py` & `vsg-3.9.0/vsg/rules/context/rule_017.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_018.py` & `vsg-3.9.0/vsg/rules/context/rule_018.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_019.py` & `vsg-3.9.0/vsg/rules/context/rule_019.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_021.py` & `vsg-3.9.0/vsg/rules/context/rule_021.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_022.py` & `vsg-3.9.0/vsg/rules/context/rule_022.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_023.py` & `vsg-3.9.0/vsg/rules/context/rule_023.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_024.py` & `vsg-3.9.0/vsg/rules/context/rule_024.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_025.py` & `vsg-3.9.0/vsg/rules/context/rule_025.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context/rule_026.py` & `vsg-3.9.0/vsg/rules/subprogram_body/rule_204.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 
-from vsg.rules import remove_excessive_blank_lines_below_line_ending_with_token
+from vsg.rules import blank_line_above_line_starting_with_token
 
-from vsg.token import context_declaration as token
+from vsg import token
 
+lTokens = []
+lTokens.append(token.subprogram_body.end_keyword)
 
-class rule_026(remove_excessive_blank_lines_below_line_ending_with_token):
+
+class rule_204(blank_line_above_line_starting_with_token):
     '''
-    This rule ensures a single blank line after the **context** keword.
+    This rule checks for blank lines above the **end** keyword.
+
+    |configuring_blank_lines_link|
 
     **Violation**
 
     .. code-block:: vhdl
 
-       context c1 is
-
+       begin
 
-
-         library ieee;
+         a <= b;
+       end function overflow;
 
     **Fix**
 
     .. code-block:: vhdl
 
-       context c1 is
+       begin
+
+         a <= b;
 
-         library ieee;
+       end function overflow;
     '''
+
     def __init__(self):
-        remove_excessive_blank_lines_below_line_ending_with_token.__init__(self, 'context', '026', [token.is_keyword])
+        blank_line_above_line_starting_with_token.__init__(self, 'subprogram_body', '204', lTokens)
```

### Comparing `vsg-3.8.0/vsg/rules/context/rule_027.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_007.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 
 from vsg.rules import remove_excessive_blank_lines_above_line_starting_with_token
 
-from vsg.token import context_declaration as token
+from vsg import token
 
+lTokens = []
+lTokens.append(token.if_statement.elsif_keyword)
 
-class rule_027(remove_excessive_blank_lines_above_line_starting_with_token):
+lOverrides = []
+lOverrides.append(token.case_statement.semicolon)
+
+
+class rule_007(remove_excessive_blank_lines_above_line_starting_with_token):
     '''
-    This rule ensures a single blank line before the **end** keword.
+    This rule checks for blank lines before the **elsif** keyword.
 
     **Violation**
 
     .. code-block:: vhdl
 
-         use ieee.std_logic_1164.all;
+        b <= '0'
 
 
 
-       end context;
+      elsif (c = '1') then
 
     **Fix**
 
     .. code-block:: vhdl
 
-         use ieee.std_logic_1164.all;
-
-       end context;
+        b <= '0'
+      elsif (c = '1') then
     '''
     def __init__(self):
-        remove_excessive_blank_lines_above_line_starting_with_token.__init__(self, 'context', '027', [token.end_keyword])
+        remove_excessive_blank_lines_above_line_starting_with_token.__init__(self, 'if', '007', lTokens, iAllow=0, lOverrides=lOverrides)
+        self.solution = 'Remove blank line(s) before the *elsif* keyword.'
```

### Comparing `vsg-3.8.0/vsg/rules/context/rule_028.py` & `vsg-3.9.0/vsg/rules/context/rule_028.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context_ref/rule_002.py` & `vsg-3.9.0/vsg/rules/context_ref/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context_ref/rule_003.py` & `vsg-3.9.0/vsg/rules/context_ref/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context_ref/rule_004.py` & `vsg-3.9.0/vsg/rules/context_ref/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context_ref/rule_005.py` & `vsg-3.9.0/vsg/rules/context_ref/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context_ref/rule_007.py` & `vsg-3.9.0/vsg/rules/context_ref/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/context_ref/rule_009.py` & `vsg-3.9.0/vsg/rules/context_ref/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/__init__.py` & `vsg-3.9.0/vsg/rules/package/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,12 +14,10 @@
 from .rule_013 import rule_013
 from .rule_014 import rule_014
 from .rule_015 import rule_015
 from .rule_016 import rule_016
 from .rule_017 import rule_017
 from .rule_018 import rule_018
 from .rule_019 import rule_019
-from .rule_020 import rule_020
 
-from .rule_200 import rule_200
-
-from .rule_600 import rule_600
+from .rule_400 import rule_400
+from .rule_401 import rule_401
```

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_002.py` & `vsg-3.9.0/vsg/rules/entity/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_003.py` & `vsg-3.9.0/vsg/rules/entity/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_004.py` & `vsg-3.9.0/vsg/rules/entity/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_005.py` & `vsg-3.9.0/vsg/rules/entity/rule_005.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,9 +24,9 @@
        entity fifo is
 
        entity fifo is
     '''
 
     def __init__(self):
         move_token_next_to_another_token.__init__(self, 'entity', '005', token.identifier, token.is_keyword)
-        self.subphase = 1
+        self.subphase = 2
         self.solution = 'Move *is* keyword next to identifier'
```

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_006.py` & `vsg-3.9.0/vsg/rules/entity/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_007.py` & `vsg-3.9.0/vsg/rules/entity/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_008.py` & `vsg-3.9.0/vsg/rules/entity/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_009.py` & `vsg-3.9.0/vsg/rules/entity/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_010.py` & `vsg-3.9.0/vsg/rules/entity/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_011.py` & `vsg-3.9.0/vsg/rules/entity/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_012.py` & `vsg-3.9.0/vsg/rules/entity/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_013.py` & `vsg-3.9.0/vsg/rules/entity/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_014.py` & `vsg-3.9.0/vsg/rules/entity/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_015.py` & `vsg-3.9.0/vsg/rules/entity/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_016.py` & `vsg-3.9.0/vsg/rules/entity/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_017.py` & `vsg-3.9.0/vsg/rules/entity/rule_017.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_018.py` & `vsg-3.9.0/vsg/rules/entity/rule_018.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_019.py` & `vsg-3.9.0/vsg/rules/entity/rule_019.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_020.py` & `vsg-3.9.0/vsg/rules/entity/rule_020.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_200.py` & `vsg-3.9.0/vsg/rules/entity/rule_200.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity/rule_600.py` & `vsg-3.9.0/vsg/rules/entity/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity_specification/rule_100.py` & `vsg-3.9.0/vsg/rules/entity_specification/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity_specification/rule_101.py` & `vsg-3.9.0/vsg/rules/entity_specification/rule_101.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity_specification/rule_500.py` & `vsg-3.9.0/vsg/rules/entity_specification/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity_specification/rule_501.py` & `vsg-3.9.0/vsg/rules/entity_specification/rule_501.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/entity_specification/rule_503.py` & `vsg-3.9.0/vsg/rules/entity_specification/rule_503.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/existence_of_tokens_which_should_not_occur.py` & `vsg-3.9.0/vsg/rules/existence_of_tokens_which_should_not_occur.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/exit_statement/rule_300.py` & `vsg-3.9.0/vsg/rules/exit_statement/rule_300.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/file_length.py` & `vsg-3.9.0/vsg/rules/file_length.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/file_statement/rule_001.py` & `vsg-3.9.0/vsg/rules/file_statement/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/file_statement/rule_002.py` & `vsg-3.9.0/vsg/rules/file_statement/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/file_statement/rule_003.py` & `vsg-3.9.0/vsg/rules/file_statement/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/formal_part_in_association_element_between_tokens.py` & `vsg-3.9.0/vsg/rules/formal_part_in_association_element_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/__init__.py` & `vsg-3.9.0/vsg/rules/function/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_001.py` & `vsg-3.9.0/vsg/rules/function/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_004.py` & `vsg-3.9.0/vsg/rules/function/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_005.py` & `vsg-3.9.0/vsg/rules/function/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_006.py` & `vsg-3.9.0/vsg/rules/function/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_008.py` & `vsg-3.9.0/vsg/rules/function/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_009.py` & `vsg-3.9.0/vsg/rules/function/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_010.py` & `vsg-3.9.0/vsg/rules/function/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_012.py` & `vsg-3.9.0/vsg/rules/function/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_013.py` & `vsg-3.9.0/vsg/rules/function/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_014.py` & `vsg-3.9.0/vsg/rules/function/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_015.py` & `vsg-3.9.0/vsg/rules/function/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_016.py` & `vsg-3.9.0/vsg/rules/function/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_017.py` & `vsg-3.9.0/vsg/rules/function/rule_017.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_100.py` & `vsg-3.9.0/vsg/rules/function/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_101.py` & `vsg-3.9.0/vsg/rules/function/rule_101.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_300.py` & `vsg-3.9.0/vsg/rules/function/rule_300.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_502.py` & `vsg-3.9.0/vsg/rules/function/rule_502.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/function/rule_506.py` & `vsg-3.9.0/vsg/rules/function/rule_506.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/__init__.py` & `vsg-3.9.0/vsg/rules/generate/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 from .rule_400 import rule_400
 from .rule_401 import rule_401
 from .rule_402 import rule_402
 from .rule_403 import rule_403
 from .rule_404 import rule_404
 from .rule_405 import rule_405
 
+from .rule_500 import rule_500
+from .rule_501 import rule_501
+
 from .rule_600 import rule_600
```

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_001.py` & `vsg-3.9.0/vsg/rules/generate/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_002.py` & `vsg-3.9.0/vsg/rules/generate/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_003.py` & `vsg-3.9.0/vsg/rules/generate/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_004.py` & `vsg-3.9.0/vsg/rules/generate/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_005.py` & `vsg-3.9.0/vsg/rules/generate/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_006.py` & `vsg-3.9.0/vsg/rules/generate/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_007.py` & `vsg-3.9.0/vsg/rules/generate/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_008.py` & `vsg-3.9.0/vsg/rules/generate/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_009.py` & `vsg-3.9.0/vsg/rules/generate/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_010.py` & `vsg-3.9.0/vsg/rules/generate/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_011.py` & `vsg-3.9.0/vsg/rules/generate/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_012.py` & `vsg-3.9.0/vsg/rules/generate/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_013.py` & `vsg-3.9.0/vsg/rules/generate/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_014.py` & `vsg-3.9.0/vsg/rules/generate/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_015.py` & `vsg-3.9.0/vsg/rules/generate/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_016.py` & `vsg-3.9.0/vsg/rules/generate/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_017.py` & `vsg-3.9.0/vsg/rules/generate/rule_017.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_018.py` & `vsg-3.9.0/vsg/rules/generate/rule_018.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_400.py` & `vsg-3.9.0/vsg/rules/generate/rule_400.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_401.py` & `vsg-3.9.0/vsg/rules/generate/rule_401.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_402.py` & `vsg-3.9.0/vsg/rules/generate/rule_402.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_403.py` & `vsg-3.9.0/vsg/rules/generate/rule_403.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_404.py` & `vsg-3.9.0/vsg/rules/generate/rule_404.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_405.py` & `vsg-3.9.0/vsg/rules/generate/rule_405.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generate/rule_600.py` & `vsg-3.9.0/vsg/rules/generate/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/__init__.py` & `vsg-3.9.0/vsg/rules/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_002.py` & `vsg-3.9.0/vsg/rules/generic/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_003.py` & `vsg-3.9.0/vsg/rules/generic/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_004.py` & `vsg-3.9.0/vsg/rules/generic/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_005.py` & `vsg-3.9.0/vsg/rules/generic/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_006.py` & `vsg-3.9.0/vsg/rules/generic/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_007.py` & `vsg-3.9.0/vsg/rules/generic/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_009.py` & `vsg-3.9.0/vsg/rules/generic/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_010.py` & `vsg-3.9.0/vsg/rules/generic/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_013.py` & `vsg-3.9.0/vsg/rules/generic/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_014.py` & `vsg-3.9.0/vsg/rules/generic/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_016.py` & `vsg-3.9.0/vsg/rules/generic/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_017.py` & `vsg-3.9.0/vsg/rules/generic/rule_017.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_018.py` & `vsg-3.9.0/vsg/rules/generic/rule_018.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_019.py` & `vsg-3.9.0/vsg/rules/generic/rule_019.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_020.py` & `vsg-3.9.0/vsg/rules/generic/rule_020.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_021.py` & `vsg-3.9.0/vsg/rules/generic/rule_021.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic/rule_600.py` & `vsg-3.9.0/vsg/rules/generic/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic_map/rule_001.py` & `vsg-3.9.0/vsg/rules/generic_map/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic_map/rule_002.py` & `vsg-3.9.0/vsg/rules/generic_map/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic_map/rule_003.py` & `vsg-3.9.0/vsg/rules/generic_map/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic_map/rule_004.py` & `vsg-3.9.0/vsg/rules/generic_map/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic_map/rule_005.py` & `vsg-3.9.0/vsg/rules/generic_map/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic_map/rule_006.py` & `vsg-3.9.0/vsg/rules/generic_map/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic_map/rule_007.py` & `vsg-3.9.0/vsg/rules/generic_map/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/generic_map/rule_008.py` & `vsg-3.9.0/vsg/rules/generic_map/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/ieee/rule_500.py` & `vsg-3.9.0/vsg/rules/ieee/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/__init__.py` & `vsg-3.9.0/vsg/rules/if_statement/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_001.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_002.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_003.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_004.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_005.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_005.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 
 from vsg import parser
 from vsg import token
 
-from vsg.rules import single_space_between_token_pairs
+from vsg.rules import single_space_after_token as Rule
 
 lTokens = []
-lTokens.append([token.if_statement.elsif_keyword, parser.open_parenthesis])
+lTokens.append(token.if_statement.elsif_keyword)
 
 
-class rule_005(single_space_between_token_pairs):
+class rule_005(Rule):
     '''
-    This rule checks for a single space between the **elsif** keyword and the (.
+    This rule checks for a single space after the **elsif** keyword.
 
     **Violation**
 
     .. code-block:: vhdl
 
       elsif(c = '1') then
 
       elsif   (c = '1') then
 
+      elsif    b = '0' then
+
     **Fix**
 
     .. code-block:: vhdl
 
       elsif (c = '1') then
 
       elsif (c = '1') then
+
+      elsif b = '0' then
     '''
     def __init__(self):
-        single_space_between_token_pairs.__init__(self, 'if', '005', lTokens)
-        self.solution = 'Ensure only a single space exists between the *elsif* keyword and {.'
+        Rule.__init__(self, 'if', '005', lTokens)
+        self.solution = 'Ensure only a single space exists after the *elsif* keyword.'
```

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_006.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_007.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_010.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 
 from vsg.rules import remove_excessive_blank_lines_above_line_starting_with_token
 
 from vsg import token
 
 lTokens = []
-lTokens.append(token.if_statement.elsif_keyword)
+lTokens.append(token.if_statement.else_keyword)
 
 lOverrides = []
 lOverrides.append(token.case_statement.semicolon)
 
 
-class rule_007(remove_excessive_blank_lines_above_line_starting_with_token):
+class rule_010(remove_excessive_blank_lines_above_line_starting_with_token):
     '''
-    This rule checks for blank lines before the **elsif** keyword.
+    This rule checks for blank lines before the **else** keyword.
 
     **Violation**
 
     .. code-block:: vhdl
 
-        b <= '0'
+        d <= '1';
 
 
-
-      elsif (c = '1') then
+      else
 
     **Fix**
 
     .. code-block:: vhdl
 
-        b <= '0'
-      elsif (c = '1') then
+        d <= '1';
+      else
     '''
     def __init__(self):
-        remove_excessive_blank_lines_above_line_starting_with_token.__init__(self, 'if', '007', lTokens, iAllow=0, lOverrides=lOverrides)
-        self.solution = 'Remove blank line(s) before the *elsif* keyword.'
+        remove_excessive_blank_lines_above_line_starting_with_token.__init__(self, 'if', '010', lTokens, iAllow=0, lOverrides=lOverrides)
+        self.solution = 'Remove blank line(s) before the *else* keyword.'
```

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_008.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_009.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_010.py` & `vsg-3.9.0/vsg/rules/if_generate_statement/rule_503.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 
-from vsg.rules import remove_excessive_blank_lines_above_line_starting_with_token
-
 from vsg import token
 
-lTokens = []
-lTokens.append(token.if_statement.else_keyword)
+from vsg.rules import token_case as Rule
 
-lOverrides = []
-lOverrides.append(token.case_statement.semicolon)
+lTokens = []
+lTokens.append(token.if_generate_statement.else_keyword)
 
 
-class rule_010(remove_excessive_blank_lines_above_line_starting_with_token):
+class rule_503(Rule):
     '''
-    This rule checks for blank lines before the **else** keyword.
+    This rule checks the *else* keyword has proper case.
+
+    |configuring_uppercase_and_lowercase_rules_link|
 
     **Violation**
 
     .. code-block:: vhdl
 
-        d <= '1';
-
-
-      else
+       ELSE generate
 
     **Fix**
 
     .. code-block:: vhdl
 
-        d <= '1';
-      else
+       else generate
     '''
+
     def __init__(self):
-        remove_excessive_blank_lines_above_line_starting_with_token.__init__(self, 'if', '010', lTokens, iAllow=0, lOverrides=lOverrides)
-        self.solution = 'Remove blank line(s) before the *else* keyword.'
+        Rule.__init__(self, 'if_generate_statement', '503', lTokens)
+        self.groups.append('case::keyword')
```

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_011.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_012.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_013.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_014.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_015.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_020.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_020.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_021.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_021.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_022.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_022.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_023.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_023.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_024.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_024.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_025.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_025.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_026.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_026.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_027.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_027.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_028.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_028.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_029.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_029.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_030.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_030.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_031.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_031.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_032.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_032.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_033.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_033.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_034.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_034.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_035.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_035.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/if_statement/rule_036.py` & `vsg-3.9.0/vsg/rules/if_statement/rule_036.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment.py` & `vsg-3.9.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment_and_not_on_same_line_as_token.py` & `vsg-3.9.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment_and_not_on_same_line_as_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment_when_between_tokens.py` & `vsg-3.9.0/vsg/rules/insert_carriage_return_after_token_if_it_is_not_followed_by_a_comment_when_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/insert_token_left_of_token_if_it_does_not_exist_between_tokens.py` & `vsg-3.9.0/vsg/rules/insert_token_left_of_token_if_it_does_not_exist_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/insert_token_left_of_token_if_it_does_not_exist_between_tokens_using_value_from_token.py` & `vsg-3.9.0/vsg/rules/insert_token_left_of_token_if_it_does_not_exist_between_tokens_using_value_from_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/insert_token_right_of_possible_tokens_if_it_does_not_exist_before_token.py` & `vsg-3.9.0/vsg/rules/insert_token_right_of_possible_tokens_if_it_does_not_exist_before_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/insert_token_right_of_token_if_it_does_not_exist_before_token.py` & `vsg-3.9.0/vsg/rules/insert_token_right_of_token_if_it_does_not_exist_before_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/insert_tokens_right_of_token_if_it_does_not_exist_before_token.py` & `vsg-3.9.0/vsg/rules/insert_tokens_right_of_token_if_it_does_not_exist_before_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/__init__.py` & `vsg-3.9.0/vsg/rules/instantiation/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_001.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_002.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_003.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_004.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_005.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_008.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_009.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_010.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_012.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_019.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_019.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_023.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_023.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_024.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_024.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_027.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_027.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_028.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_028.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_029.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_029.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_031.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_031.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_032.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_032.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_033.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_033.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_034.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_034.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_035.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_035.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_600.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/instantiation/rule_601.py` & `vsg-3.9.0/vsg/rules/instantiation/rule_601.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/is_token_value_one_of.py` & `vsg-3.9.0/vsg/rules/is_token_value_one_of.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/iteration_scheme/rule_100.py` & `vsg-3.9.0/vsg/rules/iteration_scheme/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/iteration_scheme/rule_101.py` & `vsg-3.9.0/vsg/rules/iteration_scheme/rule_101.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/iteration_scheme/rule_300.py` & `vsg-3.9.0/vsg/rules/iteration_scheme/rule_300.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/iteration_scheme/rule_301.py` & `vsg-3.9.0/vsg/rules/iteration_scheme/rule_301.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/iteration_scheme/rule_500.py` & `vsg-3.9.0/vsg/rules/iteration_scheme/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/iteration_scheme/rule_501.py` & `vsg-3.9.0/vsg/rules/iteration_scheme/rule_501.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_001.py` & `vsg-3.9.0/vsg/rules/library/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_002.py` & `vsg-3.9.0/vsg/rules/library/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_003.py` & `vsg-3.9.0/vsg/rules/library/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_004.py` & `vsg-3.9.0/vsg/rules/library/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_005.py` & `vsg-3.9.0/vsg/rules/library/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_006.py` & `vsg-3.9.0/vsg/rules/library/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_007.py` & `vsg-3.9.0/vsg/rules/library/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_008.py` & `vsg-3.9.0/vsg/rules/library/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_009.py` & `vsg-3.9.0/vsg/rules/library/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_010.py` & `vsg-3.9.0/vsg/rules/library/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_011.py` & `vsg-3.9.0/vsg/rules/library/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/library/rule_600.py` & `vsg-3.9.0/vsg/rules/library/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/line_length.py` & `vsg-3.9.0/vsg/rules/line_length.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/logical_operator/rule_500.py` & `vsg-3.9.0/vsg/rules/logical_operator/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/__init__.py` & `vsg-3.9.0/vsg/rules/loop_statement/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_001.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_002.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_003.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_004.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_005.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_006.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_007.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_100.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_101.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_101.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_102.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_102.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_103.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_103.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_104.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_104.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_200.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_200.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_201.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_201.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_202.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_202.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_203.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_203.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_300.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_300.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_301.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_301.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_302.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_302.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_500.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_501.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_501.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_502.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_502.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_503.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_503.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/loop_statement/rule_504.py` & `vsg-3.9.0/vsg/rules/loop_statement/rule_504.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/move_token.py` & `vsg-3.9.0/vsg/rules/move_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/move_token_left_to_next_non_whitespace_token.py` & `vsg-3.9.0/vsg/rules/move_token_left_to_next_non_whitespace_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     '''
 
     def __init__(self, name, identifier, token_to_move):
         structure.Rule.__init__(self, name, identifier)
         self.subphase = 2
         self.token_to_move = token_to_move
         self.bInsertWhitespace = True
+        self.bRemoveTrailingWhitespace = True
 
     def _get_tokens_of_interest(self, oFile):
         lToi = oFile.get_tokens_between_non_whitespace_token_and_token(self.token_to_move)
         lReturn = []
         for oToi in lToi:
             lTokens = oToi.get_tokens()
             if skip_based_on_whitespace(self.bInsertWhitespace, lTokens):
@@ -61,15 +62,18 @@
 
         rules_utils.insert_token(lTokens, 1, lTokens.pop())
 
         if self.bInsertWhitespace:
             rules_utils.insert_whitespace(lTokens, 1)
 
         lNewTokens = utils.remove_consecutive_whitespace_tokens(lTokens)
-        lNewTokens = utils.remove_trailing_whitespace(lNewTokens)
+
+        if self.bRemoveTrailingWhitespace:
+            lNewTokens = utils.remove_trailing_whitespace(lNewTokens)
+
         lNewTokens = utils.fix_blank_lines(lNewTokens)
 
         oViolation.set_tokens(lNewTokens)
 
 
 def does_a_whitespace_token_separate_tokens(lTokens):
     if len(lTokens) == 3 and isinstance(lTokens[1], parser.whitespace):
```

### Comparing `vsg-3.8.0/vsg/rules/move_token_next_to_another_token.py` & `vsg-3.9.0/vsg/rules/move_token_next_to_another_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/move_token_next_to_another_token_if_it_exists_between_tokens.py` & `vsg-3.9.0/vsg/rules/move_token_next_to_another_token_if_it_exists_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/move_token_sequences_left_of_token.py` & `vsg-3.9.0/vsg/rules/move_token_sequences_left_of_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/move_token_to_the_right_of_several_possible_tokens_if_it_exists_between_tokens.py` & `vsg-3.9.0/vsg/rules/move_token_to_the_right_of_several_possible_tokens_if_it_exists_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/multiline_alignment_between_tokens.py` & `vsg-3.9.0/vsg/rules/multiline_alignment_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/n_spaces_after_tokens.py` & `vsg-3.9.0/vsg/rules/n_spaces_after_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/n_spaces_before_and_after_tokens.py` & `vsg-3.9.0/vsg/rules/n_spaces_before_and_after_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/n_spaces_between_token_pairs_when_bounded_by_tokens.py` & `vsg-3.9.0/vsg/rules/n_spaces_between_token_pairs_when_bounded_by_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/number_of_lines_between_tokens.py` & `vsg-3.9.0/vsg/rules/number_of_lines_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/__init__.py` & `vsg-3.9.0/vsg/rules/type_definition/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,13 +11,11 @@
 from .rule_010 import rule_010
 from .rule_011 import rule_011
 from .rule_012 import rule_012
 from .rule_013 import rule_013
 from .rule_014 import rule_014
 from .rule_015 import rule_015
 from .rule_016 import rule_016
-from .rule_017 import rule_017
-from .rule_018 import rule_018
-from .rule_019 import rule_019
 
 from .rule_400 import rule_400
-from .rule_401 import rule_401
+
+from .rule_600 import rule_600
```

### Comparing `vsg-3.8.0/vsg/rules/package/rule_001.py` & `vsg-3.9.0/vsg/rules/package/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_002.py` & `vsg-3.9.0/vsg/rules/package/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_003.py` & `vsg-3.9.0/vsg/rules/package/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_004.py` & `vsg-3.9.0/vsg/rules/package/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_005.py` & `vsg-3.9.0/vsg/rules/package/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_006.py` & `vsg-3.9.0/vsg/rules/package/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_007.py` & `vsg-3.9.0/vsg/rules/package/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_008.py` & `vsg-3.9.0/vsg/rules/package/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_009.py` & `vsg-3.9.0/vsg/rules/package/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_010.py` & `vsg-3.9.0/vsg/rules/package/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_011.py` & `vsg-3.9.0/vsg/rules/package/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_012.py` & `vsg-3.9.0/vsg/rules/package/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_013.py` & `vsg-3.9.0/vsg/rules/package/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_014.py` & `vsg-3.9.0/vsg/rules/package/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_015.py` & `vsg-3.9.0/vsg/rules/package/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_016.py` & `vsg-3.9.0/vsg/rules/package/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_017.py` & `vsg-3.9.0/vsg/rules/package/rule_017.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_018.py` & `vsg-3.9.0/vsg/rules/package/rule_018.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_019.py` & `vsg-3.9.0/vsg/rules/package/rule_019.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_400.py` & `vsg-3.9.0/vsg/rules/package/rule_400.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package/rule_401.py` & `vsg-3.9.0/vsg/rules/package/rule_401.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/__init__.py` & `vsg-3.9.0/vsg/rules/package_body/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_001.py` & `vsg-3.9.0/vsg/rules/package_body/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_002.py` & `vsg-3.9.0/vsg/rules/package_body/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_003.py` & `vsg-3.9.0/vsg/rules/package_body/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_100.py` & `vsg-3.9.0/vsg/rules/package_body/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_101.py` & `vsg-3.9.0/vsg/rules/package_body/rule_101.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_200.py` & `vsg-3.9.0/vsg/rules/package_body/rule_200.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_201.py` & `vsg-3.9.0/vsg/rules/package_body/rule_201.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_202.py` & `vsg-3.9.0/vsg/rules/package_body/rule_202.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_203.py` & `vsg-3.9.0/vsg/rules/package_body/rule_203.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_300.py` & `vsg-3.9.0/vsg/rules/package_body/rule_300.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_301.py` & `vsg-3.9.0/vsg/rules/package_body/rule_301.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_400.py` & `vsg-3.9.0/vsg/rules/package_body/rule_400.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_401.py` & `vsg-3.9.0/vsg/rules/package_body/rule_401.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_500.py` & `vsg-3.9.0/vsg/rules/package_body/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_501.py` & `vsg-3.9.0/vsg/rules/package_body/rule_501.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_502.py` & `vsg-3.9.0/vsg/rules/package_body/rule_502.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_503.py` & `vsg-3.9.0/vsg/rules/package_body/rule_503.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_504.py` & `vsg-3.9.0/vsg/rules/package_body/rule_504.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_505.py` & `vsg-3.9.0/vsg/rules/package_body/rule_505.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_506.py` & `vsg-3.9.0/vsg/rules/package_body/rule_506.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_507.py` & `vsg-3.9.0/vsg/rules/package_body/rule_507.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_600.py` & `vsg-3.9.0/vsg/rules/package_body/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/package_body/rule_601.py` & `vsg-3.9.0/vsg/rules/package_body/rule_601.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/__init__.py` & `vsg-3.9.0/vsg/rules/port/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,7 +22,18 @@
 from .rule_021 import rule_021
 from .rule_022 import rule_022
 from .rule_023 import rule_023
 from .rule_024 import rule_024
 from .rule_025 import rule_025
 from .rule_026 import rule_026
 from .rule_027 import rule_027
+
+from .rule_600 import rule_600
+from .rule_601 import rule_601
+from .rule_602 import rule_602
+from .rule_603 import rule_603
+from .rule_604 import rule_604
+from .rule_605 import rule_605
+from .rule_606 import rule_606
+from .rule_607 import rule_607
+from .rule_608 import rule_608
+from .rule_609 import rule_609
```

### Comparing `vsg-3.8.0/vsg/rules/port/rule_001.py` & `vsg-3.9.0/vsg/rules/port/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_003.py` & `vsg-3.9.0/vsg/rules/port/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_004.py` & `vsg-3.9.0/vsg/rules/port/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_007.py` & `vsg-3.9.0/vsg/rules/port/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_008.py` & `vsg-3.9.0/vsg/rules/port/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_009.py` & `vsg-3.9.0/vsg/rules/port/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_010.py` & `vsg-3.9.0/vsg/rules/port/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_011.py` & `vsg-3.9.0/vsg/rules/port/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_012.py` & `vsg-3.9.0/vsg/rules/port/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_013.py` & `vsg-3.9.0/vsg/rules/port/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_014.py` & `vsg-3.9.0/vsg/rules/port/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_015.py` & `vsg-3.9.0/vsg/rules/port/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_016.py` & `vsg-3.9.0/vsg/rules/port/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_017.py` & `vsg-3.9.0/vsg/rules/port/rule_017.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_018.py` & `vsg-3.9.0/vsg/rules/port/rule_018.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_019.py` & `vsg-3.9.0/vsg/rules/port/rule_019.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_020.py` & `vsg-3.9.0/vsg/rules/port/rule_020.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_021.py` & `vsg-3.9.0/vsg/rules/port/rule_021.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_022.py` & `vsg-3.9.0/vsg/rules/port/rule_022.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_023.py` & `vsg-3.9.0/vsg/rules/port/rule_023.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_024.py` & `vsg-3.9.0/vsg/rules/port/rule_024.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_025.py` & `vsg-3.9.0/vsg/rules/port/rule_025.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_026.py` & `vsg-3.9.0/vsg/rules/port/rule_026.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port/rule_027.py` & `vsg-3.9.0/vsg/rules/port/rule_027.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port_map/rule_001.py` & `vsg-3.9.0/vsg/rules/port_map/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port_map/rule_002.py` & `vsg-3.9.0/vsg/rules/port_map/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port_map/rule_003.py` & `vsg-3.9.0/vsg/rules/port_map/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port_map/rule_004.py` & `vsg-3.9.0/vsg/rules/port_map/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port_map/rule_005.py` & `vsg-3.9.0/vsg/rules/port_map/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port_map/rule_007.py` & `vsg-3.9.0/vsg/rules/port_map/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port_map/rule_008.py` & `vsg-3.9.0/vsg/rules/port_map/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/port_map/rule_009.py` & `vsg-3.9.0/vsg/rules/port_map/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/previous_line.py` & `vsg-3.9.0/vsg/rules/previous_line.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/__init__.py` & `vsg-3.9.0/vsg/rules/procedure/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_001.py` & `vsg-3.9.0/vsg/rules/procedure/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_002.py` & `vsg-3.9.0/vsg/rules/procedure/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_003.py` & `vsg-3.9.0/vsg/rules/procedure/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_004.py` & `vsg-3.9.0/vsg/rules/procedure/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_005.py` & `vsg-3.9.0/vsg/rules/procedure/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_006.py` & `vsg-3.9.0/vsg/rules/procedure/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_007.py` & `vsg-3.9.0/vsg/rules/procedure/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_008.py` & `vsg-3.9.0/vsg/rules/procedure/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_009.py` & `vsg-3.9.0/vsg/rules/procedure/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_010.py` & `vsg-3.9.0/vsg/rules/procedure/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_011.py` & `vsg-3.9.0/vsg/rules/procedure/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_100.py` & `vsg-3.9.0/vsg/rules/procedure/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_101.py` & `vsg-3.9.0/vsg/rules/procedure/rule_101.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_200.py` & `vsg-3.9.0/vsg/rules/procedure/rule_200.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_401.py` & `vsg-3.9.0/vsg/rules/procedure/rule_401.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_410.py` & `vsg-3.9.0/vsg/rules/procedure/rule_410.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_411.py` & `vsg-3.9.0/vsg/rules/procedure/rule_411.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_412.py` & `vsg-3.9.0/vsg/rules/procedure/rule_412.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_500.py` & `vsg-3.9.0/vsg/rules/procedure/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_501.py` & `vsg-3.9.0/vsg/rules/procedure/rule_501.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_502.py` & `vsg-3.9.0/vsg/rules/procedure/rule_502.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_503.py` & `vsg-3.9.0/vsg/rules/procedure/rule_503.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_504.py` & `vsg-3.9.0/vsg/rules/procedure/rule_504.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_505.py` & `vsg-3.9.0/vsg/rules/procedure/rule_505.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_506.py` & `vsg-3.9.0/vsg/rules/procedure/rule_506.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure/rule_507.py` & `vsg-3.9.0/vsg/rules/procedure/rule_507.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure_call/rule_001.py` & `vsg-3.9.0/vsg/rules/procedure_call/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure_call/rule_002.py` & `vsg-3.9.0/vsg/rules/procedure_call/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure_call/rule_100.py` & `vsg-3.9.0/vsg/rules/procedure_call/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure_call/rule_300.py` & `vsg-3.9.0/vsg/rules/procedure_call/rule_300.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure_call/rule_301.py` & `vsg-3.9.0/vsg/rules/procedure_call/rule_301.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure_call/rule_500.py` & `vsg-3.9.0/vsg/rules/procedure_call/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/procedure_call/rule_501.py` & `vsg-3.9.0/vsg/rules/procedure_call/rule_501.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/__init__.py` & `vsg-3.9.0/vsg/rules/process/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_001.py` & `vsg-3.9.0/vsg/rules/process/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_002.py` & `vsg-3.9.0/vsg/rules/process/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_003.py` & `vsg-3.9.0/vsg/rules/process/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_004.py` & `vsg-3.9.0/vsg/rules/process/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_005.py` & `vsg-3.9.0/vsg/rules/process/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_006.py` & `vsg-3.9.0/vsg/rules/process/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_007.py` & `vsg-3.9.0/vsg/rules/process/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_008.py` & `vsg-3.9.0/vsg/rules/process/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_009.py` & `vsg-3.9.0/vsg/rules/process/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_010.py` & `vsg-3.9.0/vsg/rules/process/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_011.py` & `vsg-3.9.0/vsg/rules/process/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_012.py` & `vsg-3.9.0/vsg/rules/process/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_013.py` & `vsg-3.9.0/vsg/rules/process/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_014.py` & `vsg-3.9.0/vsg/rules/process/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_015.py` & `vsg-3.9.0/vsg/rules/process/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_016.py` & `vsg-3.9.0/vsg/rules/process/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_017.py` & `vsg-3.9.0/vsg/rules/process/rule_017.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_018.py` & `vsg-3.9.0/vsg/rules/process/rule_018.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_019.py` & `vsg-3.9.0/vsg/rules/process/rule_019.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_020.py` & `vsg-3.9.0/vsg/rules/process/rule_020.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_021.py` & `vsg-3.9.0/vsg/rules/process/rule_021.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_022.py` & `vsg-3.9.0/vsg/rules/process/rule_022.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_023.py` & `vsg-3.9.0/vsg/rules/process/rule_023.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_024.py` & `vsg-3.9.0/vsg/rules/process/rule_024.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_025.py` & `vsg-3.9.0/vsg/rules/process/rule_025.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_026.py` & `vsg-3.9.0/vsg/rules/process/rule_026.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_027.py` & `vsg-3.9.0/vsg/rules/process/rule_027.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_028.py` & `vsg-3.9.0/vsg/rules/process/rule_028.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_029.py` & `vsg-3.9.0/vsg/rules/process/rule_029.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_030.py` & `vsg-3.9.0/vsg/rules/process/rule_030.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_031.py` & `vsg-3.9.0/vsg/rules/process/rule_031.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_032.py` & `vsg-3.9.0/vsg/rules/process/rule_032.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_033.py` & `vsg-3.9.0/vsg/rules/process/rule_033.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_034.py` & `vsg-3.9.0/vsg/rules/process/rule_034.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_035.py` & `vsg-3.9.0/vsg/rules/process/rule_035.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_036.py` & `vsg-3.9.0/vsg/rules/process/rule_036.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_400.py` & `vsg-3.9.0/vsg/rules/process/rule_400.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/process/rule_600.py` & `vsg-3.9.0/vsg/rules/process/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/ranges/rule_001.py` & `vsg-3.9.0/vsg/rules/ranges/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/ranges/rule_002.py` & `vsg-3.9.0/vsg/rules/ranges/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/remove_blank_lines_above_line_starting_with_token.py` & `vsg-3.9.0/vsg/rules/remove_blank_lines_above_line_starting_with_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/remove_carriage_return_after_token.py` & `vsg-3.9.0/vsg/rules/remove_carriage_return_after_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/remove_carriage_returns_between_token_pairs.py` & `vsg-3.9.0/vsg/rules/remove_carriage_returns_between_token_pairs.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/remove_comments_from_end_of_lines_bounded_by_tokens.py` & `vsg-3.9.0/vsg/rules/remove_comments_from_end_of_lines_bounded_by_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/remove_excessive_blank_lines_above_line_starting_with_token.py` & `vsg-3.9.0/vsg/rules/remove_excessive_blank_lines_above_line_starting_with_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/remove_excessive_blank_lines_below_line_ending_with_token.py` & `vsg-3.9.0/vsg/rules/remove_excessive_blank_lines_below_line_ending_with_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/remove_lines_starting_with_token_between_token_pairs.py` & `vsg-3.9.0/vsg/rules/remove_lines_starting_with_token_between_token_pairs.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/remove_spaces_before_token_rule.py` & `vsg-3.9.0/vsg/rules/remove_spaces_before_token_rule.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/remove_tokens.py` & `vsg-3.9.0/vsg/rules/remove_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/remove_tokens_bounded_by_tokens_and_remove_trailing_whitespace.py` & `vsg-3.9.0/vsg/rules/remove_tokens_bounded_by_tokens_and_remove_trailing_whitespace.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/report_statement/rule_001.py` & `vsg-3.9.0/vsg/rules/report_statement/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/report_statement/rule_002.py` & `vsg-3.9.0/vsg/rules/report_statement/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/report_statement/rule_100.py` & `vsg-3.9.0/vsg/rules/report_statement/rule_100.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/report_statement/rule_101.py` & `vsg-3.9.0/vsg/rules/report_statement/rule_101.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/report_statement/rule_300.py` & `vsg-3.9.0/vsg/rules/report_statement/rule_300.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/report_statement/rule_400.py` & `vsg-3.9.0/vsg/rules/report_statement/rule_400.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/report_statement/rule_500.py` & `vsg-3.9.0/vsg/rules/report_statement/rule_500.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/report_statement/rule_501.py` & `vsg-3.9.0/vsg/rules/report_statement/rule_501.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/separate_multiple_signal_identifiers_into_individual_statements.py` & `vsg-3.9.0/vsg/rules/separate_multiple_signal_identifiers_into_individual_statements.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/sequential/rule_001.py` & `vsg-3.9.0/vsg/rules/sequential/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/sequential/rule_002.py` & `vsg-3.9.0/vsg/rules/sequential/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/sequential/rule_003.py` & `vsg-3.9.0/vsg/rules/sequential/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/sequential/rule_004.py` & `vsg-3.9.0/vsg/rules/sequential/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/sequential/rule_006.py` & `vsg-3.9.0/vsg/rules/sequential/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/sequential/rule_007.py` & `vsg-3.9.0/vsg/rules/sequential/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_001.py` & `vsg-3.9.0/vsg/rules/signal/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_002.py` & `vsg-3.9.0/vsg/rules/signal/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_003.py` & `vsg-3.9.0/vsg/rules/signal/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_004.py` & `vsg-3.9.0/vsg/rules/signal/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_005.py` & `vsg-3.9.0/vsg/rules/signal/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_006.py` & `vsg-3.9.0/vsg/rules/signal/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_007.py` & `vsg-3.9.0/vsg/rules/signal/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_008.py` & `vsg-3.9.0/vsg/rules/signal/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_011.py` & `vsg-3.9.0/vsg/rules/signal/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_012.py` & `vsg-3.9.0/vsg/rules/signal/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_014.py` & `vsg-3.9.0/vsg/rules/signal/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_015.py` & `vsg-3.9.0/vsg/rules/signal/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_016.py` & `vsg-3.9.0/vsg/rules/signal/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/signal/rule_600.py` & `vsg-3.9.0/vsg/rules/signal/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/single_space_after_token.py` & `vsg-3.9.0/vsg/rules/single_space_after_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/single_space_before_token.py` & `vsg-3.9.0/vsg/rules/single_space_before_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/single_space_before_token_if_on_same_line_as_token.py` & `vsg-3.9.0/vsg/rules/single_space_before_token_if_on_same_line_as_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/single_space_between_token_pairs.py` & `vsg-3.9.0/vsg/rules/single_space_between_token_pairs.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/single_space_between_token_pairs_bounded_by_tokens.py` & `vsg-3.9.0/vsg/rules/single_space_between_token_pairs_bounded_by_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/single_space_between_tokens.py` & `vsg-3.9.0/vsg/rules/single_space_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/source_file/rule_001.py` & `vsg-3.9.0/vsg/rules/source_file/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/spaces_before_and_after_tokens_when_bounded_by_tokens.py` & `vsg-3.9.0/vsg/rules/spaces_before_and_after_tokens_when_bounded_by_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/split_line_at_token.py` & `vsg-3.9.0/vsg/rules/split_line_at_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/split_line_at_token_if_on_same_line_as_token_if_token_pair_are_not_on_the_same_line.py` & `vsg-3.9.0/vsg/rules/split_line_at_token_if_on_same_line_as_token_if_token_pair_are_not_on_the_same_line.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/split_line_at_token_when_between_tokens.py` & `vsg-3.9.0/vsg/rules/split_line_at_token_when_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/split_line_at_token_when_between_tokens_unless_token_is_found.py` & `vsg-3.9.0/vsg/rules/split_line_at_token_when_between_tokens_unless_token_is_found.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/subprogram_body/rule_201.py` & `vsg-3.9.0/vsg/rules/subprogram_body/rule_201.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/subprogram_body/rule_202.py` & `vsg-3.9.0/vsg/rules/subprogram_body/rule_202.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/subprogram_body/rule_203.py` & `vsg-3.9.0/vsg/rules/subprogram_body/rule_203.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/subprogram_body/rule_204.py` & `vsg-3.9.0/vsg/rules/variable_assignment/rule_006.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 
-from vsg.rules import blank_line_above_line_starting_with_token
-
+from vsg import parser
 from vsg import token
 
+from vsg.rules import remove_lines_starting_with_token_between_token_pairs
+
 lTokens = []
-lTokens.append(token.subprogram_body.end_keyword)
+lTokens.append([token.simple_variable_assignment.target, token.simple_variable_assignment.semicolon])
 
+oRemoveToken = parser.comment
 
-class rule_204(blank_line_above_line_starting_with_token):
-    '''
-    This rule checks for blank lines above the **end** keyword.
 
-    |configuring_blank_lines_link|
+class rule_006(remove_lines_starting_with_token_between_token_pairs):
+    '''
+    This rule checks for comments in multiline variable assignments.
 
     **Violation**
 
     .. code-block:: vhdl
 
-       begin
-
-         a <= b;
-       end function overflow;
+         counter := 1 + 4 + 10 + 25 +
+                    -- Add in more stuff
+                    30 + 35;
 
     **Fix**
 
     .. code-block:: vhdl
 
-       begin
-
-         a <= b;
-
-       end function overflow;
+         counter := 1 + 4 + 10 + 25 +
+                    30 + 35;
     '''
 
     def __init__(self):
-        blank_line_above_line_starting_with_token.__init__(self, 'subprogram_body', '204', lTokens)
+        remove_lines_starting_with_token_between_token_pairs.__init__(self, 'variable_assignment', '006', oRemoveToken, lTokens)
+        self.solution = 'Remove comments inside variable assignment'
+        self.fixable = False
```

### Comparing `vsg-3.8.0/vsg/rules/subprogram_body/rule_205.py` & `vsg-3.9.0/vsg/rules/subprogram_body/rule_205.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/subprogram_body/rule_400.py` & `vsg-3.9.0/vsg/rules/subprogram_body/rule_400.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/subtype/rule_001.py` & `vsg-3.9.0/vsg/rules/subtype/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/subtype/rule_002.py` & `vsg-3.9.0/vsg/rules/subtype/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/subtype/rule_003.py` & `vsg-3.9.0/vsg/rules/subtype/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/subtype/rule_004.py` & `vsg-3.9.0/vsg/rules/subtype/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/subtype/rule_600.py` & `vsg-3.9.0/vsg/rules/subtype/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_case.py` & `vsg-3.9.0/vsg/rules/token_case.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_case_formal_part_of_association_element_in_map_between_tokens.py` & `vsg-3.9.0/vsg/rules/token_case_formal_part_of_association_element_in_map_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_case_in_range_bounded_by_tokens.py` & `vsg-3.9.0/vsg/rules/token_case_in_range_bounded_by_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_case_in_range_bounded_by_tokens_with_prefix_suffix.py` & `vsg-3.9.0/vsg/rules/token_case_in_range_bounded_by_tokens_with_prefix_suffix.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_case_n_token_after_tokens.py` & `vsg-3.9.0/vsg/rules/token_case_n_token_after_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_case_n_token_after_tokens_between_tokens.py` & `vsg-3.9.0/vsg/rules/token_case_n_token_after_tokens_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_case_subtype_indication.py` & `vsg-3.9.0/vsg/rules/token_case_subtype_indication.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_case_with_prefix_suffix.py` & `vsg-3.9.0/vsg/rules/token_case_with_prefix_suffix.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_does_not_exist_before_token.py` & `vsg-3.9.0/vsg/rules/token_does_not_exist_before_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_indent.py` & `vsg-3.9.0/vsg/rules/token_indent.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_indent_between_tokens.py` & `vsg-3.9.0/vsg/rules/token_indent_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_indent_unless_between_tokens.py` & `vsg-3.9.0/vsg/rules/token_indent_unless_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_prefix.py` & `vsg-3.9.0/vsg/rules/token_prefix.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_prefix_between_tokens.py` & `vsg-3.9.0/vsg/rules/token_prefix_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_suffix.py` & `vsg-3.9.0/vsg/rules/token_suffix.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/token_suffix_between_tokens.py` & `vsg-3.9.0/vsg/rules/token_suffix_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/__init__.py` & `vsg-3.9.0/vsg/rules/entity/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,11 +11,31 @@
 from .rule_010 import rule_010
 from .rule_011 import rule_011
 from .rule_012 import rule_012
 from .rule_013 import rule_013
 from .rule_014 import rule_014
 from .rule_015 import rule_015
 from .rule_016 import rule_016
+from .rule_017 import rule_017
+from .rule_018 import rule_018
+from .rule_019 import rule_019
+from .rule_020 import rule_020
+from .rule_021 import rule_021
+from .rule_022 import rule_022
+from .rule_023 import rule_023
+from .rule_024 import rule_024
+from .rule_025 import rule_025
+from .rule_026 import rule_026
+from .rule_027 import rule_027
+from .rule_028 import rule_028
+from .rule_029 import rule_029
 
-from .rule_400 import rule_400
+from .rule_200 import rule_200
+from .rule_201 import rule_201
+from .rule_202 import rule_202
+from .rule_203 import rule_203
+
+from .rule_300 import rule_300
+
+from .rule_500 import rule_500
 
 from .rule_600 import rule_600
```

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_001.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_002.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_003.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_004.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_005.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_006.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_007.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_008.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_009.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_009.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_010.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_011.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_012.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_013.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_014.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_014.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_015.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_015.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_016.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_016.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_400.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_400.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/type_definition/rule_600.py` & `vsg-3.9.0/vsg/rules/type_definition/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/utils.py` & `vsg-3.9.0/vsg/rules/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 from vsg import parser
+from vsg import token
 
 from vsg.vhdlFile import utils
 
 
 def remove_optional_item(oViolation, oInsertToken):
     lTokens = oViolation.get_tokens()
     if isinstance(lTokens[0], parser.whitespace):
@@ -238,7 +239,35 @@
     lReturn = []
     for oToi in lToi:
         lTokens = oToi.get_tokens()
         if left_most_token_is_at_the_end_of_a_line(lTokens):
             continue
         lReturn.append(oToi)
     return lReturn
+
+
+def extract_identifiers_with_mode_of_input(lToi):
+    return extract_identifiers_with_mode(lToi, token.mode.in_keyword)
+
+
+def extract_identifiers_with_mode_of_out(lToi):
+    return extract_identifiers_with_mode(lToi, token.mode.out_keyword)
+
+
+def extract_identifiers_with_mode_of_inout(lToi):
+    return extract_identifiers_with_mode(lToi, token.mode.inout_keyword)
+
+
+def extract_identifiers_with_mode_of_buffer(lToi):
+    return extract_identifiers_with_mode(lToi, token.mode.buffer_keyword)
+
+
+def extract_identifiers_with_mode_of_linkage(lToi):
+    return extract_identifiers_with_mode(lToi, token.mode.linkage_keyword)
+
+
+def extract_identifiers_with_mode(lToi, oTokenType):
+    lReturn = []
+    for oToi in lToi:
+        if oToi.token_type_exists(oTokenType):
+            lReturn.append(oToi.extract_tokens(0, 0))
+    return lReturn
```

### Comparing `vsg-3.8.0/vsg/rules/variable/rule_001.py` & `vsg-3.9.0/vsg/rules/variable/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable/rule_002.py` & `vsg-3.9.0/vsg/rules/variable/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable/rule_003.py` & `vsg-3.9.0/vsg/rules/variable/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable/rule_004.py` & `vsg-3.9.0/vsg/rules/variable/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable/rule_005.py` & `vsg-3.9.0/vsg/rules/variable/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable/rule_006.py` & `vsg-3.9.0/vsg/rules/variable/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable/rule_007.py` & `vsg-3.9.0/vsg/rules/variable/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable/rule_010.py` & `vsg-3.9.0/vsg/rules/variable/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable/rule_011.py` & `vsg-3.9.0/vsg/rules/variable/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable/rule_012.py` & `vsg-3.9.0/vsg/rules/variable/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable/rule_600.py` & `vsg-3.9.0/vsg/rules/variable/rule_600.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable_assignment/rule_001.py` & `vsg-3.9.0/vsg/rules/variable_assignment/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable_assignment/rule_002.py` & `vsg-3.9.0/vsg/rules/variable_assignment/rule_002.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable_assignment/rule_003.py` & `vsg-3.9.0/vsg/rules/variable_assignment/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/variable_assignment/rule_004.py` & `vsg-3.9.0/vsg/rules/variable_assignment/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/wait/rule_001.py` & `vsg-3.9.0/vsg/rules/wait/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/when/rule_001.py` & `vsg-3.9.0/vsg/rules/when/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace/rule_001.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_200.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,62 @@
 
 from vsg import parser
 from vsg import violation
 
-from vsg.rule_group import whitespace
+from vsg.rule_group.blank_line import Rule
+from vsg.rules import utils
 
 
-class rule_001(whitespace.Rule):
+class rule_200(Rule):
     '''
-    This rule check for trailing spaces.
+    This rule removes consecutive blank lines.
 
     **Violation**
 
-    Where periods indicate spaces:
-
     .. code-block:: vhdl
 
-        library ieee;....
+       a <= b;
+
+
+       c <= d;
 
     **Fix**
 
     .. code-block:: vhdl
 
-        library ieee;
+       a <= b;
+
+       c <= d;
     '''
 
     def __init__(self):
-
-        whitespace.Rule.__init__(self, 'whitespace', '001')
-        self.phase = 1
-        self.subphase = 0
-        self.solution = 'Remove trailing whitespace'
+        Rule.__init__(self, name='whitespace', identifier='200')
+        self.blank_lines_allowed = 1
+        self.configuration.append('blank_lines_allowed')
 
     def _get_tokens_of_interest(self, oFile):
-        return oFile.get_n_tokens_before_token(2, [parser.carriage_return])
+        lToi = oFile.get_consecutive_lines_starting_with_token(parser.blank_line)
+        lReturn = []
+        for oToi in lToi:
+            lTokens = oToi.get_tokens()
+            if len(lTokens) > ((self.blank_lines_allowed * 2) - 1):
+                lReturn.append(oToi)
+        return lReturn
 
     def _analyze(self, lToi):
         for oToi in lToi:
-            if whitespace_exists(oToi):
-                create_violation(oToi, self)
+            lTokens = oToi.get_tokens()
+            iBlankLines = utils.number_of_tokens_in_token_list(parser.blank_line, lTokens)
+
+            if iBlankLines > self.blank_lines_allowed:
+                sSolution = f'Remove {iBlankLines - self.blank_lines_allowed}'
+                oViolation = violation.New(oToi.get_line_number(), oToi, sSolution)
+                dAction = {}
+                dAction['remove_index'] = len(lTokens) - (iBlankLines - self.blank_lines_allowed) * 2
+                oViolation.set_action(dAction)
+                self.add_violation(oViolation)
 
     def _fix_violation(self, oViolation):
+        lTokens = oViolation.get_tokens()
         dAction = oViolation.get_action()
-        if need_to_remove_whitespace(dAction):
-            remove_whitespace(oViolation)
-        else:
-            remove_whitespace_and_insert_blank_line(oViolation)
-
-
-def create_violation(oToi, self):
-    lTokens = oToi.get_tokens()
-    oViolation = violation.New(oToi.get_line_number(), oToi, self.solution)
-    dAction = define_action(lTokens)
-    oViolation.set_action(dAction)
-    self.add_violation(oViolation)
-
-
-def whitespace_exists(oToi):
-    lTokens = oToi.get_tokens()
-    if isinstance(lTokens[1], parser.whitespace):
-        return True
-    return False
-
-
-def define_action(lTokens):
-    dAction = {}
-    if isinstance(lTokens[0], parser.carriage_return):
-        dAction['action'] = 'insert_blank_line'
-    else:
-        dAction['action'] = 'remove'
-    return dAction
-
-
-def need_to_remove_whitespace(dAction):
-    if dAction['action'] == 'remove':
-        return True
-    return False
-
-
-def remove_whitespace(oViolation):
-    lTokens = oViolation.get_tokens()
-    myTokens = []
-    myTokens.append(lTokens[0])
-    myTokens.append(lTokens[-1])
-    oViolation.set_tokens(myTokens)
-
-
-def remove_whitespace_and_insert_blank_line(oViolation):
-    lTokens = oViolation.get_tokens()
-    myTokens = []
-    myTokens.append(lTokens[0])
-    myTokens.append(parser.blank_line())
-    myTokens.append(lTokens[-1])
-    oViolation.set_tokens(myTokens)
+        lNewTokens = lTokens[0:dAction['remove_index']]
+        oViolation.set_tokens(lNewTokens)
```

### Comparing `vsg-3.8.0/vsg/rules/whitespace/rule_003.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_003.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace/rule_004.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_004.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace/rule_005.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_005.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace/rule_006.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_006.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace/rule_007.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_007.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace/rule_008.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_008.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace/rule_010.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_010.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace/rule_011.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_011.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace/rule_012.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_012.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace/rule_013.py` & `vsg-3.9.0/vsg/rules/whitespace/rule_013.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace_before_token.py` & `vsg-3.9.0/vsg/rules/whitespace_before_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/whitespace_before_tokens_in_between_tokens.py` & `vsg-3.9.0/vsg/rules/whitespace_before_tokens_in_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/rules/with_statement/rule_001.py` & `vsg-3.9.0/vsg/rules/with_statement/rule_001.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/severity.py` & `vsg-3.9.0/vsg/severity.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/styles/jcl.yaml` & `vsg-3.9.0/vsg/styles/jcl.yaml`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/adding_operator.py` & `vsg-3.9.0/vsg/token/adding_operator.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/alias_declaration.py` & `vsg-3.9.0/vsg/token/alias_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/architecture_body.py` & `vsg-3.9.0/vsg/token/architecture_body.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/assertion.py` & `vsg-3.9.0/vsg/token/assertion.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/assertion_statement.py` & `vsg-3.9.0/vsg/token/assertion_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/association_element.py` & `vsg-3.9.0/vsg/token/association_element.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/attribute_declaration.py` & `vsg-3.9.0/vsg/token/attribute_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/attribute_specification.py` & `vsg-3.9.0/vsg/token/attribute_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/block_statement.py` & `vsg-3.9.0/vsg/token/block_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/case_generate_alternative.py` & `vsg-3.9.0/vsg/token/case_generate_alternative.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/case_generate_statement.py` & `vsg-3.9.0/vsg/token/case_generate_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/case_statement.py` & `vsg-3.9.0/vsg/token/case_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/case_statement_alternative.py` & `vsg-3.9.0/vsg/token/case_statement_alternative.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/component.py` & `vsg-3.9.0/vsg/token/component.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/component_declaration.py` & `vsg-3.9.0/vsg/token/component_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/component_instantiation_statement.py` & `vsg-3.9.0/vsg/token/component_instantiation_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/concurrent_assertion_statement.py` & `vsg-3.9.0/vsg/token/concurrent_assertion_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/concurrent_conditional_signal_assignment.py` & `vsg-3.9.0/vsg/token/concurrent_conditional_signal_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/concurrent_procedure_call_statement.py` & `vsg-3.9.0/vsg/token/concurrent_procedure_call_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/concurrent_selected_signal_assignment.py` & `vsg-3.9.0/vsg/token/concurrent_selected_signal_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/concurrent_signal_assignment_statement.py` & `vsg-3.9.0/vsg/token/concurrent_signal_assignment_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/concurrent_simple_signal_assignment.py` & `vsg-3.9.0/vsg/token/concurrent_simple_signal_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/conditional_force_assignment.py` & `vsg-3.9.0/vsg/token/conditional_force_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/conditional_variable_assignment.py` & `vsg-3.9.0/vsg/token/conditional_variable_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/conditional_waveform_assignment.py` & `vsg-3.9.0/vsg/token/conditional_waveform_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/conditional_waveforms.py` & `vsg-3.9.0/vsg/token/conditional_waveforms.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/configuration_declaration.py` & `vsg-3.9.0/vsg/token/configuration_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/constant_declaration.py` & `vsg-3.9.0/vsg/token/constant_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/context_declaration.py` & `vsg-3.9.0/vsg/token/context_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/context_reference.py` & `vsg-3.9.0/vsg/token/context_reference.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/delay_mechanism.py` & `vsg-3.9.0/vsg/token/delay_mechanism.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/entity.py` & `vsg-3.9.0/vsg/token/entity.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/entity_aspect.py` & `vsg-3.9.0/vsg/token/entity_aspect.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/entity_declaration.py` & `vsg-3.9.0/vsg/token/entity_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/entity_name_list.py` & `vsg-3.9.0/vsg/token/entity_name_list.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/enumeration_type_definition.py` & `vsg-3.9.0/vsg/token/enumeration_type_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/exit_statement.py` & `vsg-3.9.0/vsg/token/exit_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/file_declaration.py` & `vsg-3.9.0/vsg/token/file_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/file_open_information.py` & `vsg-3.9.0/vsg/token/file_open_information.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/for_generate_statement.py` & `vsg-3.9.0/vsg/token/for_generate_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/full_type_declaration.py` & `vsg-3.9.0/vsg/token/full_type_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/function_specification.py` & `vsg-3.9.0/vsg/token/function_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/generate_statement_body.py` & `vsg-3.9.0/vsg/token/generate_statement_body.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/generic_clause.py` & `vsg-3.9.0/vsg/token/generic_clause.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/generic_map_aspect.py` & `vsg-3.9.0/vsg/token/generic_map_aspect.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/group_declaration.py` & `vsg-3.9.0/vsg/token/group_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/ieee/std_logic_1164/types.py` & `vsg-3.9.0/vsg/token/ieee/std_logic_1164/types.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/if_generate_statement.py` & `vsg-3.9.0/vsg/token/if_generate_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/if_statement.py` & `vsg-3.9.0/vsg/token/if_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/incomplete_type_declaration.py` & `vsg-3.9.0/vsg/token/incomplete_type_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/index_constraint.py` & `vsg-3.9.0/vsg/token/index_constraint.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/instantiated_unit.py` & `vsg-3.9.0/vsg/token/instantiated_unit.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/instantiation_list.py` & `vsg-3.9.0/vsg/token/instantiation_list.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/interface_constant_declaration.py` & `vsg-3.9.0/vsg/token/interface_constant_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/interface_file_declaration.py` & `vsg-3.9.0/vsg/token/interface_file_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/interface_function_specification.py` & `vsg-3.9.0/vsg/token/interface_function_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/interface_package_declaration.py` & `vsg-3.9.0/vsg/token/interface_package_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/interface_package_generic_map_aspect.py` & `vsg-3.9.0/vsg/token/interface_package_generic_map_aspect.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/interface_procedure_specification.py` & `vsg-3.9.0/vsg/token/interface_procedure_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/interface_signal_declaration.py` & `vsg-3.9.0/vsg/token/interface_signal_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/interface_unknown_declaration.py` & `vsg-3.9.0/vsg/token/interface_unknown_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/interface_variable_declaration.py` & `vsg-3.9.0/vsg/token/interface_variable_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/logical_operator.py` & `vsg-3.9.0/vsg/token/logical_operator.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/loop_statement.py` & `vsg-3.9.0/vsg/token/loop_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/miscellaneous_operator.py` & `vsg-3.9.0/vsg/token/miscellaneous_operator.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/mode.py` & `vsg-3.9.0/vsg/token/mode.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/multiplying_operator.py` & `vsg-3.9.0/vsg/token/multiplying_operator.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/next_statement.py` & `vsg-3.9.0/vsg/token/next_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/null_statement.py` & `vsg-3.9.0/vsg/token/null_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/package_body.py` & `vsg-3.9.0/vsg/token/package_body.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/package_declaration.py` & `vsg-3.9.0/vsg/token/package_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/package_instantiation_declaration.py` & `vsg-3.9.0/vsg/token/package_instantiation_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/physical_type_definition.py` & `vsg-3.9.0/vsg/token/physical_type_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/port_clause.py` & `vsg-3.9.0/vsg/token/port_clause.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/port_map_aspect.py` & `vsg-3.9.0/vsg/token/port_map_aspect.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/procedure_call.py` & `vsg-3.9.0/vsg/token/procedure_call.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/procedure_call_statement.py` & `vsg-3.9.0/vsg/token/procedure_call_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/procedure_specification.py` & `vsg-3.9.0/vsg/token/procedure_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/process_statement.py` & `vsg-3.9.0/vsg/token/process_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/protected_type_body.py` & `vsg-3.9.0/vsg/token/protected_type_body.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/protected_type_declaration.py` & `vsg-3.9.0/vsg/token/protected_type_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/record_type_definition.py` & `vsg-3.9.0/vsg/token/record_type_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/relational_operator.py` & `vsg-3.9.0/vsg/token/relational_operator.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/report_statement.py` & `vsg-3.9.0/vsg/token/report_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/return_statement.py` & `vsg-3.9.0/vsg/token/return_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/secondary_unit_declaration.py` & `vsg-3.9.0/vsg/token/secondary_unit_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/selected_force_assignment.py` & `vsg-3.9.0/vsg/token/selected_force_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/selected_variable_assignment.py` & `vsg-3.9.0/vsg/token/selected_variable_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/selected_waveform_assignment.py` & `vsg-3.9.0/vsg/token/selected_waveform_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/shared_variable_declaration.py` & `vsg-3.9.0/vsg/token/shared_variable_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/shift_operator.py` & `vsg-3.9.0/vsg/token/shift_operator.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/signal_declaration.py` & `vsg-3.9.0/vsg/token/signal_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/signature.py` & `vsg-3.9.0/vsg/token/signature.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/simple_configuration_specification.py` & `vsg-3.9.0/vsg/token/simple_configuration_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/simple_force_assignment.py` & `vsg-3.9.0/vsg/token/simple_force_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/simple_release_assignment.py` & `vsg-3.9.0/vsg/token/simple_release_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/simple_variable_assignment.py` & `vsg-3.9.0/vsg/token/simple_variable_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/simple_waveform_assignment.py` & `vsg-3.9.0/vsg/token/simple_waveform_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/subprogram_body.py` & `vsg-3.9.0/vsg/token/subprogram_body.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/subprogram_header.py` & `vsg-3.9.0/vsg/token/subprogram_header.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/subprogram_instantiation_declaration.py` & `vsg-3.9.0/vsg/token/subprogram_instantiation_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/subtype_declaration.py` & `vsg-3.9.0/vsg/token/subtype_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/type_declaration.py` & `vsg-3.9.0/vsg/token/type_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/unary_logical_operator.py` & `vsg-3.9.0/vsg/token/unary_logical_operator.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/unbounded_array_definition.py` & `vsg-3.9.0/vsg/token/unbounded_array_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/use_clause.py` & `vsg-3.9.0/vsg/token/use_clause.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/variable_declaration.py` & `vsg-3.9.0/vsg/token/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token/wait_statement.py` & `vsg-3.9.0/vsg/token/wait_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/token_map.py` & `vsg-3.9.0/vsg/token_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,17 @@
             return True
         return False
 
     def pretty_print(self):
         pp=pprint.PrettyPrinter(indent=4)
         pp.pprint(self.dMap)
 
+    def get_index_of_line(self, iLine):
+        return(self.dMap['parser']['carriage_return'][iLine - 2] + 1)
+
 
 def extract_unique_id(oToken):
     lDoc = oToken.__doc__.split()
     for iDoc, sDoc in enumerate(lDoc):
         if sDoc == 'unique_id':
             return lDoc[iDoc + 2], lDoc[iDoc + 4]
     return None, None
```

### Comparing `vsg-3.8.0/vsg/tokens.py` & `vsg-3.9.0/vsg/tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/utils.py` & `vsg-3.9.0/vsg/utils.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/version.py` & `vsg-3.9.0/vsg/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import subprocess
 import os
 
-sVersion = '3.8.0'
+sVersion = '3.9.0'
 
 try:
     from vsg import version_info
     try:
         sVersion = version_info.sVersion
     except AttributeError:
         pass
```

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/access_type_definition.py` & `vsg-3.9.0/vsg/vhdlFile/classify/access_type_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/alias_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/alias_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/architecture_body.py` & `vsg-3.9.0/vsg/vhdlFile/classify/architecture_body.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/array_type_definition.py` & `vsg-3.9.0/vsg/vhdlFile/classify/array_type_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/assertion.py` & `vsg-3.9.0/vsg/vhdlFile/classify/assertion.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/assertion_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/assertion_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/association_element.py` & `vsg-3.9.0/vsg/vhdlFile/classify/association_element.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/association_list.py` & `vsg-3.9.0/vsg/vhdlFile/classify/association_list.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/attribute_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/attribute_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/attribute_specification.py` & `vsg-3.9.0/vsg/vhdlFile/classify/attribute_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/binding_indication.py` & `vsg-3.9.0/vsg/vhdlFile/classify/binding_indication.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/block_declarative_item.py` & `vsg-3.9.0/vsg/vhdlFile/classify/block_declarative_item.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/block_header.py` & `vsg-3.9.0/vsg/vhdlFile/classify/block_header.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/block_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/block_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/case_generate_alternative.py` & `vsg-3.9.0/vsg/vhdlFile/classify/case_generate_alternative.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/case_generate_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/case_generate_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/case_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/case_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/case_statement_alternative.py` & `vsg-3.9.0/vsg/vhdlFile/classify/case_statement_alternative.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/choice.py` & `vsg-3.9.0/vsg/vhdlFile/classify/choice.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/choices.py` & `vsg-3.9.0/vsg/vhdlFile/classify/choices.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/component_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/component_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/component_instantiation_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/component_instantiation_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/component_specification.py` & `vsg-3.9.0/vsg/vhdlFile/classify/component_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/concurrent_assertion_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/concurrent_assertion_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/concurrent_conditional_signal_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/concurrent_conditional_signal_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/concurrent_procedure_call_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/concurrent_procedure_call_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/concurrent_selected_signal_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/concurrent_selected_signal_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/concurrent_signal_assignment_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/concurrent_signal_assignment_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/concurrent_simple_signal_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/concurrent_simple_signal_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/concurrent_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/concurrent_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/condition_clause.py` & `vsg-3.9.0/vsg/vhdlFile/classify/condition_clause.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/conditional_expressions.py` & `vsg-3.9.0/vsg/vhdlFile/classify/conditional_expressions.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/conditional_force_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/conditional_force_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/conditional_signal_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/conditional_signal_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/conditional_variable_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/conditional_variable_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/conditional_waveform_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/conditional_waveform_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/conditional_waveforms.py` & `vsg-3.9.0/vsg/vhdlFile/classify/conditional_waveforms.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/configuration_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/configuration_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/configuration_declarative_item.py` & `vsg-3.9.0/vsg/vhdlFile/classify/configuration_declarative_item.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/constant_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/constant_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/constrained_array_definition.py` & `vsg-3.9.0/vsg/vhdlFile/classify/constrained_array_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/context_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/context_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/context_item.py` & `vsg-3.9.0/vsg/vhdlFile/classify/context_item.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/context_reference.py` & `vsg-3.9.0/vsg/vhdlFile/classify/context_reference.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/delay_mechanism.py` & `vsg-3.9.0/vsg/vhdlFile/classify/delay_mechanism.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/discrete_range.py` & `vsg-3.9.0/vsg/vhdlFile/classify/discrete_range.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/element_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/element_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/entity_aspect.py` & `vsg-3.9.0/vsg/vhdlFile/classify/entity_aspect.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/entity_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/entity_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/entity_declarative_item.py` & `vsg-3.9.0/vsg/vhdlFile/classify/entity_declarative_item.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/entity_name_list.py` & `vsg-3.9.0/vsg/vhdlFile/classify/entity_name_list.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/entity_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/entity_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/enumeration_type_definition.py` & `vsg-3.9.0/vsg/vhdlFile/classify/enumeration_type_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/exit_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/exit_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/expression.py` & `vsg-3.9.0/vsg/vhdlFile/classify/expression.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/file_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/file_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/file_open_information.py` & `vsg-3.9.0/vsg/vhdlFile/classify/file_open_information.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/file_type_definition.py` & `vsg-3.9.0/vsg/vhdlFile/classify/file_type_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/for_generate_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/for_generate_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/full_type_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/full_type_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/function_specification.py` & `vsg-3.9.0/vsg/vhdlFile/classify/function_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/generate_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/generate_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/generate_statement_body.py` & `vsg-3.9.0/vsg/vhdlFile/classify/generate_statement_body.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/generic_clause.py` & `vsg-3.9.0/vsg/vhdlFile/classify/generic_clause.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/generic_map_aspect.py` & `vsg-3.9.0/vsg/vhdlFile/classify/generic_map_aspect.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/group_constituent_list.py` & `vsg-3.9.0/vsg/vhdlFile/classify/group_constituent_list.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/group_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/group_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/identifier_list.py` & `vsg-3.9.0/vsg/vhdlFile/classify/identifier_list.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/if_generate_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/if_generate_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/if_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/if_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/incomplete_type_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/incomplete_type_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/index_constraint.py` & `vsg-3.9.0/vsg/vhdlFile/classify/index_constraint.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/index_subtype_definition.py` & `vsg-3.9.0/vsg/vhdlFile/classify/index_subtype_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/instantiated_unit.py` & `vsg-3.9.0/vsg/vhdlFile/classify/instantiated_unit.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/instantiation_list.py` & `vsg-3.9.0/vsg/vhdlFile/classify/instantiation_list.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_constant_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_constant_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_file_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_file_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_function_specification.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_function_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_incomplete_type_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_incomplete_type_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_list.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_list.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_object_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_object_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_package_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_package_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_package_generic_map_aspect.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_package_generic_map_aspect.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_procedure_specification.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_procedure_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_signal_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_signal_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_subprogram_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_subprogram_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_subprogram_specification.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_subprogram_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_unknown_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_unknown_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/interface_variable_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/interface_variable_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/iteration_scheme.py` & `vsg-3.9.0/vsg/vhdlFile/classify/iteration_scheme.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/library_clause.py` & `vsg-3.9.0/vsg/vhdlFile/classify/library_clause.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/logical_name_list.py` & `vsg-3.9.0/vsg/vhdlFile/classify/logical_name_list.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/loop_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/loop_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/mode.py` & `vsg-3.9.0/vsg/vhdlFile/classify/mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     mode ::=
         in | out | inout | buffer | linkage
     '''
 
     iCurrent = utils.assign_next_token_if('in', token.in_keyword, iToken, lObjects)
     iCurrent = utils.assign_next_token_if('out', token.out_keyword, iCurrent, lObjects)
     iCurrent = utils.assign_next_token_if('inout', token.inout_keyword, iCurrent, lObjects)
-    iCurrent = utils.assign_next_token_if('buffer', token.inout_keyword, iCurrent, lObjects)
-    iCurrent = utils.assign_next_token_if('linkage', token.inout_keyword, iCurrent, lObjects)
+    iCurrent = utils.assign_next_token_if('buffer', token.buffer_keyword, iCurrent, lObjects)
+    iCurrent = utils.assign_next_token_if('linkage', token.linkage_keyword, iCurrent, lObjects)
 
     return iCurrent
```

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/name.py` & `vsg-3.9.0/vsg/vhdlFile/classify/name.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/next_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/next_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/null_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/null_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/package_body.py` & `vsg-3.9.0/vsg/vhdlFile/classify/package_body.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/package_body_declarative_item.py` & `vsg-3.9.0/vsg/vhdlFile/classify/package_body_declarative_item.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/package_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/package_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/package_declarative_item.py` & `vsg-3.9.0/vsg/vhdlFile/classify/package_declarative_item.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/package_header.py` & `vsg-3.9.0/vsg/vhdlFile/classify/package_header.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/package_instantiation_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/package_instantiation_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/parameter_specification.py` & `vsg-3.9.0/vsg/vhdlFile/classify/parameter_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/physical_type_definition.py` & `vsg-3.9.0/vsg/vhdlFile/classify/physical_type_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/port_clause.py` & `vsg-3.9.0/vsg/vhdlFile/classify/port_clause.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/port_map_aspect.py` & `vsg-3.9.0/vsg/vhdlFile/classify/port_map_aspect.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/primary_unit.py` & `vsg-3.9.0/vsg/vhdlFile/classify/primary_unit.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/procedure_call.py` & `vsg-3.9.0/vsg/vhdlFile/classify/procedure_call.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/procedure_call_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/procedure_call_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/procedure_specification.py` & `vsg-3.9.0/vsg/vhdlFile/classify/procedure_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/process_declarative_item.py` & `vsg-3.9.0/vsg/vhdlFile/classify/process_declarative_item.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/process_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/process_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/protected_type_body.py` & `vsg-3.9.0/vsg/vhdlFile/classify/protected_type_body.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/protected_type_body_declarative_item.py` & `vsg-3.9.0/vsg/vhdlFile/classify/protected_type_body_declarative_item.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/protected_type_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/protected_type_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/protected_type_declarative_item.py` & `vsg-3.9.0/vsg/vhdlFile/classify/protected_type_declarative_item.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/range_constraint.py` & `vsg-3.9.0/vsg/vhdlFile/classify/range_constraint.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/record_type_definition.py` & `vsg-3.9.0/vsg/vhdlFile/classify/record_type_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/report_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/report_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/return_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/return_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/scalar_type_definition.py` & `vsg-3.9.0/vsg/vhdlFile/classify/scalar_type_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/secondary_unit_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/secondary_unit_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/selected_expressions.py` & `vsg-3.9.0/vsg/vhdlFile/classify/selected_expressions.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/selected_force_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/selected_force_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/selected_signal_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/selected_signal_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/selected_variable_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/selected_variable_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/selected_waveform_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/selected_waveform_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/selected_waveforms.py` & `vsg-3.9.0/vsg/vhdlFile/classify/selected_waveforms.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/sensitivity_clause.py` & `vsg-3.9.0/vsg/vhdlFile/classify/sensitivity_clause.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/sensitivity_list.py` & `vsg-3.9.0/vsg/vhdlFile/classify/sensitivity_list.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/sequential_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/sequential_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/signal_assignment_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/signal_assignment_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/signal_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/signal_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/signal_kind.py` & `vsg-3.9.0/vsg/vhdlFile/classify/signal_kind.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/signature.py` & `vsg-3.9.0/vsg/vhdlFile/classify/signature.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/simple_configuration_specification.py` & `vsg-3.9.0/vsg/vhdlFile/classify/simple_configuration_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/simple_force_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/simple_force_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/simple_release_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/simple_release_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/simple_signal_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/simple_signal_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/simple_variable_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/simple_variable_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/simple_waveform_assignment.py` & `vsg-3.9.0/vsg/vhdlFile/classify/simple_waveform_assignment.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/subprogram_body.py` & `vsg-3.9.0/vsg/vhdlFile/classify/subprogram_body.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/subprogram_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/subprogram_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/subprogram_declarative_item.py` & `vsg-3.9.0/vsg/vhdlFile/classify/subprogram_declarative_item.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/subprogram_header.py` & `vsg-3.9.0/vsg/vhdlFile/classify/subprogram_header.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/subprogram_instantiation_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/subprogram_instantiation_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/subprogram_kind.py` & `vsg-3.9.0/vsg/vhdlFile/classify/subprogram_kind.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/subprogram_specification.py` & `vsg-3.9.0/vsg/vhdlFile/classify/subprogram_specification.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/subtype_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/subtype_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/subtype_indication.py` & `vsg-3.9.0/vsg/vhdlFile/classify/subtype_indication.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/timeout_clause.py` & `vsg-3.9.0/vsg/vhdlFile/classify/timeout_clause.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/type_definition.py` & `vsg-3.9.0/vsg/vhdlFile/classify/type_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/unbounded_array_definition.py` & `vsg-3.9.0/vsg/vhdlFile/classify/unbounded_array_definition.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/use_clause.py` & `vsg-3.9.0/vsg/vhdlFile/classify/use_clause.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/variable_assignment_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/variable_assignment_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/variable_declaration.py` & `vsg-3.9.0/vsg/vhdlFile/classify/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/wait_statement.py` & `vsg-3.9.0/vsg/vhdlFile/classify/wait_statement.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/waveform.py` & `vsg-3.9.0/vsg/vhdlFile/classify/waveform.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/waveform_element.py` & `vsg-3.9.0/vsg/vhdlFile/classify/waveform_element.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/classify/whitespace.py` & `vsg-3.9.0/vsg/vhdlFile/classify/whitespace.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/code_tags.py` & `vsg-3.9.0/vsg/vhdlFile/code_tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
           if sValue.startswith('-- vsg_on'):
               lValues = sValue.split()
               if len(lValues) == 2:
                   self.clear()
               else:
                  for sCodeTag in lValues[2:]:
                      self.remove(sCodeTag)
+              return True
           elif sValue.startswith('-- vsg_off'):
               lValues = sValue.split()
               if len(lValues) == 2:
                   self.clear()
                   self.add('all')
               else:
                  for sCodeTag in lValues[2:]:
@@ -54,7 +55,8 @@
               self.bIgnoreNextCarriageReturn = True
       elif isinstance(oToken, parser.carriage_return):
           self.iLine += 1
           if self.bIgnoreNextCarriageReturn:
               self.bIgnoreNextCarriageReturn = False
           else:
               self.next_line_code_tags.clear()
+      return False
```

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/__init__.py` & `vsg-3.9.0/vsg/vhdlFile/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_association_elements_between_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_association_elements_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_blank_lines_below_line_ending_with_several_possible_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_blank_lines_below_line_ending_with_several_possible_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_blank_lines_below_line_ending_with_token.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_blank_lines_below_line_ending_with_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_consecutive_lines_starting_with_token.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_line_preceeding_line.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,65 @@
 
-from vsg.vhdlFile.extract import tokens
-from vsg.vhdlFile.extract import utils
+from vsg import parser
 
+from vsg.vhdlFile.extract import tokens
 
-def get_consecutive_lines_starting_with_token(search_token, min_num_lines, lAllTokens, oTokenMap):
+import bisect
 
-    lReturn = []
-    lSearchIndexes = utils.filter_tokens_which_start_a_line(search_token, oTokenMap)
 
-    lSearchLines = []
-    for iSearchIndex in lSearchIndexes:
-        lSearchLines.append(oTokenMap.get_line_number_of_index(iSearchIndex))
+def get_line_preceeding_line(iLine, lAllTokens, iNumLines, oTokenMap, bSkipComments=False):
 
-    iStart = None
-    for iIndex, iLine in enumerate(lSearchLines):
+    lCarriageReturns = oTokenMap.get_token_indexes(parser.carriage_return)
 
-        if iStart is None:
-            iStart = iLine
-            iStartLine = iLine
-            iStartIndex = iIndex
-            iCurrent = iLine
+    if not bSkipComments:
+        iAdjust = -2
+        iStartIndex = iLine - iNumLines + iAdjust
+        if iStartIndex < 0:
+            iStart = 0
+        else:
+            iStart = lCarriageReturns[iStartIndex] + 1
+        iEnd = lCarriageReturns[iLine + iAdjust]
+        lTemp = lAllTokens[iStart:iEnd]
+    #    print(f'{iLine} | {iStart} | {iEnd} | {lTemp}')
+        return tokens.New(iStart, iLine, lTemp)
+    else:
+
+        iStartIndex = _get_start_index(lCarriageReturns, iLine, oTokenMap)
+
+        if iStartIndex == 0:
+            iTokenStartIndex = 0
+            iTokenEndIndex = lCarriageReturns[iTokenStartIndex]
         else:
-            if iLine == iCurrent + 1:
-                iCurrent = iLine
-                iEndIndex = iIndex
-            else:
-                if lSearchLines[iIndex - 1] - iStartLine >= min_num_lines - 1:
-                    iStartToken = oTokenMap.get_index_of_carriage_return_before_index(lSearchIndexes[iStartIndex]) + 1
-                    iEndToken = oTokenMap.get_index_of_carriage_return_after_index(lSearchIndexes[iEndIndex])
-                    lTemp = lAllTokens[iStartToken:iEndToken]
-                    lReturn.append(tokens.New(iStartToken, iStartLine, lTemp))
-                iStart = iLine
-                iStartLine = iLine
-                iStartIndex = iIndex
-                iCurrent = iLine
-
-    if lSearchLines[iIndex - 1] - iStartLine >= min_num_lines - 1:
-        iStartToken = oTokenMap.get_index_of_carriage_return_before_index(lSearchIndexes[iStartIndex]) + 1
-        iEndToken = oTokenMap.get_index_of_carriage_return_after_index(lSearchIndexes[iEndIndex])
-        lTemp = lAllTokens[iStartToken:iEndToken]
-        lReturn.append(tokens.New(iStartToken, iStartLine, lTemp))
+            iTokenStartIndex = lCarriageReturns[iStartIndex - 1] + 1
+            iTokenEndIndex = lCarriageReturns[iStartIndex]
 
-    return lReturn
+        iLine = iStartIndex + 2
+        lTokens = lAllTokens[iTokenStartIndex:iTokenEndIndex]
+        return tokens.New(iTokenStartIndex, iLine, lTokens)
+
+
+def _build_index_list(oTokenMap):
+        lTemp = oTokenMap.get_token_indexes(parser.comment).copy()
+        lTemp.extend(oTokenMap.get_token_indexes(parser.whitespace).copy())
+        lTemp.extend(oTokenMap.get_token_indexes(parser.carriage_return).copy())
+        lTemp.sort()
+        return lTemp
+
+
+def _get_start_index(lCarriageReturns, iLine, oTokenMap):
+        lTemp = _build_index_list(oTokenMap)
+        iCurrent = lCarriageReturns[iLine - 2]
+#        print(f'lCarraigeReturns = {lCarriageReturns}')
+#        print(f'Index = {iCurrent}')
+#        print(f'lTemp            = {lTemp}')
+        iTempIndex = lTemp.index(iCurrent) - 1
+#        print(f'iTempIndex = {iTempIndex}')
+        for i in range(iTempIndex, -1, -1):
+#            print(i)
+#            print(f'lTemp[i] | {iCurrent - 1}')
+            if lTemp[i] != iCurrent - 1:
+                break
+            iCurrent = lTemp[i]
+#        print(f'iCurrent = {iCurrent}')
+#        iStartIndex = lCarriageReturns.index(iCurrent)
+        iStartIndex = bisect.bisect_left(lCarriageReturns, iCurrent)
+        return iStartIndex
```

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_consecutive_lines_starting_with_token_and_stopping_when_token_starting_line_is_found.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_consecutive_lines_starting_with_token_and_stopping_when_token_starting_line_is_found.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_if_statement_conditions.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_if_statement_conditions.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_interface_elements_between_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_interface_elements_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_line_above_line_starting_with_token.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_line_above_line_starting_with_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_line_above_line_starting_with_token_with_hierarchy.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_line_above_line_starting_with_token_with_hierarchy.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_several_possible_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_several_possible_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_token.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_token_with_hierarchy.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_line_below_line_ending_with_token_with_hierarchy.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_line_count_between_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_line_count_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_line_which_includes_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_line_which_includes_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_lines_with_length_that_exceed_column.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_lines_with_length_that_exceed_column.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_m_tokens_before_and_n_tokens_after_token.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_m_tokens_before_and_n_tokens_after_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_n_token_after_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_n_token_after_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_n_token_after_tokens_between_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_n_token_after_tokens_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_n_tokens_before_and_after_tokens_bounded_by_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_n_tokens_before_and_after_tokens_bounded_by_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_sequence_of_tokens_matching.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_sequence_of_tokens_matching.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_sequence_of_tokens_matching_bounded_by_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_sequence_of_tokens_matching_bounded_by_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_sequence_of_tokens_not_matching.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_sequence_of_tokens_not_matching.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_token_and_n_tokens_after_it_when_between_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_token_and_n_tokens_after_it_when_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_token_and_n_tokens_before_it_in_between_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_token_and_n_tokens_before_it_in_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_token_and_n_tokens_before_it_in_between_tokens_unless_token_is_found.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_token_and_n_tokens_before_it_in_between_tokens_unless_token_is_found.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching_between_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching_unless_between_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_at_beginning_of_line_matching_unless_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_between_non_whitespace_token_and_token.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_between_non_whitespace_token_and_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_between_tokens_inclusive_while_storing_value_from_token.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_between_tokens_inclusive_while_storing_value_from_token.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_bounded_by.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_bounded_by.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_bounded_by_token_when_between_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_bounded_by_token_when_between_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_bounded_by_tokens_if_token_is_between_them.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_bounded_by_tokens_if_token_is_between_them.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_bounded_by_unless_between.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_bounded_by_unless_between.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_matching_in_range_bounded_by_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_matching_in_range_bounded_by_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_starting_with_token_and_ending_with_one_of_possible_tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_starting_with_token_and_ending_with_one_of_possible_tokens.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/get_tokens_where_line_starts_with_token_until_ending_token_is_found.py` & `vsg-3.9.0/vsg/vhdlFile/extract/get_tokens_where_line_starts_with_token_until_ending_token_is_found.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/tokens.py` & `vsg-3.9.0/vsg/vhdlFile/extract/tokens.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,26 @@
 
     def get_start_index(self):
         return self.iStartIndex
 
     def get_end_index(self):
         return self.iEndIndex
 
+    def get_first_token_matching(self, oTokenType):
+        for oToken in self.lTokens:
+            if isinstance(oToken, oTokenType):
+                return oToken
+        return None
+
+    def token_type_exists(self, oTokenType):
+        for oToken in self.lTokens:
+            if isinstance(oToken, oTokenType):
+                return True
+        return False
+
 
 def calculate_end_index(iStartIndex, lTokens):
     try:
         iReturn = iStartIndex
         for oToken in lTokens:
             if not isinstance(oToken, parser.beginning_of_file):
                 iReturn += 1
```

### Comparing `vsg-3.8.0/vsg/vhdlFile/extract/utils.py` & `vsg-3.9.0/vsg/vhdlFile/extract/utils.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg/vhdlFile/indent/indent_config.yaml` & `vsg-3.9.0/vsg/vhdlFile/indent/indent_config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,17 @@
             end_keyword:
                 token : '-1'
                 after : '-1'
         entity_declaration:
             entity_keyword:
                 token : 0
                 after : 1
+            begin_keyword:
+                token : 0
+                after : 1
             end_keyword:
                 token : 0
                 after : 0
         enumeration_type_definition:
             open_parenthesis:
                 token : current
                 after : '+1'
```

### Comparing `vsg-3.8.0/vsg/vhdlFile/indent/set_token_indent.py` & `vsg-3.9.0/vsg/vhdlFile/indent/set_token_indent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 from vsg import parser
 from vsg import token
 
 
 def set_token_indent(dIndentMap, lTokens):
-
     lTokenKeys, dIndents = process_indent_map(dIndentMap)
 
     iIndent = 0
     bLibraryFound = False
     bArchitectureFound = False
     dVars = {}
     dVars['insideConcurrentSignalAssignment'] = False
@@ -79,14 +78,19 @@
             bLibraryFound = False
             continue
 
         ### Comments
         if isinstance(oToken, parser.comment):
             if bLibraryFound:
                 oToken.set_indent(iIndent + 1)
+            elif oToken.is_block_comment:
+                if oToken.block_comment_indent == 0:
+                    oToken.set_indent(0)
+                else:
+                    oToken.set_indent(iIndent)
             else:
                 oToken.set_indent(iIndent)
             continue
 
         ### Concurrent signal assignment
         if isinstance(oToken, token.concurrent_signal_assignment_statement.label_name):
             dVars['insideConcurrentSignalAssignment'] = True
```

### Comparing `vsg-3.8.0/vsg/vhdlFile/utils.py` & `vsg-3.9.0/vsg/vhdlFile/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 
 from vsg import exceptions
 from vsg import parser
 
 from vsg.token import direction
+from vsg.token import choice
+from vsg.token import element_association
 from vsg.token.ieee.std_logic_1164 import types
 
 
 def assign_tokens_until(sToken, token, iToken, lObjects):
     iCurrent = iToken
     while not is_next_token(sToken, iCurrent, lObjects):
         iCurrent = assign_next_token(token, iCurrent, lObjects)
@@ -593,14 +595,20 @@
 def count_carriage_returns(lTokens):
     iReturn = 0
     for oToken in lTokens:
         iReturn = increment_line_number(iReturn, oToken)
     return iReturn
 
 
+def increment_comment_counter(iComment, oToken):
+    if isinstance(oToken, parser.comment):
+        return iComment + 1
+    return iComment
+
+
 def find_carriage_return(lTokens, iToken=0):
     for iIndex in range(iToken, len(lTokens)):
         if isinstance(lTokens[iIndex], parser.carriage_return):
             return iIndex
     return None
 
 
@@ -782,9 +790,13 @@
         assign_token(lObjects, iCurrent, types.integer)
     elif sValue.lower() == 'signed':
         assign_token(lObjects, iCurrent, types.signed)
     elif sValue.lower() == 'unsigned':
         assign_token(lObjects, iCurrent, types.unsigned)
     elif sValue.lower() == 'natural':
         assign_token(lObjects, iCurrent, types.natural)
+    elif sValue.lower() == 'others':
+        assign_token(lObjects, iCurrent, choice.others_keyword)
+    elif sValue.lower() == '=>':
+        assign_token(lObjects, iCurrent, element_association.assignment)
     else:
         assign_token(lObjects, iCurrent, oType)
```

### Comparing `vsg-3.8.0/vsg/vhdlFile/vhdlFile.py` & `vsg-3.9.0/vsg/vhdlFile/vhdlFile.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,16 +480,17 @@
             if sValue.lower() == 'std_ulogic':
                 lTokens[iToken] = types.std_ulogic(sValue)
 
             if len(sValue) == 3 and sValue.startswith("'") and sValue.endswith("'"):
                 lTokens[iToken] = parser.character_literal(sValue)
                 continue
         else:
-            oCodeTags.update(oToken)
-            oToken.set_code_tags(oCodeTags.get_tags())
+            bVsgOn = oCodeTags.update(oToken)
+            if not bVsgOn:
+                oToken.set_code_tags(oCodeTags.get_tags())
             sValue = oToken.get_value()
             if sValue  == '+':
                 if utils.are_previous_consecutive_token_types_ignoring_whitespace([parser.open_parenthesis], iToken - 1, lTokens):
                     lTokens[iToken] = sign.plus()
                 elif utils.are_previous_consecutive_token_types_ignoring_whitespace([parser.keyword], iToken - 1, lTokens):
                     lTokens[iToken] = sign.plus()
                 else:
```

### Comparing `vsg-3.8.0/vsg/violation.py` & `vsg-3.9.0/vsg/violation.py`

 * *Files identical despite different names*

### Comparing `vsg-3.8.0/vsg.egg-info/PKG-INFO` & `vsg-3.9.0/vsg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: vsg
-Version: 3.8.0
+Version: 3.9.0
 Summary: VHDL Style Guide
 Home-page: https://github.com/jeremiah-c-leary/vhdl-style-guide
 Author: Jeremiah C Leary
 Author-email: jeremiah.c.leary@gmail.com
 License: GNU General Public License
 Download-URL: https://github.com/jeremiah-c-leary/vhdl-style-guide
 Description: VHDL Style Guide (VSG)
```

### Comparing `vsg-3.8.0/vsg.egg-info/SOURCES.txt` & `vsg-3.9.0/vsg.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -258,14 +258,19 @@
 vsg/rules/case/rule_017.py
 vsg/rules/case/rule_018.py
 vsg/rules/case/rule_019.py
 vsg/rules/case/rule_020.py
 vsg/rules/case/rule_021.py
 vsg/rules/case/rule_200.py
 vsg/rules/case/rule_201.py
+vsg/rules/case_generate_alternative/__init__.py
+vsg/rules/case_generate_alternative/rule_500.py
+vsg/rules/case_generate_statement/__init__.py
+vsg/rules/case_generate_statement/rule_500.py
+vsg/rules/case_generate_statement/rule_501.py
 vsg/rules/comment/__init__.py
 vsg/rules/comment/rule_004.py
 vsg/rules/comment/rule_010.py
 vsg/rules/comment/rule_011.py
 vsg/rules/comment/rule_100.py
 vsg/rules/component/__init__.py
 vsg/rules/component/rule_001.py
@@ -353,14 +358,17 @@
 vsg/rules/context_ref/rule_003.py
 vsg/rules/context_ref/rule_004.py
 vsg/rules/context_ref/rule_005.py
 vsg/rules/context_ref/rule_006.py
 vsg/rules/context_ref/rule_007.py
 vsg/rules/context_ref/rule_008.py
 vsg/rules/context_ref/rule_009.py
+vsg/rules/element_association/__init__.py
+vsg/rules/element_association/rule_100.py
+vsg/rules/element_association/rule_101.py
 vsg/rules/entity/__init__.py
 vsg/rules/entity/rule_001.py
 vsg/rules/entity/rule_002.py
 vsg/rules/entity/rule_003.py
 vsg/rules/entity/rule_004.py
 vsg/rules/entity/rule_005.py
 vsg/rules/entity/rule_006.py
@@ -374,29 +382,46 @@
 vsg/rules/entity/rule_014.py
 vsg/rules/entity/rule_015.py
 vsg/rules/entity/rule_016.py
 vsg/rules/entity/rule_017.py
 vsg/rules/entity/rule_018.py
 vsg/rules/entity/rule_019.py
 vsg/rules/entity/rule_020.py
+vsg/rules/entity/rule_021.py
+vsg/rules/entity/rule_022.py
+vsg/rules/entity/rule_023.py
+vsg/rules/entity/rule_024.py
+vsg/rules/entity/rule_025.py
+vsg/rules/entity/rule_026.py
+vsg/rules/entity/rule_027.py
+vsg/rules/entity/rule_028.py
+vsg/rules/entity/rule_029.py
 vsg/rules/entity/rule_200.py
+vsg/rules/entity/rule_201.py
+vsg/rules/entity/rule_202.py
+vsg/rules/entity/rule_203.py
+vsg/rules/entity/rule_300.py
+vsg/rules/entity/rule_500.py
 vsg/rules/entity/rule_600.py
 vsg/rules/entity_specification/__init__.py
 vsg/rules/entity_specification/rule_100.py
 vsg/rules/entity_specification/rule_101.py
 vsg/rules/entity_specification/rule_500.py
 vsg/rules/entity_specification/rule_501.py
 vsg/rules/entity_specification/rule_502.py
 vsg/rules/entity_specification/rule_503.py
 vsg/rules/exit_statement/__init__.py
 vsg/rules/exit_statement/rule_300.py
 vsg/rules/file_statement/__init__.py
 vsg/rules/file_statement/rule_001.py
 vsg/rules/file_statement/rule_002.py
 vsg/rules/file_statement/rule_003.py
+vsg/rules/for_generate_statement/__init__.py
+vsg/rules/for_generate_statement/rule_500.py
+vsg/rules/for_generate_statement/rule_501.py
 vsg/rules/for_loop/__init__.py
 vsg/rules/for_loop/rule_001.py
 vsg/rules/for_loop/rule_002.py
 vsg/rules/for_loop/rule_003.py
 vsg/rules/for_loop/rule_004.py
 vsg/rules/for_loop/rule_005.py
 vsg/rules/function/__init__.py
@@ -446,14 +471,16 @@
 vsg/rules/generate/rule_018.py
 vsg/rules/generate/rule_400.py
 vsg/rules/generate/rule_401.py
 vsg/rules/generate/rule_402.py
 vsg/rules/generate/rule_403.py
 vsg/rules/generate/rule_404.py
 vsg/rules/generate/rule_405.py
+vsg/rules/generate/rule_500.py
+vsg/rules/generate/rule_501.py
 vsg/rules/generate/rule_600.py
 vsg/rules/generic/__init__.py
 vsg/rules/generic/rule_001.py
 vsg/rules/generic/rule_002.py
 vsg/rules/generic/rule_003.py
 vsg/rules/generic/rule_004.py
 vsg/rules/generic/rule_005.py
@@ -478,14 +505,19 @@
 vsg/rules/generic_map/rule_004.py
 vsg/rules/generic_map/rule_005.py
 vsg/rules/generic_map/rule_006.py
 vsg/rules/generic_map/rule_007.py
 vsg/rules/generic_map/rule_008.py
 vsg/rules/ieee/__init__.py
 vsg/rules/ieee/rule_500.py
+vsg/rules/if_generate_statement/__init__.py
+vsg/rules/if_generate_statement/rule_500.py
+vsg/rules/if_generate_statement/rule_501.py
+vsg/rules/if_generate_statement/rule_502.py
+vsg/rules/if_generate_statement/rule_503.py
 vsg/rules/if_statement/__init__.py
 vsg/rules/if_statement/rule_001.py
 vsg/rules/if_statement/rule_002.py
 vsg/rules/if_statement/rule_003.py
 vsg/rules/if_statement/rule_004.py
 vsg/rules/if_statement/rule_005.py
 vsg/rules/if_statement/rule_006.py
@@ -673,14 +705,24 @@
 vsg/rules/port/rule_021.py
 vsg/rules/port/rule_022.py
 vsg/rules/port/rule_023.py
 vsg/rules/port/rule_024.py
 vsg/rules/port/rule_025.py
 vsg/rules/port/rule_026.py
 vsg/rules/port/rule_027.py
+vsg/rules/port/rule_600.py
+vsg/rules/port/rule_601.py
+vsg/rules/port/rule_602.py
+vsg/rules/port/rule_603.py
+vsg/rules/port/rule_604.py
+vsg/rules/port/rule_605.py
+vsg/rules/port/rule_606.py
+vsg/rules/port/rule_607.py
+vsg/rules/port/rule_608.py
+vsg/rules/port/rule_609.py
 vsg/rules/port_map/__init__.py
 vsg/rules/port_map/rule_001.py
 vsg/rules/port_map/rule_002.py
 vsg/rules/port_map/rule_003.py
 vsg/rules/port_map/rule_004.py
 vsg/rules/port_map/rule_005.py
 vsg/rules/port_map/rule_007.py
@@ -871,14 +913,15 @@
 vsg/rules/whitespace/rule_006.py
 vsg/rules/whitespace/rule_007.py
 vsg/rules/whitespace/rule_008.py
 vsg/rules/whitespace/rule_010.py
 vsg/rules/whitespace/rule_011.py
 vsg/rules/whitespace/rule_012.py
 vsg/rules/whitespace/rule_013.py
+vsg/rules/whitespace/rule_200.py
 vsg/rules/with_statement/__init__.py
 vsg/rules/with_statement/rule_001.py
 vsg/styles/__init__.py
 vsg/styles/indent_only.yaml
 vsg/styles/jcl.yaml
 vsg/token/__init__.py
 vsg/token/access_type_definition.py
@@ -919,14 +962,15 @@
 vsg/token/configuration_declaration.py
 vsg/token/constant_declaration.py
 vsg/token/constrained_array_definition.py
 vsg/token/context_declaration.py
 vsg/token/context_reference.py
 vsg/token/delay_mechanism.py
 vsg/token/direction.py
+vsg/token/element_association.py
 vsg/token/element_declaration.py
 vsg/token/entity.py
 vsg/token/entity_aspect.py
 vsg/token/entity_declaration.py
 vsg/token/entity_designator.py
 vsg/token/entity_name_list.py
 vsg/token/entity_specification.py
```

