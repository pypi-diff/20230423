# Comparing `tmp/je_editor_dev-0.0.8.tar.gz` & `tmp/je_editor_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_editor_dev-0.0.8.tar", last modified: Fri Jan 14 18:37:02 2022, max compression
+gzip compressed data, was "je_editor_dev-0.0.9.tar", last modified: Fri Jan 14 21:02:54 2022, max compression
```

## Comparing `je_editor_dev-0.0.8.tar` & `je_editor_dev-0.0.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.407095 je_editor_dev-0.0.8/
--rw-rw-rw-   0        0        0     1085 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1481 2022-01-14 18:37:02.406096 je_editor_dev-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      860 2022-01-06 12:40:47.000000 je_editor_dev-0.0.8/README.md
--rw-rw-rw-   0        0        0      909 2022-01-14 18:36:19.000000 je_editor_dev-0.0.8/dev_setup.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:01.983773 je_editor_dev-0.0.8/je_editor/
--rw-rw-rw-   0        0        0      608 2022-01-14 18:33:11.000000 je_editor_dev-0.0.8/je_editor/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:01.997826 je_editor_dev-0.0.8/je_editor/ui/
--rw-rw-rw-   0        0        0       28 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.023777 je_editor_dev-0.0.8/je_editor/ui/editor_main_ui/
--rw-rw-rw-   0        0        0       43 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/editor_main_ui/__init__.py
--rw-rw-rw-   0        0        0    10916 2022-01-14 12:09:36.000000 je_editor_dev-0.0.8/je_editor/ui/editor_main_ui/tkinter_editor.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.028774 je_editor_dev-0.0.8/je_editor/ui/ui_event/
--rw-rw-rw-   0        0        0       37 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.032824 je_editor_dev-0.0.8/je_editor/ui/ui_event/auto_save/
--rw-rw-rw-   0        0        0       47 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/auto_save/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.042813 je_editor_dev-0.0.8/je_editor/ui/ui_event/auto_save/start_auto_save/
--rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/auto_save/start_auto_save/__init__.py
--rw-rw-rw-   0        0        0      460 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/auto_save/start_auto_save/start_auto_save.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.051814 je_editor_dev-0.0.8/je_editor/ui/ui_event/change_font/
--rw-rw-rw-   0        0        0       49 2022-01-06 12:40:47.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/change_font/__init__.py
--rw-rw-rw-   0        0        0      844 2022-01-14 11:49:29.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/change_font/change_font.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.060773 je_editor_dev-0.0.8/je_editor/ui/ui_event/close/
--rw-rw-rw-   0        0        0       43 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/close/__init__.py
--rw-rw-rw-   0        0        0      532 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/close/close_event.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.084772 je_editor_dev-0.0.8/je_editor/ui/ui_event/encoding/
--rw-rw-rw-   0        0        0       46 2022-01-14 11:46:17.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/encoding/__init__.py
--rw-rw-rw-   0        0        0       89 2022-01-14 11:49:29.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/encoding/set_encoding.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.095773 je_editor_dev-0.0.8/je_editor/ui/ui_event/execute/
--rw-rw-rw-   0        0        0       45 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/execute/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.111771 je_editor_dev-0.0.8/je_editor/ui/ui_event/execute/execute_code/
--rw-rw-rw-   0        0        0       58 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/execute/execute_code/__init__.py
--rw-rw-rw-   0        0        0      538 2022-01-09 13:01:31.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/execute/execute_code/exec_code.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.128773 je_editor_dev-0.0.8/je_editor/ui/ui_event/execute/execute_shell_command/
--rw-rw-rw-   0        0        0       67 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/execute/execute_shell_command/__init__.py
--rw-rw-rw-   0        0        0      726 2022-01-06 02:44:24.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/execute/execute_shell_command/run_on_shell.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.144772 je_editor_dev-0.0.8/je_editor/ui/ui_event/language/
--rw-rw-rw-   0        0        0       46 2022-01-14 12:08:46.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/language/__init__.py
--rw-rw-rw-   0        0        0       89 2022-01-14 12:08:46.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/language/set_language.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.146772 je_editor_dev-0.0.8/je_editor/ui/ui_event/open_file/
--rw-rw-rw-   0        0        0        2 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/open_file/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.155771 je_editor_dev-0.0.8/je_editor/ui/ui_event/open_file/open_file_to_read/
--rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/open_file/open_file_to_read/__init__.py
--rw-rw-rw-   0        0        0      655 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/open_file/open_file_to_read/open_file_to_read.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.172771 je_editor_dev-0.0.8/je_editor/ui/ui_event/open_file/open_last_edit_file/
--rw-rw-rw-   0        0        0       67 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/open_file/open_last_edit_file/__init__.py
--rw-rw-rw-   0        0        0      638 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/open_file/open_last_edit_file/open_last_edit_file.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.174772 je_editor_dev-0.0.8/je_editor/ui/ui_event/save_file/
--rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/save_file/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.190772 je_editor_dev-0.0.8/je_editor/ui/ui_event/save_file/save_file_to_open/
--rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/save_file/save_file_to_open/__init__.py
--rw-rw-rw-   0        0        0      593 2022-01-06 18:18:59.000000 je_editor_dev-0.0.8/je_editor/ui/ui_event/save_file/save_file_to_open/save_file_to_open.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.194773 je_editor_dev-0.0.8/je_editor/ui/ui_utils/
--rw-rw-rw-   0        0        0       37 2022-01-06 12:40:47.000000 je_editor_dev-0.0.8/je_editor/ui/ui_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.210776 je_editor_dev-0.0.8/je_editor/ui/ui_utils/font/
--rw-rw-rw-   0        0        0       42 2022-01-06 12:40:47.000000 je_editor_dev-0.0.8/je_editor/ui/ui_utils/font/__init__.py
--rw-rw-rw-   0        0        0      292 2022-01-06 12:40:47.000000 je_editor_dev-0.0.8/je_editor/ui/ui_utils/font/font.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.215803 je_editor_dev-0.0.8/je_editor/utils/
--rw-rw-rw-   0        0        0       31 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.226828 je_editor_dev-0.0.8/je_editor/utils/code_tag/
--rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/code_tag/__init__.py
--rw-rw-rw-   0        0        0       96 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/code_tag/keyword_list.py
--rw-rw-rw-   0        0        0     1805 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/code_tag/tag_keyword.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.235772 je_editor_dev-0.0.8/je_editor/utils/editor_content/
--rw-rw-rw-   0        0        0       46 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/editor_content/__init__.py
--rw-rw-rw-   0        0        0     1519 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/editor_content/content_save.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.252809 je_editor_dev-0.0.8/je_editor/utils/encoding/
--rw-rw-rw-   0        0        0       40 2022-01-14 11:17:11.000000 je_editor_dev-0.0.8/je_editor/utils/encoding/__init__.py
--rw-rw-rw-   0        0        0     1717 2022-01-14 11:17:11.000000 je_editor_dev-0.0.8/je_editor/utils/encoding/encoding_data_module.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.266975 je_editor_dev-0.0.8/je_editor/utils/exception/
--rw-rw-rw-   0        0        0       41 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      497 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/exception/je_editor_exception_tag.py
--rw-rw-rw-   0        0        0      488 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/exception/je_editor_exceptions.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.270985 je_editor_dev-0.0.8/je_editor/utils/file/
--rw-rw-rw-   0        0        0       36 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.286985 je_editor_dev-0.0.8/je_editor/utils/file/open/
--rw-rw-rw-   0        0        0       41 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0     1532 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.309986 je_editor_dev-0.0.8/je_editor/utils/file/save/
--rw-rw-rw-   0        0        0       39 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0     2423 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.318989 je_editor_dev-0.0.8/je_editor/utils/language/
--rw-rw-rw-   0        0        0       40 2022-01-14 11:56:38.000000 je_editor_dev-0.0.8/je_editor/utils/language/__init__.py
--rw-rw-rw-   0        0        0       68 2022-01-14 12:01:15.000000 je_editor_dev-0.0.8/je_editor/utils/language/language_data_module.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.331985 je_editor_dev-0.0.8/je_editor/utils/string_translate/
--rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/string_translate/__init__.py
--rw-rw-rw-   0        0        0       54 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/string_translate/used_string.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.342985 je_editor_dev-0.0.8/je_editor/utils/text_process/
--rw-rw-rw-   0        0        0       44 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/text_process/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.354625 je_editor_dev-0.0.8/je_editor/utils/text_process/program_exec/
--rw-rw-rw-   0        0        0       57 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/text_process/program_exec/__init__.py
--rw-rw-rw-   0        0        0     5984 2022-01-14 18:36:19.000000 je_editor_dev-0.0.8/je_editor/utils/text_process/program_exec/exec_text.py
--rw-rw-rw-   0        0        0      327 2022-01-07 18:49:28.000000 je_editor_dev-0.0.8/je_editor/utils/text_process/program_exec/process_error.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.363478 je_editor_dev-0.0.8/je_editor/utils/text_process/shell/
--rw-rw-rw-   0        0        0       50 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/text_process/shell/__init__.py
--rw-rw-rw-   0        0        0      448 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/text_process/shell/shell_text.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.369425 je_editor_dev-0.0.8/je_editor/utils/theme/
--rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/theme/__init__.py
--rw-rw-rw-   0        0        0       96 2022-01-03 07:43:33.000000 je_editor_dev-0.0.8/je_editor/utils/theme/theme.py
-drwxrwxrwx   0        0        0        0 2022-01-14 18:37:02.405095 je_editor_dev-0.0.8/je_editor_dev.egg-info/
--rw-rw-rw-   0        0        0     1481 2022-01-14 18:37:00.000000 je_editor_dev-0.0.8/je_editor_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2968 2022-01-14 18:37:00.000000 je_editor_dev-0.0.8/je_editor_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-14 18:37:00.000000 je_editor_dev-0.0.8/je_editor_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-01-14 18:37:00.000000 je_editor_dev-0.0.8/je_editor_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-14 18:37:02.408092 je_editor_dev-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      901 2022-01-13 14:16:52.000000 je_editor_dev-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.296718 je_editor_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1481 2022-01-14 21:02:54.294720 je_editor_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/README.md
+-rw-rw-rw-   0        0        0      909 2022-01-14 21:02:51.000000 je_editor_dev-0.0.9/dev_setup.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.033720 je_editor_dev-0.0.9/je_editor/
+-rw-rw-rw-   0        0        0      608 2022-01-14 18:33:11.000000 je_editor_dev-0.0.9/je_editor/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.036723 je_editor_dev-0.0.9/je_editor/ui/
+-rw-rw-rw-   0        0        0       28 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.041717 je_editor_dev-0.0.9/je_editor/ui/editor_main_ui/
+-rw-rw-rw-   0        0        0       43 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/editor_main_ui/__init__.py
+-rw-rw-rw-   0        0        0    11111 2022-01-14 21:02:13.000000 je_editor_dev-0.0.9/je_editor/ui/editor_main_ui/tkinter_editor.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.043734 je_editor_dev-0.0.9/je_editor/ui/ui_event/
+-rw-rw-rw-   0        0        0       37 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.046718 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/
+-rw-rw-rw-   0        0        0       47 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.052732 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/start_auto_save/
+-rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/start_auto_save/__init__.py
+-rw-rw-rw-   0        0        0      460 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/start_auto_save/start_auto_save.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.057723 je_editor_dev-0.0.9/je_editor/ui/ui_event/change_font/
+-rw-rw-rw-   0        0        0       49 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/change_font/__init__.py
+-rw-rw-rw-   0        0        0      844 2022-01-14 11:49:29.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/change_font/change_font.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.064718 je_editor_dev-0.0.9/je_editor/ui/ui_event/close/
+-rw-rw-rw-   0        0        0       43 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/close/__init__.py
+-rw-rw-rw-   0        0        0      532 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/close/close_event.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.069721 je_editor_dev-0.0.9/je_editor/ui/ui_event/encoding/
+-rw-rw-rw-   0        0        0       46 2022-01-14 11:46:17.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/encoding/__init__.py
+-rw-rw-rw-   0        0        0       89 2022-01-14 11:49:29.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/encoding/set_encoding.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.071718 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/
+-rw-rw-rw-   0        0        0       45 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.076726 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_code/
+-rw-rw-rw-   0        0        0       58 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_code/__init__.py
+-rw-rw-rw-   0        0        0      538 2022-01-09 13:01:31.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_code/exec_code.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.082720 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_shell_command/
+-rw-rw-rw-   0        0        0       67 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_shell_command/__init__.py
+-rw-rw-rw-   0        0        0      726 2022-01-06 02:44:24.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_shell_command/run_on_shell.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.087718 je_editor_dev-0.0.9/je_editor/ui/ui_event/language/
+-rw-rw-rw-   0        0        0       46 2022-01-14 12:08:46.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/language/__init__.py
+-rw-rw-rw-   0        0        0       89 2022-01-14 12:08:46.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/language/set_language.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.090719 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/
+-rw-rw-rw-   0        0        0        2 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.096719 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_file_to_read/
+-rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_file_to_read/__init__.py
+-rw-rw-rw-   0        0        0      655 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_file_to_read/open_file_to_read.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.103719 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_last_edit_file/
+-rw-rw-rw-   0        0        0       67 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_last_edit_file/__init__.py
+-rw-rw-rw-   0        0        0      638 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_last_edit_file/open_last_edit_file.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.105717 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/
+-rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.112718 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/save_file_to_open/
+-rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/save_file_to_open/__init__.py
+-rw-rw-rw-   0        0        0      593 2022-01-06 18:18:59.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/save_file_to_open/save_file_to_open.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.115717 je_editor_dev-0.0.9/je_editor/ui/ui_utils/
+-rw-rw-rw-   0        0        0       37 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.122717 je_editor_dev-0.0.9/je_editor/ui/ui_utils/font/
+-rw-rw-rw-   0        0        0       42 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_utils/font/__init__.py
+-rw-rw-rw-   0        0        0      292 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_utils/font/font.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.126718 je_editor_dev-0.0.9/je_editor/utils/
+-rw-rw-rw-   0        0        0       31 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.140721 je_editor_dev-0.0.9/je_editor/utils/code_tag/
+-rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/code_tag/__init__.py
+-rw-rw-rw-   0        0        0       96 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/code_tag/keyword_list.py
+-rw-rw-rw-   0        0        0     1805 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/code_tag/tag_keyword.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.153718 je_editor_dev-0.0.9/je_editor/utils/editor_content/
+-rw-rw-rw-   0        0        0       46 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/editor_content/__init__.py
+-rw-rw-rw-   0        0        0     1519 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/editor_content/content_save.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.164717 je_editor_dev-0.0.9/je_editor/utils/encoding/
+-rw-rw-rw-   0        0        0       40 2022-01-14 11:17:11.000000 je_editor_dev-0.0.9/je_editor/utils/encoding/__init__.py
+-rw-rw-rw-   0        0        0     1717 2022-01-14 11:17:11.000000 je_editor_dev-0.0.9/je_editor/utils/encoding/encoding_data_module.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.176718 je_editor_dev-0.0.9/je_editor/utils/exception/
+-rw-rw-rw-   0        0        0       41 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      497 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/exception/je_editor_exception_tag.py
+-rw-rw-rw-   0        0        0      488 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/exception/je_editor_exceptions.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.179718 je_editor_dev-0.0.9/je_editor/utils/file/
+-rw-rw-rw-   0        0        0       36 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.184719 je_editor_dev-0.0.9/je_editor/utils/file/open/
+-rw-rw-rw-   0        0        0       41 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0     1532 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.190721 je_editor_dev-0.0.9/je_editor/utils/file/save/
+-rw-rw-rw-   0        0        0       39 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0     2423 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.196718 je_editor_dev-0.0.9/je_editor/utils/language/
+-rw-rw-rw-   0        0        0       40 2022-01-14 11:56:38.000000 je_editor_dev-0.0.9/je_editor/utils/language/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-01-14 12:01:15.000000 je_editor_dev-0.0.9/je_editor/utils/language/language_data_module.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.206727 je_editor_dev-0.0.9/je_editor/utils/string_translate/
+-rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/string_translate/__init__.py
+-rw-rw-rw-   0        0        0       54 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/string_translate/used_string.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.212718 je_editor_dev-0.0.9/je_editor/utils/text_process/
+-rw-rw-rw-   0        0        0       44 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.228718 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/
+-rw-rw-rw-   0        0        0       57 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/__init__.py
+-rw-rw-rw-   0        0        0     5984 2022-01-14 18:36:19.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/exec_text.py
+-rw-rw-rw-   0        0        0      327 2022-01-07 18:49:28.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/process_error.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.237720 je_editor_dev-0.0.9/je_editor/utils/text_process/shell/
+-rw-rw-rw-   0        0        0       50 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/shell/__init__.py
+-rw-rw-rw-   0        0        0      448 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/shell/shell_text.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.242718 je_editor_dev-0.0.9/je_editor/utils/theme/
+-rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/theme/__init__.py
+-rw-rw-rw-   0        0        0       96 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/theme/theme.py
+drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.290718 je_editor_dev-0.0.9/je_editor_dev.egg-info/
+-rw-rw-rw-   0        0        0     1481 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2968 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-01-14 21:02:54.296718 je_editor_dev-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      901 2022-01-13 14:16:52.000000 je_editor_dev-0.0.9/setup.py
```

### Comparing `je_editor_dev-0.0.8/LICENSE` & `je_editor_dev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/PKG-INFO` & `je_editor_dev-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_editor_dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: simple editor
 Home-page: https://github.com/JE-Chen/je_editor
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `je_editor_dev-0.0.8/README.md` & `je_editor_dev-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/dev_setup.py` & `je_editor_dev-0.0.9/dev_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as README:
     long_description = README.read()
 
 setuptools.setup(
     name="je_editor_dev",
-    version="0.0.08",
+    version="0.0.09",
     author="JE-Chen",
     author_email="zenmailman@gmail.com",
     description="simple editor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JE-Chen/je_editor",
     packages=setuptools.find_packages(),
```

### Comparing `je_editor_dev-0.0.8/je_editor/__init__.py` & `je_editor_dev-0.0.9/je_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/ui/editor_main_ui/tkinter_editor.py` & `je_editor_dev-0.0.9/je_editor/ui/editor_main_ui/tkinter_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,27 +98,29 @@
         self.run_result_frame = ttk.Frame(self.main_window, padding="3 3 12 12")
         self.run_result_frame.grid(column=0, row=1, sticky=(N, W, E, S))
         # Text start and end position
         self.start_position = "1.0"
         self.end_position = "end-1c"
         # set code edit
         self.code_editor = Text(self.code_edit_frame, undo=True, autoseparators=True, maxundo=-1)
-        self.code_editor_scrollbar_y = ttk.Scrollbar(orient="vertical", command=self.code_editor.yview)
-        self.code_editor["yscrollcommand"] = self.code_editor_scrollbar_y.set
         self.code_editor.grid(column=0, row=0, sticky=(N, W, E, S))
-        self.code_editor_scrollbar_y.grid(column=1, row=0)
         self.code_editor.configure(state="normal")
+        self.code_editor_scrollbar_y = ttk.Scrollbar(self.code_edit_frame, orient="vertical",
+                                                     command=self.code_editor.yview)
+        self.code_editor["yscrollcommand"] = self.code_editor_scrollbar_y.set
+        self.code_editor_scrollbar_y.grid(column=1, row=0, sticky="ns")
         # run result
         self.run_result = Text(self.run_result_frame)
-        self.run_result_scrollbar_y = ttk.Scrollbar(orient="vertical", command=self.run_result.yview)
-        self.run_result["yscrollcommand"] = self.run_result_scrollbar_y.set
         self.run_result.grid(column=0, row=1, sticky=(N, W, E, S))
-        self.run_result_scrollbar_y.grid(column=1, row=1)
         self.run_result.configure(state="disabled")
         self.run_result.bind("<1>", lambda event: self.run_result.focus_set())
+        self.run_result_scrollbar_y = ttk.Scrollbar(self.run_result_frame, orient="vertical",
+                                                    command=self.run_result.yview)
+        self.run_result["yscrollcommand"] = self.run_result_scrollbar_y.set
+        self.run_result_scrollbar_y.grid(column=1, row=1, sticky="ns")
         # Menubar
         # Main menu
         self.menu = tkinter.Menu(self.main_window)
         # File menu
         self.file_menu = tkinter.Menu(self.menu, tearoff=0)
         self.file_menu.add_command(label="Save File", command=self.save_file_to_open)
         self.file_menu.add_command(label="Open File", command=self.open_file_to_read)
@@ -138,15 +140,16 @@
         self.text_menu = tkinter.Menu(self.menu, tearoff=0)
         self.text_font_sub_menu = tkinter.Menu(self.text_menu, tearoff=0)
         self.text_size_sub_menu = tkinter.Menu(self.text_menu, tearoff=0)
         self.font_tuple = get_font(self.main_window)
         for i in range(len(self.font_tuple)):
             self.text_font_sub_menu.add_command(
                 label=str(self.font_tuple[i]),
-                command=lambda choose_font=self.font_tuple[i]: change_font(self.code_editor, self.run_result, choose_font)
+                command=lambda choose_font=self.font_tuple[i]:
+                change_font(self.code_editor, self.run_result, choose_font)
             )
         for i in range(12, 36, 2):
             self.text_size_sub_menu.add_command(
                 label=str(i),
                 command=lambda font_size=i: change_font_size(self.code_editor, self.run_result, font_size)
             )
         self.text_menu.add_cascade(label="Font", menu=self.text_font_sub_menu)
```

### Comparing `je_editor_dev-0.0.8/je_editor/ui/ui_event/change_font/change_font.py` & `je_editor_dev-0.0.9/je_editor/ui/ui_event/change_font/change_font.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/ui/ui_event/close/close_event.py` & `je_editor_dev-0.0.9/je_editor/ui/ui_event/close/close_event.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/ui/ui_event/execute/execute_code/exec_code.py` & `je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_code/exec_code.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/ui/ui_event/execute/execute_shell_command/run_on_shell.py` & `je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_shell_command/run_on_shell.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/ui/ui_event/open_file/open_file_to_read/open_file_to_read.py` & `je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_file_to_read/open_file_to_read.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/ui/ui_event/open_file/open_last_edit_file/open_last_edit_file.py` & `je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_last_edit_file/open_last_edit_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/ui/ui_event/save_file/save_file_to_open/save_file_to_open.py` & `je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/save_file_to_open/save_file_to_open.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/utils/code_tag/tag_keyword.py` & `je_editor_dev-0.0.9/je_editor/utils/code_tag/tag_keyword.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/utils/editor_content/content_save.py` & `je_editor_dev-0.0.9/je_editor/utils/editor_content/content_save.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/utils/encoding/encoding_data_module.py` & `je_editor_dev-0.0.9/je_editor/utils/encoding/encoding_data_module.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/utils/file/open/open_file.py` & `je_editor_dev-0.0.9/je_editor/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/utils/file/save/save_file.py` & `je_editor_dev-0.0.9/je_editor/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor/utils/text_process/program_exec/exec_text.py` & `je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/exec_text.py`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/je_editor_dev.egg-info/PKG-INFO` & `je_editor_dev-0.0.9/je_editor_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-editor-dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: simple editor
 Home-page: https://github.com/JE-Chen/je_editor
 Author: JE-Chen
 Author-email: zenmailman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `je_editor_dev-0.0.8/je_editor_dev.egg-info/SOURCES.txt` & `je_editor_dev-0.0.9/je_editor_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.8/setup.py` & `je_editor_dev-0.0.9/setup.py`

 * *Files identical despite different names*

