# Comparing `tmp/vunit_hdl-4.6.2.tar.gz` & `tmp/vunit_hdl-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vunit_hdl-4.6.2.tar", last modified: Wed Feb 22 06:11:36 2023, max compression
+gzip compressed data, was "vunit_hdl-4.7.0.tar", last modified: Sun Apr 23 18:15:19 2023, max compression
```

## Comparing `vunit_hdl-4.6.2.tar` & `vunit_hdl-4.7.0.tar`

### file list

```diff
@@ -1,812 +1,828 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.317053 vunit_hdl-4.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-02-22 06:11:36.317053 vunit_hdl-4.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 06:11:36.317053 vunit_hdl-4.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.169054 vunit_hdl-4.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.169054 vunit_hdl-4.6.2/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/acceptance/test_artificial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/acceptance/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/acceptance/test_external_run_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.169054 vunit_hdl-4.6.2/tests/lint/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/lint/test_license.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/lint/test_mypy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/lint/test_pycodestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/lint/test_pylint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.177054 vunit_hdl-4.6.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/non_utf8_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_activehdl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_cds_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_check_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_dependency_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_ghdl_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    44287 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_incisive_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_location_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_modelsim_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_ostools.py
--rw-r--r--   0 runner    (1001) docker     (123)    57200 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_rivierapro_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_simulator_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    32550 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_test_bench.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_test_bench_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13978 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_test_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    44043 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_verilog_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    29251 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_verilog_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_verilog_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18782 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_vhdl_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/tests/unit/test_vhdl_standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.185054 vunit_hdl-4.6.2/vunit/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/check_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/color_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.185054 vunit_hdl-4.6.2/vunit/com/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/com/codec_datatype_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/com/codec_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/com/codec_vhdl_array_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/com/codec_vhdl_enumeration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/com/codec_vhdl_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/com/codec_vhdl_record_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/dependency_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/design_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/json4vhdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/location_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/ostools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.185054 vunit_hdl-4.6.2/vunit/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/parsing/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/parsing/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.185054 vunit_hdl-4.6.2/vunit/parsing/verilog/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/parsing/verilog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/parsing/verilog/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/parsing/verilog/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/parsing/verilog/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/parsing/verilog/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/persistent_tcl_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    23395 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.189054 vunit_hdl-4.6.2/vunit/sim_if/
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/sim_if/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/sim_if/activehdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/sim_if/cds_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/sim_if/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/sim_if/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/sim_if/ghdl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/sim_if/incisive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/sim_if/modelsim.py
--rw-r--r--   0 runner    (1001) docker     (123)    14074 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/sim_if/rivierapro.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/sim_if/tcl_read_eval_loop.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/sim_if/vsim_simulator_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/source_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.189054 vunit_hdl-4.6.2/vunit/test/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/test/bench.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/test/bench_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/test/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/test/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/test/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/test/suites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.189054 vunit_hdl-4.6.2/vunit/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    36821 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/ui/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/ui/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/ui/packagefacade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/ui/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/ui/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/ui/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/ui/testbench.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.189054 vunit_hdl-4.6.2/vunit/verilog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.149054 vunit_hdl-4.6.2/vunit/verilog/check/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.189054 vunit_hdl-4.6.2/vunit/verilog/check/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/verilog/check/test/check_tb.sv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.189054 vunit_hdl-4.6.2/vunit/verilog/include/
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/verilog/include/vunit_defines.svh
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/verilog/vunit_pkg.sv
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/verilog.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/version_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.189054 vunit_hdl-4.6.2/vunit/vhdl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.189054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.153054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.189054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.193054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/data/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/data/Boards0.json
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/data/Boards1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/data/Boards2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.193054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/examples/Boards0.vhdl
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/examples/Boards1.vhdl
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/examples/Boards2.vhdl
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/examples/Boards_VUnit.vhdl
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/examples/Encodings_VUnit.vhdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.193054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/src/Encodings.pkg.vhdl
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/src/JSON.ctx.vhdl
--rw-r--r--   0 runner    (1001) docker     (123)    89640 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/src/JSON.pkg.vhdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.193054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.193054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/JSONTestSuite.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/TopLevel.vhdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.257054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_object_key_lone_2nd_surrogate.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_1st_surrogate_but_2nd_missing.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_1st_valid_surrogate_2nd_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_UTF-16LE_with_BOM.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_UTF-8_invalid_sequence.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_incomplete_surrogate_and_escape_valid.json
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_incomplete_surrogate_pair.json
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_incomplete_surrogates_escape_valid.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_invalid_lonely_surrogate.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_invalid_surrogate.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_inverted_surrogates_U+1D11E.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_lone_second_surrogate.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_not_in_unicode_range.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_truncated-utf-8.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_unicode_U+10FFFE_nonchar.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_unicode_U+1FFFE_nonchar.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_unicode_U+FDD0_nonchar.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_unicode_U+FFFE_nonchar.json
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_structure_500_nested_arrays.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_structure_UTF-8_BOM_empty_object.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_1_true_without_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_a_invalid_utf8.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_colon_instead_of_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_comma_after_close.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_comma_and_number.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_double_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_double_extra_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_extra_close.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_extra_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_incomplete.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_incomplete_invalid_value.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_inner_array_no_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_invalid_utf8.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_items_separated_by_semicolon.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_just_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_just_minus.json
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_missing_value.json
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_newlines_unclosed.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_number_and_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_number_and_several_commas.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_spaces_vertical_tab_formfeed.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_star_inside.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_unclosed.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_unclosed_trailing_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_unclosed_with_new_lines.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_unclosed_with_object_inside.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_incomplete_false.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_incomplete_null.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_incomplete_true.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_++.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_+1.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_+Inf.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_-01.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_-1.0..json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_-2..json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_-NaN.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_.-1.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_.2e-3.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0.1.2.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0.3e+.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0.3e.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0.e1.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0_capital_E+.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0_capital_E.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0e+.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0e.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_1.0e+.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_1.0e-.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_1.0e.json
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_1_000.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_1eE2.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_2.e+3.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_2.e-3.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_2.e3.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_9.e+.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_Inf.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_NaN.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_U+FF11_fullwidth_digit_one.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_expression.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_hex_1_digit.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_hex_2_digits.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_infinity.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_invalid+-.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_invalid-negative-real.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_invalid-utf-8-in-bigger-int.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_invalid-utf-8-in-exponent.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_invalid-utf-8-in-int.json
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_minus_infinity.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_minus_sign_with_trailing_garbage.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_minus_space_1.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_neg_int_starting_with_zero.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_neg_real_without_int_part.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_neg_with_garbage_at_end.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_real_garbage_after_e.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_real_with_invalid_utf8_after_e.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_real_without_fractional_part.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_starting_with_dot.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_then_00.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_with_alpha.json
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_with_alpha_char.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_with_leading_zero.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_bad_value.json
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_bracket_key.json
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_comma_instead_of_colon.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_double_colon.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_emoji.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_garbage_at_end.json
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_key_with_single_quotes.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_missing_colon.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_missing_key.json
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_missing_semicolon.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_missing_value.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_no-colon.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_non_string_key.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_non_string_key_but_huge_number_instead.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_pi_in_key_and_trailing_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_repeated_null_null.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_several_trailing_commas.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_single_quote.json
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_trailing_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_trailing_comment.json
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_trailing_comment_open.json
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_trailing_comment_slash_open.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_trailing_comment_slash_open_incomplete.json
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_two_commas_in_a_row.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_unquoted_key.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_unterminated-value.json
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_with_single_string.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_with_trailing_garbage.json
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_single_space.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_1_surrogate_then_escape u.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_1_surrogate_then_escape u1.json
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_1_surrogate_then_escape u1x.json
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_1_surrogate_then_escape.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_UTF8_surrogate_U+D800.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_accentuated_char_no_quotes.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_backslash_00.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_escape_x.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_escaped_backslash_bad.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_escaped_ctrl_char_tab.json
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_escaped_emoji.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_incomplete_escape.json
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_incomplete_escaped_character.json
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_incomplete_surrogate.json
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_incomplete_surrogate_escape_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_invalid-utf-8-in-escape.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_invalid_backslash_esc.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_invalid_unicode_escape.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_invalid_utf-8.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_invalid_utf8_after_escape.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_iso_latin_1.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_leading_uescaped_thinspace.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_lone_utf8_continuation_byte.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_no_quotes_with_bad_escape.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_overlong_sequence_2_bytes.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_overlong_sequence_6_bytes.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_overlong_sequence_6_bytes_null.json
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_single_doublequote.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_single_quote.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_single_string_no_double_quotes.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_start_escape_unclosed.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_unescaped_crtl_char.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_unescaped_newline.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_unescaped_tab.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_unicode_CapitalU.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_with_trailing_garbage.json
--rw-r--r--   0 runner    (1001) docker     (123)   100000 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_100000_opening_arrays.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_U+2060_word_joined.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_UTF8_BOM_no_data.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure__._.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure__null_.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_array_trailing_garbage.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_array_with_extra_array_close.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_array_with_unclosed_string.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_ascii-unicode-identifier.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_capitalized_True.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_close_unopened_array.json
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_comma_instead_of_closing_brace.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_double_array.json
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_end_array.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_incomplete_UTF8_BOM.json
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_lone-invalid-utf-8.json
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_lone-open-bracket.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_no_data.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_null-byte-outside-string.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_number_with_trailing_garbage.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_object_followed_by_closing_object.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_object_unclosed_no_value.json
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_object_with_comment.json
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_object_with_trailing_garbage.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_apostrophe.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)   250001 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_object.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_open_object.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_open_string.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_string.json
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object_close_array.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object_comma.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object_open_array.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object_open_string.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object_string_with_apostrophes.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_open.json
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_single_point.json
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_single_star.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_trailing_#.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_uescaped_LF_before_string.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unclosed_array.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unclosed_array_partial_null.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unclosed_array_unfinished_false.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unclosed_array_unfinished_true.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unclosed_object.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unicode-identifier.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_whitespace_U+2060_word_joiner.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_whitespace_formfeed.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_arraysWithSpaces.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_empty-string.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_empty.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_ending_with_newline.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_false.json
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_heterogeneous.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_null.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_with_1_and_newline.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_with_leading_space.json
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_with_several_null.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_with_trailing_space.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_0e+1.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_0e1.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_after_space.json
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_double_close_to_zero.json
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_double_huge_neg_exp.json
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_huge_exp.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_int_with_exp.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_minus_zero.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_neg_int_huge_exp.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_negative_int.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_negative_one.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_negative_zero.json
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_pos_double_huge_exp.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_capital_e.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_capital_e_neg_exp.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_capital_e_pos_exp.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_exponent.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_fraction_exponent.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_neg_exp.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_neg_overflow.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_pos_exponent.json
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_pos_overflow.json
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_underflow.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_simple_int.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_simple_real.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_too_big_neg_int.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_too_big_pos_int.json
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_very_big_negative_int.json
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_basic.json
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_duplicated_key.json
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_duplicated_key_and_value.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_empty.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_empty_key.json
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_escaped_null_in_key.json
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_extreme_numbers.json
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_long_strings.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_string_unicode.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_with_newlines.json
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_1_2_3_bytes_UTF-8_sequences.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_accepted_surrogate_pair.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_accepted_surrogate_pairs.json
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_allowed_escapes.json
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_backslash_and_u_escaped_zero.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_backslash_doublequotes.json
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_comments.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_double_escape_a.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_double_escape_n.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_escaped_control_character.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_escaped_noncharacter.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_in_array.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_in_array_with_leading_space.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_last_surrogates_1_and_2.json
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_newline_uescaped.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_nonCharacterInUTF-8_U+10FFFF.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_nonCharacterInUTF-8_U+1FFFF.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_nonCharacterInUTF-8_U+FFFF.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_null_escape.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_one-byte-utf-8.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_pi.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_simple_ascii.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_space.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_surrogates_U+1D11E_MUSICAL_SYMBOL_G_CLEF.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_three-byte-utf-8.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_two-byte-utf-8.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_u+2028_line_sep.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_u+2029_par_sep.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_uEscape.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unescaped_char_delete.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicode.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicodeEscapedBackslash.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicode_2.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicode_U+200B_ZERO_WIDTH_SPACE.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicode_U+2064_invisible_plus.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicode_escaped_double_quote.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_utf16BE_no_BOM.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_utf16LE_no_BOM.json
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_utf8.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_with_del_character.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_false.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_int.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_negative_real.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_null.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_string.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_true.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_string_empty.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_trailing_newline.json
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_true_in_array.json
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_whitespace_array.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.257054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_1.0.json
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_1.000000000000000005.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_1000000000000000.json
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_10000000000000000999.json
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_1e-999.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_1e6.json
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/object_key_nfc_nfd.json
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/object_key_nfd_nfc.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/object_same_key_different_values.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/object_same_key_same_value.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/object_same_key_unclear_values.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_1_escaped_invalid_codepoint.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_1_invalid_codepoint.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_2_escaped_invalid_codepoints.json
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_2_invalid_codepoints.json
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_3_escaped_invalid_codepoints.json
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_3_invalid_codepoints.json
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_with_escaped_NULL.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.261054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Lattice/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Lattice/Lattice.ldf
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Lattice/Lattice.lpf
--rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Lattice/Lattice1.sty
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.261054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Lattice/impl_1/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Lattice/impl_1/Lattice_impl_1.lpf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.261054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Lattice/impl_2/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Lattice/impl_2/Lattice_impl_2.lpf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.261054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/QuestaSim/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/QuestaSim/Boards2.cmd
--rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/QuestaSim/Boards2.log
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.261054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/VUnit/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/VUnit/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.261054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/
--rw-r--r--   0 runner    (1001) docker     (123)    37132 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/JSON.xise
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.261054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/iseconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/iseconfig/filter.filter
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.261054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Xilinx Vivado/
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Xilinx Vivado/Xilinx Vivado.xpr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.265054 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/ghdl/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.cmd
--rw-r--r--   0 runner    (1001) docker     (123)    33740 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.log
--rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.265054 vunit_hdl-4.6.2/vunit/vhdl/array/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/array/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.265054 vunit_hdl-4.6.2/vunit/vhdl/array/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/array/src/array_pkg.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.265054 vunit_hdl-4.6.2/vunit/vhdl/array/test/
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/array/test/tb_array.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.265054 vunit_hdl-4.6.2/vunit/vhdl/check/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.269054 vunit_hdl-4.6.2/vunit/vhdl/check/src/
--rw-r--r--   0 runner    (1001) docker     (123)   193163 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/src/check.vhd
--rw-r--r--   0 runner    (1001) docker     (123)   105782 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/src/check_api.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/src/check_deprecated_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/src/checker_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/src/checker_pkg.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.277054 vunit_hdl-4.6.2/vunit/vhdl/check/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_equal_real.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_failed.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_false.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_implication.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_next.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_not_unknown.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_one_hot.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_passed.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_relation.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_relation_2008p.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_sequence.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    32863 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_stable.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_zero_one_hot.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_checker.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_deprecated.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_result.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/test/test_support.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.277054 vunit_hdl-4.6.2/vunit/vhdl/check/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    26613 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/tools/generate_check_equal.py
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/check/tools/generate_check_match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.277054 vunit_hdl-4.6.2/vunit/vhdl/com/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.281054 vunit_hdl-4.6.2/vunit/vhdl/com/src/
--rw-r--r--   0 runner    (1001) docker     (123)    23419 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/src/com.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    11504 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/src/com_api.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/src/com_common.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/src/com_context.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/src/com_debug_codec_builder.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    35937 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/src/com_deprecated.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    42072 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/src/com_messenger.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/src/com_string.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/src/com_support.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    26525 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/src/com_types.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.285054 vunit_hdl-4.6.2/vunit/vhdl/com/test/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/test/constants.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/test/custom_types.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/test/more_constants.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    61111 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/test/tb_com.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/test/tb_com_codec.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    19833 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/test/tb_com_deprecated.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/com/test/tb_com_msg_building.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/compile_vunit_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.157054 vunit_hdl-4.6.2/vunit/vhdl/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.285054 vunit_hdl-4.6.2/vunit/vhdl/core/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/core/src/core_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/core/src/stop_body_2008p.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/core/src/stop_body_93-2002.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/core/src/stop_pkg.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.285054 vunit_hdl-4.6.2/vunit/vhdl/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.289054 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.289054 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/api/external_integer_vector_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/api/external_string_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/byte_vector_ptr_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/codec-2008p.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    18954 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/codec.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/codec_builder-2008p.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    13964 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/codec_builder.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/data_types_context.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    11057 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/dict_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_array_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_array_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_vector_ptr_pkg-body-2002p.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_vector_ptr_pkg-body-93.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_vector_ptr_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_vector_ptr_pool_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/queue_pkg-2008p.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/queue_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/queue_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/queue_pool_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/string_ptr_pkg-body-2002p.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/string_ptr_pkg-body-93.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/string_ptr_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/string_ptr_pool_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/src/types.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.289054 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_byte_vector_ptr.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_codec-2008p.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_codec.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_dict.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_integer_array.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_integer_vector_ptr.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_integer_vector_ptr_pool.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_queue-2008p.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_queue.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_queue_pool.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_string_ptr.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_string_ptr_pool.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.289054 vunit_hdl-4.6.2/vunit/vhdl/dictionary/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/dictionary/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.289054 vunit_hdl-4.6.2/vunit/vhdl/dictionary/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/dictionary/src/dictionary.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.289054 vunit_hdl-4.6.2/vunit/vhdl/dictionary/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/dictionary/test/tb_dictionary.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.289054 vunit_hdl-4.6.2/vunit/vhdl/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.289054 vunit_hdl-4.6.2/vunit/vhdl/logging/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/ansi_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/file_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/location_pkg-body-2008m.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/location_pkg-body-2019p.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/location_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/log_deprecated_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/log_handler_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/log_handler_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/log_levels_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/log_levels_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    44107 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/logger_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/logger_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/print_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/src/print_pkg.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.293053 vunit_hdl-4.6.2/vunit/vhdl/logging/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/test/tb_deprecated.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/test/tb_location.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    33408 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/test/tb_log.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/test/tb_log_levels.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/logging/test/test_support_pkg.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/osvvm/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-22 06:11:24.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/.git
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)   270802 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/AlertLogPkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    33976 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (123)   385772 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/CoveragePkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    56384 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/MemoryPkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/MessageListPkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/MessagePkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/NamePkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/NameStorePkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/OsvvmContext.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/OsvvmGlobalPkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/RandomBasePkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    88709 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/RandomPkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/RandomProcedurePkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/ResizePkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/ResolutionPkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)   115778 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/ScoreboardGenericPkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/ScoreboardPkg_int.vhd
--rw-r--r--   0 runner    (1001) docker     (123)   112869 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/ScoreboardPkg_int_c.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/ScoreboardPkg_slv.vhd
--rw-r--r--   0 runner    (1001) docker     (123)   112946 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/ScoreboardPkg_slv_c.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/SortListPkg_int.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    37408 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/TbUtilPkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/TextUtilPkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/TranscriptPkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/VendorCovApiPkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/VendorCovApiPkg_Aldec.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/osvvm/demo/
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/demo/AlertLog_Demo_Global.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/demo/AlertLog_Demo_Hierarchy.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/demo/Demo_Rand.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/osvvm.pro
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-02-22 06:11:25.000000 vunit_hdl-4.6.2/vunit/vhdl/osvvm/osvvm_old.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/path/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/path/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/path/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/path/src/path.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/path/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/path/test/tb_path.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/random/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/random/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/random/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/random/src/random_pkg.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/random/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/random/test/tb_random_pkg.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/run/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/run/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/run/src/
--rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/run/src/run.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/run/src/run_api.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/run/src/run_deprecated_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/run/src/run_types.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/run/src/runner_pkg.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/run/test/
--rw-r--r--   0 runner    (1001) docker     (123)    43944 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/run/test/run_tests.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/run/test/tb_run.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/run/test/tb_watchdog.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/string_ops/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/string_ops/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.297053 vunit_hdl-4.6.2/vunit/vhdl/string_ops/src/
--rw-r--r--   0 runner    (1001) docker     (123)    19248 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/string_ops/src/string_ops.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.301054 vunit_hdl-4.6.2/vunit/vhdl/string_ops/test/
--rw-r--r--   0 runner    (1001) docker     (123)    28595 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/string_ops/test/tb_string_ops.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.301054 vunit_hdl-4.6.2/vunit/vhdl/verification_components/
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.309054 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_master.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_sink.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_slave.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_source.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_stream_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_lite_master.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_lite_master_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_read_slave.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_slave_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_slave_private_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_statistics_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_master.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_monitor.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    32286 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_private_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_protocol_checker.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_slave.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_write_slave.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/bus2memory.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    13129 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/bus_master_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/bus_master_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    17847 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/memory_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/memory_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/memory_utils_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/ram_master.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/signal_checker_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/std_logic_checker.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/stream_master_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/stream_master_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/stream_slave_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/stream_slave_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/sync_pkg-body.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/sync_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/uart_master.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/uart_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/uart_slave.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/vc_context.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/wishbone_master.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/wishbone_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/wishbone_slave.vhd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.317053 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_master.gtkw
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_master.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_slave.gtkw
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_slave.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_stream.gtkw
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_stream.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_stream_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_lite_master.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_read_slave.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_slave_private_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_statistics_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    31309 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_stream.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    21785 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_stream_protocol_checker.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    22640 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_write_slave.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_bus_master_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_memory.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_memory_utils_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_ram_master.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_std_logic_checker.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_sync_pkg.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_uart.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_wishbone_master.gtkw
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_wishbone_master.vhd
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_wishbone_slave.gtkw
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_wishbone_slave.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/vunit_context.vhd
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl/vunit_run_context.vhd
--rw-r--r--   0 runner    (1001) docker     (123)    36633 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vhdl_standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.317053 vunit_hdl-4.6.2/vunit/vivado/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vivado/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.317053 vunit_hdl-4.6.2/vunit/vivado/tcl/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vivado/tcl/extract_compile_order.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vivado/vivado.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-02-22 06:11:23.000000 vunit_hdl-4.6.2/vunit/vunit_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 06:11:36.317053 vunit_hdl-4.6.2/vunit_hdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-02-22 06:11:36.000000 vunit_hdl-4.6.2/vunit_hdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    46034 2023-02-22 06:11:36.000000 vunit_hdl-4.6.2/vunit_hdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 06:11:36.000000 vunit_hdl-4.6.2/vunit_hdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 06:11:36.000000 vunit_hdl-4.6.2/vunit_hdl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 06:11:36.000000 vunit_hdl-4.6.2/vunit_hdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-22 06:11:36.000000 vunit_hdl-4.6.2/vunit_hdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.356518 vunit_hdl-4.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-23 18:15:19.352518 vunit_hdl-4.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:15:19.356518 vunit_hdl-4.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.260511 vunit_hdl-4.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.260511 vunit_hdl-4.7.0/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/acceptance/test_artificial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/acceptance/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/acceptance/test_external_run_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.260511 vunit_hdl-4.7.0/tests/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/lint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/lint/test_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/lint/test_mypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/lint/test_pycodestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/lint/test_pylint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.264511 vunit_hdl-4.7.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/non_utf8_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_activehdl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_cds_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_check_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_dependency_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_ghdl_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44287 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_incisive_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_location_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_modelsim_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_ostools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58076 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_rivierapro_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_simulator_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32550 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_test_bench_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13978 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_test_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48247 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_verilog_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29251 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_verilog_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_verilog_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24982 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_vhdl_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/tests/unit/test_vhdl_standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.268511 vunit_hdl-4.7.0/vunit/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/about.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11454 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/check_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/color_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.268511 vunit_hdl-4.7.0/vunit/com/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/com/codec_datatype_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/com/codec_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/com/codec_vhdl_array_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/com/codec_vhdl_enumeration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/com/codec_vhdl_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/com/codec_vhdl_record_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/dependency_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/design_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/json4vhdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/location_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/ostools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.268511 vunit_hdl-4.7.0/vunit/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/parsing/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/parsing/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.272512 vunit_hdl-4.7.0/vunit/parsing/verilog/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/parsing/verilog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/parsing/verilog/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/parsing/verilog/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/parsing/verilog/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/parsing/verilog/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/persistent_tcl_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24263 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.272512 vunit_hdl-4.7.0/vunit/sim_if/
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/activehdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/cds_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/ghdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/incisive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/modelsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/nvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/rivierapro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/tcl_read_eval_loop.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/sim_if/vsim_simulator_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/source_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.272512 vunit_hdl-4.7.0/vunit/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19745 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/test/bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/test/bench_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/test/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/test/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/test/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10008 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/test/suites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.272512 vunit_hdl-4.7.0/vunit/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    40101 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/ui/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/ui/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/ui/packagefacade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/ui/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/ui/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/ui/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/ui/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/ui/testbench.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.272512 vunit_hdl-4.7.0/vunit/verilog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.256510 vunit_hdl-4.7.0/vunit/verilog/check/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.276512 vunit_hdl-4.7.0/vunit/verilog/check/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/verilog/check/test/check_tb.sv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.276512 vunit_hdl-4.7.0/vunit/verilog/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/verilog/include/vunit_defines.svh
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/verilog/vunit_pkg.sv
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/verilog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/version_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.276512 vunit_hdl-4.7.0/vunit/vhdl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.276512 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-23 18:15:06.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.256510 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.276512 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.276512 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/data/Boards0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/data/Boards1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/data/Boards2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.276512 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/examples/Boards0.vhdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/examples/Boards1.vhdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/examples/Boards2.vhdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/examples/Boards_VUnit.vhdl
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/examples/Encodings_VUnit.vhdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.276512 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/src/Encodings.pkg.vhdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/src/JSON.ctx.vhdl
+-rw-r--r--   0 runner    (1001) docker     (123)    89640 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/src/JSON.pkg.vhdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.276512 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.276512 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/JSONTestSuite.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/TopLevel.vhdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.316515 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_object_key_lone_2nd_surrogate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_1st_surrogate_but_2nd_missing.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_1st_valid_surrogate_2nd_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_UTF-16LE_with_BOM.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_UTF-8_invalid_sequence.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_incomplete_surrogate_and_escape_valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_incomplete_surrogate_pair.json
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_incomplete_surrogates_escape_valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_invalid_lonely_surrogate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_invalid_surrogate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_inverted_surrogates_U+1D11E.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_lone_second_surrogate.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_not_in_unicode_range.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_truncated-utf-8.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_unicode_U+10FFFE_nonchar.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_unicode_U+1FFFE_nonchar.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_unicode_U+FDD0_nonchar.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_string_unicode_U+FFFE_nonchar.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_structure_500_nested_arrays.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/i_structure_UTF-8_BOM_empty_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_1_true_without_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_a_invalid_utf8.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_colon_instead_of_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_comma_after_close.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_comma_and_number.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_double_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_double_extra_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_extra_close.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_extra_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_incomplete.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_incomplete_invalid_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_inner_array_no_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_invalid_utf8.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_items_separated_by_semicolon.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_just_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_just_minus.json
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_missing_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_newlines_unclosed.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_number_and_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_number_and_several_commas.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_spaces_vertical_tab_formfeed.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_star_inside.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_unclosed.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_unclosed_trailing_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_unclosed_with_new_lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_array_unclosed_with_object_inside.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_incomplete_false.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_incomplete_null.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_incomplete_true.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_++.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_+1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_+Inf.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_-01.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_-1.0..json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_-2..json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_-NaN.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_.-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_.2e-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0.1.2.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0.3e+.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0.3e.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0.e1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0_capital_E+.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0_capital_E.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0e+.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_0e.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_1.0e+.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_1.0e-.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_1.0e.json
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_1_000.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_1eE2.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_2.e+3.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_2.e-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_2.e3.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_9.e+.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_Inf.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_NaN.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_U+FF11_fullwidth_digit_one.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_expression.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_hex_1_digit.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_hex_2_digits.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_infinity.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_invalid+-.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_invalid-negative-real.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_invalid-utf-8-in-bigger-int.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_invalid-utf-8-in-exponent.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_invalid-utf-8-in-int.json
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_minus_infinity.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_minus_sign_with_trailing_garbage.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_minus_space_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_neg_int_starting_with_zero.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_neg_real_without_int_part.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_neg_with_garbage_at_end.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_real_garbage_after_e.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_real_with_invalid_utf8_after_e.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_real_without_fractional_part.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_starting_with_dot.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_then_00.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_with_alpha.json
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_with_alpha_char.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_number_with_leading_zero.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_bad_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_bracket_key.json
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_comma_instead_of_colon.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_double_colon.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_emoji.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_garbage_at_end.json
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_key_with_single_quotes.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_missing_colon.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_missing_key.json
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_missing_semicolon.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_missing_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_no-colon.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_non_string_key.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_non_string_key_but_huge_number_instead.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_pi_in_key_and_trailing_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_repeated_null_null.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_several_trailing_commas.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_single_quote.json
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_trailing_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_trailing_comment.json
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_trailing_comment_open.json
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_trailing_comment_slash_open.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_trailing_comment_slash_open_incomplete.json
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_two_commas_in_a_row.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_unquoted_key.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_unterminated-value.json
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_with_single_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_object_with_trailing_garbage.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_single_space.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_1_surrogate_then_escape u.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_1_surrogate_then_escape u1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_1_surrogate_then_escape u1x.json
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_1_surrogate_then_escape.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_UTF8_surrogate_U+D800.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_accentuated_char_no_quotes.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_backslash_00.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_escape_x.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_escaped_backslash_bad.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_escaped_ctrl_char_tab.json
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_escaped_emoji.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_incomplete_escape.json
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_incomplete_escaped_character.json
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_incomplete_surrogate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_incomplete_surrogate_escape_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_invalid-utf-8-in-escape.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_invalid_backslash_esc.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_invalid_unicode_escape.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_invalid_utf-8.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_invalid_utf8_after_escape.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_iso_latin_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_leading_uescaped_thinspace.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_lone_utf8_continuation_byte.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_no_quotes_with_bad_escape.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_overlong_sequence_2_bytes.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_overlong_sequence_6_bytes.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_overlong_sequence_6_bytes_null.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_single_doublequote.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_single_quote.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_single_string_no_double_quotes.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_start_escape_unclosed.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_unescaped_crtl_char.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_unescaped_newline.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_unescaped_tab.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_unicode_CapitalU.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_string_with_trailing_garbage.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100000 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_100000_opening_arrays.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_U+2060_word_joined.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_UTF8_BOM_no_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure__._.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure__null_.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_array_trailing_garbage.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_array_with_extra_array_close.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_array_with_unclosed_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_ascii-unicode-identifier.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_capitalized_True.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_close_unopened_array.json
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_comma_instead_of_closing_brace.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_double_array.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_end_array.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_incomplete_UTF8_BOM.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_lone-invalid-utf-8.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_lone-open-bracket.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_no_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_null-byte-outside-string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_number_with_trailing_garbage.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_object_followed_by_closing_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_object_unclosed_no_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_object_with_comment.json
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_object_with_trailing_garbage.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_apostrophe.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)   250001 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_open_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_open_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_array_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object_close_array.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object_comma.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object_open_array.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object_open_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_object_string_with_apostrophes.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_open_open.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_single_point.json
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_single_star.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_trailing_#.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_uescaped_LF_before_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unclosed_array.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unclosed_array_partial_null.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unclosed_array_unfinished_false.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unclosed_array_unfinished_true.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unclosed_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_unicode-identifier.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_whitespace_U+2060_word_joiner.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/n_structure_whitespace_formfeed.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_arraysWithSpaces.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_empty-string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_empty.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_ending_with_newline.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_false.json
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_heterogeneous.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_null.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_with_1_and_newline.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_with_leading_space.json
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_with_several_null.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_array_with_trailing_space.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_0e+1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_0e1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_after_space.json
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_double_close_to_zero.json
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_double_huge_neg_exp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_huge_exp.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_int_with_exp.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_minus_zero.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_neg_int_huge_exp.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_negative_int.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_negative_one.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_negative_zero.json
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_pos_double_huge_exp.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_capital_e.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_capital_e_neg_exp.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_capital_e_pos_exp.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_exponent.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_fraction_exponent.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_neg_exp.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_neg_overflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_pos_exponent.json
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_pos_overflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_real_underflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_simple_int.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_simple_real.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_too_big_neg_int.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_too_big_pos_int.json
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_number_very_big_negative_int.json
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_basic.json
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_duplicated_key.json
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_duplicated_key_and_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_empty.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_empty_key.json
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_escaped_null_in_key.json
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_extreme_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_long_strings.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_string_unicode.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_object_with_newlines.json
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_1_2_3_bytes_UTF-8_sequences.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_accepted_surrogate_pair.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_accepted_surrogate_pairs.json
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_allowed_escapes.json
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_backslash_and_u_escaped_zero.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_backslash_doublequotes.json
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_comments.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_double_escape_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_double_escape_n.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_escaped_control_character.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_escaped_noncharacter.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_in_array.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_in_array_with_leading_space.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_last_surrogates_1_and_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_newline_uescaped.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_nonCharacterInUTF-8_U+10FFFF.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_nonCharacterInUTF-8_U+1FFFF.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_nonCharacterInUTF-8_U+FFFF.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_null_escape.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_one-byte-utf-8.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_pi.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_simple_ascii.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_space.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_surrogates_U+1D11E_MUSICAL_SYMBOL_G_CLEF.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_three-byte-utf-8.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_two-byte-utf-8.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_u+2028_line_sep.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_u+2029_par_sep.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_uEscape.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unescaped_char_delete.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicode.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicodeEscapedBackslash.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicode_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicode_U+200B_ZERO_WIDTH_SPACE.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicode_U+2064_invisible_plus.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_unicode_escaped_double_quote.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_utf16BE_no_BOM.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_utf16LE_no_BOM.json
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_utf8.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_string_with_del_character.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_false.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_int.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_negative_real.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_null.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_lonely_true.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_string_empty.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_trailing_newline.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_true_in_array.json
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_parsing/y_structure_whitespace_array.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_1.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_1.000000000000000005.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_1000000000000000.json
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_10000000000000000999.json
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_1e-999.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/number_1e6.json
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/object_key_nfc_nfd.json
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/object_key_nfd_nfc.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/object_same_key_different_values.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/object_same_key_same_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/object_same_key_unclear_values.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_1_escaped_invalid_codepoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_1_invalid_codepoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_2_escaped_invalid_codepoints.json
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_2_invalid_codepoints.json
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_3_escaped_invalid_codepoints.json
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_3_invalid_codepoints.json
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/test_transform/string_with_escaped_NULL.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Lattice/Lattice.ldf
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Lattice/Lattice.lpf
+-rw-r--r--   0 runner    (1001) docker     (123)    13632 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Lattice/Lattice1.sty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Lattice/impl_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Lattice/impl_1/Lattice_impl_1.lpf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Lattice/impl_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Lattice/impl_2/Lattice_impl_2.lpf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/QuestaSim/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/QuestaSim/Boards2.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)    23797 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/QuestaSim/Boards2.log
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/VUnit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/VUnit/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/
+-rw-r--r--   0 runner    (1001) docker     (123)    37132 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/JSON.xise
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/iseconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/iseconfig/filter.filter
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Xilinx Vivado/
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Xilinx Vivado/Xilinx Vivado.xpr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/ghdl/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)    33740 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.log
+-rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-04-23 18:15:08.000000 vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/array/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/array/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/array/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/array/src/array_pkg.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/array/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/array/test/tb_array.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.320515 vunit_hdl-4.7.0/vunit/vhdl/check/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   229146 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/src/check.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)   124043 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/src/check_api.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/src/check_deprecated_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/src/checker_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/src/checker_pkg.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.324516 vunit_hdl-4.7.0/vunit/vhdl/check/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_equal_real.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_failed.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_false.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_implication.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    14267 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_next.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_not_unknown.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_one_hot.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_passed.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_relation.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_relation_2008p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_sequence.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    32863 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_stable.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_zero_one_hot.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_checker.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_deprecated.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_result.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/test/test_support.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.324516 vunit_hdl-4.7.0/vunit/vhdl/check/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    33230 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/tools/generate_check_equal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/check/tools/generate_check_match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.324516 vunit_hdl-4.7.0/vunit/vhdl/com/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.324516 vunit_hdl-4.7.0/vunit/vhdl/com/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/src/com.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/src/com_api.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/src/com_common.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/src/com_context.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/src/com_debug_codec_builder.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    35996 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/src/com_deprecated.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    45149 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/src/com_messenger.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/src/com_string.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/src/com_support.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    27050 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/src/com_types.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.324516 vunit_hdl-4.7.0/vunit/vhdl/com/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/test/constants.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/test/custom_types.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/test/more_constants.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    66599 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/test/tb_com.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/test/tb_com_codec.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    19833 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/test/tb_com_deprecated.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/com/test/tb_com_msg_building.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/compile_vunit_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.256510 vunit_hdl-4.7.0/vunit/vhdl/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.328516 vunit_hdl-4.7.0/vunit/vhdl/core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/core/src/core_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/core/src/stop_body_2008p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/core/src/stop_body_93-2002.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/core/src/stop_pkg.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.328516 vunit_hdl-4.7.0/vunit/vhdl/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.332516 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.332516 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/api/external_integer_vector_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/api/external_string_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/byte_vector_ptr_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/codec-2008p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    18954 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/codec.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/codec_builder-2008p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    13964 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/codec_builder.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/data_types_context.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/data_types_private_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/dict_pkg-2008p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    24016 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/dict_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/dict_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/event_common_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/event_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/event_private_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/id_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_array_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_array_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_vector_ptr_pkg-body-2002p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_vector_ptr_pkg-body-93.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_vector_ptr_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_vector_ptr_pool_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/queue_pkg-2008p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/queue_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/queue_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/queue_pool_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/string_ptr_pkg-body-2002p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/string_ptr_pkg-body-93.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/string_ptr_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/string_ptr_pool_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/src/types.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.332516 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_byte_vector_ptr.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_codec-2008p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_codec.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_dict-2008p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_dict.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_event_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_event_private_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    12814 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_id.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_integer_array.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_integer_vector_ptr.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_integer_vector_ptr_pool.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_queue-2008p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_queue.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_queue_pool.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_string_ptr.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_string_ptr_pool.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.332516 vunit_hdl-4.7.0/vunit/vhdl/data_types/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/data_types/tools/generate_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.332516 vunit_hdl-4.7.0/vunit/vhdl/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/dictionary/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.332516 vunit_hdl-4.7.0/vunit/vhdl/dictionary/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/dictionary/src/dictionary.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.332516 vunit_hdl-4.7.0/vunit/vhdl/dictionary/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/dictionary/test/tb_dictionary.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.332516 vunit_hdl-4.7.0/vunit/vhdl/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.336516 vunit_hdl-4.7.0/vunit/vhdl/logging/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/ansi_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/file_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/location_pkg-body-2008m.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/location_pkg-body-2019p.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/location_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/log_deprecated_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/log_handler_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/log_handler_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/log_levels_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/log_levels_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    43627 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/logger_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    17437 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/logger_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/print_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/src/print_pkg.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.336516 vunit_hdl-4.7.0/vunit/vhdl/logging/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/test/tb_deprecated.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/test/tb_location.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    35135 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/test/tb_log.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/test/tb_log_levels.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/logging/test/test_support_pkg.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.340517 vunit_hdl-4.7.0/vunit/vhdl/osvvm/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-23 18:15:06.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/.git
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)   285835 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/AlertLogPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    36024 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)   436825 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/CoveragePkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    56709 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/MemoryPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/MessageListPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/MessagePkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/NamePkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/NameStorePkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/OsvvmContext.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/OsvvmGlobalPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24542 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/RandomBasePkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    89151 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/RandomPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/RandomProcedurePkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/ReportPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/ResizePkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/ResolutionPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)   115778 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/ScoreboardGenericPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/ScoreboardPkg_int.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)   112869 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/ScoreboardPkg_int_c.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/ScoreboardPkg_slv.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)   112946 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/ScoreboardPkg_slv_c.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/SortListPkg_int.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    37408 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/TbUtilPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/TextUtilPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/TranscriptPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/VendorCovApiPkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/VendorCovApiPkg_Aldec.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.340517 vunit_hdl-4.7.0/vunit/vhdl/osvvm/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/demo/AlertLog_Demo_Global.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/demo/AlertLog_Demo_Hierarchy.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/demo/Demo_Rand.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/osvvm.pro
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-23 18:15:09.000000 vunit_hdl-4.7.0/vunit/vhdl/osvvm/osvvm_old.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.340517 vunit_hdl-4.7.0/vunit/vhdl/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/path/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/path/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/path/src/path.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/path/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/path/test/tb_path.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/random/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/random/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/random/src/random_pkg.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/random/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/random/test/tb_random_pkg.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/run/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/run/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/run/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/run/src/run.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/run/src/run_api.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/run/src/run_deprecated_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/run/src/run_types.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    23607 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/run/src/runner_pkg.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/run/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    44951 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/run/test/run_tests.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/run/test/tb_run.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/run/test/tb_watchdog.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/string_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/string_ops/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/string_ops/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/string_ops/src/string_ops.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/string_ops/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    28595 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/string_ops/test/tb_string_ops.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.344517 vunit_hdl-4.7.0/vunit/vhdl/verification_components/
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.348518 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_master.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_sink.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_slave.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_source.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_stream_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_lite_master.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_lite_master_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_read_slave.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    14153 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_slave_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_slave_private_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_statistics_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_master.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_monitor.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    32286 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_private_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_protocol_checker.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_slave.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_write_slave.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/bus2memory.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    13129 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/bus_master_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/bus_master_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    17847 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/memory_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/memory_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/memory_utils_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/ram_master.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/signal_checker_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/std_logic_checker.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/stream_master_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/stream_master_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/stream_slave_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/stream_slave_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/sync_pkg-body.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/sync_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/uart_master.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/uart_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/uart_slave.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/vc_context.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/wishbone_master.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/wishbone_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/wishbone_slave.vhd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.352518 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_master.gtkw
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_master.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_slave.gtkw
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_slave.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_stream.gtkw
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_stream.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_stream_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    14700 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_lite_master.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_read_slave.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_slave_private_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_statistics_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_stream.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    21763 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_stream_protocol_checker.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    22640 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_write_slave.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_bus_master_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_memory.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_memory_utils_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_ram_master.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_std_logic_checker.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_sync_pkg.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_uart.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_wishbone_master.gtkw
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_wishbone_master.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_wishbone_slave.gtkw
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_wishbone_slave.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/vunit_context.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl/vunit_run_context.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)    37274 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vhdl_standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.352518 vunit_hdl-4.7.0/vunit/vivado/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vivado/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.352518 vunit_hdl-4.7.0/vunit/vivado/tcl/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vivado/tcl/extract_compile_order.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vivado/vivado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-23 18:15:05.000000 vunit_hdl-4.7.0/vunit/vunit_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:15:19.352518 vunit_hdl-4.7.0/vunit_hdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-23 18:15:19.000000 vunit_hdl-4.7.0/vunit_hdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-04-23 18:15:19.000000 vunit_hdl-4.7.0/vunit_hdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:15:19.000000 vunit_hdl-4.7.0/vunit_hdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:15:19.000000 vunit_hdl-4.7.0/vunit_hdl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 18:15:19.000000 vunit_hdl-4.7.0/vunit_hdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:15:19.000000 vunit_hdl-4.7.0/vunit_hdl.egg-info/top_level.txt
```

### Comparing `vunit_hdl-4.6.2/LICENSE.rst` & `vunit_hdl-4.7.0/LICENSE.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 **VUnit**, except for the projects below, is released under the terms of `Mozilla Public License, v. 2.0`_.
-|copy| 2014-2021 Lars Asplund, lars.anders.asplund@gmail.com.
+|copy| 2014-2023 Lars Asplund, lars.anders.asplund@gmail.com.
 
 The following libraries are `redistributed`_ with VUnit for convenience:
 
 * **OSVVM** (``vunit/vhdl/osvvm``): these files are licensed under the terms of `Apache License, v 2.0`_,
-  |copy| 2010 - 2021 by `SynthWorks Design Inc`_. All rights reserved.
+  |copy| 2010 - 2023 by `SynthWorks Design Inc`_. All rights reserved.
 
 * **JSON-for-VHDL** (``vunit/vhdl/JSON-for-VHDL``): these files are licensed under the terms of `Apache License,
-  v 2.0`_, |copy| 2015 - 2021 Patrick Lehmann.
+  v 2.0`_, |copy| 2015 - 2023 Patrick Lehmann.
 
 The font used in VUnit's logo and illustrations is 'Tratex', the traffic sign typeface used on swedish road signs:
 
 - `transportstyrelsen.se: Teckensnitt <https://transportstyrelsen.se/sv/vagtrafik/Trafikregler/Om-vagmarken/Teckensnitt/>`__
 - `Wikipedia: Tratex <https://en.wikipedia.org/wiki/Tratex>`__
```

### Comparing `vunit_hdl-4.6.2/PKG-INFO` & `vunit_hdl-4.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: vunit_hdl
-Version: 4.6.2
+Version: 4.7.0
 Summary: VUnit is an open source unit testing framework for VHDL/SystemVerilog.
 Home-page: https://github.com/VUnit/vunit
 Author: Lars Asplund
 Author-email: lars.anders.asplund@gmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
@@ -32,23 +33,23 @@
 `Website <https://vunit.github.io>`__
 
 Contributing in the form of code, feedback, ideas or bug reports are
 welcome. Read our `contribution guide
 <https://vunit.github.io/contributing.html>`__ to get started.
 
 **VUnit**, except for the projects below, is released under the terms of `Mozilla Public License, v. 2.0`_.
-|copy| 2014-2021 Lars Asplund, lars.anders.asplund@gmail.com.
+|copy| 2014-2023 Lars Asplund, lars.anders.asplund@gmail.com.
 
 The following libraries are `redistributed`_ with VUnit for convenience:
 
 * **OSVVM** (``vunit/vhdl/osvvm``): these files are licensed under the terms of `Apache License, v 2.0`_,
-  |copy| 2010 - 2021 by `SynthWorks Design Inc`_. All rights reserved.
+  |copy| 2010 - 2023 by `SynthWorks Design Inc`_. All rights reserved.
 
 * **JSON-for-VHDL** (``vunit/vhdl/JSON-for-VHDL``): these files are licensed under the terms of `Apache License,
-  v 2.0`_, |copy| 2015 - 2021 Patrick Lehmann.
+  v 2.0`_, |copy| 2015 - 2023 Patrick Lehmann.
 
 The font used in VUnit's logo and illustrations is 'Tratex', the traffic sign typeface used on swedish road signs:
 
 - `transportstyrelsen.se: Teckensnitt <https://transportstyrelsen.se/sv/vagtrafik/Trafikregler/Om-vagmarken/Teckensnitt/>`__
 - `Wikipedia: Tratex <https://en.wikipedia.org/wiki/Tratex>`__
```

### Comparing `vunit_hdl-4.6.2/README.md` & `vunit_hdl-4.7.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 <p align="center">
+  <a title="PyPI vunit_hdl"
+     href="https://pypi.org/project/vunit-hdl/"
+  ><img src="https://img.shields.io/pypi/v/vunit_hdl?longCache=true&style=flat-square&label=PyPI&logo=PyPI&logoColor=FFF"
+  /></a><!--
+  -->
   <a title="vunit.github.io"
      href="http://vunit.github.io"
   ><img src="https://img.shields.io/website.svg?label=vunit.github.io&longCache=true&style=flat-square&url=http%3A%2F%2Fvunit.github.io%2Findex.html"
   /></a><!--
   -->
   <a title="Join the chat at https://gitter.im/VUnit/vunit"
      href="https://gitter.im/VUnit/vunit"
-  ><img src="https://img.shields.io/gitter/room/VUnit/vunit.svg?longCache=true&style=flat-square&logo=gitter&logoColor=4db797&color=4db797"
+  ><img src="https://img.shields.io/gitter/room/VUnit/vunit.svg?longCache=true&style=flat-square&logo=gitter&logoColor=fff&color=4db797"
   /></a><!--
   -->
   <a title="@VUnitFramework"
      href="https://www.twitter.com/VUnitFramework"
   ><img src="https://img.shields.io/twitter/follow/VUnitFramework.svg?longCache=true&style=flat-square&color=1DA1F2&label=%40VUnitFramework&logo=twitter&logoColor=fff"
   /></a>
 </p>
 
 <p align="center">
-  <a title="PyPI vunit_hdl"
-     href="https://pypi.org/project/vunit-hdl/"
-  ><img src="https://img.shields.io/pypi/v/vunit_hdl?longCache=true&style=flat-square&label=PyPI&logo=PyPI&logoColor=FFF"
-  /></a><!--
-  -->
+  <a href="http://vunit.github.io"><img width="450px" src="docs/_static/VUnit_banner.png"/></a>
+</p>
+
+<p align="center">
   <a title="Commits since latest release"
      href="https://github.com/VUnit/vunit/releases"
   ><img src="https://img.shields.io/github/commits-since/VUnit/vunit/latest.svg?longCache=true&style=flat-square&logo=git&logoColor=fff"
   /></a><!--
   -->
   <a title="'docs' workflow Status"
-     href="https://github.com/VUnit/vunit/actions?query=workflow%3Adocs"
-  ><img alt="'docs' workflow Status" src="https://img.shields.io/github/workflow/status/VUnit/vunit/docs/master?longCache=true&style=flat-square&label=docs"
+     href="https://github.com/VUnit/vunit/actions/workflows/docs.yml"
+  ><img alt="'docs' workflow Status" src="https://img.shields.io/github/actions/workflow/status/VUnit/vunit/docs.yml?branch=master&longCache=true&style=flat-square&label=docs&logo=GitHub%20Actions&logoColor=fff"
   /></a><!--
   -->
   <a title="'images' workflow Status"
-     href="https://github.com/VUnit/vunit/actions?query=workflow%3Aimages"
-  ><img alt="'images' workflow Status" src="https://img.shields.io/github/workflow/status/VUnit/vunit/images/master?longCache=true&style=flat-square&label=imgs"
+     href="https://github.com/VUnit/vunit/actions/workflows/images.yml"
+  ><img alt="'images' workflow Status" src="https://img.shields.io/github/actions/workflow/status/VUnit/vunit/images.yml?branch=master&longCache=true&style=flat-square&label=imgs&logo=GitHub%20Actions&logoColor=fff"
   /></a><!--
   -->
   <a title="'push' workflow Status"
-     href="https://github.com/VUnit/vunit/actions?query=workflow%3Apush"
-  ><img alt="'push' workflow Status" src="https://img.shields.io/github/workflow/status/VUnit/vunit/push/master?longCache=true&style=flat-square&label=push"
+     href="https://github.com/VUnit/vunit/actions/workflows/push.yml"
+  ><img alt="'push' workflow Status" src="https://img.shields.io/github/actions/workflow/status/VUnit/vunit/push.yml?branch=master&longCache=true&style=flat-square&label=push&logo=GitHub%20Actions&logoColor=fff"
   /></a><!--
   -->
   <a title="'coverage' workflow Status"
-     href="https://github.com/VUnit/vunit/actions?query=workflow%3Acoverage"
-  ><img alt="'coverage' workflow Status" src="https://img.shields.io/github/workflow/status/VUnit/vunit/coverage/master?longCache=true&style=flat-square&label=coverage"
+     href="https://github.com/VUnit/vunit/actions/workflows/coverage.yml"
+  ><img alt="'coverage' workflow Status" src="https://img.shields.io/github/actions/workflow/status/VUnit/vunit/coverage.yml?branch=master&longCache=true&style=flat-square&label=coverage&logo=GitHub%20Actions&logoColor=fff"
   /></a>
 </p>
 
 **VUnit** is an [open source](LICENSE.rst) unit testing framework for VHDL/SystemVerilog. It features the functionality
 needed to realize continuous and automated testing of your HDL code. VUnit doesn't replace but rather complements
 traditional testing methodologies by supporting a *test early and often* approach through automation.
 **Read more** [about VUnit](http://vunit.github.io/about.html).
 
 Contributing in the form of code, docs, feedback, ideas or bug reports is welcome.
-Read our [contribution guide](https://vunit.github.io/contributing.html) to get started.
+Read our [contributing guide](https://vunit.github.io/contributing.html) to get started.
 
 <p align="center">
   <a href="http://vunit.github.io"><img width="550px" src="docs/_static/vunit_demo.gif"/></a>
 </p>
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-                           [https://img.shields.io/
+      [https://img.shields.io/pypi/v/vunit_hdl?longCache=true&style=flat-
+      square&label=PyPI&logo=PyPI&logoColor=FFF] [https://img.shields.io/
          website.svg?label=vunit.github.io&longCache=true&style=flat-
 square&url=http%3A%2F%2Fvunit.github.io%2Findex.html] [https://img.shields.io/
             gitter/room/VUnit/vunit.svg?longCache=true&style=flat-
-  square&logo=gitter&logoColor=4db797&color=4db797] [https://img.shields.io/
-         twitter/follow/VUnitFramework.svg?longCache=true&style=flat-
+square&logo=gitter&logoColor=fff&color=4db797] [https://img.shields.io/twitter/
+             follow/VUnitFramework.svg?longCache=true&style=flat-
     square&color=1DA1F2&label=%40VUnitFramework&logo=twitter&logoColor=fff]
-      [https://img.shields.io/pypi/v/vunit_hdl?longCache=true&style=flat-
-  square&label=PyPI&logo=PyPI&logoColor=FFF] [https://img.shields.io/github/
-        commits-since/VUnit/vunit/latest.svg?longCache=true&style=flat-
-  square&logo=git&logoColor=fff] ['docs'_workflow_Status] ['images'_workflow
-         Status] ['push'_workflow_Status] ['coverage'_workflow_Status]
+                        [docs/_static/VUnit_banner.png]
+           [https://img.shields.io/github/commits-since/VUnit/vunit/
+  latest.svg?longCache=true&style=flat-square&logo=git&logoColor=fff] ['docs'
+     workflow_Status] ['images'_workflow_Status] ['push'_workflow_Status]
+                         ['coverage'_workflow_Status]
 **VUnit** is an [open source](LICENSE.rst) unit testing framework for VHDL/
 SystemVerilog. It features the functionality needed to realize continuous and
 automated testing of your HDL code. VUnit doesn't replace but rather
 complements traditional testing methodologies by supporting a *test early and
 often* approach through automation. **Read more** [about VUnit](http://
 vunit.github.io/about.html). Contributing in the form of code, docs, feedback,
-ideas or bug reports is welcome. Read our [contribution guide](https://
+ideas or bug reports is welcome. Read our [contributing guide](https://
 vunit.github.io/contributing.html) to get started.
                          [docs/_static/vunit_demo.gif]
```

### Comparing `vunit_hdl-4.6.2/setup.py` & `vunit_hdl-4.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     zip_safe=False,
     url="https://github.com/VUnit/vunit",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Natural Language :: English",
         "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
```

### Comparing `vunit_hdl-4.6.2/tests/acceptance/test_artificial.py` & `vunit_hdl-4.7.0/tests/acceptance/test_artificial.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,19 +129,19 @@
                 ("passed", "lib.tb_magic_paths.Test magic paths are correct"),
                 ("passed", "lib.tb_with_define.test 1"),
                 ("failed", "lib.tb_fail_on_warning.fail"),
                 ("failed", "lib.tb_fail_on_fatal_and_early_finish.fatal0"),
                 ("failed", "lib.tb_fail_on_fatal_and_early_finish.fatal1"),
                 ("failed", "lib.tb_fail_on_fatal_and_early_finish.finish0"),
                 ("failed", "lib.tb_fail_on_fatal_and_early_finish.finish1"),
-                ("passed", "lib.tb_with_parameter_config.Test 0"),
-                ("passed", "lib.tb_with_parameter_config.cfg.Test 1"),
-                ("passed", "lib.tb_with_parameter_config.Test 2"),
-                ("passed", "lib.tb_with_parameter_config.cfg.Test 3"),
-                ("passed", "lib.tb_with_parameter_config.cfg.Test 4"),
+                ("passed", "lib2.tb_with_parameter_config.Test 0"),
+                ("passed", "lib2.tb_with_parameter_config.cfg.Test 1"),
+                ("passed", "lib2.tb_with_parameter_config.Test 2"),
+                ("passed", "lib2.tb_with_parameter_config.cfg.Test 3"),
+                ("passed", "lib2.tb_with_parameter_config.cfg.Test 4"),
                 ("passed", "lib.tb_same_sim_all_pass.cfg.Test 1"),
                 ("passed", "lib.tb_same_sim_all_pass.cfg.Test 2"),
                 ("passed", "lib.tb_same_sim_all_pass.cfg.Test 3"),
                 ("passed", "lib.tb_same_sim_some_fail.Test 1"),
                 ("failed", "lib.tb_same_sim_some_fail.Test 2"),
                 ("skipped", "lib.tb_same_sim_some_fail.Test 3"),
                 ("passed", "lib.tb_with_runner.pass"),
@@ -196,15 +196,15 @@
     ("passed", "lib.tb_same_sim_all_pass.cfg.Test 3"),
     ("passed", "lib.tb_same_sim_some_fail.Test 1"),
     ("failed", "lib.tb_same_sim_some_fail.Test 2"),
     ("skipped", "lib.tb_same_sim_some_fail.Test 3"),
     ("passed", "lib.tb_with_checks.Test passing check"),
     ("failed", "lib.tb_with_checks.Test failing check"),
     ("failed", "lib.tb_with_checks.Test non-stopping failing check"),
-    ("passed", "lib.tb_set_generic.all"),
+    ("passed", "lib2.tb_set_generic.all"),
     ("passed", "lib.tb_with_generic_config.Test 0"),
     ("passed", "lib.tb_with_generic_config.cfg.Test 1"),
     ("passed", "lib.tb_with_generic_config.Test 2"),
     ("passed", "lib.tb_with_generic_config.cfg.Test 3"),
     ("passed", "lib.tb_with_generic_config.cfg.Test 4"),
     ("passed", "lib.tb_no_generic_override.all"),
     ("passed", "lib.tb_ieee_warning.pass"),
```

### Comparing `vunit_hdl-4.6.2/tests/acceptance/test_dependencies.py` & `vunit_hdl-4.7.0/tests/acceptance/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/acceptance/test_external_run_scripts.py` & `vunit_hdl-4.7.0/tests/acceptance/test_external_run_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,18 @@
             self.report_file,
             [
                 ("passed", "tb_lib.tb_composite_generics.VGA.Test 1"),
                 ("passed", "tb_lib.tb_composite_generics.tiny.Test 1"),
             ],
         )
 
-    @mark.skipif(not simulator_is("ghdl"), reason="Support complex JSON strings as generic")
+    @mark.xfail(
+        not (simulator_is("ghdl") or simulator_is("nvc")),
+        reason="Support complex JSON strings as generic",
+    )
     def test_vhdl_json4vhdl_example_project(self):
         self.check(ROOT / "examples/vhdl/json4vhdl/run.py")
 
     def test_vhdl_array_example_project(self):
         self.check(ROOT / "examples/vhdl/array/run.py")
 
     @mark.xfail(
```

### Comparing `vunit_hdl-4.6.2/tests/common.py` & `vunit_hdl-4.7.0/tests/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 @contextlib.contextmanager
 def create_tempdir(path: Path = None):
     """
     Create a temporary directory that is removed after the unit test
     """
 
     if path is None:
-        path = Path(__file__).parent / ("tempdir_%i" % random.randint(0, 2 ** 64 - 1))
+        path = Path(__file__).parent / ("tempdir_%i" % random.randint(0, 2**64 - 1))
 
     if path.exists():
         shutil.rmtree(path)
 
     os.makedirs(str(path))
 
     try:
```

### Comparing `vunit_hdl-4.6.2/tests/lint/test_license.py` & `vunit_hdl-4.7.0/tests/lint/test_license.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/lint/test_mypy.py` & `vunit_hdl-4.7.0/tests/lint/test_mypy.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/lint/test_pycodestyle.py` & `vunit_hdl-4.7.0/tests/lint/test_pycodestyle.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/lint/test_pylint.py` & `vunit_hdl-4.7.0/tests/lint/test_pylint.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_activehdl_interface.py` & `vunit_hdl-4.7.0/tests/unit/test_activehdl_interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,20 +44,20 @@
 class TestActiveHDLInterface(unittest.TestCase):
     """
     Test the ActiveHDL interface
     """
 
     @mock.patch("vunit.sim_if.check_output", autospec=True, return_value="")
     @mock.patch("vunit.sim_if.activehdl.Process", autospec=True)
-    def test_compile_project_vhdl_2008(self, process, check_output):
+    def _test_compile_project_vhdl(self, standard, process, check_output):
         simif = ActiveHDLInterface(prefix="prefix", output_path=self.output_path)
         project = Project()
         project.add_library("lib", "lib_path")
         write_file("file.vhd", "")
-        project.add_source_file("file.vhd", "lib", file_type="vhdl", vhdl_standard=VHDL.standard("2008"))
+        project.add_source_file("file.vhd", "lib", file_type="vhdl", vhdl_standard=VHDL.standard(standard))
         simif.compile_project(project)
         process.assert_any_call(
             [str(Path("prefix") / "vlib"), "lib", "lib_path"],
             cwd=self.output_path,
             env=simif.get_env(),
         )
         process.assert_called_with(
@@ -67,87 +67,33 @@
         )
         check_output.assert_called_once_with(
             [
                 str(Path("prefix") / "vcom"),
                 "-quiet",
                 "-j",
                 self.output_path,
-                "-2008",
+                f"-{standard}",
                 "-work",
                 "lib",
                 "file.vhd",
             ],
             env=simif.get_env(),
         )
 
-    @mock.patch("vunit.sim_if.check_output", autospec=True, return_value="")
-    @mock.patch("vunit.sim_if.activehdl.Process", autospec=True)
-    def test_compile_project_vhdl_2002(self, process, check_output):
-        simif = ActiveHDLInterface(prefix="prefix", output_path=self.output_path)
-        project = Project()
-        project.add_library("lib", "lib_path")
-        write_file("file.vhd", "")
-        project.add_source_file("file.vhd", "lib", file_type="vhdl", vhdl_standard=VHDL.standard("2002"))
-        simif.compile_project(project)
-        process.assert_any_call(
-            [str(Path("prefix") / "vlib"), "lib", "lib_path"],
-            cwd=self.output_path,
-            env=simif.get_env(),
-        )
-        process.assert_called_with(
-            [str(Path("prefix") / "vmap"), "lib", "lib_path"],
-            cwd=self.output_path,
-            env=simif.get_env(),
-        )
-        check_output.assert_called_once_with(
-            [
-                str(Path("prefix") / "vcom"),
-                "-quiet",
-                "-j",
-                self.output_path,
-                "-2002",
-                "-work",
-                "lib",
-                "file.vhd",
-            ],
-            env=simif.get_env(),
-        )
+    def test_compile_project_vhdl_2019(self):
+        self._test_compile_project_vhdl("2019")
 
-    @mock.patch("vunit.sim_if.check_output", autospec=True, return_value="")
-    @mock.patch("vunit.sim_if.activehdl.Process", autospec=True)
-    def test_compile_project_vhdl_93(self, process, check_output):
-        simif = ActiveHDLInterface(prefix="prefix", output_path=self.output_path)
-        project = Project()
-        project.add_library("lib", "lib_path")
-        write_file("file.vhd", "")
-        project.add_source_file("file.vhd", "lib", file_type="vhdl", vhdl_standard=VHDL.standard("93"))
-        simif.compile_project(project)
-        process.assert_any_call(
-            [str(Path("prefix") / "vlib"), "lib", "lib_path"],
-            cwd=self.output_path,
-            env=simif.get_env(),
-        )
-        process.assert_called_with(
-            [str(Path("prefix") / "vmap"), "lib", "lib_path"],
-            cwd=self.output_path,
-            env=simif.get_env(),
-        )
-        check_output.assert_called_once_with(
-            [
-                str(Path("prefix") / "vcom"),
-                "-quiet",
-                "-j",
-                self.output_path,
-                "-93",
-                "-work",
-                "lib",
-                "file.vhd",
-            ],
-            env=simif.get_env(),
-        )
+    def test_compile_project_vhdl_2008(self):
+        self._test_compile_project_vhdl("2008")
+
+    def test_compile_project_vhdl_2002(self):
+        self._test_compile_project_vhdl("2002")
+
+    def test_compile_project_vhdl_93(self):
+        self._test_compile_project_vhdl("93")
 
     @mock.patch("vunit.sim_if.check_output", autospec=True, return_value="")
     @mock.patch("vunit.sim_if.activehdl.Process", autospec=True)
     def test_compile_project_vhdl_extra_flags(self, process, check_output):
         simif = ActiveHDLInterface(prefix="prefix", output_path=self.output_path)
         project = Project()
         project.add_library("lib", "lib_path")
```

### Comparing `vunit_hdl-4.6.2/tests/unit/test_builtins.py` & `vunit_hdl-4.7.0/tests/unit/test_builtins.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_cds_file.py` & `vunit_hdl-4.7.0/tests/unit/test_cds_file.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_check_preprocessor.py` & `vunit_hdl-4.7.0/tests/unit/test_check_preprocessor.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_configuration.py` & `vunit_hdl-4.7.0/tests/unit/test_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
             self._call_post_check,
             post_check,
             output_path="output_path",
             read_output=read_output,
         )
 
     def test_call_post_check_with_output(self):
-
         output_string = "123___foo\n\nbar"
 
         def read_output():
             """
             Should never be called
             """
             return output_string
```

### Comparing `vunit_hdl-4.6.2/tests/unit/test_csv_logs.py` & `vunit_hdl-4.7.0/tests/unit/test_csv_logs.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_database.py` & `vunit_hdl-4.7.0/tests/unit/test_database.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_dependency_graph.py` & `vunit_hdl-4.7.0/tests/unit/test_dependency_graph.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_ghdl_interface.py` & `vunit_hdl-4.7.0/tests/unit/test_ghdl_interface.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_incisive_interface.py` & `vunit_hdl-4.7.0/tests/unit/test_incisive_interface.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_location_preprocessor.py` & `vunit_hdl-4.7.0/tests/unit/test_location_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,60 +111,60 @@
 another_sub_prog("6");
 sub_prog_2;
 """
         self._verify_result(code, expected_result=code)
 
     def test_that_sub_program_declarations_are_ignored(self):
         code = """
-procedure sub_prog(foo1);
- function  sub_prog (foo3) ;
+PROcedure sub_prog(foo1);
+ functION  sub_prog (foo3) ;
 """
         self._verify_result(code, expected_result=code)
 
     def test_that_sub_program_definitions_are_ignored(self):
         code = """
-procedure sub_prog(foo4) is
+procedURE sub_prog(foo4) is
 begin
     null;
 end;
-function sub_prog(foo4) return boolean is
+funCTIon sub_prog(foo4) return boolean is
 begin
     return true;
 end;
 """
 
         self._verify_result(code, expected_result=code)
 
     def test_that_already_located_calls_are_left_untouched(self):
         code = """
-procedure sub_prog(foo4) is
+proCEDure sub_prog(foo4) is
 begin
     sub_prog("foo", line_num=> 17);
 end;
-procedure sub_prog(foo4) is
+prOCedure sub_prog(foo4) is
 begin
     sub_prog("foo",
              file_name=>"foo.vhd");
 end;
-procedure sub_prog(foo4) is
+proceDUre sub_prog(foo4) is
 begin
     sub_prog("foo", line_num => 17, file_name => "foo.vhd");
 end;
 """
         expected_result = """
-procedure sub_prog(foo4) is
+proCEDure sub_prog(foo4) is
 begin
     sub_prog("foo", line_num=> 17, file_name => "foo.vhd");
 end;
-procedure sub_prog(foo4) is
+prOCedure sub_prog(foo4) is
 begin
     sub_prog("foo",
              file_name=>"foo.vhd", line_num => 8);
 end;
-procedure sub_prog(foo4) is
+proceDUre sub_prog(foo4) is
 begin
     sub_prog("foo", line_num => 17, file_name => "foo.vhd");
 end;
 """
         self._verify_result(code, expected_result)
 
     def test_that_asserts_with_severity_level_are_not_affected_despite_name_conflict_with_log_functions(
```

### Comparing `vunit_hdl-4.6.2/tests/unit/test_modelsim_interface.py` & `vunit_hdl-4.7.0/tests/unit/test_modelsim_interface.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_ostools.py` & `vunit_hdl-4.7.0/tests/unit/test_ostools.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_project.py` & `vunit_hdl-4.7.0/tests/unit/test_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     def test_recovers_from_parse_error(self, logger):
         self.project.add_library("lib", "work_path")
         source_file = self.add_source_file(
             "lib",
             "file.vhd",
             """\
 entity foo is
- port (;);
+ port (foo : in bit;
 end entity;
 """,
         )
         logger.error.assert_called_once_with("Failed to parse %s", "file.vhd")
         self.assertEqual(source_file.design_units, [])
 
     def test_finds_entity_instantiation_dependencies(self):
@@ -619,14 +619,64 @@
 end architecture;
 """,
         )
 
         self.assert_compiles(ent_a1, before=top1)
         self.assert_compiles(ent_a2, before=top2)
 
+    def test_error_on_ambiguous_architecture(self):
+        self.project.add_library("lib", "lib_path")
+
+        self.add_source_file(
+            "lib",
+            "ent.vhd",
+            """
+entity ent is
+end entity;
+""",
+        )
+
+        self.add_source_file(
+            "lib",
+            "ent_a1.vhd",
+            """
+architecture a1 of ent is
+begin
+end architecture;
+""",
+        )
+
+        self.add_source_file(
+            "lib",
+            "ent_a2.vhd",
+            """
+architecture a2 of ent is
+begin
+end architecture;
+""",
+        )
+
+        self.add_source_file(
+            "lib",
+            "top.vhd",
+            """
+entity top is
+end entity;
+
+architecture a of top is
+begin
+  inst : entity work.ent;
+end architecture;
+""",
+        )
+        self.assertRaises(
+            RuntimeError,
+            self.project.create_dependency_graph,
+        )
+
     def test_work_library_reference_non_lower_case(self):
         """
         Bug discovered in #556
         """
         self.project.add_library("UPPER", "lib_path")
 
         self.add_source_file(
@@ -1801,15 +1851,14 @@
         for std in ("93", "2002", "2008", "2019"):
             project = Project()
             project.add_library("lib", "lib_path")
             source_file = project.add_source_file("file.vhd", library_name="lib", file_type="vhdl", vhdl_standard=std)
             self.assertEqual(source_file.get_vhdl_standard(), std)
 
     def test_add_source_file_has_no_parse_vhdl(self):
-
         for no_parse in (True, False):
             project = Project()
             file_name = "file.vhd"
             write_file(
                 file_name,
                 """
     entity ent is
@@ -1819,15 +1868,14 @@
             project.add_library("lib", "work_path")
             source_file = project.add_source_file(
                 file_name, "lib", file_type=file_type_of(file_name), no_parse=no_parse
             )
             self.assertEqual(len(source_file.design_units), int(not no_parse))
 
     def test_add_source_file_has_no_parse_verilog(self):
-
         for no_parse in (True, False):
             project = Project()
             file_name = "file.v"
             write_file(
                 file_name,
                 """
     module mod;
```

### Comparing `vunit_hdl-4.6.2/tests/unit/test_rivierapro_interface.py` & `vunit_hdl-4.7.0/tests/unit/test_rivierapro_interface.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_simulator_interface.py` & `vunit_hdl-4.7.0/tests/unit/test_simulator_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,22 +250,22 @@
         self._test_ok(option, True)
         self._test_ok(option, False)
         self._test_not_ok(option, None, "Option 'optname' must be a boolean. Got None")
 
     def test_string_option(self):
         option = StringOption("optname")
         self._test_ok(option, "hello")
-        self._test_ok(option, u"hello")
+        self._test_ok(option, "hello")
         self._test_not_ok(option, False, "Option 'optname' must be a string. Got False")
         self._test_not_ok(option, ["foo"], "Option 'optname' must be a string. Got ['foo']")
 
     def test_list_of_string_option(self):
         option = ListOfStringOption("optname")
         self._test_ok(option, ["hello", "foo"])
-        self._test_ok(option, [u"hello"])
+        self._test_ok(option, ["hello"])
         self._test_not_ok(option, [True], "Option 'optname' must be a list of strings. " "Got [True]")
         self._test_not_ok(
             option,
             [["foo"]],
             "Option 'optname' must be a list of strings. " "Got [['foo']]",
         )
         self._test_not_ok(option, "foo", "Option 'optname' must be a list of strings. " "Got 'foo'")
```

### Comparing `vunit_hdl-4.6.2/tests/unit/test_test_bench.py` & `vunit_hdl-4.7.0/tests/unit/test_test_bench.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_test_bench_list.py` & `vunit_hdl-4.7.0/tests/unit/test_test_bench_list.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_test_report.py` & `vunit_hdl-4.7.0/tests/unit/test_test_report.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_test_runner.py` & `vunit_hdl-4.7.0/tests/unit/test_test_runner.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_test_suites.py` & `vunit_hdl-4.7.0/tests/unit/test_test_suites.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_tokenizer.py` & `vunit_hdl-4.7.0/tests/unit/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_ui.py` & `vunit_hdl-4.7.0/tests/unit/test_ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from tests.common import set_env, with_tempdir, create_vhdl_test_bench_file
 from vunit.ui import VUnit
 from vunit.source_file import VHDL_EXTENSIONS, VERILOG_EXTENSIONS
 from vunit.ostools import renew_path
 from vunit.builtins import add_verilog_include_dir
 from vunit.sim_if import SimulatorInterface
 from vunit.vhdl_standard import VHDL
+from vunit.ui.preprocessor import Preprocessor
 
 
 class TestUi(unittest.TestCase):
     """
     Testing the VUnit public interface class
     """
 
@@ -154,14 +155,51 @@
         with (Path(self._preprocessed_path) / "lib" / Path(file_name2).name).open() as fread:
             expectd = pp_source.substitute(
                 entity="ent2",
                 report='log("Here I am!"); -- VUnitfier preprocessor: Report turned off, keeping original code.',
             )
             self.assertEqual(fread.read(), expectd)
 
+    def test_that_application_order_of_preprocessors_can_be_controlled(self):
+        ui = self._create_ui()
+        ui.add_library("lib")
+        ui.add_preprocessor(TestPreprocessor2(order=1))
+        ui.enable_location_preprocessing(order=-1)
+        ui.enable_check_preprocessing(order=-2)
+        ui.add_preprocessor(TestPreprocessor())
+
+        entity_file = Path(self.create_entity_file())
+        ui.add_source_files(str(entity_file), "lib")
+
+        pp_source = Template(
+            """\
+-- TestPreprocessor2
+-- check_relation(a = b);
+
+library vunit_lib;
+context vunit_lib.vunit_context;
+
+entity $entity is
+end entity;
+
+architecture arch of $entity is
+begin
+    log("Hello World", line_num => 10, file_name => "$file");
+    check_relation(1 /= 2, context_msg => "Expected 1 /= 2. Left is \
+" & to_string(1) & ". Right is " & to_string(2) & ".", line_num => 11, file_name => "$file");
+    report "Here I am!";
+end architecture;
+"""
+        )
+        with (Path(self._preprocessed_path) / "lib" / entity_file.name).open() as fread:
+            self.assertEqual(
+                fread.read(),
+                pp_source.substitute(entity="ent0", file=entity_file.name),
+            )
+
     @mock.patch("vunit.ui.LOGGER.error", autospec=True)
     def test_recovers_from_preprocessing_error(self, logger):
         ui = self._create_ui()
         ui.add_library("lib")
         ui.enable_location_preprocessing()
         ui.enable_check_preprocessing()
 
@@ -230,16 +268,14 @@
 
     def test_no_exception_on_adding_zero_files_when_allowed(self):
         ui = self._create_ui()
         lib = ui.add_library("lib")
         lib.add_source_files(str(Path(__file__).parent / "missing.vhd"), allow_empty=True)
 
     def test_get_test_benchs_and_test(self):
-        ui = self._create_ui()
-        lib = ui.add_library("lib")
         self.create_file(
             "tb_ent.vhd",
             """
 entity tb_ent is
   generic (runner_cfg : string);
 end entity;
 
@@ -264,37 +300,88 @@
 
 architecture a of tb_ent2 is
 begin
 end architecture;
         """,
         )
 
+        self.create_file(
+            "tb_ent3.vhd",
+            """
+entity tb_ent3 is
+  generic (runner_cfg : string);
+end entity;
+
+architecture a of tb_ent3 is
+begin
+end architecture;
+        """,
+        )
+
         ui = self._create_ui()
-        lib = ui.add_library("lib")
-        lib.add_source_file("tb_ent.vhd")
-        lib.add_source_file("tb_ent2.vhd")
-        self.assertEqual(lib.test_bench("tb_ent").name, "tb_ent")
-        self.assertEqual(lib.test_bench("tb_ent2").name, "tb_ent2")
-        self.assertEqual(lib.test_bench("tb_ent").library.name, "lib")
+        lib1 = ui.add_library("lib1")
+        lib2 = ui.add_library("lib2")
+        lib1.add_source_file("tb_ent.vhd")
+        lib1.add_source_file("tb_ent2.vhd")
+        lib2.add_source_file("tb_ent3.vhd")
+        self.assertEqual(lib1.test_bench("tb_ent").name, "tb_ent")
+        self.assertEqual(lib1.test_bench("tb_ent2").name, "tb_ent2")
+        self.assertEqual(lib1.test_bench("tb_ent").library.name, "lib1")
 
         self.assertEqual(
-            [test_bench.name for test_bench in lib.get_test_benches()],
+            [test_bench.name for test_bench in lib1.get_test_benches()],
             ["tb_ent", "tb_ent2"],
         )
-        self.assertEqual([test_bench.name for test_bench in lib.get_test_benches("*2")], ["tb_ent2"])
+        self.assertEqual([test_bench.name for test_bench in lib1.get_test_benches("*2")], ["tb_ent2"])
 
-        self.assertEqual(lib.test_bench("tb_ent").test("test1").name, "test1")
-        self.assertEqual(lib.test_bench("tb_ent").test("test2").name, "test2")
+        libs = ui.get_libraries("lib*")
+        self.assertEqual(
+            [test_bench.name for test_bench in libs.get_test_benches()],
+            ["tb_ent", "tb_ent2", "tb_ent3"],
+        )
+        self.assertEqual([test_bench.name for test_bench in libs.get_test_benches("*3")], ["tb_ent3"])
+
+        self.assertEqual(lib1.test_bench("tb_ent").test("test1").name, "test1")
+        self.assertEqual(lib1.test_bench("tb_ent").test("test2").name, "test2")
 
         self.assertEqual(
-            [test.name for test in lib.test_bench("tb_ent").get_tests()],
+            [test.name for test in lib1.test_bench("tb_ent").get_tests()],
+            ["test1", "test2"],
+        )
+        self.assertEqual([test.name for test in lib1.test_bench("tb_ent").get_tests("*1")], ["test1"])
+        self.assertEqual([test.name for test in lib1.test_bench("tb_ent2").get_tests()], [])
+
+    def test_get_test_bench_with_explicit_constant_runner_cfg(self):
+        self.create_file(
+            "tb_ent.vhd",
+            """
+entity tb_ent is
+  generic (constant runner_cfg : in string);
+end entity;
+
+architecture a of tb_ent is
+begin
+  main : process
+  begin
+    if run("test1") then
+    elsif run("test2") then
+    end if;
+  end process;
+end architecture;
+        """,
+        )
+
+        ui = self._create_ui()
+        lib1 = ui.add_library("lib1")
+        lib1.add_source_file("tb_ent.vhd")
+        self.assertEqual(lib1.test_bench("tb_ent").name, "tb_ent")
+        self.assertEqual(
+            [test.name for test in lib1.test_bench("tb_ent").get_tests()],
             ["test1", "test2"],
         )
-        self.assertEqual([test.name for test in lib.test_bench("tb_ent").get_tests("*1")], ["test1"])
-        self.assertEqual([test.name for test in lib.test_bench("tb_ent2").get_tests()], [])
 
     def test_get_entities_case_insensitive(self):
         ui = self._create_ui()
         lib = ui.add_library("lib")
         self.create_file(
             "tb_ent.vhd",
             """
@@ -403,20 +490,56 @@
         file_name = self.create_entity_file()
         lib1.add_source_file(file_name)
         lib2.add_source_file(file_name)
 
         self.assertEqual(len(ui.get_source_files(file_name)), 2)
         self.assertEqual(len(lib1.get_source_files(file_name)), 1)
         self.assertEqual(len(lib2.get_source_files(file_name)), 1)
+        self.assertEqual(len(ui.get_libraries("lib*").get_source_files(file_name)), 2)
+        self.assertEqual(len(ui.get_libraries("lib2").get_source_files(file_name)), 1)
 
         ui.get_source_file(file_name, library_name="lib1")
         ui.get_source_file(file_name, library_name="lib2")
         lib1.get_source_file(file_name)
         lib2.get_source_file(file_name)
 
+    def test_get_libraries(self):
+        ui = self._create_ui()
+
+        libs = ui.get_libraries()
+        self.assertEqual(len(libs), 1)
+        self.assertEqual(libs[0].name, "vunit_lib")
+
+        ui.add_library("lib1")
+        ui.add_library("lib2")
+
+        self.assertEqual(len(ui.get_libraries()), 3)
+        self.assertEqual(len(ui.get_libraries("lib*")), 2)
+        libs = ui.get_libraries("lib1")
+        self.assertEqual(len(libs), 1)
+        self.assertEqual(libs[0].name, "lib1")
+        libs = ui.get_libraries("*2")
+        self.assertEqual(len(libs), 1)
+        self.assertEqual(libs[0].name, "lib2")
+
+    def test_get_libraries_errors(self):
+        ui = self._create_ui()
+        ui.add_library("lib1")
+        ui.add_library("lib2")
+        non_existant_name = "non_existant"
+
+        self.assertRaisesRegex(
+            ValueError,
+            f".*{non_existant_name}.*allow_empty.*",
+            ui.get_libraries,
+            non_existant_name,
+        )
+
+        self.assertEqual(len(ui.get_libraries(non_existant_name, allow_empty=True)), 0)
+
     def test_get_compile_order_smoke_test(self):
         ui = self._create_ui()
         lib1 = ui.add_library("lib1")
         lib2 = ui.add_library("lib2")
         file_name = self.create_entity_file()
         lib1.add_source_file(file_name)
         lib2.add_source_file(file_name)
@@ -797,15 +920,15 @@
         file_name = "foo.vhd"
         self.create_file(file_name)
         ui = self._create_ui()
         lib = ui.add_library("lib")
         source_file = lib.add_source_file(file_name)
 
         # Use methods on all types of interface objects
-        for obj in [source_file, ui, lib, lib.get_source_files(file_name)]:
+        for obj in [source_file, ui, lib, lib.get_source_files(file_name), ui.get_libraries("lib")]:
             obj.set_compile_option("ghdl.flags", [])
             self.assertEqual(source_file.get_compile_option("ghdl.flags"), [])
 
             obj.add_compile_option("ghdl.flags", ["1"])
             self.assertEqual(source_file.get_compile_option("ghdl.flags"), ["1"])
 
             obj.add_compile_option("ghdl.flags", ["2"])
@@ -1073,21 +1196,24 @@
 
     def test_set_sim_option_before_adding_file(self):
         """
         From GitHub issue #250
         """
         ui = self._create_ui()
         lib = ui.add_library("lib")
-        for method in (lib.set_sim_option, ui.set_sim_option):
+        libs = ui.get_libraries("lib")
+        for method in (lib.set_sim_option, ui.set_sim_option, libs.set_sim_option):
             method("disable_ieee_warnings", True, allow_empty=True)
             self.assertRaises(ValueError, method, "disable_ieee_warnings", True)
 
         for method in (
             lib.set_compile_option,
             lib.add_compile_option,
+            libs.set_compile_option,
+            libs.add_compile_option,
             ui.set_compile_option,
             ui.add_compile_option,
         ):
             method("ghdl.elab_flags", [], allow_empty=True)
             self.assertRaises(ValueError, method, "ghdl.elab_flags", [])
 
     def test_get_testbench_files(self):
@@ -1213,25 +1339,38 @@
             file_name = Path(file_name)
         with file_name.open("w") as fprt:
             fprt.write(contents)
 
 
 class TestPreprocessor(object):
     """
-    A preprocessor that appends a check_relation call before the orginal code
+    A preprocessor that adds a check_relation call before the orginal code
     """
 
     def __init__(self):
         pass
 
     @staticmethod
     def run(code, file_name):  # pylint: disable=unused-argument
         return "-- check_relation(a = b);\n" + code
 
 
+class TestPreprocessor2(Preprocessor):
+    """
+    A preprocessor that adds a comment before the orginal code
+    """
+
+    def __init__(self, order):
+        super().__init__(order)
+
+    @staticmethod
+    def run(code, file_name):  # pylint: disable=unused-argument
+        return "-- TestPreprocessor2\n" + code
+
+
 class VUnitfier(object):
     """
     A preprocessor that replaces report statments with log calls
     """
 
     def __init__(self):
         self._report_pattern = re.compile(r'^(?P<indent>\s*)report\s*(?P<note>"[^"]*")\s*;', MULTILINE)
```

### Comparing `vunit_hdl-4.6.2/tests/unit/test_verilog_parser.py` & `vunit_hdl-4.7.0/tests/unit/test_verilog_parser.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_verilog_preprocessor.py` & `vunit_hdl-4.7.0/tests/unit/test_verilog_preprocessor.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_verilog_tokenizer.py` & `vunit_hdl-4.7.0/tests/unit/test_verilog_tokenizer.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/tests/unit/test_vhdl_parser.py` & `vunit_hdl-4.7.0/tests/unit/test_vhdl_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -239,14 +239,43 @@
         #        self.assertEqual(generics[0].subtypeIndication.constraint, "range 2-2 to 2**10")
         self.assertEqual(generics[1].identifier, "enable_foo")
         self.assertEqual(generics[1].init_value, None)
         self.assertEqual(generics[1].mode, None)
         self.assertEqual(generics[1].subtype_indication.code, "boolean")
         self.assertEqual(generics[1].subtype_indication.type_mark, "boolean")
 
+    def test_parsing_entity_with_generics_and_trailing_semicolon(self):
+        entity = self.parse_single_entity(
+            """\
+entity name is
+   generic (max_value : integer range 2-2 to 2**10 := (2-19)*4;
+            enable_foo : boolean  ;
+   );
+end entity;
+"""
+        )
+        self.assertEqual(entity.identifier, "name")
+        self.assertNotEqual(entity.generics, [])
+        self.assertEqual(entity.ports, [])
+        generics = entity.generics
+        self.assertEqual(len(generics), 2)
+
+        self.assertEqual(generics[0].identifier, "max_value")
+        self.assertEqual(generics[0].init_value, "(2-19)*4")
+        self.assertEqual(generics[0].mode, None)
+        self.assertEqual(generics[0].subtype_indication.code, "integer range 2-2 to 2**10")
+        self.assertEqual(generics[0].subtype_indication.type_mark, "integer")
+        # @TODO does not work
+        #        self.assertEqual(generics[0].subtypeIndication.constraint, "range 2-2 to 2**10")
+        self.assertEqual(generics[1].identifier, "enable_foo")
+        self.assertEqual(generics[1].init_value, None)
+        self.assertEqual(generics[1].mode, None)
+        self.assertEqual(generics[1].subtype_indication.code, "boolean")
+        self.assertEqual(generics[1].subtype_indication.type_mark, "boolean")
+
     def test_parsing_entity_with_generics_corner_cases(self):
         self.parse_single_entity(
             """\
 entity name is end entity;
 """
         )
 
@@ -289,44 +318,150 @@
 g : t
 );
 end entity;
 """
         )
         self.assertEqual(len(entity.generics), 0)
 
-    def test_parsing_entity_with_ports(self):
-        entity = self.parse_single_entity(
-            """\
-entity name is
-   port (clk : in std_logic;
-         data : out std_logic_vector(11-1 downto 0));
-end entity;
-"""
-        )
-
+    def _check_entity_with_ports(self, entity):
         self.assertEqual(entity.identifier, "name")
         self.assertEqual(entity.generics, [])
         self.assertNotEqual(entity.ports, [])
 
         ports = entity.ports
-        self.assertEqual(len(ports), 2)
+        self.assertEqual(len(ports), 12)
 
         self.assertEqual(ports[0].identifier, "clk")
         self.assertEqual(ports[0].init_value, None)
         self.assertEqual(ports[0].mode, "in")
         self.assertEqual(ports[0].subtype_indication.code, "std_logic")
         self.assertEqual(ports[0].subtype_indication.type_mark, "std_logic")
 
         self.assertEqual(ports[1].identifier, "data")
         self.assertEqual(ports[1].init_value, None)
         self.assertEqual(ports[1].mode, "out")
         self.assertEqual(ports[1].subtype_indication.code, "std_logic_vector(11-1 downto 0)")
         self.assertEqual(ports[1].subtype_indication.type_mark, "std_logic_vector")
         self.assertEqual(ports[1].subtype_indication.constraint, "(11-1 downto 0)")
 
+        self.assertEqual(ports[2].identifier, "signal_data2")
+        self.assertEqual(ports[2].init_value, None)
+        self.assertEqual(ports[2].mode, "in")
+        self.assertEqual(ports[2].subtype_indication.code, "std_logic")
+        self.assertEqual(ports[2].subtype_indication.type_mark, "std_logic")
+        self.assertEqual(ports[2].subtype_indication.constraint, None)
+
+        self.assertEqual(ports[3].identifier, "data3")
+        self.assertEqual(ports[3].init_value, None)
+        self.assertEqual(ports[3].mode, "in")
+        self.assertEqual(ports[3].subtype_indication.code, "signal_type")
+        self.assertEqual(ports[3].subtype_indication.type_mark, "signal_type")
+        self.assertEqual(ports[3].subtype_indication.constraint, None)
+
+        self.assertEqual(ports[4].identifier, "data4_signal")
+        self.assertEqual(ports[4].init_value, None)
+        self.assertEqual(ports[4].mode, "in")
+        self.assertEqual(ports[4].subtype_indication.code, "std_logic")
+        self.assertEqual(ports[4].subtype_indication.type_mark, "std_logic")
+        self.assertEqual(ports[4].subtype_indication.constraint, None)
+
+        self.assertEqual(ports[5].identifier, "data5")
+        self.assertEqual(ports[5].init_value, None)
+        self.assertEqual(ports[5].mode, "in")
+        self.assertEqual(ports[5].subtype_indication.code, "type_signal")
+        self.assertEqual(ports[5].subtype_indication.type_mark, "type_signal")
+        self.assertEqual(ports[5].subtype_indication.constraint, None)
+
+        self.assertEqual(ports[6].identifier, "clk2")
+        self.assertEqual(ports[6].init_value, None)
+        self.assertEqual(ports[6].mode, "in")
+        self.assertEqual(ports[6].subtype_indication.code, "std_logic")
+        self.assertEqual(ports[6].subtype_indication.type_mark, "std_logic")
+
+        self.assertEqual(ports[7].identifier, "data7")
+        self.assertEqual(ports[7].init_value, None)
+        self.assertEqual(ports[7].mode, "out")
+        self.assertEqual(ports[7].subtype_indication.code, "std_logic_vector(11-1 downto 0)")
+        self.assertEqual(ports[7].subtype_indication.type_mark, "std_logic_vector")
+        self.assertEqual(ports[7].subtype_indication.constraint, "(11-1 downto 0)")
+
+        self.assertEqual(ports[8].identifier, "signal_data8")
+        self.assertEqual(ports[8].init_value, None)
+        self.assertEqual(ports[8].mode, "in")
+        self.assertEqual(ports[8].subtype_indication.code, "std_logic")
+        self.assertEqual(ports[8].subtype_indication.type_mark, "std_logic")
+        self.assertEqual(ports[8].subtype_indication.constraint, None)
+
+        self.assertEqual(ports[9].identifier, "data9")
+        self.assertEqual(ports[9].init_value, None)
+        self.assertEqual(ports[9].mode, "in")
+        self.assertEqual(ports[9].subtype_indication.code, "signal_type")
+        self.assertEqual(ports[9].subtype_indication.type_mark, "signal_type")
+        self.assertEqual(ports[9].subtype_indication.constraint, None)
+
+        self.assertEqual(ports[10].identifier, "data10_signal")
+        self.assertEqual(ports[10].init_value, None)
+        self.assertEqual(ports[10].mode, "in")
+        self.assertEqual(ports[10].subtype_indication.code, "std_logic")
+        self.assertEqual(ports[10].subtype_indication.type_mark, "std_logic")
+        self.assertEqual(ports[10].subtype_indication.constraint, None)
+
+        self.assertEqual(ports[11].identifier, "data11")
+        self.assertEqual(ports[11].init_value, None)
+        self.assertEqual(ports[11].mode, "in")
+        self.assertEqual(ports[11].subtype_indication.code, "type_signal")
+        self.assertEqual(ports[11].subtype_indication.type_mark, "type_signal")
+        self.assertEqual(ports[11].subtype_indication.constraint, None)
+
+    def test_parsing_entity_with_ports(self):
+        entity = self.parse_single_entity(
+            """\
+entity name is
+port (
+    clk : in std_logic;
+ \t data : out std_logic_vector(11-1 downto 0);
+    signal_data2 : in std_logic;
+\t  data3 :\tin signal_type;
+    data4_signal : in\tstd_logic;
+    data5\t: in type_signal;
+\t\tsignal clk2 : in std_logic;
+    signal\tdata7 : out std_logic_vector(11-1 downto 0);
+    signal signal_data8 : in std_logic;
+    signal\t data9 : in signal_type;
+    signal data10_signal :\tin std_logic;\t
+    signal \t data11 : in type_signal
+);
+end entity;
+"""
+        )
+        self._check_entity_with_ports(entity)
+
+    def test_parsing_entity_with_ports_and_trailing_semicolon(self):
+        entity = self.parse_single_entity(
+            """\
+entity name is
+port (
+    clk : in std_logic;
+ \t data : out std_logic_vector(11-1 downto 0);
+    signal_data2 : in std_logic;
+\t  data3 :\tin signal_type;
+    data4_signal : in\tstd_logic;
+    data5\t: in type_signal;
+\t\tsignal clk2 : in std_logic;
+    signal\tdata7 : out std_logic_vector(11-1 downto 0);
+    signal signal_data8 : in std_logic;
+    signal\t data9 : in signal_type;
+    signal data10_signal :\tin std_logic;\t
+    signal \t data11 : in type_signal
+;);
+end entity;
+"""
+        )
+        self._check_entity_with_ports(entity)
+
     def test_parsing_simple_package_body(self):
         package_body = self.parse_single_package_body(
             """\
 package body simple is
 begin
 end package body;
 """
```

### Comparing `vunit_hdl-4.6.2/tests/unit/test_vhdl_standard.py` & `vunit_hdl-4.7.0/tests/unit/test_vhdl_standard.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/__init__.py` & `vunit_hdl-4.7.0/vunit/__init__.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/about.py` & `vunit_hdl-4.7.0/vunit/about.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
 def license_text():
     """
     Returns licence text
     """
     return """\
 **VUnit**, except for the projects below, is released under the terms of `Mozilla Public License, v. 2.0`_.
-|copy| 2014-2021 Lars Asplund, lars.anders.asplund@gmail.com.
+|copy| 2014-2023 Lars Asplund, lars.anders.asplund@gmail.com.
 
 The following libraries are `redistributed`_ with VUnit for convenience:
 
 * **OSVVM** (``vunit/vhdl/osvvm``): these files are licensed under the terms of `Apache License, v 2.0`_,
-  |copy| 2010 - 2021 by `SynthWorks Design Inc`_. All rights reserved.
+  |copy| 2010 - 2023 by `SynthWorks Design Inc`_. All rights reserved.
 
 * **JSON-for-VHDL** (``vunit/vhdl/JSON-for-VHDL``): these files are licensed under the terms of `Apache License,
-  v 2.0`_, |copy| 2015 - 2021 Patrick Lehmann.
+  v 2.0`_, |copy| 2015 - 2023 Patrick Lehmann.
 
 The font used in VUnit's logo and illustrations is 'Tratex', the traffic sign typeface used on swedish road signs:
 
 - `transportstyrelsen.se: Teckensnitt <https://transportstyrelsen.se/sv/vagtrafik/Trafikregler/Om-vagmarken/Teckensnitt/>`__
 - `Wikipedia: Tratex <https://en.wikipedia.org/wiki/Tratex>`__
 
 
@@ -65,8 +65,8 @@
 def version():
     """
     Returns VUnit version
     """
     return VERSION
 
 
-VERSION = "4.6.2"
+VERSION = "4.7.0"
```

### Comparing `vunit_hdl-4.6.2/vunit/builtins.py` & `vunit_hdl-4.7.0/vunit/builtins.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,22 @@
 """
 Functions to add builtin VHDL code to a project for compilation
 """
 
 from pathlib import Path
 from glob import glob
 from warnings import warn
+import logging
+
 from vunit.vhdl_standard import VHDL, VHDLStandard
 from vunit.ui.common import get_checked_file_names_from_globs
 
+
+LOGGER = logging.getLogger(__name__)
+
 VHDL_PATH = (Path(__file__).parent / "vhdl").resolve()
 VERILOG_PATH = (Path(__file__).parent / "verilog").resolve()
 
 
 class Builtins(object):
     """
     Manage VUnit builtins and their dependencies
@@ -126,24 +131,34 @@
         """
         Add verification component library
         """
         if not self._vhdl_standard >= VHDL.STD_2008:
             raise RuntimeError("Verification component library only supports vhdl 2008 and later")
         self._add_files(VHDL_PATH / "verification_components" / "src" / "*.vhd")
 
+    def _add_library_if_not_exist(self, library_name, message):
+        """
+        Check if a library name exists in the project. If not, add it and return a handle.
+        """
+        if library_name.lower() in [
+            library.lower() for library in self._vunit_obj._project._libraries  # pylint: disable=protected-access
+        ]:
+            LOGGER.warning(message)
+            return None
+        return self._vunit_obj.add_library(library_name)
+
     def _add_osvvm(self):
         """
         Add osvvm library
         """
-        library_name = "osvvm"
-
-        try:
-            library = self._vunit_obj.library(library_name)
-        except KeyError:
-            library = self._vunit_obj.add_library(library_name)
+        library = self._add_library_if_not_exist(
+            "osvvm", "Library 'OSVVM' previously defined. Skipping addition of builtin OSVVM (2022.04)."
+        )
+        if library is None:
+            return
 
         simulator_coverage_api = self._simulator_class.get_osvvm_coverage_api()
         supports_vhdl_package_generics = self._simulator_class.supports_vhdl_package_generics()
 
         if not osvvm_is_installed():
             raise RuntimeError(
                 """
@@ -171,50 +186,97 @@
                     "ScoreboardGenericPkg.vhd",
                     "ScoreboardPkg_int.vhd",
                     "ScoreboardPkg_slv.vhd",
                 ]
             ):
                 continue
 
+            if supports_vhdl_package_generics and (
+                bname
+                in [
+                    "ScoreboardPkg_int_c.vhd",
+                    "ScoreboardPkg_slv_c.vhd",
+                ]
+            ):
+                continue
+
             library.add_source_files(file_name, preprocessors=[])
 
     def _add_json4vhdl(self):
         """
         Add JSON-for-VHDL library
         """
-        library_name = "JSON"
-
-        try:
-            library = self._vunit_obj.library(library_name)
-        except KeyError:
-            library = self._vunit_obj.add_library(library_name)
+        library = self._add_library_if_not_exist(
+            "JSON", "Library 'JSON' previously defined. Skipping addition of builtin JSON-for-VHDL (95e848b8)."
+        )
+        if library is None:
+            return
 
         library.add_source_files(VHDL_PATH / "JSON-for-VHDL" / "src" / "*.vhdl")
 
+    def _add_vhdl_logging(self):
+        """
+        Add logging functionality
+        """
+
+        use_call_paths = self._simulator_class.supports_vhdl_call_paths() and (
+            self._vhdl_standard in VHDL.STD_2019.and_later
+        )
+        if use_call_paths:
+            self._vunit_lib.add_source_file(VHDL_PATH / "logging" / "src" / "location_pkg-body-2019p.vhd")
+        else:
+            self._vunit_lib.add_source_file(VHDL_PATH / "logging" / "src" / "location_pkg-body-2008m.vhd")
+
+        for file_name in get_checked_file_names_from_globs(VHDL_PATH / "logging" / "src" / "*.vhd", allow_empty=False):
+            base_file_name = Path(file_name).name
+
+            if base_file_name.startswith("location_pkg-body"):
+                continue
+
+            standards = set()
+            for standard in VHDL.STANDARDS:
+                standard_name = str(standard)
+                if standard_name + "p" in base_file_name:
+                    standards.update(standard.and_later)
+                elif standard_name + "m" in base_file_name:
+                    standards.update(standard.and_earlier)
+                elif standard_name in base_file_name:
+                    standards.add(standard)
+
+            if standards and self._vhdl_standard not in standards:
+                continue
+
+            self._vunit_lib.add_source_file(file_name)
+
     def add_verilog_builtins(self):
         """
         Add Verilog builtins
         """
         self._vunit_lib.add_source_files(VERILOG_PATH / "vunit_pkg.sv")
 
     def add_vhdl_builtins(self, external=None):
         """
         Add vunit VHDL builtin libraries
 
         :param external: struct to provide bridges for the external VHDL API.
-                         {
-                             'string': ['path/to/custom/file'],
-                             'integer': ['path/to/custom/file']
-                         }.
+
+        :example:
+
+        .. code-block:: python
+
+            Builtins.add_vhdl_builtins(external={
+                'string': ['path/to/custom/file'],
+                'integer': ['path/to/custom/file']
+            })
         """
         self._add_data_types(external=external)
+        self._add_vhdl_logging()
         self._add_files(VHDL_PATH / "*.vhd")
         for path in (
             "core",
-            "logging",
             "string_ops",
             "check",
             "dictionary",
             "run",
             "path",
         ):
             self._add_files(VHDL_PATH / path / "src" / "*.vhd")
```

### Comparing `vunit_hdl-4.6.2/vunit/cached.py` & `vunit_hdl-4.7.0/vunit/cached.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/check_preprocessor.py` & `vunit_hdl-4.7.0/vunit/check_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,33 +5,32 @@
 # Copyright (c) 2014-2023, Lars Asplund lars.anders.asplund@gmail.com
 
 """
 Preprocessing of check functions
 """
 
 import re
+from vunit.ui.preprocessor import Preprocessor
 
 
-class CheckPreprocessor(object):
+class CheckPreprocessor(Preprocessor):
     """
-    Preprocessing of check functions adding helpful message to check_relation calls
+    Preprocessing of check functions adding helpful message to check_relation calls.
     """
 
-    def __init__(self):
+    def __init__(self, order=2000):
+        super().__init__(order)
         self._find_operators = re.compile(r"\?/=|\?<=|\?>=|\?<|\?>|\?=|/=|<=|>=|<|>|=", re.MULTILINE)
         self._find_quotes = re.compile(r'"|' + r"'", re.MULTILINE)
         self._find_comments = re.compile(r"--|/\*|\*/", re.MULTILINE)
         self._actual_formal = re.compile(r"=>(?P<actual>.*)", re.MULTILINE)
         self._leading_paranthesis = re.compile(r"[\s(]*")
         self._trailing_paranthesis = re.compile(r"[\s)]*")
 
     def run(self, code, file_name):  # pylint: disable=unused-argument
-        """
-        Preprocess code and return result also given the file_name of the original file
-        """
         check_relation_pattern = re.compile(r"[^a-zA-Z0-9_](?P<call>check_relation)\s*(?P<parameters>\()", re.MULTILINE)
 
         check_relation_calls = list(check_relation_pattern.finditer(code))
         check_relation_calls.reverse()
 
         for match in check_relation_calls:
             (
```

### Comparing `vunit_hdl-4.6.2/vunit/color_printer.py` & `vunit_hdl-4.7.0/vunit/color_printer.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,32 +25,30 @@
     RED = "r"
     INTENSITY = "i"
     WHITE = RED + GREEN + BLUE
 
     def __init__(self):
         pass
 
-    @staticmethod
-    def write(text, output_file=None, fg=None, bg=None):  # pylint: disable=unused-argument
+    def write(self, text, output_file=None, fg=None, bg=None):  # pylint: disable=unused-argument
         """
         Print the text in color to the output_file
         uses stdout if output_file is None
         """
 
 
 class NoColorPrinter(ColorPrinter):
     """
     Dummy printer that does not print in color
     """
 
     def __init__(self):
         ColorPrinter.__init__(self)
 
-    @staticmethod
-    def write(text, output_file=None, fg=None, bg=None):  # pylint: disable=unused-argument
+    def write(self, text, output_file=None, fg=None, bg=None):  # pylint: disable=unused-argument
         """
         Print the text in color to the output_file
         uses stdout if output_file is None
         """
         if output_file is None:
             output_file = sys.stdout
         output_file.write(text)
```

### Comparing `vunit_hdl-4.6.2/vunit/com/codec_datatype_template.py` & `vunit_hdl-4.7.0/vunit/com/codec_datatype_template.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/com/codec_generator.py` & `vunit_hdl-4.7.0/vunit/com/codec_generator.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/com/codec_vhdl_array_type.py` & `vunit_hdl-4.7.0/vunit/com/codec_vhdl_array_type.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/com/codec_vhdl_enumeration_type.py` & `vunit_hdl-4.7.0/vunit/com/codec_vhdl_enumeration_type.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/com/codec_vhdl_package.py` & `vunit_hdl-4.7.0/vunit/com/codec_vhdl_package.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,18 @@
             declarations += self._template.get_msg_type_declaration.substitute(
                 type=all_msg_types_enumeration_type.identifier
             )
             definitions += self._template.get_msg_type_definition.substitute(
                 type=all_msg_types_enumeration_type.identifier
             )
 
-        (new_declarations, new_definitions,) = self._generate_enumeration_codec_and_to_string_functions(
+        (
+            new_declarations,
+            new_definitions,
+        ) = self._generate_enumeration_codec_and_to_string_functions(
             all_msg_types_enumeration_type, msg_type_enumeration_types
         )
         declarations += new_declarations
         definitions += new_definitions
 
         # Arrays
         (
@@ -173,15 +176,14 @@
 
         declarations = ""
         definitions = ""
         enumeration_offset = 0
         for enum in self.enumeration_types + (
             [all_msg_types_enumeration_type] if all_msg_types_enumeration_type is not None else []
         ):
-
             if enum.identifier in msg_type_enumeration_types:
                 offset = enumeration_offset
                 enumeration_offset += len(enum.literals)
             else:
                 offset = 0
 
             (
@@ -224,15 +226,15 @@
                         if identifier != "msg_type":
                             parameter_list.append(f"    constant {identifier!s} : {element.subtype_indication.code!s}")
                             parameter_type_list.append(element.subtype_indication.type_mark)
                             encoding_list.append(f"encode({identifier!s})")
                         else:
                             encoding_list.append(f"encode({element.subtype_indication.code!s}'({value!s}))")
 
-                if parameter_list == []:
+                if not parameter_list:
                     parameter_part = ""
                     alias_signature = value + "[return string];"
                 else:
                     parameter_part = " (\n" + ";\n".join(parameter_list) + ")"
                     alias_signature = value + "[" + ", ".join(parameter_type_list) + " return string];"
 
                 encodings = " & ".join(encoding_list)
```

### Comparing `vunit_hdl-4.6.2/vunit/com/codec_vhdl_record_type.py` & `vunit_hdl-4.7.0/vunit/com/codec_vhdl_record_type.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/configuration.py` & `vunit_hdl-4.7.0/vunit/configuration.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/csv_logs.py` & `vunit_hdl-4.7.0/vunit/csv_logs.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/database.py` & `vunit_hdl-4.7.0/vunit/database.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/dependency_graph.py` & `vunit_hdl-4.7.0/vunit/dependency_graph.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/design_unit.py` & `vunit_hdl-4.7.0/vunit/design_unit.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/json4vhdl.py` & `vunit_hdl-4.7.0/vunit/json4vhdl.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/library.py` & `vunit_hdl-4.7.0/vunit/library.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/location_preprocessor.py` & `vunit_hdl-4.7.0/vunit/location_preprocessor.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,55 +7,34 @@
 """
 Preprocessing of VHDL files to add file_name and line_num arguments to function calls
 to enable better messages
 """
 
 
 import re
+from vunit.ui.preprocessor import Preprocessor
 
 
-class LocationPreprocessor(object):
+class LocationPreprocessor(Preprocessor):
     """
     Preprocessing of VHDL files to add file_name and line_num
     arguments to calls of known function and procedures
     """
 
-    def __init__(self):
+    def __init__(self, order=1000):
+        super().__init__(order)
         self._subprograms_with_arguments = [
             "log",
-            "verbose_high2",
-            "verbose_high1",
-            "verbose",
-            "verbose_low1",
-            "verbose_low2",
-            "debug_high2",
-            "debug_high1",
+            "trace",
             "debug",
-            "debug_low1",
-            "debug_low2",
-            "info_high2",
-            "info_high1",
+            "pass",
             "info",
-            "info_low1",
-            "info_low2",
-            "warning_high2",
-            "warning_high1",
             "warning",
-            "warning_low1",
-            "warning_low2",
-            "error_high2",
-            "error_high1",
             "error",
-            "error_low1",
-            "error_low2",
-            "failure_high2",
-            "failure_high1",
             "failure",
-            "failure_low1",
-            "failure_low2",
             "check",
             "check_failed",
             "check_true",
             "check_false",
             "check_implication",
             "check_stable",
             "check_equal",
@@ -65,14 +44,17 @@
             "check_next",
             "check_sequence",
             "check_relation",
             "lock_entry",
             "lock_exit",
             "unlock_entry",
             "unlock_exit",
+            "test_runner_watchdog",
+            "is_active_msg",
+            "log_active",
         ]
         self._subprograms_without_arguments = []
 
     def add_subprogram(self, subprogram):
         """
         Add a subprogram name to the list of known names to preprocess
         """
@@ -105,21 +87,18 @@
             balance += 1 if match.group() == "(" else -1
             if balance == 0:
                 return match.start()
         return None
 
     _already_fixed_file_name_pattern = re.compile(r"file_name\s*=>", re.MULTILINE)
     _already_fixed_line_num_pattern = re.compile(r"line_num\s*=>", re.MULTILINE)
-    _subprogram_declaration_start_backwards_pattern = re.compile(r"\s+(erudecorp|noitcnuf)")
+    _subprogram_declaration_start_backwards_pattern = re.compile(r"\s+(erudecorp|noitcnuf)", re.IGNORECASE)
     _assignment_pattern = re.compile(r"\s*(:=|<=)", re.MULTILINE)
 
     def run(self, code, file_name):
-        """
-        Return preprocessed code given file_name of original file
-        """
         potential_subprogram_call_with_arguments_pattern = re.compile(
             r"[^a-zA-Z0-9_](?P<subprogram>" + "|".join(self._subprograms_with_arguments) + r")\s*(?P<args>\()",
             re.MULTILINE,
         )
 
         potential_subprogram_call_without_arguments_pattern = re.compile(
             r"[^a-zA-Z0-9_](?P<subprogram>" + "|".join(self._subprograms_without_arguments) + r")\s*;",
```

### Comparing `vunit_hdl-4.6.2/vunit/ostools.py` & `vunit_hdl-4.7.0/vunit/ostools.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/parsing/tokenizer.py` & `vunit_hdl-4.7.0/vunit/parsing/tokenizer.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/parsing/verilog/parser.py` & `vunit_hdl-4.7.0/vunit/parsing/verilog/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,14 @@
         """
         idx = 0
         name = None
         balance = 0
         results = []
         parameters = []
         while idx < len(tokens):
-
             if tokens[idx].kind == MODULE:
                 if balance == 0:
                     name = tokens[idx + 1].value
                     parameters = []
                 balance += 1
 
             elif tokens[idx].kind == ENDMODULE:
```

### Comparing `vunit_hdl-4.6.2/vunit/parsing/verilog/preprocess.py` & `vunit_hdl-4.7.0/vunit/parsing/verilog/preprocess.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/parsing/verilog/tokenizer.py` & `vunit_hdl-4.7.0/vunit/parsing/verilog/tokenizer.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/parsing/verilog/tokens.py` & `vunit_hdl-4.7.0/vunit/parsing/verilog/tokens.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/persistent_tcl_shell.py` & `vunit_hdl-4.7.0/vunit/persistent_tcl_shell.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/project.py` & `vunit_hdl-4.7.0/vunit/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,26 +194,42 @@
     def _find_vhdl_library_reference(self, library_name):
         """
         Find a VHDL library reference that is case insensitive or raise KeyError
         """
         real_library_name = self._lower_library_names_dict[library_name.lower()]
         return self._libraries[real_library_name]
 
+    @staticmethod
+    def _handle_ambiguous_architecture(source_file, ref, primary_unit):
+        """
+        Pretty print architecture ambiguity
+        """
+        LOGGER.error(
+            "Ambiguous direct entity instantiation of %s.%s in %s.\n  "
+            "Remove all but one architecture or specify one of:\n  %s",
+            ref.library,
+            ref.design_unit,
+            source_file.name,
+            "\n  ".join(
+                f"{idx}. {name} ({location})"
+                for idx, (name, location) in enumerate(primary_unit.architecture_names.items(), 1)
+            ),
+        )
+
     def _find_other_vhdl_design_unit_dependencies(  # pylint: disable=too-many-branches
         self, source_file, depend_on_package_body, implementation_dependencies
     ):
         """
         Iterate over the dependencies on other design unit of the source_file
         """
         for ref in source_file.dependencies:
             try:
                 library = self._find_vhdl_library_reference(ref.library)
             except KeyError:
                 if ref.library not in self._builtin_libraries:
-
                     LOGGER.warning("%s: failed to find library '%s'", source_file.name, ref.library)
                 continue
 
             if ref.is_entity_reference() and ref.design_unit in library.modules:
                 # Is a verilog module instantiation
                 yield library.modules[ref.design_unit].source_file
                 continue
@@ -242,14 +258,17 @@
                     names = primary_unit.architecture_names.keys()
                 else:
                     names = [ref.name_within]
 
                 for name in names:
                     if name is None:
                         # Was not a reference to a specific architecture
+                        if len(primary_unit.architecture_names) > 1:
+                            self._handle_ambiguous_architecture(source_file, ref, primary_unit)
+                            raise RuntimeError(f"Ambiguous use of {ref.library}.{ref.design_unit}")
                         continue
 
                     if name in primary_unit.architecture_names:
                         file_name = primary_unit.architecture_names[name]
                         yield library.get_source_file(file_name)
                     else:
                         LOGGER.warning(
```

### Comparing `vunit_hdl-4.6.2/vunit/sim_if/__init__.py` & `vunit_hdl-4.7.0/vunit/sim_if/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,21 @@
     @staticmethod
     def supports_vhdl_contexts():
         """
         Returns True when this simulator supports VHDL contexts
         """
         return True
 
+    @classmethod
+    def supports_vhdl_call_paths(cls):
+        """
+        Returns True when this simulator supports VHDL-2019 call paths
+        """
+        return False
+
     @staticmethod
     def find_executable(executable):
         """
         Return a list of all executables found in PATH
         """
         path = environ.get("PATH", None)
         if path is None:
@@ -173,15 +180,15 @@
     @staticmethod
     def supports_coverage():
         """
         Returns True when the simulator supports coverage
         """
         return False
 
-    def merge_coverage(self, file_name, args):  # pylint: disable=unused-argument, no-self-use
+    def merge_coverage(self, file_name, args):  # pylint: disable=unused-argument
         """
         Hook for simulator interface to creating coverage reports
         """
         raise RuntimeError("This simulator does not support merging coverage")
 
     def add_simulator_specific(self, project):
         """
@@ -312,15 +319,18 @@
 
 
 def isfile(file_name):
     """
     Case insensitive Path.is_file()
     """
     fpath = Path(file_name)
-    if not fpath.is_file():
+    try:
+        if not fpath.is_file():
+            return False
+    except PermissionError:
         return False
 
     return str(fpath.name) in listdir(str(fpath.parent))
 
 
 def run_command(command, cwd=None, env=None):
     """
```

### Comparing `vunit_hdl-4.6.2/vunit/sim_if/activehdl.py` & `vunit_hdl-4.7.0/vunit/sim_if/activehdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from functools import total_ordering
 from pathlib import Path
 import os
 import re
 import logging
 from ..exceptions import CompileError
 from ..ostools import Process, write_file, file_exists, renew_path
-from ..vhdl_standard import VHDL
 from ..test.suites import get_result_file_name
 from . import SimulatorInterface, ListOfStringOption, StringOption
 from .vsim_simulator_mixin import get_is_test_suite_done_tcl, fix_path
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -50,14 +49,21 @@
         return cls(prefix=cls.find_prefix(), output_path=output_path, gui=args.gui)
 
     @classmethod
     def find_prefix_from_path(cls):
         return cls.find_toolchain(["vsim", "avhdl"])
 
     @classmethod
+    def supports_vhdl_call_paths(cls):
+        """
+        Returns True when this simulator supports VHDL-2019 call paths
+        """
+        return True
+
+    @classmethod
     def supports_vhdl_package_generics(cls):
         """
         Returns True when this simulator supports VHDL package generics
         """
         proc = Process([str(Path(cls.find_prefix()) / "vcom"), "-version"], env=cls.get_env())
         consumer = VersionConsumer()
         proc.consume_output(consumer)
@@ -105,18 +111,15 @@
         raise CompileError
 
     @staticmethod
     def _std_str(vhdl_standard):
         """
         Convert standard to format of Active-HDL command line flag
         """
-        if vhdl_standard <= VHDL.STD_2008:
-            return f"-{vhdl_standard!s}"
-
-        raise ValueError(f"Invalid VHDL standard {vhdl_standard!s}")
+        return f"-{vhdl_standard!s}"
 
     def compile_vhdl_file_command(self, source_file):
         """
         Returns the command to compile a VHDL file
         """
         return (
             [
@@ -251,15 +254,15 @@
 
         if config.sim_options.get("disable_ieee_warnings", False):
             vsim_flags.append("-ieee_nowarn")
 
         # Add the the testbench top-level unit last as coverage is
         # only collected for the top-level unit specified last
 
-        vhdl_assert_stop_level_mapping = dict(warning=1, error=2, failure=3)
+        vhdl_assert_stop_level_mapping = {"warning": 1, "error": 2, "failure": 3}
 
         tcl = f"""
 proc vunit_load {{}} {{
     {set_generic_str}
     set vsim_failed [catch {{
         vsim {' '.join(vsim_flags)}
     }}]
```

### Comparing `vunit_hdl-4.6.2/vunit/sim_if/cds_file.py` & `vunit_hdl-4.7.0/vunit/sim_if/cds_file.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/sim_if/common.py` & `vunit_hdl-4.7.0/vunit/sim_if/common.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/sim_if/factory.py` & `vunit_hdl-4.7.0/vunit/sim_if/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 import os
 from .activehdl import ActiveHDLInterface
 from .ghdl import GHDLInterface
 from .incisive import IncisiveInterface
 from .modelsim import ModelSimInterface
+from .nvc import NVCInterface
 from .rivierapro import RivieraProInterface
 from . import BooleanOption, ListOfStringOption, VHDLAssertLevelOption
 
 
 class SimulatorFactory(object):
     """
     Create simulator instances
@@ -29,14 +30,15 @@
         """
         return [
             ModelSimInterface,
             RivieraProInterface,
             ActiveHDLInterface,
             GHDLInterface,
             IncisiveInterface,
+            NVCInterface,
         ]
 
     def _extract_compile_options(self):
         """
         Return all supported compile options
         """
         result = dict((opt.name, opt) for opt in [BooleanOption("enable_coverage")])
```

### Comparing `vunit_hdl-4.6.2/vunit/sim_if/ghdl.py` & `vunit_hdl-4.7.0/vunit/sim_if/ghdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         self._gui = gui
         self._gtkwave_fmt = "ghw" if gui and gtkwave_fmt is None else gtkwave_fmt
         self._gtkwave_args = gtkwave_args
         self._backend = backend
         self._vhdl_standard = None
         self._coverage_test_dirs = set()
 
-    def has_valid_exit_code(self):
+    def has_valid_exit_code(self):  # pylint: disable=arguments-differ
         """
         Return if the simulation should fail with nonzero exit codes
         """
         return self._vhdl_standard >= VHDL.STD_2008
 
     @classmethod
     def _get_version_output(cls, prefix):
@@ -247,15 +247,15 @@
         for library in self._project.get_libraries():
             cmd += [f"-P{library.directory!s}"]
 
         a_flags = source_file.compile_options.get("ghdl.a_flags", [])
         flags = source_file.compile_options.get("ghdl.flags", [])
         if flags != []:
             warn(
-                ("'ghdl.flags' is deprecated and it will be removed in future releases; " "use 'ghdl.a_flags' instead"),
+                ("'ghdl.flags' is deprecated and it will be removed in future releases; use 'ghdl.a_flags' instead"),
                 Warning,
             )
             a_flags += flags
 
         cmd += a_flags
 
         if source_file.compile_options.get("enable_coverage", False):
```

### Comparing `vunit_hdl-4.6.2/vunit/sim_if/incisive.py` & `vunit_hdl-4.7.0/vunit/sim_if/incisive.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/sim_if/modelsim.py` & `vunit_hdl-4.7.0/vunit/sim_if/modelsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
         # a space in the path even with escaping, see issue #36
         if " " not in self._sim_cfg_file_name:
             vsim_flags.insert(0, f"-modelsimini {fix_path(self._sim_cfg_file_name)!s}")
 
         for library in self._libraries:
             vsim_flags += ["-L", library.name]
 
-        vhdl_assert_stop_level_mapping = dict(warning=1, error=2, failure=3)
+        vhdl_assert_stop_level_mapping = {"warning": 1, "error": 2, "failure": 3}
 
         tcl = """
 proc vunit_load {{{{vsim_extra_args ""}}}} {{
     set vsim_failed [catch {{
         eval vsim ${{vsim_extra_args}} {{{vsim_flags}}}
     }}]
```

### Comparing `vunit_hdl-4.6.2/vunit/sim_if/rivierapro.py` & `vunit_hdl-4.7.0/vunit/sim_if/rivierapro.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,21 @@
         if version.year is not None:
             if (version.year == 2016 and version.month >= 10) or (version.year > 2016):
                 return cls.name
 
         return None
 
     @classmethod
+    def supports_vhdl_call_paths(cls):
+        """
+        Returns True when this simulator supports VHDL-2019 call paths
+        """
+        return True
+
+    @classmethod
     def supports_vhdl_package_generics(cls):
         """
         Returns True when this simulator supports VHDL package generics
         """
         return True
 
     @staticmethod
@@ -304,23 +311,23 @@
         vsim_flags += ["-lib", config.library_name, config.entity_name]
 
         if config.architecture_name is not None:
             vsim_flags.append(config.architecture_name)
 
         tcl = """
 proc vunit_load {{}} {{
-    # Make the variable 'aldec' visible; otherwise, the Matlab interface
-    # is broken because vsim does not find the library aldec_matlab_cosim.
-    global aldec
-    # Make the variable 'LICENSE_QUEUE' visible (if set); otherwise vsim
-    # will not wait for simulation licenses.
-    global LICENSE_QUEUE
+    # Run the 'vsim' command in the global variable context using 'uplevel'.
+    # This will make variables such as 'aldec' and 'LICENSE_QUEUE' visible, if set.
+    # Otherwise:
+    # - The Matlab interface is broken because vsim does not find the
+    #   library aldec_matlab_cosim
+    # - vsim will not wait for simulation licenses
 
     set vsim_failed [catch {{
-        eval vsim {{{vsim_flags}}}
+        uplevel #0 vsim {{{vsim_flags}}}
     }}]
 
     if {{${{vsim_failed}}}} {{
         return true
     }}
 
     if {{[_vunit_source_init_files_after_load]}} {{
```

### Comparing `vunit_hdl-4.6.2/vunit/sim_if/vsim_simulator_mixin.py` & `vunit_hdl-4.7.0/vunit/sim_if/vsim_simulator_mixin.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/source_file.py` & `vunit_hdl-4.7.0/vunit/source_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,14 @@
     ):
         SourceFile.__init__(self, str(name), library, "vhdl")
         self.dependencies = []  # type: ignore
         self.depending_components = []  # type: ignore
         self._vhdl_standard = vhdl_standard
 
         if not no_parse:
-
             try:
                 design_file = vhdl_parser.parse(self.name)
             except KeyboardInterrupt as exk:
                 raise KeyboardInterrupt from exk
             except:  # pylint: disable=bare-except
                 traceback.print_exc()
                 LOGGER.error("Failed to parse %s", self.name)
```

### Comparing `vunit_hdl-4.6.2/vunit/test/bench.py` & `vunit_hdl-4.7.0/vunit/test/bench.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         Return the test case with name or raise KeyError
         """
         for test_case in self._test_cases:
             if test_case.name == name:
                 return test_case
         raise KeyError(name)
 
-    def get_configuration_dicts(self):
+    def get_configuration_dicts(self):  # pylint: disable=arguments-differ
         """
         Get all configurations within the test bench
 
         If running all tests in the same simulation there are no individual test configurations
         """
         if self._individual_tests:
             configs = []
@@ -354,15 +354,15 @@
         self._check_enabled()
         return self._configs[DEFAULT_NAME]
 
     def _check_enabled(self):
         if not self._enable_configuration:
             raise RuntimeError("Individual test configuration is not possible with run_all_in_same_sim")
 
-    def get_configuration_dicts(self):
+    def get_configuration_dicts(self):  # pylint: disable=arguments-differ
         """
         Get all configurations of this test
         """
         return [self._configs]
 
     def _get_configurations_to_run(self):
         """
@@ -491,15 +491,14 @@
 def _check_duplicates(attrs, file_name, test_name=None):
     """
     Check for duplicate attributes, if test_name is None it is a file global attribute
     """
     previous = {}
     for attr in attrs:
         if attr.name in previous:
-
             loc = (
                 "" if test_name is None else f"test {test_name!s} in "
             ) + f"{file_name!s} line {attr.location.lineno:d}"
 
             raise RuntimeError(
                 f"Duplicate attribute {attr.name!s} of {loc!s}, "
                 f"previously defined on line {previous[attr.name].location.lineno:d}"
```

### Comparing `vunit_hdl-4.6.2/vunit/test/bench_list.py` & `vunit_hdl-4.7.0/vunit/test/bench_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             TB_PATTERN,
             generic_type,
             design_unit.file_name,
         )
 
     elif has_runner_cfg and not has_tb_name:
         LOGGER.warning(
-            "%s %s has runner_cfg %s but the file name and the %s name does not match regex %s\n" "in file %s",
+            "%s %s has runner_cfg %s but the file name and the %s name does not match regex %s\nin file %s",
             design_unit_type,
             design_unit.name,
             generic_type,
             design_unit_type.lower(),
             TB_PATTERN,
             design_unit.file_name,
         )
```

### Comparing `vunit_hdl-4.6.2/vunit/test/list.py` & `vunit_hdl-4.7.0/vunit/test/list.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/test/report.py` & `vunit_hdl-4.7.0/vunit/test/report.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/test/runner.py` & `vunit_hdl-4.7.0/vunit/test/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,14 @@
             for fptr in (ptr for ptr in [output_file, color_output_file] if ptr is not None):
                 fptr.flush()
                 fptr.close()
 
         any_not_passed = any(value != PASSED for value in results.values())
 
         with self._stdout_lock():
-
             if (color_output_file is not None) and (any_not_passed or self._is_verbose) and not self._is_quiet:
                 self._print_output(color_output_file_name)
 
             self._add_results(test_suite, results, start_time, num_tests, output_file_name)
 
             if self._fail_fast and any_not_passed:
                 self._abort = True
```

### Comparing `vunit_hdl-4.6.2/vunit/test/suites.py` & `vunit_hdl-4.7.0/vunit/test/suites.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
         return self._simulator_if.simulate(
             output_path=output_path,
             test_suite_name=self._test_suite_name,
             config=config,
             elaborate_only=self._elaborate_only,
         )
 
-    def _read_test_results(self, file_name):
+    def _read_test_results(self, file_name):  # pylint: disable=too-many-branches
         """
         Read test results from vunit_results file
         """
 
         results = {}
         for name in self._test_cases:
             results[name] = FAILED
@@ -254,30 +254,29 @@
             return results
 
         test_results = ostools.read_file(file_name)
         test_starts = []
         test_suite_done = False
 
         for line in test_results.splitlines():
-
             if line.startswith("test_start:"):
                 test_name = line[len("test_start:") :]
-                test_starts.append(test_name)
+                if test_name not in test_starts:
+                    test_starts.append(test_name)
 
             elif line.startswith("test_suite_done"):
                 test_suite_done = True
 
         for idx, test_name in enumerate(test_starts):
             last_start = idx == len(test_starts) - 1
 
             if test_suite_done or not last_start:
                 results[test_name] = PASSED
 
         for test_name in self._test_cases:
-
             # Anonymous test case
             if test_name is None:
                 results[test_name] = PASSED if test_suite_done else FAILED
                 continue
 
             if test_name not in test_starts:
                 results[test_name] = SKIPPED
```

### Comparing `vunit_hdl-4.6.2/vunit/ui/__init__.py` & `vunit_hdl-4.7.0/vunit/ui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import traceback
 import logging
 import json
 import os
 from typing import Optional, Set, Union
 from pathlib import Path
 from fnmatch import fnmatch
+
 from ..database import PickledDataBase, DataBase
 from .. import ostools
 from ..vunit_cli import VUnitCLI
 from ..sim_if.factory import SIMULATOR_FACTORY
 from ..sim_if import SimulatorInterface
 from ..color_printer import COLOR_PRINTER, NO_COLOR_PRINTER
 
@@ -35,15 +36,15 @@
 from ..vhdl_standard import VHDL, VHDLStandard
 from ..test.bench_list import TestBenchList
 from ..test.report import TestReport
 from ..test.runner import TestRunner
 
 from .common import LOGGER, TEST_OUTPUT_PATH, select_vhdl_standard, check_not_empty
 from .source import SourceFile, SourceFileList
-from .library import Library
+from .library import Library, LibraryList
 from .results import Results
 
 
 class VUnit(object):  # pylint: disable=too-many-instance-attributes, too-many-public-methods
     """
     The public interface of VUnit
 
@@ -68,19 +69,31 @@
         :param compile_builtins: Do not compile builtins. Used for VUnit internal testing.
         :param vhdl_standard: The VHDL standard used to compile files,
                               if None the VUNIT_VHDL_STANDARD environment variable is used
         :returns: A :class:`.VUnit` object instance
 
         :example:
 
-        .. code-block:: python
+          .. code-block:: python
 
-           from vunit import VUnit
-           prj = VUnit.from_argv()
+             from vunit import VUnit
+             prj = VUnit.from_argv()
 
+        .. IMPORTANT::
+          Option ``compile_builtins`` is deprecated and it will be removed in an upcoming release.
+          VHDL users will need to call method :meth:`add_vhdl_builtins` explicitly in order to preserve the
+          functionality.
+          See :vunit_issue:`777`.
+          It is therefore recommended to now use the following procedure:
+
+          .. code-block:: python
+
+             from vunit import VUnit
+             prj = VUnit.from_argv(compile_builtins=False)
+             prj.add_vhdl_builtins()
         """
         args = VUnitCLI().parse_args(argv=argv)
         return cls.from_args(args, compile_builtins=compile_builtins, vhdl_standard=vhdl_standard)
 
     @classmethod
     def from_args(
         cls,
@@ -96,14 +109,19 @@
 
         :param args: The parsed argument namespace object
         :param compile_builtins: Do not compile builtins. Used for VUnit internal testing.
         :param vhdl_standard: The VHDL standard used to compile files,
                               if None the VUNIT_VHDL_STANDARD environment variable is used
         :returns: A :class:`.VUnit` object instance
 
+        .. IMPORTANT::
+          Option ``compile_builtins`` is deprecated and it will be removed in an upcoming release.
+          VHDL users will need to call method :meth:`add_vhdl_builtins` explicitly in order to preserve the
+          functionality.
+          See :vunit_issue:`777`.
         """
         return cls(args, compile_builtins=compile_builtins, vhdl_standard=vhdl_standard)
 
     def __init__(
         self,
         args,
         compile_builtins: Optional[bool] = True,
@@ -127,17 +145,15 @@
             if args.without_attributes is not None:
                 keep = keep and set(args.without_attributes).isdisjoint(attribute_names)
             return keep
 
         self._test_filter = test_filter
         self._vhdl_standard: VHDLStandard = select_vhdl_standard(vhdl_standard)
 
-        self._external_preprocessors = []  # type: ignore
-        self._location_preprocessor = None
-        self._check_preprocessor = None
+        self._preprocessors = []  # type: ignore
 
         self._simulator_class = SIMULATOR_FACTORY.select_simulator()
 
         # Use default simulator options if no simulator was present
         if self._simulator_class is None:
             simulator_class = SimulatorInterface
             self._simulator_output_path = str(Path(self._output_path) / "none")
@@ -153,15 +169,29 @@
             depend_on_package_body=simulator_class.package_users_depend_on_bodies,
         )
 
         self._test_bench_list = TestBenchList(database=database)
 
         self._builtins = Builtins(self, self._vhdl_standard, simulator_class)
         if compile_builtins:
-            self.add_builtins()
+            self.add_vhdl_builtins()
+            hline = "=" * 75
+            print(hline)
+            LOGGER.warning(
+                """Option 'compile_builtins' of methods 'from_args' and 'from_argv' is deprecated.
+In future releases, it will be removed and builtins will need to be added explicitly.
+To prepare for upcoming changes, it is recommended to apply the following modifications in the run script now:
+
+* Use `from_argv(compile_builtins=False)` or `from_args(compile_builtins=False)`.
+* Add an explicit call to 'add_vhdl_builtins'.
+
+See https://github.com/VUnit/vunit/issues/777.
+"""
+            )
+            print(hline)
 
     def _create_database(self):
         """
         Create a persistent database to store expensive parse results
 
         Check for Python version used to create the database is the
         same as the running python instance or re-create
@@ -236,15 +266,15 @@
 
         :param project_csv_path: path to csv project specification, each line contains the name
                                  of the library and the path to one file 'lib_name,filename'
                                  note that all filenames are relative to the parent folder of the
                                  csv file
         :param vhdl_standard: The VHDL standard used to compile files,
                               if None, the VUNIT_VHDL_STANDARD environment variable is used
-        :returns: A list of files (:class `.SourceFileList`) that were added
+        :returns: A list of files (:class:`.SourceFileList`) that were added
 
         """
         libs: Set[str] = set()
         files = SourceFileList([])
 
         ppath = Path(project_csv_path)
 
@@ -301,14 +331,38 @@
         :param library_name: The name of the library
         :returns: A :class:`.Library` object
         """
         if not self._project.has_library(library_name):
             raise KeyError(library_name)
         return Library(library_name, self, self._project, self._test_bench_list)
 
+    def get_libraries(
+        self,
+        pattern="*",
+        allow_empty: Optional[bool] = False,
+    ):
+        """
+        Get a list of libraries
+
+        :param pattern: A wildcard pattern matching the library name
+        :param allow_empty: To disable an error if no labraries matched the pattern
+        :returns: A :class:`.LibraryList` object
+        """
+        results = []
+
+        for library in self._project.get_libraries():
+            if not fnmatch(library.name, pattern):
+                continue
+
+            results.append(self.library(library.name))
+
+        check_not_empty(results, allow_empty, f"Pattern {pattern} did not match any library")
+
+        return LibraryList(results)
+
     def set_attribute(self, name: str, value: str, allow_empty: Optional[bool] = False):
         """
         Set a value of attribute in all |configurations|
 
         :param name: The name of the attribute
         :param value: The value of the attribute
         :param allow_empty: To disable an error when no test benches were found
@@ -577,28 +631,28 @@
             no_parse=no_parse,
             file_type=file_type,
         )
 
     def _preprocess(self, library_name: str, file_name: Union[str, Path], preprocessors):
         """
         Preprocess file_name within library_name using explicit preprocessors
-        if preprocessors is None then use implicit globally defined processors
+        if preprocessors is None then use implicit globally defined preprocessors.
         """
         # @TODO dependency checking etc...
 
         if preprocessors is None:
-            preprocessors = [self._location_preprocessor, self._check_preprocessor]
-            preprocessors = [p for p in preprocessors if p is not None]
-            preprocessors = self._external_preprocessors + preprocessors
+            preprocessors = self._preprocessors
 
         fstr = str(file_name)
 
         if not preprocessors:
             return fstr
 
+        preprocessors.sort(key=lambda x: 0 if not hasattr(x, "order") else x.order)
+
         fname = str(Path(file_name).name)
 
         try:
             code = ostools.read_file(file_name, encoding=HDL_FILE_ENCODING)
             for preprocessor in preprocessors:
                 code = preprocessor.run(code, fname)
         except KeyboardInterrupt as exk:
@@ -619,50 +673,59 @@
                 idx += 1
 
             ostools.write_file(pp_file_name, code, encoding=HDL_FILE_ENCODING)
             return pp_file_name
 
     def add_preprocessor(self, preprocessor):
         """
-        Add a custom preprocessor to be used on all files, must be called before adding any files
+        Adds a custom preprocessor to be used on all files. Must be called before adding any files.
+
+        :param preprocessor: Instance of of :class:`.Preprocessor`
         """
-        self._external_preprocessors.append(preprocessor)
+        self._preprocessors.append((preprocessor))
 
-    def enable_location_preprocessing(self, additional_subprograms=None, exclude_subprograms=None):
+    def enable_location_preprocessing(self, additional_subprograms=None, exclude_subprograms=None, order=100):
         """
         Inserts file name and line number information into VUnit check and log subprograms calls. Custom
         subprograms can also be added. Must be called before adding any files.
 
         :param additional_subprograms: List of custom subprograms to add the line_num and file_name parameters to.
         :param exclude_subprograms: List of VUnit subprograms to exclude from location preprocessing. Used to \
 avoid location preprocessing of other functions sharing name with a VUnit log or check subprogram.
+        :param order: Integer controlling in which order the location preprocessor is applied in relation to \
+other preprocessors. Lowest value first. The order between preprocessors with the same value is undefined.
 
         :example:
 
         .. code-block:: python
 
            prj.enable_location_preprocessing(additional_subprograms=['my_check'],
                                              exclude_subprograms=['log'])
 
         """
-        preprocessor = LocationPreprocessor()
+        preprocessor = LocationPreprocessor(order)
         if additional_subprograms is not None:
             for subprogram in additional_subprograms:
                 preprocessor.add_subprogram(subprogram)
 
         if exclude_subprograms is not None:
             for subprogram in exclude_subprograms:
                 preprocessor.remove_subprogram(subprogram)
-        self._location_preprocessor = preprocessor
 
-    def enable_check_preprocessing(self):
+        self.add_preprocessor(preprocessor)
+
+    def enable_check_preprocessing(self, order=200):
         """
-        Inserts error context information into VUnit check_relation calls
+        Inserts error context information into VUnit check_relation calls.
+
+        :param order: Integer controlling in which order the check preprocessor is applied in relation to \
+other preprocessors. Lowest value first. The order between preprocessors with the same value is undefined.
+
         """
-        self._check_preprocessor = CheckPreprocessor()
+        self.add_preprocessor(CheckPreprocessor(order))
 
     def main(self, post_run=None):
         """
         Run vunit main function and exit
 
         :param post_run: A callback function which is called after
           running tests. The function must accept a single `results`
@@ -783,18 +846,18 @@
         Main function when exporting to JSON
         """
 
         file_objects = self.get_compile_order()
         files = []
         for source_file in file_objects:
             files.append(
-                dict(
-                    file_name=str(Path(source_file.name).resolve()),
-                    library_name=source_file.library.name,
-                )
+                {
+                    "file_name": str(Path(source_file.name).resolve()),
+                    "library_name": source_file.library.name,
+                }
             )
 
         tests = []
         for test_suite in self._create_tests(simulator_if=None):
             test_information = test_suite.test_information
             test_configuration = test_suite.test_configuration
             for name in test_suite.test_names:
@@ -804,33 +867,33 @@
                 attributes = {}
                 for attr in info.attributes:
                     attributes[attr.name] = attr.value
 
                 attributes.update(config.attributes)
 
                 tests.append(
-                    dict(
-                        name=name,
-                        location=dict(
-                            file_name=str(info.location.file_name),
-                            offset=info.location.offset,
-                            length=info.location.length,
-                        ),
-                        attributes=attributes,
-                    )
+                    {
+                        "name": name,
+                        "location": {
+                            "file_name": str(info.location.file_name),
+                            "offset": info.location.offset,
+                            "length": info.location.length,
+                        },
+                        "attributes": attributes,
+                    }
                 )
 
-        json_data = dict(
+        json_data = {
             # The semantic version (https://semver.org/) of the JSON export data format
-            export_format_version=dict(major=1, minor=0, patch=0),
+            "export_format_version": {"major": 1, "minor": 0, "patch": 0},
             # The set of files added to the project
-            files=files,
+            "files": files,
             # The list of all tests
-            tests=tests,
-        )
+            "tests": tests,
+        }
 
         with Path(json_file_name).open("w", encoding="utf-8") as fptr:
             json.dump(json_data, fptr, sort_keys=True, indent=4, separators=(",", ": "))
 
         return True
 
     def _main_list_files_only(self):
@@ -921,23 +984,45 @@
             num_threads=self._args.num_threads,
             fail_fast=self._args.fail_fast,
             dont_catch_exceptions=self._args.dont_catch_exceptions,
             no_color=self._args.no_color,
         )
         runner.run(test_cases)
 
-    def add_builtins(self, external=None):
+    def add_verilog_builtins(self):
+        """
+        Add VUnit Verilog builtin libraries.
+
+        .. IMPORTANT::
+          Class ``vunit.verilog`` is deprecated and it will be removed in an upcoming release.
+          Verilog users will need to call this method explicitly in order to preserve the functionality.
+          See :vunit_issue:`777`.
         """
-        Add vunit VHDL builtin libraries
+        self._builtins.add_verilog_builtins()
+
+    def add_vhdl_builtins(self, external=None):
+        """
+        Add VUnit VHDL builtin libraries.
 
         :param external: struct to provide bridges for the external VHDL API.
-                         {
-                             'string': ['path/to/custom/file'],
-                             'integer': ['path/to/custom/file']
-                         }.
+
+        :example:
+
+        .. code-block:: python
+
+            VU.add_vhdl_builtins(external={
+                'string': ['path/to/custom/file'],
+                'integer': ['path/to/custom/file']}
+            )
+
+        .. IMPORTANT::
+          Option ``compile_builtins`` of methods :meth:`from_argv` and :meth:`from_args` is deprecated and it will be
+          removed in an upcoming release.
+          VHDL users will need to call this method explicitly in order to preserve the functionality.
+          See :vunit_issue:`777`.
         """
         self._builtins.add_vhdl_builtins(external=external)
 
     def add_com(self):
         """
         Add communication package
         """
@@ -983,15 +1068,15 @@
         can be successfully compiled.
 
         This is **not** the same as all files required to successfully elaborate **A**.
         For example using component instantiation in VHDL there is no
         compile order dependency but the component instance will not
         elaborate if there is no binding component.
 
-        :param source_files: A list of :class:`.SourceFile` objects or `None` meaing all
+        :param source_files: A list of :class:`.SourceFile` objects or `None` meaning all
         :returns: A list of :class:`.SourceFile` objects in compile order.
         """
         if source_files is None:
             source_files = self.get_source_files(allow_empty=True)
 
         target_files = [source_file._source_file for source_file in source_files]  # pylint: disable=protected-access
         source_files = self._project.get_dependencies_in_compile_order(target_files)
```

### Comparing `vunit_hdl-4.6.2/vunit/ui/common.py` & `vunit_hdl-4.7.0/vunit/ui/common.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/ui/packagefacade.py` & `vunit_hdl-4.7.0/vunit/ui/packagefacade.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/ui/results.py` & `vunit_hdl-4.7.0/vunit/ui/results.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/ui/source.py` & `vunit_hdl-4.7.0/vunit/ui/source.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/ui/test.py` & `vunit_hdl-4.7.0/vunit/ui/test.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/ui/testbench.py` & `vunit_hdl-4.7.0/vunit/ui/testbench.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .test import Test
 
 
 class TestBench(object):
     """
     User interface of a test bench.
     A test bench consists of one or more :class:`.Test` cases. Setting options for a test
-    bench will apply that option all test cases belonging to that test bench.
+    bench will apply that option to all test cases belonging to that test bench.
     """
 
     def __init__(self, test_bench, library):
         self._test_bench = test_bench
         self._library = library
 
     @property
@@ -205,17 +205,17 @@
                 continue
 
             results.append(Test(test_case))
         return results
 
     def scan_tests_from_file(self, file_name):
         """
-        Scan tests from another file than the one containg the test
+        Scan tests from another file than the one containing the test
         bench.  Useful for when the top level test bench does not
-        contain the tests.
+        contain any tests.
 
         Such a structure is not the preferred way of doing things in
         VUnit but this method exists to accommodate legacy needs.
 
         :param file_name: The name of another file to scan for tests
 
         .. warning::
```

### Comparing `vunit_hdl-4.6.2/vunit/verilog/check/test/check_tb.sv` & `vunit_hdl-4.7.0/vunit/verilog/check/test/check_tb.sv`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -244,8 +244,8 @@
                $sformat(test_expected, "CHECK_EQUAL_VARIANCE failed! Got tc_data1.data_time=%0d expected %0d +-%0d. ", tc_data1.data_time, tc_data2.data_time, `TEST_VARIANCE);
                check_macro_output(test_output, test_expected);
                test_output = "";
             end
          end
       end
    end
-endmodule
+endmodule
```

### Comparing `vunit_hdl-4.6.2/vunit/verilog/include/vunit_defines.svh` & `vunit_hdl-4.7.0/vunit/verilog/include/vunit_defines.svh`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // This Source Code Form is subject to the terms of the Mozilla Public
 // License, v. 2.0. If a copy of the MPL was not distributed with this file,
 // You can obtain one at http://mozilla.org/MPL/2.0/.
 //
-// Copyright (c) 2015-2021, Lars Asplund lars.anders.asplund@gmail.com
+// Copyright (c) 2014-2023, Lars Asplund lars.anders.asplund@gmail.com
 
 `define WATCHDOG(runtime) \
    initial begin \
       __runner__.watchdog((runtime) / 1ns); \
    end
 
 `define TEST_SUITE_FROM_PARAMETER(parameter_name) \
@@ -83,8 +83,8 @@
          expected_str ="";\
          variance_str="";\
          `CREATE_ARG_STRING(got, got_str); \
          `CREATE_ARG_STRING(expected, expected_str); \
          `CREATE_ARG_STRING(variance, variance_str); \
              full_msg = {"CHECK_EQUAL_VARIANCE failed! Got ",`"got`", "=",  got_str, " expected ", expected_str, " +-", variance_str, ". ", msg}; \
              `__ERROR_FUNC(full_msg); \
-          end
+          end
```

### Comparing `vunit_hdl-4.6.2/vunit/verilog/vunit_pkg.sv` & `vunit_hdl-4.7.0/vunit/verilog/vunit_pkg.sv`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/version_check.py` & `vunit_hdl-4.7.0/vunit/version_check.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/LICENSE.md` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/README.md` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/README.md`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/data/Boards2.json` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/data/Boards2.json`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/examples/Boards0.vhdl` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/examples/Boards0.vhdl`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/examples/Boards1.vhdl` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/examples/Boards1.vhdl`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/examples/Boards2.vhdl` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/examples/Boards2.vhdl`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/examples/Boards_VUnit.vhdl` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/examples/Boards_VUnit.vhdl`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/examples/Encodings_VUnit.vhdl` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/examples/Encodings_VUnit.vhdl`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/src/Encodings.pkg.vhdl` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/src/Encodings.pkg.vhdl`

 * *Files 19% similar despite different names*

```diff
@@ -33,23 +33,20 @@
       result(2 * x - 1 to 2 * x) := lower(to_hex_string(
         to_ufixed(character'pos(str_i(x)), 7, 0)
       )(1 to 2));
     end loop;
     return result;
   end function;
 
-  function base16_decode(constant str: string) return string is
+  function base16_decode(constant str : string) return string is
     alias str_i : string(1 to str'length) is str;
-    variable result: string (1 to (str'length + 1) / 2);
+    variable result : string (1 to (str'length + 1) / 2);
+    variable byte_as_hex : string(1 to 2);
   begin
     for x in result'range loop
-      result(x) := character'val(to_integer(
-        to_unsigned(from_hex_string(
-          str_i(2 * x - 1 to 2 * x),
-          7, 0
-        ), 8)
-      ));
+      byte_as_hex := str_i(2 * x - 1 to 2 * x);
+      result(x) := character'val(to_integer(to_unsigned(from_hex_string(byte_as_hex, 7, 0), 8)));
     end loop;
     return result;
   end function;
 
 end package body;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/src/JSON.ctx.vhdl` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/src/JSON.ctx.vhdl`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/src/JSON.pkg.vhdl` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/src/JSON.pkg.vhdl`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/JSONTestSuite.ps1` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/JSONTestSuite.ps1`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/LICENSE.md` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/TopLevel.vhdl` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/JSONTestSuite/TopLevel.vhdl`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Lattice/Lattice.ldf` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Lattice/Lattice.ldf`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Lattice/Lattice1.sty` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Lattice/Lattice1.sty`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/QuestaSim/Boards2.cmd` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/QuestaSim/Boards2.cmd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/QuestaSim/Boards2.log` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/QuestaSim/Boards2.log`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/VUnit/run.py` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/VUnit/run.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/JSON.xise` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/JSON.xise`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/iseconfig/filter.filter` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Xilinx ISE/iseconfig/filter.filter`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/Xilinx Vivado/Xilinx Vivado.xpr` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/Xilinx Vivado/Xilinx Vivado.xpr`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.cmd` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.cmd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.log` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.log`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.sh` & `vunit_hdl-4.7.0/vunit/vhdl/JSON-for-VHDL/tests/ghdl/Boards2.sh`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/array/src/array_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/array/src/array_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/array/test/tb_array.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/array/test/tb_array.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/run.py` & `vunit_hdl-4.7.0/vunit/vhdl/check/run.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/src/check.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/src/check.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -8,64 +8,38 @@
 
 library ieee;
 use ieee.std_logic_1164.all;
 use ieee.numeric_std.all;
 use std.textio.all;
 use work.checker_pkg.all;
 use work.string_ops.all;
+use work.location_pkg.all;
+use work.integer_vector_ptr_pkg.all;
 
 package body check_pkg is
   type boolean_vector is array (natural range <>) of boolean;
 
+  function result(str : string := "") return string is
+  begin
+    return decorate(str);
+  end;
+
   function logical_right_shift (
     constant arg   : boolean_vector;
     constant count : natural)
     return boolean_vector is
     variable ret_val : boolean_vector(0 to arg'length - 1) := (others => false);
     constant temp    : boolean_vector(0 to arg'length - 1) := arg;
   begin
     ret_val(count to ret_val'right) := temp(0 to ret_val'right - count);
 
     return ret_val;
   end function logical_right_shift;
   constant max_supported_num_of_bits_in_integer_implementation : natural := 256;
 
-  function std_msg (
-    constant check_result : string;
-    constant msg          : string;
-    constant ctx          : string)
-    return string is
-    constant msg_i : string(1 to msg'length) := msg;
-
-    function replace_result_tag (msg, check_result : string) return string is
-    begin
-      if msg'length < check_result_tag'length then
-        return msg;
-      elsif msg(1 to check_result_tag'length) = check_result_tag then
-        return check_result & msg(check_result_tag'length + 1 to msg'right);
-      else
-        return msg;
-      end if;
-    end function replace_result_tag;
-
-    function append_context (msg, ctx : string) return string is
-    begin
-      if msg = "" then
-        return ctx;
-      elsif ctx = "" then
-        return msg;
-      else
-        return msg & " - " & ctx;
-      end if;
-    end function append_context;
-  begin
-    return append_context(replace_result_tag(msg_i, check_result), ctx);
-  end function std_msg;
-
-
   procedure get_checker_stat (
     variable stat : out checker_stat_t) is
   begin
     get_checker_stat(default_checker, stat);
   end;
 
   impure function get_checker_stat
@@ -116,26 +90,14 @@
     elsif active_clock_edge = both_edges then
       return falling_edge(clock) or rising_edge(clock);
     else
       return false;
     end if;
   end start_condition;
 
-  function result (msg : string := "") return string is
-  begin
-    if msg = "" then
-      return check_result_tag;
-    elsif msg(msg'left) = '.' or msg(msg'left) = ',' or msg(msg'left) = ':' or
-      msg(msg'left) = ';' or msg(msg'left) = '?' or msg(msg'left) = '!' then
-      return check_result_tag & msg;
-    else
-      return check_result_tag & " " & msg;
-    end if;
-  end;
-
   function to_ordinal_number (num : unsigned) return string is
     constant num_str      : string := to_integer_string(num);
     variable ordinal_unit : string(1 to 2);
   begin
     case num_str(num_str'right) is
       when '1'    => ordinal_unit := "st";
       when '2'    => ordinal_unit := "nd";
@@ -148,14 +110,40 @@
         ordinal_unit := "th";
       end if;
     end if;
 
     return num_str & ordinal_unit;
   end function to_ordinal_number;
 
+  procedure log(check_result : check_result_t) is
+  begin
+    -- pragma translate_off
+    if check_result.p_is_pass then
+      if is_pass_visible(check_result.p_checker) and (check_result.p_msg /= null_string_ptr) then
+        log_passing_check(check_result.p_checker, to_string(check_result.p_msg), 0, check_result.p_line_num, to_string(check_result.p_file_name));
+      else
+        log_passing_check(check_result.p_checker);
+      end if;
+    else
+      p_handle(check_result);
+      log_failing_check(check_result.p_checker, to_string(check_result.p_msg), check_result.p_level, 0, check_result.p_line_num, to_string(check_result.p_file_name));
+    end if;
+
+    p_recycle_check_result(check_result);
+    -- pragma translate_on
+  end;
+
+  procedure notify_if_fail(check_result : check_result_t; signal event : inout any_event_t) is
+  begin
+    if not check_result.p_is_pass then
+      notify(event);
+    end if;
+    log(check_result);
+  end;
+
   -----------------------------------------------------------------------------
   -- check
   -----------------------------------------------------------------------------
   procedure check(
     constant checker           : in checker_t;
     signal clock               : in std_logic;
     signal en                  : in std_logic;
@@ -183,21 +171,21 @@
     constant line_num    : in  natural     := 0;
     constant file_name   : in  string      := "") is
   begin
     -- pragma translate_off
     if expr then
       pass := true;
       if is_pass_visible(checker) then
-        passing_check(checker, std_msg("Check passed", msg, ""), path_offset, line_num, file_name);
+        passing_check(checker, p_std_msg("Check passed", msg, ""), path_offset, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
-      failing_check(checker, std_msg("Check failed", msg, ""), level, path_offset, line_num, file_name);
+      failing_check(checker, p_std_msg("Check failed", msg, ""), level, path_offset, line_num, file_name);
     end if;
   -- pragma translate_on
   end;
 
   procedure check(
     constant checker     : in checker_t;
     constant expr        : in boolean;
@@ -253,14 +241,26 @@
   begin
     -- pragma translate_off
     check(default_checker, pass, expr, msg, level, path_offset, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check(
+    constant expr        : in boolean;
+    constant msg         : in string      := check_result_tag & ".";
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    return check(default_checker, expr, msg, level, path_offset, line_num, file_name);
+  end;
+
   procedure check(
     signal clock               : in std_logic;
     signal en                  : in std_logic;
     signal expr                : in std_logic;
     constant msg               : in string      := check_result_tag & ".";
     constant level             : in log_level_t := null_log_level;
     constant active_clock_edge : in edge_t      := rising_edge;
@@ -285,27 +285,58 @@
     variable pass : boolean;
   begin
     -- pragma translate_off
     check(checker, pass, expr, msg, level, path_offset, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
+
+  impure function check(
+    constant checker     : in checker_t;
+    constant expr        : in boolean;
+    constant msg         : in string      := check_result_tag & ".";
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => expr,
+      msg => msg,
+      std_pass_msg => "Check passed",
+      std_fail_msg => "Check failed",
+      std_pass_ctx => "",
+      std_fail_ctx => "",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
   -----------------------------------------------------------------------------
   -- check_passed
   -----------------------------------------------------------------------------
   procedure check_passed(
     constant checker     : in checker_t;
     constant msg         : in string  := check_result_tag & ".";
     constant path_offset : in natural := 0;
     constant line_num    : in natural := 0;
     constant file_name   : in string  := "") is
   begin
     -- pragma translate_off
     if is_pass_visible(checker) then
-      passing_check(checker, std_msg("Unconditional check passed", msg, ""), path_offset, line_num, file_name);
+      passing_check(checker, p_std_msg("Unconditional check passed", msg, ""), path_offset, line_num, file_name);
     else
       passing_check(checker);
     end if;
   -- pragma translate_on
   end;
 
   procedure check_passed(
@@ -327,27 +358,27 @@
     constant msg         : in string      := check_result_tag & ".";
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "") is
   begin
     -- pragma translate_off
-    failing_check(checker, std_msg("Unconditional check failed", msg, ""), level, path_offset, line_num, file_name);
+    failing_check(checker, p_std_msg("Unconditional check failed", msg, ""), level, path_offset, line_num, file_name);
   -- pragma translate_on
   end;
 
   procedure check_failed(
     constant msg         : in string      := check_result_tag & ".";
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "") is
   begin
     -- pragma translate_off
-    failing_check(default_checker, std_msg("Unconditional check failed", msg, ""), level, path_offset, line_num, file_name);
+    failing_check(default_checker, p_std_msg("Unconditional check failed", msg, ""), level, path_offset, line_num, file_name);
   -- pragma translate_on
   end;
 
   -----------------------------------------------------------------------------
   -- check_true
   -----------------------------------------------------------------------------
   procedure check_true(
@@ -378,21 +409,21 @@
     constant line_num    : in  natural     := 0;
     constant file_name   : in  string      := "") is
   begin
     -- pragma translate_off
     if expr then
       pass := true;
       if is_pass_visible(checker) then
-        passing_check(checker, std_msg("True check passed", msg, ""), path_offset, line_num, file_name);
+        passing_check(checker, p_std_msg("True check passed", msg, ""), path_offset, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
-      failing_check(checker, std_msg("True check failed", msg, ""), level, path_offset, line_num, file_name);
+      failing_check(checker, p_std_msg("True check failed", msg, ""), level, path_offset, line_num, file_name);
     end if;
   -- pragma translate_on
   end;
 
   procedure check_true(
     constant checker     : in checker_t;
     constant expr        : in boolean;
@@ -448,14 +479,26 @@
   begin
     -- pragma translate_off
     check_true(default_checker, pass, expr, msg, level, path_offset, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_true(
+    constant expr        : in boolean;
+    constant msg         : in string      := check_result_tag & ".";
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    return check_true(default_checker, expr, msg, level, path_offset, line_num, file_name);
+  end;
+
   procedure check_true(
     signal clock               : in std_logic;
     signal en                  : in std_logic;
     signal expr                : in std_logic;
     constant msg               : in string      := check_result_tag & ".";
     constant level             : in log_level_t := null_log_level;
     constant active_clock_edge : in edge_t      := rising_edge;
@@ -480,14 +523,44 @@
     variable pass : boolean;
   begin
     -- pragma translate_off
     check_true(checker, pass, expr, msg, level, path_offset, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
+
+  impure function check_true(
+    constant checker     : in checker_t;
+    constant expr        : in boolean;
+    constant msg         : in string      := check_result_tag & ".";
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => expr,
+      msg => msg,
+      std_pass_msg => "True check passed",
+      std_fail_msg => "True check failed",
+      std_pass_ctx => "",
+      std_fail_ctx => "",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
   -----------------------------------------------------------------------------
   -- check_false
   -----------------------------------------------------------------------------
   procedure check_false(
     constant checker           : in checker_t;
     signal clock               : in std_logic;
     signal en                  : in std_logic;
@@ -515,21 +588,21 @@
     constant line_num    : in  natural     := 0;
     constant file_name   : in  string      := "") is
   begin
     -- pragma translate_off
     if not expr then
       pass := true;
       if is_pass_visible(checker) then
-        passing_check(checker, std_msg("False check passed", msg, ""), path_offset, line_num, file_name);
+        passing_check(checker, p_std_msg("False check passed", msg, ""), path_offset, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
-      failing_check(checker, std_msg("False check failed", msg, ""), level, path_offset, line_num, file_name);
+      failing_check(checker, p_std_msg("False check failed", msg, ""), level, path_offset, line_num, file_name);
     end if;
   -- pragma translate_on
   end;
 
   procedure check_false(
     constant checker     : in checker_t;
     constant expr        : in boolean;
@@ -659,24 +732,24 @@
   begin
     -- pragma translate_off
     if (not antecedent_expr) or consequent_expr then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Implication check passed", msg,
             "Got " & boolean'image(antecedent_expr) & " -> " & boolean'image(consequent_expr) & "."),
           path_offset, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
-      failing_check(checker, std_msg("Implication check failed", msg, ""), level, path_offset, line_num, file_name);
+      failing_check(checker, p_std_msg("Implication check failed", msg, ""), level, path_offset, line_num, file_name);
     end if;
   -- pragma translate_on
   end;
 
   procedure check_implication(
     signal clock               : in std_logic;
     signal en                  : in std_logic;
@@ -817,43 +890,43 @@
     begin
       clock_edge_counter := x"0000000000000001";
       ref                := to_x01(expr);
       open_ok            := true;
       if is_x(start_event) then
         open_ok := false;
         failing_check(checker,
-                      std_msg("Stability check failed", msg,
+                      p_std_msg("Stability check failed", msg,
                               "Start event is " & format(start_event) & "."),
                       level, path_offset, line_num, file_name);
       elsif is_x(expr) then
         open_ok := false;
         failing_check(checker,
-                      std_msg("Stability check failed", msg,
+                      p_std_msg("Stability check failed", msg,
                               "Got " & format(expr) &
                               " at 1st active and enabled clock edge."),
                       level, path_offset, line_num, file_name);
       end if;
     end procedure;
 
     procedure close_window(cycle : unsigned; is_ok : boolean) is
       variable close_ok    : boolean := is_ok;
       variable pass_msg_en : boolean;
     begin
       if is_x(end_event) then
         close_ok := false;
         failing_check(checker,
-                      std_msg("Stability check failed", msg,
+                      p_std_msg("Stability check failed", msg,
                               "End event is " & format(end_event) & "."),
                       level, path_offset, line_num, file_name);
       end if;
 
       if close_ok then
         if is_pass_visible(checker) then
           passing_check(checker,
-                        std_msg("Stability check passed", msg,
+                        p_std_msg("Stability check passed", msg,
                                 "Got " & format(ref) &
                                 " for " & to_integer_string(cycle) &
                                 " active and enabled clock edges."),
                         path_offset, line_num, file_name);
         else
           passing_check(checker);
         end if;
@@ -890,15 +963,15 @@
             exit_stability_check := true;
             return;
           end if;
 
         elsif ref /= to_x01(expr) then
           is_stable := false;
           failing_check(checker,
-                        std_msg("Stability check failed", msg,
+                        p_std_msg("Stability check failed", msg,
                                 "Got " & format(expr) &
                                 " at " & to_ordinal_number(clock_edge_counter) &
                                 " active and enabled clock edge. Expected " &
                                 format(ref) & "."), level, path_offset, line_num, file_name);
         end if;
 
         if to_x01(end_event) /= '0' then
@@ -1050,25 +1123,25 @@
     constant file_name   : in  string      := "") is
   begin
     -- pragma translate_off
     if not is_x(expr) then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(checker,
-                      std_msg("Not unknown check passed",
+                      p_std_msg("Not unknown check passed",
                               msg,
                               "Got " & to_nibble_string(expr) & " (" & to_integer_string(expr) & ")" & "."),
                       path_offset, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(checker,
-                    std_msg("Not unknown check failed",
+                    p_std_msg("Not unknown check failed",
                             msg,
                             "Got " & to_nibble_string(expr) & "."),
                     level, path_offset, line_num, file_name);
     end if;
   -- pragma translate_on
   end;
 
@@ -1194,25 +1267,25 @@
     constant file_name   : in  string      := "") is
   begin
     -- pragma translate_off
     if not is_x(expr) then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(checker,
-                      std_msg("Not unknown check passed",
+                      p_std_msg("Not unknown check passed",
                               msg,
                               "Got " & std_logic'image(expr)(2) & "."),
                       path_offset, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(checker,
-                    std_msg("Not unknown check failed",
+                    p_std_msg("Not unknown check failed",
                             msg,
                             "Got " & std_logic'image(expr)(2) & "."),
                     level, path_offset, line_num, file_name);
     end if;
   -- pragma translate_on
   end;
 
@@ -1360,24 +1433,24 @@
     constant file_name   : in  string      := "") is
   begin
     -- pragma translate_off
     if n_hot_in_valid_range(expr, 0, 1) then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(checker,
-                      std_msg("Zero one-hot check passed", msg,
+                      p_std_msg("Zero one-hot check passed", msg,
                               "Got " & to_nibble_string(expr) & "."),
                       path_offset, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(checker,
-                    std_msg("Zero one-hot check failed", msg,
+                    p_std_msg("Zero one-hot check failed", msg,
                             "Got " & to_nibble_string(expr) & "."),
                     level, path_offset, line_num, file_name);
     end if;
   -- pragma translate_on
   end;
 
   procedure check_zero_one_hot(
@@ -1505,24 +1578,24 @@
     constant file_name   : in  string      := "") is
   begin
     -- pragma translate_off
     if n_hot_in_valid_range(expr, 1, 1) then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(checker,
-                      std_msg("One-hot check passed", msg,
+                      p_std_msg("One-hot check passed", msg,
                               "Got " & to_nibble_string(expr) & "."),
                       path_offset, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(checker,
-                    std_msg("One-hot check failed", msg,
+                    p_std_msg("One-hot check failed", msg,
                             "Got " & to_nibble_string(expr) & "."),
                     level, path_offset, line_num, file_name);
     end if;
   -- pragma translate_on
   end;
 
   procedure check_one_hot(
@@ -1669,21 +1742,21 @@
       return schedule(1 to schedule'right) /= no_pending_checks;
     end function pending_check;
 
     procedure check_expr is
     begin
       if to_x01(expr) = '1' then
         if is_pass_visible(checker) then
-          passing_check(checker, std_msg("Next check passed", msg, ""), path_offset, line_num, file_name);
+          passing_check(checker, p_std_msg("Next check passed", msg, ""), path_offset, line_num, file_name);
         else
           passing_check(checker);
         end if;
       else
         failing_check(checker,
-                      std_msg("Next check failed", msg,
+                      p_std_msg("Next check failed", msg,
                               "Got " & std_logic'image(expr)(2) &
                               " at the " & to_ordinal_number(to_unsigned(num_cks, 32)) &
                               " active and enabled clock edge."),
                       level, path_offset, line_num, file_name);
       end if;
     end procedure check_expr;
 
@@ -1692,35 +1765,35 @@
     while true loop
       wait_on_edge(clock, en, active_clock_edge);
       clock_cycles_after_start_event := clock_cycles_after_start_event + 1;
 
       if to_x01(start_event) = '1' then
         if pending_check(schedule) and not allow_overlapping then
           failing_check(checker,
-                        std_msg("Next check failed", msg,
+                        p_std_msg("Next check failed", msg,
                                 "Got overlapping start event at the " &
                                 to_ordinal_number(to_unsigned(clock_cycles_after_start_event, 32)) &
                                 " active and enabled clock edge."),
                         level, path_offset, line_num, file_name);
         else
           schedule_check(schedule, num_cks);
           clock_cycles_after_start_event := 0;
         end if;
       elsif to_x01(start_event) = 'X' then
         failing_check(checker,
-                      std_msg("Next check failed", msg,
+                      p_std_msg("Next check failed", msg,
                               "Start event is " & std_logic'image(start_event)(2) & "."),
                       level, path_offset, line_num, file_name);
       end if;
 
       if check_is_scheduled(schedule) then
         check_expr;
       elsif (to_x01(expr) = '1') and not allow_missing_start then
         failing_check(checker,
-                      std_msg("Next check failed", msg,
+                      p_std_msg("Next check failed", msg,
                               "Missing start event for true expression."),
                       level, path_offset, line_num, file_name);
       end if;
 
 
       update_remaining_times_to_scheduled_checks(schedule, num_cks);
     end loop;
@@ -1802,15 +1875,15 @@
           tracks(i) := (tracks(i - 1) and (to_x01(seq(i)) = '1'));
         end if;
       end loop;
 
       -- FIXME: check moved out of loop to work with GHDL 0.33.
       if unknown_event_in_sequence then
         failing_check(checker,
-                      std_msg("Sequence check failed", msg,
+                      p_std_msg("Sequence check failed", msg,
                               "Got " & to_nibble_string(seq) & "."),
                       level, path_offset, line_num, file_name);
       end if;
     end find_new_and_update_existing_tracks;
 
     procedure update_expectations_on_events_in_next_cycle (
       constant tracks            : in    boolean_vector;
@@ -1829,37 +1902,37 @@
       constant event_sequence    : in std_logic_vector) is
       constant seq : std_logic_vector(0 to event_sequence'length - 1) := event_sequence;
     begin
       for i in 1 to seq'right loop
         if expected_events(i) then
           if to_x01(seq(i)) /= '1' then
             failing_check(checker,
-                          std_msg("Sequence check failed", msg,
+                          p_std_msg("Sequence check failed", msg,
                                   "Missing required event at " &
                                   to_ordinal_number(to_unsigned(i, 32)) &
                                   " active and enabled clock edge."),
                           level, path_offset, line_num, file_name);
           elsif i = seq'right then
             if is_pass_visible(checker) then
-              passing_check(checker, std_msg("Sequence check passed", msg, ""), path_offset, line_num, file_name);
+              passing_check(checker, p_std_msg("Sequence check passed", msg, ""), path_offset, line_num, file_name);
             else
               passing_check(checker);
             end if;
           end if;
         end if;
       end loop;
     end procedure verify_expected_events;
 
     variable valid_event_sequence_length : boolean;
   begin
     -- pragma translate_off
     valid_event_sequence_length := event_sequence'length >= 2;
     if not valid_event_sequence_length then
       failing_check(checker,
-                    std_msg("Sequence check failed", msg,
+                    p_std_msg("Sequence check failed", msg,
                             "Event sequence length must be at least 2. Got " &
                             natural'image(event_sequence'length) & "."),
                     level, path_offset, line_num, file_name);
     end if;
 
     wait_on_edge(clock, en, active_clock_edge);
     while valid_event_sequence_length loop
@@ -1921,21 +1994,21 @@
     constant line_num    : in  natural     := 0;
     constant file_name   : in  string      := "") is
   begin
     -- pragma translate_off
     if expr then
       pass := true;
       if is_pass_visible(checker) then
-        passing_check(checker, std_msg("Relation check passed", msg, context_msg), path_offset, line_num, file_name);
+        passing_check(checker, p_std_msg("Relation check passed", msg, context_msg), path_offset, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
-      failing_check(checker, std_msg("Relation check failed", msg, context_msg), level, path_offset, line_num, file_name);
+      failing_check(checker, p_std_msg("Relation check failed", msg, context_msg), level, path_offset, line_num, file_name);
     end if;
   -- pragma translate_on
   end;
 
   procedure check_relation(
     constant expr        : in boolean;
     constant msg         : in string      := check_result_tag;
@@ -2370,15 +2443,15 @@
     constant max_diff    : in real        := 0.0;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "") is
   begin
     -- pragma translate_off
-    check_equal(default_checker, got, expected, msg, max_diff, level, path_offset, line_num, file_name);
+    check_equal(default_checker, got, expected, msg, max_diff, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
   end;
 
 
   procedure check_equal(
     constant checker     : in checker_t;
     constant got         : in real;
@@ -2391,25 +2464,25 @@
     constant file_name   : in string      := "") is
   begin
     -- pragma translate_off
     if abs (got - expected) <= max_diff then
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got abs (" & real'image(got) & " - " & real'image(expected) & ") <= " & real'image(max_diff) & "."),
           path_offset, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got abs (" & real'image(got) & " - " & real'image(expected) & ") > " & real'image(max_diff) & "."),
         level, path_offset, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
 
@@ -2459,26 +2532,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
           "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -2530,14 +2603,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in unsigned;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ".",
+      std_fail_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in unsigned;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in unsigned;
     constant expected    : in natural;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -2577,26 +2697,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
           "Expected " & to_string(expected) & " (" & to_nibble_string(to_sufficient_unsigned(expected, got'length)) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -2648,14 +2768,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in unsigned;
+    constant expected    : in natural;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ".",
+      std_fail_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". Expected " & to_string(expected) & " (" & to_nibble_string(to_sufficient_unsigned(expected, got'length)) & ")" & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in unsigned;
+    constant expected    : in natural;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in natural;
     constant expected    : in unsigned;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -2695,26 +2862,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_unsigned(got, expected'length)) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_unsigned(got, expected'length)) & ")" & ". " &
           "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -2766,14 +2933,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in natural;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_unsigned(got, expected'length)) & ")" & ".",
+      std_fail_ctx => "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_unsigned(got, expected'length)) & ")" & ". Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in natural;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in unsigned;
     constant expected    : in std_logic_vector;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -2813,26 +3027,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
           "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -2884,14 +3098,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in unsigned;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ".",
+      std_fail_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in unsigned;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in std_logic_vector;
     constant expected    : in unsigned;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -2931,26 +3192,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
           "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -3002,14 +3263,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in std_logic_vector;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ".",
+      std_fail_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in std_logic_vector;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in std_logic_vector;
     constant expected    : in std_logic_vector;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -3049,26 +3357,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
           "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -3120,14 +3428,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in std_logic_vector;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ".",
+      std_fail_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in std_logic_vector;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in std_logic_vector;
     constant expected    : in natural;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -3167,26 +3522,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
           "Expected " & to_string(expected) & " (" & to_nibble_string(to_sufficient_unsigned(expected, got'length)) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -3238,14 +3593,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in std_logic_vector;
+    constant expected    : in natural;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ".",
+      std_fail_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". Expected " & to_string(expected) & " (" & to_nibble_string(to_sufficient_unsigned(expected, got'length)) & ")" & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in std_logic_vector;
+    constant expected    : in natural;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in natural;
     constant expected    : in std_logic_vector;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -3285,26 +3687,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_unsigned(got, expected'length)) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_unsigned(got, expected'length)) & ")" & ". " &
           "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -3356,14 +3758,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in natural;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_unsigned(got, expected'length)) & ")" & ".",
+      std_fail_ctx => "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_unsigned(got, expected'length)) & ")" & ". Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in natural;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in signed;
     constant expected    : in signed;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -3403,26 +3852,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
           "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -3474,14 +3923,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in signed;
+    constant expected    : in signed;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ".",
+      std_fail_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in signed;
+    constant expected    : in signed;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in signed;
     constant expected    : in integer;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -3521,26 +4017,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
           "Expected " & to_string(expected) & " (" & to_nibble_string(to_sufficient_signed(expected, got'length)) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -3592,14 +4088,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in signed;
+    constant expected    : in integer;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ".",
+      std_fail_ctx => "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". Expected " & to_string(expected) & " (" & to_nibble_string(to_sufficient_signed(expected, got'length)) & ")" & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in signed;
+    constant expected    : in integer;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in integer;
     constant expected    : in signed;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -3639,26 +4182,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_signed(got, expected'length)) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_signed(got, expected'length)) & ")" & ". " &
           "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -3710,14 +4253,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in integer;
+    constant expected    : in signed;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_signed(got, expected'length)) & ")" & ".",
+      std_fail_ctx => "Got " & to_string(got) & " (" & to_nibble_string(to_sufficient_signed(got, expected'length)) & ")" & ". Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in integer;
+    constant expected    : in signed;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in integer;
     constant expected    : in integer;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -3757,26 +4347,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_string(got) & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_string(got) & ". " &
           "Expected " & to_string(expected) & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -3828,14 +4418,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in integer;
+    constant expected    : in integer;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_string(got) & ".",
+      std_fail_ctx => "Got " & to_string(got) & ". Expected " & to_string(expected) & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in integer;
+    constant expected    : in integer;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in std_logic;
     constant expected    : in std_logic;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -3875,26 +4512,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_string(got) & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_string(got) & ". " &
           "Expected " & to_string(expected) & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -3946,14 +4583,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in std_logic;
+    constant expected    : in std_logic;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_string(got) & ".",
+      std_fail_ctx => "Got " & to_string(got) & ". Expected " & to_string(expected) & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in std_logic;
+    constant expected    : in std_logic;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in std_logic;
     constant expected    : in boolean;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -3993,26 +4677,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_string(got) & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_string(got) & ". " &
           "Expected " & to_string(expected) & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -4064,14 +4748,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in std_logic;
+    constant expected    : in boolean;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_string(got) & ".",
+      std_fail_ctx => "Got " & to_string(got) & ". Expected " & to_string(expected) & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in std_logic;
+    constant expected    : in boolean;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in boolean;
     constant expected    : in std_logic;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -4111,26 +4842,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_string(got) & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_string(got) & ". " &
           "Expected " & to_string(expected) & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -4182,14 +4913,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in boolean;
+    constant expected    : in std_logic;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_string(got) & ".",
+      std_fail_ctx => "Got " & to_string(got) & ". Expected " & to_string(expected) & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in boolean;
+    constant expected    : in std_logic;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in boolean;
     constant expected    : in boolean;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -4229,26 +5007,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_string(got) & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_string(got) & ". " &
           "Expected " & to_string(expected) & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -4300,14 +5078,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in boolean;
+    constant expected    : in boolean;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_string(got) & ".",
+      std_fail_ctx => "Got " & to_string(got) & ". Expected " & to_string(expected) & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in boolean;
+    constant expected    : in boolean;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in string;
     constant expected    : in string;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -4347,26 +5172,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_string(got) & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_string(got) & ". " &
           "Expected " & to_string(expected) & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -4418,14 +5243,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in string;
+    constant expected    : in string;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_string(got) & ".",
+      std_fail_ctx => "Got " & to_string(got) & ". Expected " & to_string(expected) & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in string;
+    constant expected    : in string;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in character;
     constant expected    : in character;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -4465,26 +5337,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_string(got) & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_string(got) & ". " &
           "Expected " & to_string(expected) & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -4536,14 +5408,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in character;
+    constant expected    : in character;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_string(got) & ".",
+      std_fail_ctx => "Got " & to_string(got) & ". Expected " & to_string(expected) & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in character;
+    constant expected    : in character;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   procedure check_equal(
     constant got         : in time;
     constant expected    : in time;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -4583,26 +5502,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & to_string(got) & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & to_string(got) & ". " &
           "Expected " & to_string(expected) & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -4654,14 +5573,61 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in time;
+    constant expected    : in time;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & to_string(got) & ".",
+      std_fail_ctx => "Got " & to_string(got) & ". Expected " & to_string(expected) & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in time;
+    constant expected    : in time;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
   -----------------------------------------------------------------------------
   -- check_match
   -----------------------------------------------------------------------------
   procedure check_match(
     constant got         : in unsigned;
     constant expected    : in unsigned;
     constant msg         : in string      := check_result_tag;
@@ -4705,27 +5671,27 @@
     -- pragma translate_off
     if std_match(got, expected) then
       pass := true;
 
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Match check passed", msg,
             "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
             "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Match check failed", msg,
           "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
           "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -4825,27 +5791,27 @@
     -- pragma translate_off
     if std_match(got, expected) then
       pass := true;
 
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Match check passed", msg,
             "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
             "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Match check failed", msg,
           "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
           "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -4945,27 +5911,27 @@
     -- pragma translate_off
     if std_match(got, expected) then
       pass := true;
 
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Match check passed", msg,
             "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
             "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Match check failed", msg,
           "Got " & to_nibble_string(got) & " (" & to_integer_string(got) & ")" & ". " &
           "Expected " & to_nibble_string(expected) & " (" & to_integer_string(expected) & ")" & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -5065,27 +6031,27 @@
     -- pragma translate_off
     if std_match(got, expected) then
       pass := true;
 
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Match check passed", msg,
             "Got " & to_string(got) & ". " &
             "Expected " & to_string(expected) & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Match check failed", msg,
           "Got " & to_string(got) & ". " &
           "Expected " & to_string(expected) & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/src/check_api.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/src/check_api.vhd`

 * *Files 8% similar despite different names*

```diff
@@ -10,32 +10,42 @@
 library ieee;
 use ieee.std_logic_1164.all;
 use ieee.numeric_std.all;
 use std.textio.all;
 use work.checker_pkg.all;
 use work.logger_pkg.all;
 use work.log_levels_pkg.all;
+use work.string_ops.all;
+use work.event_common_pkg.all;
+use work.string_ptr_pkg.all;
 
 package check_pkg is
 
   constant default_checker : checker_t := new_checker("check");
   constant check_logger : logger_t := get_logger(default_checker);
 
   signal check_enabled : std_logic := '1';
 
   procedure get_checker_stat (variable stat : out checker_stat_t);
   impure function get_checker_stat return checker_stat_t;
   procedure reset_checker_stat;
 
-  constant check_result_tag : string    := "<+/->";
-  function result (msg : string := "") return string;
+  -- TODO: Make an alias when NVC compiles correctly
+  --alias check_result_tag is decorate_tag;
+  constant check_result_tag : string := "<+/->";
+  --alias result is decorate[string return string];
+  function result(str : string := "") return string;
 
   type edge_t is (rising_edge, falling_edge, both_edges);
   type trigger_event_t is (first_pipe, first_no_pipe, penultimate);
 
+  procedure log(check_result : check_result_t);
+
+  procedure notify_if_fail(check_result : check_result_t; signal event : inout any_event_t);
+
   -----------------------------------------------------------------------------
   -- check
   -----------------------------------------------------------------------------
   procedure check(
     constant checker           : in checker_t;
     signal clock               : in std_logic;
     signal en                  : in std_logic;
@@ -88,14 +98,23 @@
     constant msg         : in string      := check_result_tag & ".";
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check(
+    constant expr        : in boolean;
+    constant msg         : in string      := check_result_tag & ".";
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check(
     signal clock               : in std_logic;
     signal en                  : in std_logic;
     signal expr                : in std_logic;
     constant msg               : in string      := check_result_tag & ".";
     constant level             : in log_level_t := null_log_level;
     constant active_clock_edge : in edge_t      := rising_edge;
@@ -109,14 +128,25 @@
     constant msg         : in string      := check_result_tag & ".";
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check(
+    constant checker     : in checker_t;
+    constant expr        : in boolean;
+    constant msg         : in string      := check_result_tag & ".";
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+
   -----------------------------------------------------------------------------
   -- check_passed
   -----------------------------------------------------------------------------
   procedure check_passed(
     constant checker     : in checker_t;
     constant msg         : in string  := check_result_tag & ".";
     constant path_offset : in natural := 0;
@@ -203,14 +233,23 @@
     constant msg         : in string      := check_result_tag & ".";
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_true(
+    constant expr        : in boolean;
+    constant msg         : in string      := check_result_tag & ".";
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_true(
     signal clock               : in std_logic;
     signal en                  : in std_logic;
     signal expr                : in std_logic;
     constant msg               : in string      := check_result_tag & ".";
     constant level             : in log_level_t := null_log_level;
     constant active_clock_edge : in edge_t      := rising_edge;
@@ -224,14 +263,24 @@
     constant msg         : in string      := check_result_tag & ".";
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_true(
+    constant checker     : in checker_t;
+    constant expr        : in boolean;
+    constant msg         : in string      := check_result_tag & ".";
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   -----------------------------------------------------------------------------
   -- check_false
   -----------------------------------------------------------------------------
   procedure check_false(
     constant checker     : in checker_t;
     constant expr        : in boolean;
     constant msg         : in string      := check_result_tag & ".";
@@ -1113,14 +1162,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in unsigned;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in unsigned;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in unsigned;
     constant expected    : in natural;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1174,14 +1244,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in unsigned;
+    constant expected    : in natural;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in unsigned;
+    constant expected    : in natural;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in natural;
     constant expected    : in unsigned;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1235,14 +1326,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in natural;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in natural;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in unsigned;
     constant expected    : in std_logic_vector;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1296,14 +1408,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in unsigned;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in unsigned;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in std_logic_vector;
     constant expected    : in unsigned;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1357,14 +1490,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in std_logic_vector;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in std_logic_vector;
+    constant expected    : in unsigned;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in std_logic_vector;
     constant expected    : in std_logic_vector;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1418,14 +1572,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in std_logic_vector;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in std_logic_vector;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in std_logic_vector;
     constant expected    : in natural;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1479,14 +1654,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in std_logic_vector;
+    constant expected    : in natural;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in std_logic_vector;
+    constant expected    : in natural;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in natural;
     constant expected    : in std_logic_vector;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1540,14 +1736,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in natural;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in natural;
+    constant expected    : in std_logic_vector;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in signed;
     constant expected    : in signed;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1601,14 +1818,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in signed;
+    constant expected    : in signed;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in signed;
+    constant expected    : in signed;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in signed;
     constant expected    : in integer;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1662,14 +1900,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in signed;
+    constant expected    : in integer;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in signed;
+    constant expected    : in integer;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in integer;
     constant expected    : in signed;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1723,14 +1982,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in integer;
+    constant expected    : in signed;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in integer;
+    constant expected    : in signed;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in integer;
     constant expected    : in integer;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1784,14 +2064,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in integer;
+    constant expected    : in integer;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in integer;
+    constant expected    : in integer;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in std_logic;
     constant expected    : in std_logic;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1845,14 +2146,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in std_logic;
+    constant expected    : in std_logic;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in std_logic;
+    constant expected    : in std_logic;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in std_logic;
     constant expected    : in boolean;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1906,14 +2228,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in std_logic;
+    constant expected    : in boolean;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in std_logic;
+    constant expected    : in boolean;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in boolean;
     constant expected    : in std_logic;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -1967,14 +2310,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in boolean;
+    constant expected    : in std_logic;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in boolean;
+    constant expected    : in std_logic;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in boolean;
     constant expected    : in boolean;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -2028,14 +2392,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in boolean;
+    constant expected    : in boolean;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in boolean;
+    constant expected    : in boolean;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in string;
     constant expected    : in string;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -2089,14 +2474,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in string;
+    constant expected    : in string;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in string;
+    constant expected    : in string;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in character;
     constant expected    : in character;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -2150,14 +2556,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in character;
+    constant expected    : in character;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in character;
+    constant expected    : in character;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   procedure check_equal(
     constant got         : in time;
     constant expected    : in time;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
@@ -2211,14 +2638,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in time;
+    constant expected    : in time;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in time;
+    constant expected    : in time;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
   -----------------------------------------------------------------------------
   -- check_match
   -----------------------------------------------------------------------------
   procedure check_match(
     constant got         : in unsigned;
     constant expected    : in unsigned;
     constant msg         : in string      := check_result_tag;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/src/check_deprecated_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/src/check_deprecated_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_implication.vhd`

 * *Files 25% similar despite different names*

```diff
@@ -1,308 +1,237 @@
--- This test suite verifies the check checker.
+-- This test suite verifies the check_implication checker.
 --
 -- This Source Code Form is subject to the terms of the Mozilla Public
 -- License, v. 2.0. If a copy of the MPL was not distributed with this file,
 -- You can obtain one at http://mozilla.org/MPL/2.0/.
 --
 -- Copyright (c) 2014-2023, Lars Asplund lars.anders.asplund@gmail.com
 
 -- vunit: run_all_in_same_sim
 
 library ieee;
 use ieee.std_logic_1164.all;
 library vunit_lib;
+use vunit_lib.run_types_pkg.all;
+use vunit_lib.run_pkg.all;
+use vunit_lib.runner_pkg.all;
 use vunit_lib.log_levels_pkg.all;
 use vunit_lib.logger_pkg.all;
 use vunit_lib.checker_pkg.all;
 use vunit_lib.check_pkg.all;
-use vunit_lib.run_types_pkg.all;
-use vunit_lib.run_pkg.all;
-use vunit_lib.runner_pkg.all;
 use work.test_support.all;
-use ieee.numeric_std.all;
-entity tb_check is
+
+entity tb_check_implication is
   generic (
-    use_check_not_check_true : boolean := true;
     runner_cfg : string);
-end entity tb_check;
+end entity tb_check_implication;
 
-architecture test_fixture of tb_check is
+architecture test_fixture of tb_check_implication is
   signal clk : std_logic := '0';
-  signal check_in_1, check_in_2, check_in_3, check_in_4 : std_logic := '1';
-  signal check_en_1, check_en_2, check_en_3, check_en_4 : std_logic := '1';
 
-  constant check_checker : checker_t := new_checker("checker");
-  constant check_checker2 : checker_t := new_checker("checker2");
-  constant check_checker3 : checker_t := new_checker("checker3", default_log_level => info);
-  constant check_checker4 : checker_t := new_checker("checker4");
+  signal check_implication_in_1,
+    check_implication_in_2,
+    check_implication_in_3,
+    check_implication_in_4 : std_logic_vector(1 to 2) := "00";
+  alias antecedent_1 : std_logic is check_implication_in_1(1);
+  alias consequent_1 : std_logic is check_implication_in_1(2);
+  alias antecedent_2 : std_logic is check_implication_in_2(1);
+  alias consequent_2 : std_logic is check_implication_in_2(2);
+  alias antecedent_3 : std_logic is check_implication_in_3(1);
+  alias consequent_3 : std_logic is check_implication_in_3(2);
+  alias antecedent_4 : std_logic is check_implication_in_4(1);
+  alias consequent_4 : std_logic is check_implication_in_4(2);
+  signal check_implication_en_1, check_implication_en_2, check_implication_en_3, check_implication_en_4 : std_logic := '1';
+
+  constant my_checker : checker_t := new_checker("my_checker1");
+  constant my_checker2 : checker_t := new_checker("my_checker2");
+  constant my_checker3 : checker_t := new_checker("my_checker3", default_log_level => info);
+  constant my_checker4 : checker_t := new_checker("my_checker4");
 
 begin
   clock: process is
   begin
     while get_phase(runner_state) < test_runner_exit loop
       clk <= '1', '0' after 5 ns;
       wait for 10 ns;
     end loop;
     wait;
   end process clock;
 
-  concurrent_checks: if use_check_not_check_true generate
-    check_1 : check(clk, check_en_1, check_in_1);
-    check_2 : check(check_checker2, clk, check_en_2, check_in_2, active_clock_edge => falling_edge);
-    check_3 : check(check_checker3, clk, check_en_3, check_in_3);
-    check_4 : check(check_checker4, clk, check_en_4, check_in_4);
-  end generate concurrent_checks;
-
-  concurrent_true_checks: if not use_check_not_check_true generate
-    check_1 : check_true(clk, check_en_1, check_in_1);
-    check_2 : check_true(check_checker2, clk, check_en_2, check_in_2, active_clock_edge => falling_edge);
-    check_3 : check_true(check_checker3, clk, check_en_3, check_in_3);
-    check_4 : check_true(check_checker4, clk, check_en_4, check_in_4);
-  end generate concurrent_true_checks;
+  check_implication_1 : check_implication(clk, check_implication_en_1, antecedent_1, consequent_1);
+  check_implication_2 : check_implication(my_checker2, clk, check_implication_en_2, antecedent_2, consequent_2, active_clock_edge => falling_edge);
+  check_implication_3 : check_implication(my_checker3, clk, check_implication_en_3, antecedent_3, consequent_3);
+  check_implication_4 : check_implication(my_checker4, clk, check_implication_en_4,
+                                          antecedent_4, consequent_4, result("between x and y."));
 
-  check_runner : process
+  check_implication_runner : process
     variable passed : boolean;
+    type boolean_vector is array (natural range <>) of boolean;
+    constant test_antecedents : boolean_vector(1 to 4) := (false, false, true, true);
+    constant test_consequents : boolean_vector(1 to 4) := (false, true, false, true);
+    constant test_implication_expected_result : boolean_vector(1 to 4) := (true, true, false, true);
     variable stat : checker_stat_t;
     constant default_level : log_level_t := error;
 
-    function prefix return string is
-    begin
-      if use_check_not_check_true then
-        return "Check ";
-      else
-        return "True check ";
-      end if;
-    end function prefix;
-
     procedure test_concurrent_check (
       signal clk                        : in  std_logic;
-      signal check_input                : out std_logic;
+      signal check_input                : out std_logic_vector;
       checker                           : checker_t;
       constant level                    : in  log_level_t := error;
       constant active_rising_clock_edge : in  boolean := true) is
     begin
-      -- Verify that one log is generated on false and that that log is
-      -- generated on the correct clock edge. No log on true.
+      -- Verify all combinations of antecedent/consequent inputs
       wait until clock_edge(clk, active_rising_clock_edge);
       wait for 1 ns;
       get_checker_stat(checker, stat);
-      apply_sequence("0", clk, check_input, active_rising_clock_edge);
-      wait until clock_edge(clk, not active_rising_clock_edge);
+      apply_sequence("000110", clk, check_input, active_rising_clock_edge);
       wait for 1 ns;
-      verify_passed_checks(checker, stat, 0);
+      verify_passed_checks(checker, stat, 2);
       verify_failed_checks(checker, stat, 0);
       mock(get_logger(checker));
       wait until clock_edge(clk, active_rising_clock_edge);
       wait for 1 ns;
-      check_only_log(get_logger(checker), prefix & "failed.", level);
+      check_only_log(get_logger(checker), "Implication check failed.", level);
       unmock(get_logger(checker));
-      verify_passed_checks(checker, stat, 0);
+      verify_passed_checks(checker, stat, 2);
       verify_failed_checks(checker, stat, 1);
-      apply_sequence("1", clk, check_input, active_rising_clock_edge);
+      apply_sequence("11", clk, check_input, active_rising_clock_edge);
       wait until clock_edge(clk, active_rising_clock_edge);
       wait for 1 ns;
-      verify_passed_checks(checker, stat, 1);
+      verify_passed_checks(checker, stat, 3);
       verify_failed_checks(checker, stat, 1);
       reset_checker_stat(checker);
     end procedure test_concurrent_check;
 
-    procedure internal_check(
-      checker   : checker_t;
-      variable pass      : out   boolean;
-      constant expr      : in    boolean;
-      constant msg       : in    string := result(".")) is
-    begin
-      if use_check_not_check_true then
-        check(checker, pass, expr, msg);
-      else
-        check_true(checker, pass, expr, msg);
-      end if;
-    end;
-
-    procedure internal_check(
-      checker   : checker_t;
-      constant expr      : in    boolean;
-      constant msg       : in    string := result(".")) is
-    begin
-      if use_check_not_check_true then
-        check(checker, expr, msg);
-      else
-        check_true(checker, expr, msg);
-      end if;
-    end;
-
-    procedure internal_check(
-      constant expr      : in boolean;
-      constant msg       : in string := result(".")) is
-    begin
-      if use_check_not_check_true then
-        check(expr, msg);
-      else
-        check_true(expr, msg);
-      end if;
-    end;
-
-    procedure internal_check(
-      variable pass      : out boolean;
-      constant expr      : in  boolean;
-      constant msg       : in  string := result(".")) is
-    begin
-      if use_check_not_check_true then
-        check(pass, expr, msg);
-      else
-        check_true(pass, expr, msg);
+    procedure verify_result (
+      constant iteration : in    natural;
+      checker            : checker_t;
+      variable stat      : inout    checker_stat_t) is
+    begin
+      if test_implication_expected_result(iteration) then
+        verify_passed_checks(checker, stat, 1);
+        verify_failed_checks(checker, stat, 0);
+        check_only_log(get_logger(checker),
+                       "Implication check passed. - Got " &
+                       boolean'image(test_antecedents(iteration)) &" -> " & boolean'image(test_consequents(iteration)) &
+                       ".", pass);
+      else
+        verify_passed_checks(checker, stat, 0);
+        verify_failed_checks(checker, stat, 1);
+        check_only_log(get_logger(checker), "Implication check failed.", default_level);
       end if;
-    end;
-
-    impure function internal_check(
-      constant expr      : in boolean;
-      constant msg       : in string := result("."))
-      return boolean is
-    begin
-      if use_check_not_check_true then
-        return check(expr, msg);
-      else
-        return check_true(expr, msg);
-      end if;
-    end;
+      reset_checker_stat(checker);
 
-    impure function internal_check(checker : checker_t; expr : boolean; msg : string := result("."))
-      return boolean is
-    begin
-      if use_check_not_check_true then
-        return check(checker, expr, msg);
-      else
-        return check_true(checker, expr, msg);
-      end if;
-    end;
+    end verify_result;
 
   begin
     test_runner_setup(runner, runner_cfg);
 
     while test_suite loop
-      if run("Test should pass on true inputs to sequential checks") then
-        get_checker_stat(stat);
-        internal_check(true);
-        internal_check(passed, true);
-        assert_true(passed, "Should return pass = true on passing check");
-        passed := internal_check(true);
-        assert_true(passed, "Should return pass = true on passing check");
-        verify_passed_checks(stat, 3);
-
-        get_checker_stat(check_checker, stat);
-        internal_check(check_checker, true);
-        internal_check(check_checker, passed, true);
-        assert_true(passed, "Should return pass = true on passing check");
-        passed := internal_check(check_checker, true);
-        assert_true(passed, "Should return pass = true on passing check");
-        verify_passed_checks(check_checker, stat, 3);
-
-      elsif run("Test pass message") then
-        mock(check_logger);
-        internal_check(true);
-        check_only_log(check_logger, prefix & "passed.", pass);
-
-        internal_check(true, "");
-        check_only_log(check_logger, "", pass);
-
-        internal_check(true, "Checking my data.");
-        check_only_log(check_logger, "Checking my data.", pass);
-
-        internal_check(true, result("for my data."));
-        check_only_log(check_logger, prefix & "passed for my data.", pass);
-        unmock(check_logger);
-
-      elsif run("Test should fail on false inputs to sequential checks") then
-        get_checker_stat(stat);
-        mock(check_logger);
-        internal_check(false);
-        check_only_log(check_logger, prefix & "failed.", default_level);
-
-        internal_check(false, "");
-        check_only_log(check_logger, "", default_level);
-
-        internal_check(passed, false, "Checking my data.");
-        assert_true(not passed, "Should return pass = false on failing check");
-        check_only_log(check_logger, "Checking my data.", default_level);
-
-        passed := internal_check(false, result("for my data."));
-        assert_true(not passed, "Should return pass = false on failing check");
-        check_only_log(check_logger, prefix & "failed for my data.", default_level);
-        unmock(check_logger);
-        verify_failed_checks(stat, 4);
-        reset_checker_stat;
-
-        get_checker_stat(check_checker, stat);
-        mock(get_logger(check_checker));
-        internal_check(check_checker, false);
-        check_only_log(get_logger(check_checker), prefix & "failed.", default_level);
-
-        internal_check(check_checker, passed, false, result("for my data."));
-        assert_true(not passed, "Should return pass = false on failing check");
-        check_only_log(get_logger(check_checker), prefix & "failed for my data.", default_level);
-
-        passed := internal_check(check_checker, false, result("for my data."));
-        assert_true(not passed, "Should return pass = false on failing check");
-        check_only_log(get_logger(check_checker), prefix & "failed for my data.", default_level);
-        unmock(get_logger(check_checker));
-        verify_failed_checks(check_checker, stat, 3);
-        reset_checker_stat(check_checker);
+      if run("Test sequential checkers should fail on true implies false but pass on other inputs") then
+        for i in test_antecedents'range loop
+          mock(check_logger);
+          get_checker_stat(stat);
+          check_implication(test_antecedents(i), test_consequents(i));
+          verify_result(i, default_checker, stat);
+          unmock(check_logger);
+
+          mock(get_logger(my_checker));
+          get_checker_stat(my_checker, stat);
+          check_implication(my_checker, test_antecedents(i), test_consequents(i));
+          verify_result(i, my_checker, stat);
+          unmock(get_logger(my_checker));
+
+          mock(check_logger);
+          get_checker_stat(stat);
+          check_implication(passed, test_antecedents(i), test_consequents(i));
+          verify_result(i, default_checker, stat);
+          unmock(check_logger);
+
+          mock(check_logger);
+          get_checker_stat(stat);
+          passed := check_implication(test_antecedents(i), test_consequents(i));
+          verify_result(i, default_checker, stat);
+          unmock(check_logger);
+
+          mock(get_logger(my_checker));
+          get_checker_stat(my_checker, stat);
+          check_implication(my_checker, passed, test_antecedents(i), test_consequents(i));
+          verify_result(i, my_checker, stat);
+          unmock(get_logger(my_checker));
+
+          mock(get_logger(my_checker));
+          get_checker_stat(my_checker, stat);
+          passed := check_implication(my_checker, test_antecedents(i), test_consequents(i));
+          verify_result(i, my_checker, stat);
+          unmock(get_logger(my_checker));
+        end loop;
 
       elsif run("Test should be possible to use concurrently") then
-        test_concurrent_check(clk, check_in_1, default_checker);
+        test_concurrent_check(clk, check_implication_in_1, default_checker);
 
       elsif run("Test should be possible to use concurrently with negative active clock edge") then
-        test_concurrent_check(clk, check_in_2, check_checker2, error, false);
+        test_concurrent_check(clk, check_implication_in_2, my_checker2, error, false);
 
       elsif run("Test should be possible to use concurrently with custom checker") then
-        test_concurrent_check(clk, check_in_3, check_checker3, info);
-
-      elsif run("Test should pass on weak high but fail on other meta values") then
+        test_concurrent_check(clk, check_implication_in_3, my_checker3, info);
 
+      elsif run("Test should handle weak known meta values as known values and others as unknowns") then
         wait until rising_edge(clk);
         wait for 1 ns;
-        get_checker_stat(check_checker4, stat);
-        apply_sequence("1H1", clk, check_in_4);
+        get_checker_stat(my_checker4, stat);
+        apply_sequence("000XLXH1HH00", clk, check_implication_in_4);
+        wait for 1 ns;
+        verify_passed_checks(my_checker4, stat, 5);
+        verify_failed_checks(my_checker4, stat, 0);
+        mock(get_logger(my_checker4));
+        apply_sequence("00HL00", clk, check_implication_in_4);
+        wait until rising_edge(clk);
+        wait for 1 ns;
+        check_log(get_logger(my_checker4), "Implication check passed between x and y. - Got false -> false.", pass);
+        check_log(get_logger(my_checker4), "Implication check failed between x and y.", default_level);
+        check_log(get_logger(my_checker4), "Implication check passed between x and y. - Got false -> false.", pass);
+        check_no_log;
+        verify_passed_checks(my_checker4, stat, 7);
+        verify_failed_checks(my_checker4, stat, 1);
+        apply_sequence("00H000", clk, check_implication_in_4);
         wait until rising_edge(clk);
         wait for 1 ns;
-        mock(get_logger(check_checker4));
-        verify_passed_checks(check_checker4, stat, 3);
-        get_checker_stat(check_checker4, stat);
-        apply_sequence("1UXZWL-1", clk, check_in_4);
+        check_log(get_logger(my_checker4), "Implication check passed between x and y. - Got false -> false.", pass);
+        check_log(get_logger(my_checker4), "Implication check failed between x and y.", default_level);
+        check_log(get_logger(my_checker4), "Implication check passed between x and y. - Got false -> false.", pass);
+        check_no_log;
+        verify_passed_checks(my_checker4, stat, 9);
+        verify_failed_checks(my_checker4, stat, 2);
+        apply_sequence("00HX00", clk, check_implication_in_4);
         wait until rising_edge(clk);
         wait for 1 ns;
-        check_log(get_logger(check_checker4), prefix & "passed.", pass);
-        check_log(get_logger(check_checker4), prefix & "failed.", default_level);
-        check_log(get_logger(check_checker4), prefix & "failed.", default_level);
-        check_log(get_logger(check_checker4), prefix & "failed.", default_level);
-        check_log(get_logger(check_checker4), prefix & "failed.", default_level);
-        check_log(get_logger(check_checker4), prefix & "failed.", default_level);
-        check_log(get_logger(check_checker4), prefix & "failed.", default_level);
-        check_log(get_logger(check_checker4), prefix & "passed.", pass);
-        unmock(get_logger(check_checker4));
-        verify_passed_checks(check_checker4, stat, 2);
-        verify_failed_checks(check_checker4, stat, 6);
-        reset_checker_stat(check_checker4);
+        check_log(get_logger(my_checker4), "Implication check passed between x and y. - Got false -> false.", pass);
+        check_log(get_logger(my_checker4), "Implication check failed between x and y.", default_level);
+        check_log(get_logger(my_checker4), "Implication check passed between x and y. - Got false -> false.", pass);
+        unmock(get_logger(my_checker4));
+        verify_passed_checks(my_checker4, stat, 11);
+        verify_failed_checks(my_checker4, stat, 3);
+        reset_checker_stat(my_checker4);
 
-      elsif run("Test should pass on logic low inputs when not enabled") then
+      elsif run("Test should pass on true implies false when not enabled") then
         wait until rising_edge(clk);
         wait for 1 ns;
         get_checker_stat(stat);
-        check_en_1 <= '0';
-        apply_sequence("01", clk, check_in_1);
-        check_en_1 <= '1';
-        wait until rising_edge(clk);
-        check_en_1 <= 'L';
-        apply_sequence("01", clk, check_in_1);
-        check_en_1 <= 'H';
-        wait until rising_edge(clk);
-        check_en_1 <= 'X';
-        apply_sequence("01", clk, check_in_1);
-        check_en_1 <= '1';
+        check_implication_en_1 <= '0';
+        apply_sequence("1000", clk, check_implication_in_1);
+        check_implication_en_1 <= '1';
+        wait until rising_edge(clk);
+        check_implication_en_1 <= 'L';
+        apply_sequence("1000", clk, check_implication_in_1);
+        check_implication_en_1 <= 'H';
+        wait until rising_edge(clk);
+        check_implication_en_1 <= 'X';
+        apply_sequence("1000", clk, check_implication_in_1);
+        check_implication_en_1 <= '1';
         wait until rising_edge(clk);
         wait for 1 ns;
         verify_passed_checks(stat, 3);
         verify_failed_checks(stat, 0);
       end if;
     end loop;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_equal_real.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_equal_real.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_failed.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_failed.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_false.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_false.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_next.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_next.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_not_unknown.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_not_unknown.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_one_hot.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_one_hot.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_passed.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_passed.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_relation.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_relation.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_relation_2008p.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_relation_2008p.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_sequence.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_sequence.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_stable.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_stable.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_check_zero_one_hot.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_check_zero_one_hot.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_checker.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_checker.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_deprecated.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_deprecated.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/tb_result.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/tb_result.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/test/test_support.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/check/test/test_support.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/tools/generate_check_equal.py` & `vunit_hdl-4.7.0/vunit/vhdl/check/tools/generate_check_equal.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,14 +64,35 @@
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
     constant path_offset : in natural     := 0;
     constant line_num    : in natural     := 0;
     constant file_name   : in string      := "")
     return boolean;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in $got_type;
+    constant expected    : in $expected_type;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
+  impure function check_equal(
+    constant got         : in $got_type;
+    constant expected    : in $expected_type;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t;
+
 """
 
 impl_template = """  procedure check_equal(
     constant got         : in $got_type;
     constant expected    : in $expected_type;
     constant msg         : in string      := check_result_tag;
     constant level       : in log_level_t := null_log_level;
@@ -113,26 +134,26 @@
   begin
     -- pragma translate_off
     if got = expected then
       pass := true;
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Equality check passed", msg,
             "Got " & $got_str & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Equality check failed", msg,
           "Got " & $got_str & ". " &
           "Expected " & $expected_str & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
@@ -184,100 +205,212 @@
   begin
     -- pragma translate_off
     check_equal(checker, pass, got, expected, msg, level, path_offset + 1, line_num, file_name);
     -- pragma translate_on
     return pass;
   end;
 
+  impure function check_equal(
+    constant checker     : in checker_t;
+    constant got         : in $got_type;
+    constant expected    : in $expected_type;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+    variable check_result : check_result_t;
+  begin
+    -- pragma translate_off
+    check_result := p_build_result(
+      checker => checker,
+      is_pass => got = expected,
+      msg => msg,
+      std_pass_msg => "Equality check passed",
+      std_fail_msg => "Equality check failed",
+      std_pass_ctx => "Got " & $got_str & ".",
+      std_fail_ctx => "Got " & $got_str & ". Expected " & $expected_str & ".",
+      level => level,
+      path_offset => path_offset + 1,
+      line_num => line_num,
+      file_name => file_name
+    );
+    -- pragma translate_on
+
+    return check_result;
+  end;
+
+  impure function check_equal(
+    constant got         : in $got_type;
+    constant expected    : in $expected_type;
+    constant msg         : in string      := check_result_tag;
+    constant level       : in log_level_t := null_log_level;
+    constant path_offset : in natural     := 0;
+    constant line_num    : in natural     := 0;
+    constant file_name   : in string      := "")
+    return check_result_t is
+  begin
+    -- pragma translate_off
+    return check_equal(default_checker, got, expected, msg, level, path_offset + 1, line_num, file_name);
+    -- pragma translate_on
+  end;
+
+
 """
 
 test_template = """\
 
       elsif run("Test should pass on $left_type equal $right_type") then
         get_checker_stat(stat);
         check_equal($left_pass, $right_pass);
         check_equal(passed, $left_pass, $right_pass);
         assert_true(passed, "Should return pass = true on passing check");
         passed := check_equal($left_pass, $right_pass);
         assert_true(passed, "Should return pass = true on passing check");
+        check_result := check_equal($left_pass, $right_pass);
+        assert_true(check_result.p_is_pass, "Should return check_result.p_is_pass = true on passing check");
+        assert_true(check_result.p_checker = default_checker);
         check_equal($left_min, $right_min);
         check_equal($left_max, $right_max);
-        verify_passed_checks(stat, 5);
+        verify_passed_checks(stat, 6);
 
         get_checker_stat(my_checker, stat);
         check_equal(my_checker, $left_pass, $right_pass);
         check_equal(my_checker, passed, $left_pass, $right_pass);
         assert_true(passed, "Should return pass = true on passing check");
         passed := check_equal(my_checker, $left_pass, $right_pass);
         assert_true(passed, "Should return pass = true on passing check");
-        verify_passed_checks(my_checker, stat, 3);
+        check_result := check_equal(my_checker, $left_pass, $right_pass);
+        assert_true(check_result.p_is_pass, "Should return check_result.p_is_pass = true on passing check");
+        assert_true(check_result.p_checker = my_checker);
+        verify_passed_checks(my_checker, stat, 4);
 
       elsif run("Test pass message on $left_type equal $right_type") then
         mock(check_logger);
         check_equal($left_pass, $right_pass);
         check_only_log(check_logger, "Equality check passed - Got $left_pass_str.", pass);
+        check_result := check_equal($left_pass, $right_pass);
+        assert_true(
+          to_string(check_result.p_msg) = "Equality check passed - Got $left_pass_str.",
+          "Got: " & to_string(check_result.p_msg)
+        );
+        assert_true(check_result.p_level = pass);
 
         check_equal($left_pass, $right_pass, "");
         check_only_log(check_logger, "Got $left_pass_str.", pass);
+        check_result := check_equal($left_pass, $right_pass, "");
+        assert_true(to_string(check_result.p_msg) = "Got $left_pass_str.");
+        assert_true(check_result.p_level = pass);
 
         check_equal($left_pass, $right_pass, "Checking my data");
         check_only_log(check_logger, "Checking my data - Got $left_pass_str.", pass);
+        check_result := check_equal($left_pass, $right_pass, "Checking my data");
+        assert_true(to_string(check_result.p_msg) = "Checking my data - Got $left_pass_str.");
+        assert_true(check_result.p_level = pass);
 
         check_equal($left_pass, $right_pass, result("for my data"));
         check_only_log(check_logger, "Equality check passed for my data - Got $left_pass_str.", pass);
+        check_result := check_equal($left_pass, $right_pass, result("for my data"));
+        assert_true(to_string(check_result.p_msg) = "Equality check passed for my data - Got $left_pass_str.");
+        assert_true(check_result.p_level = pass);
         unmock(check_logger);
 
       elsif run("Test should fail on $left_type not equal $right_type") then
         get_checker_stat(stat);
         mock(check_logger);
         check_equal($left_pass, $right_fail);
         check_only_log(check_logger, "Equality check failed - Got $left_pass_str. Expected $fail_str.",
                        default_level);
+        check_result := check_equal($left_pass, $right_fail);
+        assert_true(not check_result.p_is_pass);
+        assert_true(check_result.p_checker = default_checker);
+        assert_true(to_string(check_result.p_msg) = "Equality check failed - Got $left_pass_str. Expected $fail_str.");
+        assert_true(check_result.p_level = default_level);
+        p_handle(check_result);
 
         check_equal($left_pass, $right_fail, "");
         check_only_log(check_logger, "Got $left_pass_str. Expected $fail_str.", default_level);
+        check_result := check_equal($left_pass, $right_fail, "");
+        assert_true(not check_result.p_is_pass);
+        assert_true(check_result.p_checker = default_checker);
+        assert_true(to_string(check_result.p_msg) = "Got $left_pass_str. Expected $fail_str.");
+        assert_true(check_result.p_level = default_level);
+        p_handle(check_result);
 
         check_equal($left_pass, $right_fail, "Checking my data");
         check_only_log(check_logger, "Checking my data - Got $left_pass_str. Expected $fail_str.", default_level);
+        check_result := check_equal($left_pass, $right_fail, "Checking my data");
+        assert_true(not check_result.p_is_pass);
+        assert_true(check_result.p_checker = default_checker);
+        assert_true(to_string(check_result.p_msg) = "Checking my data - Got $left_pass_str. Expected $fail_str.");
+        assert_true(check_result.p_level = default_level);
+        p_handle(check_result);
 
         check_equal($left_pass, $right_fail, result("for my data"));
         check_only_log(check_logger, "Equality check failed for my data - Got $left_pass_str. Expected $fail_str.",
                        default_level);
+        check_result := check_equal($left_pass, $right_fail, result("for my data"));
+        assert_true(not check_result.p_is_pass);
+        assert_true(check_result.p_checker = default_checker);
+        assert_true(to_string(check_result.p_msg) = "Equality check failed for my data - Got $left_pass_str. Expected $fail_str.");
+        assert_true(check_result.p_level = default_level);
+        p_handle(check_result);
 
         check_equal(passed, $left_pass, $right_fail);
         assert_true(not passed, "Should return pass = false on failing check");
         check_only_log(check_logger, "Equality check failed - Got $left_pass_str. Expected $fail_str.",
                        default_level);
 
         passed := check_equal($left_pass, $right_fail);
         assert_true(not passed, "Should return pass = false on failing check");
         check_only_log(check_logger, "Equality check failed - Got $left_pass_str. Expected $fail_str.",
                        default_level);
         unmock(check_logger);
         verify_passed_checks(stat, 0);
-        verify_failed_checks(stat, 6);
+        verify_failed_checks(stat, 10);
         reset_checker_stat;
 
         get_checker_stat(my_checker, stat);
         mock(my_logger);
         check_equal(my_checker, $left_pass, $right_fail);
         check_only_log(my_logger, "Equality check failed - Got $left_pass_str. Expected $fail_str.", default_level);
+        check_result := check_equal(my_checker, $left_pass, $right_fail);
+        assert_true(not check_result.p_is_pass);
+        assert_true(check_result.p_checker = my_checker);
+        assert_true(to_string(check_result.p_msg) = "Equality check failed - Got $left_pass_str. Expected $fail_str.");
+        assert_true(check_result.p_level = default_level);
+        p_handle(check_result);
 
         check_equal(my_checker, passed, $left_pass, $right_fail);
         assert_true(not passed, "Should return pass = false on failing check");
         check_only_log(my_logger, "Equality check failed - Got $left_pass_str. Expected $fail_str.", default_level);
 
         passed := check_equal(my_checker, $left_pass, $right_fail);
         assert_true(not passed, "Should return pass = false on failing check");
         check_only_log(my_logger, "Equality check failed - Got $left_pass_str. Expected $fail_str.", default_level);
 
         unmock(my_logger);
         verify_passed_checks(my_checker, stat, 0);
-        verify_failed_checks(my_checker, stat, 3);
+        verify_failed_checks(my_checker, stat, 4);
         reset_checker_stat(my_checker);
+
+      elsif run("Test that unhandled pass result for $left_type equal $right_type passes") then
+        check_result := check_equal($left_pass, $right_pass);
+        assert_true(not p_has_unhandled_checks);
+
+      elsif run("Test that unhandled failed result for $left_type equal $right_type fails") then
+        check_result := check_equal(my_checker, $left_pass, $right_fail);
+        assert_true(p_has_unhandled_checks);
+        mock_core_failure;
+        test_runner_cleanup(runner);
+        check_core_failure("Unhandled checks.");
+        unmock_core_failure;
+        p_handle(check_result);
+
 """
 
 combinations = [
     (
         "unsigned",
         "unsigned",
         """unsigned'(X"A5")""",
@@ -605,14 +738,16 @@
 use ieee.std_logic_1164.all;
 use ieee.numeric_std.all;
 library vunit_lib;
 use vunit_lib.checker_pkg.all;
 use vunit_lib.check_pkg.all;
 use vunit_lib.run_types_pkg.all;
 use vunit_lib.run_pkg.all;
+use vunit_lib.string_ptr_pkg.all;
+use vunit_lib.core_pkg.all;
 use work.test_support.all;
 
 use vunit_lib.log_levels_pkg.all;
 use vunit_lib.logger_pkg.all;
 
 entity tb_check_equal is
   generic (
@@ -622,14 +757,15 @@
 architecture test_fixture of tb_check_equal is
 begin
   check_equal_runner : process
     variable stat : checker_stat_t;
     variable my_checker : checker_t := new_checker("my_checker");
     variable my_logger : logger_t := get_logger(my_checker);
     variable passed : boolean;
+    variable check_result : check_result_t;
     constant default_level : log_level_t := error;
 
   begin
     test_runner_setup(runner, runner_cfg);
 
     while test_suite loop
       if run("Test should handle comparison of vectors longer than 32 bits") then
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/check/tools/generate_check_match.py` & `vunit_hdl-4.7.0/vunit/vhdl/check/tools/generate_check_match.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,27 +115,27 @@
     -- pragma translate_off
     if std_match(got, expected) then
       pass := true;
 
       if is_pass_visible(checker) then
         passing_check(
           checker,
-          std_msg(
+          p_std_msg(
             "Match check passed", msg,
             "Got " & $got_str & ". " &
             "Expected " & $expected_str & "."),
           path_offset + 1, line_num, file_name);
       else
         passing_check(checker);
       end if;
     else
       pass := false;
       failing_check(
         checker,
-        std_msg(
+        p_std_msg(
           "Match check failed", msg,
           "Got " & $got_str & ". " &
           "Expected " & $expected_str & "."),
         level, path_offset + 1, line_num, file_name);
     end if;
     -- pragma translate_on
   end;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/run.py` & `vunit_hdl-4.7.0/vunit/vhdl/com/run.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/src/com.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/src/com.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -33,24 +33,43 @@
     inbox_size  : positive := positive'high;
     outbox_size : positive := positive'high
     ) return actor_t is
   begin
     return messenger.create(name, inbox_size, outbox_size);
   end;
 
+  impure function new_actor (
+    id : id_t;
+    inbox_size : positive := positive'high;
+    outbox_size : positive := positive'high
+  ) return actor_t is
+  begin
+    return messenger.create(id, inbox_size, outbox_size);
+  end;
+
   impure function find (name : string; enable_deferred_creation : boolean := true) return actor_t is
   begin
     return messenger.find(name, enable_deferred_creation);
   end;
 
+  impure function find (id : id_t; enable_deferred_creation : boolean := true) return actor_t is
+  begin
+    return messenger.find(id, enable_deferred_creation);
+  end;
+
   impure function name (actor : actor_t) return string is
   begin
     return messenger.name(actor);
   end;
 
+  impure function get_id(actor : actor_t) return id_t is
+  begin
+    return messenger.get_id(actor);
+  end;
+
   procedure destroy (actor : inout actor_t) is
   begin
     messenger.destroy(actor);
   end;
 
   procedure reset_messenger is
   begin
@@ -125,25 +144,25 @@
       check(not messenger.is_full(receiver, mailbox_id), full_inbox_error);
     end if;
 
     messenger.send(receiver, mailbox_id, msg);
 
     if msg.sender /= null_actor then
       if messenger.has_subscribers(msg.sender, outbound) then
-        wait_on_subscribers(msg.sender, (0             => outbound), timeout - (now - t_start));
+        wait_on_subscribers(msg.sender, (0 => outbound), timeout - (now - t_start));
         messenger.internal_publish(msg.sender, msg, (0 => outbound));
       end if;
     end if;
 
     if (mailbox_id = inbox) and messenger.has_subscribers(receiver, inbound) then
-      wait_on_subscribers(receiver, (0             => inbound), timeout - (now - t_start));
+      wait_on_subscribers(receiver, (0 => inbound), timeout - (now - t_start));
       messenger.internal_publish(receiver, msg, (0 => inbound));
     end if;
 
-    notify(net);
+    notify_net(net);
     msg.data := null_queue;
   end;
 
   procedure send (
     signal net        : inout network_t;
     constant receiver : in    actor_t;
     variable msg      : inout msg_t;
@@ -247,15 +266,15 @@
     signal net       : inout network_t;
     constant sender  : in    actor_t;
     variable msg     : inout msg_t;
     constant timeout : in    time := max_timeout) is
   begin
     wait_on_subscribers(sender, (published, outbound), timeout);
     messenger.publish(sender, msg, (published, outbound));
-    notify(net);
+    notify_net(net);
     recycle(queue_pool, msg.data);
   end;
 
   impure function peek_message(
     actor      : actor_t;
     position   : natural      := 0;
     mailbox_id : mailbox_id_t := inbox) return msg_t is
@@ -375,15 +394,15 @@
     started_with_full_mailbox := messenger.is_full(actor, mailbox_id);
 
     msg      := messenger.get_all_but_payload(actor, position, mailbox_id);
     msg.data := decode(messenger.get_payload(actor, position, mailbox_id));
     messenger.delete_envelope(actor, position, mailbox_id);
 
     if started_with_full_mailbox then
-      notify(net);
+      notify_net(net);
     end if;
   end;
 
   procedure get_message (signal net : inout network_t; receiver : actor_t; variable msg : inout msg_t) is
   begin
     check(messenger.has_messages(receiver), null_message_error);
     get_message(net, receiver, 0, inbox, msg);
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/src/com_api.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/src/com_api.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -10,38 +10,57 @@
 library ieee;
 use ieee.std_logic_1164.all;
 
 use work.com_types_pkg.all;
 use work.queue_pkg.all;
 use work.integer_vector_ptr_pkg.all;
 use work.string_ptr_pkg.all;
+use work.id_pkg.all;
+use work.event_private_pkg.all;
 
 package com_pkg is
   -- Global predefined network. See network_t description in com_types.vhd for
   -- more information.
-  signal net : network_t := idle_network;
+  signal net : network_t := new_basic_event(com_net_event);
 
   -----------------------------------------------------------------------------
   -- Handling of actors
   -----------------------------------------------------------------------------
-  -- Create a new actor. Any number of unnamed actors (name = "") can be
-  -- created. Named actors must be unique
+  -- Create a new actor from name. Names must be unique and if no name is given
+  -- (name = "") the actor will be assigned a unique name internally. For each
+  -- new actor an identity for that name will be created if it doesn't already
+  -- exist.
   impure function new_actor (
     name : string := "";
     inbox_size : positive := positive'high;
     outbox_size : positive := positive'high
-    ) return actor_t;
+  ) return actor_t;
+
+  -- Create a new actor an identity. Only one actor can be created for each
+  -- identity.
+  impure function new_actor (
+    id : id_t;
+    inbox_size : positive := positive'high;
+    outbox_size : positive := positive'high
+  ) return actor_t;
 
   -- Find named actor by name. Enable deferred creation to create a deferred
   -- actor when no actor is found
   impure function find (name : string; enable_deferred_creation : boolean := true) return actor_t;
 
+  -- Find named actor by identity. Enable deferred creation to create a deferred
+  -- actor when no actor is found
+  impure function find (id : id_t; enable_deferred_creation : boolean := true) return actor_t;
+
   -- Name of actor
   impure function name (actor : actor_t) return string;
 
+  -- Return identity of actor
+  impure function get_id(actor : actor_t) return id_t;
+
   -- Destroy actor. Mailboxes are deallocated and dependent subscriptions are
   -- removed. Returns null_actor.
   procedure destroy (actor : inout actor_t);
 
   -- Reset communication system. All actors are destroyed.
   procedure reset_messenger;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/src/com_common.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/src/com_common.vhd`

 * *Files 22% similar despite different names*

```diff
@@ -7,32 +7,31 @@
 --
 -- Copyright (c) 2014-2023, Lars Asplund lars.anders.asplund@gmail.com
 library ieee;
 use ieee.std_logic_1164.all;
 
 use work.com_messenger_pkg.all;
 use work.com_types_pkg.all;
+use work.event_common_pkg.all;
+use work.event_private_pkg.all;
 
 package com_common_pkg is
   shared variable messenger :       messenger_t;
 
-  procedure notify (signal net : inout network_t);
-
+  procedure notify_net(signal net : inout basic_event_t);
   impure function no_error_status (status : com_status_t; old_api : boolean := false) return boolean;
 end package com_common_pkg;
 
 package body com_common_pkg is
-  procedure notify (signal net : inout network_t) is
+  procedure notify_net(signal net : inout basic_event_t) is
   begin
-    if net /= network_event then
-      net <= network_event;
-      wait until net = network_event;
-      net <= idle_network;
+    if not is_active(net) then
+      notify(net, n_delta_cycles => 0);
     end if;
-  end procedure notify;
+  end;
 
   impure function no_error_status (status : com_status_t; old_api : boolean := false) return boolean is
   begin
     return (status = ok) or ((status = timeout) and messenger.timeout_is_allowed and old_api);
   end;
 
 end package body com_common_pkg;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/src/com_context.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/src/com_context.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/src/com_debug_codec_builder.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/src/com_debug_codec_builder.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/src/com_deprecated.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/src/com_deprecated.vhd`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 use work.codec_pkg.all;
 use work.com_support_pkg.all;
 use work.com_messenger_pkg.all;
 use work.com_types_pkg.all;
 use work.com_pkg.all;
 use work.com_common_pkg.all;
+use work.event_common_pkg.all;
 
 use std.textio.all;
 
 package com_deprecated_pkg is
   -----------------------------------------------------------------------------
   -- Handling of actors
   -----------------------------------------------------------------------------
@@ -319,15 +320,15 @@
       wait on net until not messenger.is_full(receiver, mailbox_id) for timeout;
       check(not messenger.is_full(receiver, mailbox_id), full_inbox_error);
     end if;
 
     messenger.send(message.sender, receiver, mailbox_id, message.request_id, message.payload.all, receipt);
     message.id       := receipt.id;
     message.receiver := receiver;
-    notify(net);
+    notify_net(net);
 
     if not keep_message then
       delete(message);
     end if;
   end;
 
   procedure send (
@@ -356,15 +357,15 @@
       return;
     end if;
 
     if status = ok then
       started_with_full_inbox := messenger.is_full(receiver, inbox);
       message                 := get_message(receiver);
       if started_with_full_inbox then
-        notify(net);
+        notify_net(net);
       end if;
     else
       message          := new message_t;
       message.receiver := receiver;
       message.status   := status;
     end if;
   end;
@@ -404,23 +405,23 @@
       started_with_full_inbox := messenger.is_full(receiver, inbox);
     end if;
 
     if messenger.has_reply_stash_message(receiver, request_id) then
       return;
     elsif messenger.find_and_stash_reply_message(receiver, request_id, mailbox_id) then
       if started_with_full_inbox then
-        notify(net);
+        notify_net(net);
       end if;
       return;
     else
       wait on net until messenger.find_and_stash_reply_message(receiver, request_id, mailbox_id) for timeout;
       if not messenger.has_reply_stash_message(receiver, request_id) then
         status := work.com_types_pkg.timeout;
       elsif started_with_full_inbox then
-        notify(net);
+        notify_net(net);
       end if;
     end if;
   end procedure wait_for_reply_stash_message;
 
   impure function get_reply_stash_message (
     receiver          : actor_t;
     clear_reply_stash : boolean := true)
@@ -484,15 +485,15 @@
 
     if messenger.subscriber_inbox_is_full(message.sender, (published, outbound)) then
       wait on net until not messenger.subscriber_inbox_is_full(sender, (published, outbound)) for timeout;
       check(not messenger.subscriber_inbox_is_full(message.sender, (published, outbound)), full_inbox_error);
     end if;
 
     messenger.publish(message.sender, message.payload.all);
-    notify(net);
+    notify_net(net);
 
     if not keep_message then
       delete(message);
     end if;
   end;
   procedure send (
     signal net            : inout network_t;
@@ -510,15 +511,15 @@
       wait on net until not messenger.is_full(receiver, inbox) for timeout;
       check(not messenger.is_full(receiver, inbox), full_inbox_error);
     end if;
 
     messenger.send(message.sender, receiver, inbox, message.request_id, message.payload.all, receipt);
     message.id       := receipt.id;
     message.receiver := receiver;
-    notify(net);
+    notify_net(net);
 
     if not keep_message then
       delete(message);
     end if;
   end;
 
   --
@@ -874,15 +875,15 @@
     status := ok;
     if messenger.subscriber_inbox_is_full(message.sender, (published, outbound)) then
       wait on net until not messenger.subscriber_inbox_is_full(message.sender, (published, outbound)) for timeout;
       check(not messenger.subscriber_inbox_is_full(message.sender, (published, outbound)), full_inbox_error);
     end if;
 
     messenger.publish(message.sender, message.payload.all);
-    notify(net);
+    notify_net(net);
 
     if not keep_message then
       delete(message);
     end if;
   end;
 
   -----------------------------------------------------------------------------
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/src/com_messenger.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/src/com_messenger.vhd`

 * *Files 10% similar despite different names*

```diff
@@ -11,31 +11,39 @@
 use work.com_support_pkg.all;
 use work.queue_pkg.all;
 use work.queue_pool_pkg.all;
 use work.string_ptr_pkg.all;
 use work.codec_pkg.all;
 use work.logger_pkg.all;
 use work.log_levels_pkg.all;
+use work.id_pkg.all;
 
 use std.textio.all;
 
 package com_messenger_pkg is
   type subscription_traffic_types_t is array (natural range <>) of subscription_traffic_type_t;
 
   type messenger_t is protected
     -----------------------------------------------------------------------------
     -- Handling of actors
     -----------------------------------------------------------------------------
     impure function create (
+      id : id_t;
+      inbox_size : positive := positive'high;
+      outbox_size : positive := positive'high
+      ) return actor_t;
+    impure function create (
       name : string := "";
       inbox_size : positive := positive'high;
       outbox_size : positive := positive'high
       ) return actor_t;
     impure function find (name  : string; enable_deferred_creation : boolean := true) return actor_t;
+    impure function find (id  : id_t; enable_deferred_creation : boolean := true) return actor_t;
     impure function name (actor : actor_t) return string;
+    impure function get_id (actor : actor_t) return id_t;
 
     procedure destroy (actor : inout actor_t);
     procedure reset_messenger;
 
     impure function num_of_actors return natural;
     impure function get_all_actors return actor_vec_t;
     impure function is_deferred(actor : actor_t) return boolean;
@@ -193,30 +201,30 @@
     next_item : subscriber_item_ptr_t;
   end record subscriber_item_t;
 
   type subscribers_t is array (subscription_traffic_type_t range published to inbound) of subscriber_item_ptr_t;
 
   type actor_item_t is record
     actor             : actor_t;
-    name              : line;
+    id                : id_t;
     deferred_creation : boolean;
     inbox             : mailbox_ptr_t;
     outbox            : mailbox_ptr_t;
     reply_stash       : envelope_ptr_t;
     subscribers       : subscribers_t;
   end record actor_item_t;
 
   type actor_item_array_t is array (natural range <>) of actor_item_t;
   type actor_item_array_ptr_t is access actor_item_array_t;
 
   type messenger_t is protected
     body
       variable null_actor_item : actor_item_t := (
         actor             => null_actor,
-        name              => null,
+        id                => null_id,
         deferred_creation => false,
         inbox             => create(0),
         outbox            => create(0),
         reply_stash       => null,
         subscribers       => (null, null, null));  --
     variable envelope_recycle_bin : envelope_ptr_array(1 to 1000);
     variable n_recycled_envelopes : natural      := 0;
@@ -264,111 +272,183 @@
   variable actors : actor_item_array_ptr_t := init_actors;
 
   impure function find_actor (name : string) return actor_t is
     variable ret_val : actor_t;
   begin
     for i in actors'reverse_range loop
       ret_val := actors(i).actor;
-      if actors(i).name /= null then
-        exit when actors(i).name.all = name;
+      if actors(i).id /= null_id then
+        exit when full_name(actors(i).id) = name;
+      end if;
+    end loop;
+
+    return ret_val;
+  end;
+
+  impure function find_actor (id : id_t) return actor_t is
+    variable ret_val : actor_t;
+  begin
+    for i in actors'reverse_range loop
+      ret_val := actors(i).actor;
+      if actors(i).id /= null_id then
+        exit when actors(i).id = id;
       end if;
     end loop;
 
     return ret_val;
   end;
 
   impure function create_actor (
-    name              :    string  := "";
+    id : id_t;
     deferred_creation : in boolean := false;
     inbox_size        : in natural := natural'high;
     outbox_size        : in natural := natural'high)
     return actor_t is
     variable old_actors : actor_item_array_ptr_t;
+    variable actor_id_number : integer;
+    variable resolved_id : id_t;
   begin
     old_actors := actors;
     actors     := new actor_item_array_t(0 to actors'length);
     actors(0)  := null_actor_item;
     for i in old_actors'range loop
       actors(i) := old_actors(i);
     end loop;
     deallocate(old_actors);
-    actors(actors'length - 1) := ((id => actors'length - 1), new string'(name),
+    actor_id_number := actors'length - 1;
+    if id = null_id then
+      resolved_id := get_id("_actor_" & to_string(actor_id_number));
+    else
+      resolved_id := id;
+    end if;
+    actors(actors'length - 1) := ((p_id_number => actor_id_number), resolved_id,
                                   deferred_creation, create(inbox_size), create(outbox_size), null, (null, null, null));
 
     return actors(actors'length - 1).actor;
   end function;
 
+  impure function create_actor (
+    name              :    string  := "";
+    deferred_creation : in boolean := false;
+    inbox_size        : in natural := natural'high;
+    outbox_size        : in natural := natural'high)
+    return actor_t is
+    variable id : id_t;
+  begin
+    id := null_id when name = "" else get_id(name);
+
+    return create_actor(id, deferred_creation, inbox_size, outbox_size);
+  end function;
+
+  impure function find (id : id_t; enable_deferred_creation : boolean := true) return actor_t is
+    constant actor : actor_t := find_actor(id);
+  begin
+    if (id = null_id) or (id = root_id) then
+      return null_actor;
+    elsif (actor = null_actor) and enable_deferred_creation then
+      return create_actor(id, true, 1);
+    else
+      return actor;
+    end if;
+  end;
+
   impure function find (name : string; enable_deferred_creation : boolean := true) return actor_t is
     constant actor : actor_t := find_actor(name);
   begin
     if name = "" then
       return null_actor;
     elsif (actor = null_actor) and enable_deferred_creation then
       return create_actor(name, true, 1);
     else
       return actor;
     end if;
   end;
 
   impure function name (actor : actor_t) return string is
   begin
-    if actors(actor.id).name /= null then
-      return actors(actor.id).name.all;
+    if actors(actor.p_id_number).id /= null_id then
+      return full_name(actors(actor.p_id_number).id);
     else
       return "";
     end if;
 
   end;
 
+  impure function get_id (actor : actor_t) return id_t is
+  begin
+    return actors(actor.p_id_number).id;
+  end;
+
+  impure function create (
+    id : id_t;
+    inbox_size : positive := positive'high;
+    outbox_size : positive := positive'high
+    ) return actor_t is
+    variable actor : actor_t := find_actor(id);
+  begin
+    if id = root_id then
+      check_failed(new_actor_from_root_id_error);
+    elsif actor = null_actor then
+      actor := create_actor(id, false, inbox_size, outbox_size);
+    elsif actors(actor.p_id_number).deferred_creation then
+      actors(actor.p_id_number).deferred_creation := false;
+      actors(actor.p_id_number).inbox.size        := inbox_size;
+      actors(actor.p_id_number).outbox.size       := outbox_size;
+    else
+      check_failed(duplicate_actor_name_error);
+    end if;
+
+    return actor;
+  end;
 
   impure function create (
     name : string := "";
     inbox_size : positive := positive'high;
     outbox_size : positive := positive'high
     ) return actor_t is
     variable actor : actor_t := find_actor(name);
   begin
-    if (actor = null_actor) or (name = "") then
+    if actor = null_actor then
       actor := create_actor(name, false, inbox_size, outbox_size);
-    elsif actors(actor.id).deferred_creation then
-      actors(actor.id).deferred_creation := false;
-      actors(actor.id).inbox.size        := inbox_size;
-      actors(actor.id).outbox.size       := outbox_size;
+    elsif actors(actor.p_id_number).deferred_creation then
+      actors(actor.p_id_number).deferred_creation := false;
+      actors(actor.p_id_number).inbox.size        := inbox_size;
+      actors(actor.p_id_number).outbox.size       := outbox_size;
     else
       check_failed(duplicate_actor_name_error);
     end if;
 
     return actor;
   end;
 
   impure function is_subscriber (
     subscriber   : actor_t;
     publisher    : actor_t;
     traffic_type : subscription_traffic_type_t) return boolean is
-    variable item : subscriber_item_ptr_t := actors(publisher.id).subscribers(traffic_type);
+    variable item : subscriber_item_ptr_t := actors(publisher.p_id_number).subscribers(traffic_type);
   begin
     while item /= null loop
       if item.actor = subscriber then
         return true;
       end if;
       item := item.next_item;
     end loop;
 
     return false;
   end;
 
   procedure remove_subscriber (subscriber : actor_t; publisher : actor_t; traffic_type : subscription_traffic_type_t) is
     variable item, previous_item : subscriber_item_ptr_t;
   begin
-    item          := actors(publisher.id).subscribers(traffic_type);
+    item          := actors(publisher.p_id_number).subscribers(traffic_type);
     previous_item := null;
     while item /= null loop
       if item.actor = subscriber then
         if previous_item = null then
-          actors(publisher.id).subscribers(traffic_type) := item.next_item;
+          actors(publisher.p_id_number).subscribers(traffic_type) := item.next_item;
         else
           previous_item.next_item := item.next_item;
         end if;
         deallocate(item);
         return;
       end if;
       previous_item := item;
@@ -380,41 +460,40 @@
 
   procedure destroy (actor : inout actor_t) is
     variable envelope           : envelope_ptr_t;
     variable item               : subscriber_item_ptr_t;
   begin
     check(not unknown_actor(actor), unknown_actor_error);
 
-    while actors(actor.id).inbox.first_envelope /= null loop
-      envelope                              := actors(actor.id).inbox.first_envelope;
-      actors(actor.id).inbox.first_envelope := envelope.next_envelope;
+    while actors(actor.p_id_number).inbox.first_envelope /= null loop
+      envelope                              := actors(actor.p_id_number).inbox.first_envelope;
+      actors(actor.p_id_number).inbox.first_envelope := envelope.next_envelope;
       deallocate(envelope.message.payload);
       deallocate_envelope(envelope);
     end loop;
 
     for t in subscription_traffic_type_t'left to subscription_traffic_type_t'right loop
-      while actors(actor.id).subscribers(t) /= null loop
-        item                            := actors(actor.id).subscribers(t);
-        actors(actor.id).subscribers(t) := item.next_item;
+      while actors(actor.p_id_number).subscribers(t) /= null loop
+        item                            := actors(actor.p_id_number).subscribers(t);
+        actors(actor.p_id_number).subscribers(t) := item.next_item;
         deallocate(item);
       end loop;
     end loop;
 
     for i in actors'range loop
       for t in subscription_traffic_type_t'left to subscription_traffic_type_t'right loop
         if is_subscriber(actor, actors(i).actor, t) then
           remove_subscriber(actor, actors(i).actor, t);
         end if;
       end loop;
     end loop;
 
-    deallocate(actors(actor.id).name);
-    deallocate(actors(actor.id).inbox);
-    deallocate(actors(actor.id).outbox);
-    actors(actor.id) := null_actor_item;
+    deallocate(actors(actor.p_id_number).inbox);
+    deallocate(actors(actor.p_id_number).outbox);
+    actors(actor.p_id_number) := null_actor_item;
     actor            := null_actor;
   end;
 
   procedure reset_messenger is
   begin
     for i in actors'range loop
       if actors(i).actor /= null_actor then
@@ -452,15 +531,15 @@
 
     return result;
   end;
 
 
   impure function is_deferred(actor : actor_t) return boolean is
   begin
-    return actors(actor.id).deferred_creation;
+    return actors(actor.p_id_number).deferred_creation;
   end;
 
   impure function num_of_deferred_creations return natural is
     variable n_deferred_actors : natural := 0;
   begin
     for i in actors'range loop
       if actors(i).deferred_creation then
@@ -469,54 +548,54 @@
     end loop;
 
     return n_deferred_actors;
   end;
 
   impure function unknown_actor (actor : actor_t) return boolean is
   begin
-    if (actor.id = 0) or (actor.id > actors'length - 1) then
+    if (actor.p_id_number = 0) or (actor.p_id_number > actors'length - 1) then
       return true;
-    elsif actors(actor.id).actor = null_actor then
+    elsif actors(actor.p_id_number).actor = null_actor then
       return true;
     end if;
 
     return false;
   end function unknown_actor;
 
   impure function deferred (actor : actor_t) return boolean is
   begin
-    return actors(actor.id).deferred_creation;
+    return actors(actor.p_id_number).deferred_creation;
   end function deferred;
 
   impure function is_full (actor : actor_t; mailbox_id : mailbox_id_t) return boolean is
   begin
     if mailbox_id = inbox then
-      return actors(actor.id).inbox.num_of_messages >= actors(actor.id).inbox.size;
+      return actors(actor.p_id_number).inbox.num_of_messages >= actors(actor.p_id_number).inbox.size;
     else
-      return actors(actor.id).outbox.num_of_messages >= actors(actor.id).outbox.size;
+      return actors(actor.p_id_number).outbox.num_of_messages >= actors(actor.p_id_number).outbox.size;
     end if;
   end function;
 
   impure function num_of_messages (actor : actor_t; mailbox_id : mailbox_id_t) return natural is
   begin
     if mailbox_id = inbox then
-      return actors(actor.id).inbox.num_of_messages;
+      return actors(actor.p_id_number).inbox.num_of_messages;
     else
-      return actors(actor.id).outbox.num_of_messages;
+      return actors(actor.p_id_number).outbox.num_of_messages;
     end if;
   end function;
 
   procedure resize_mailbox (actor : actor_t; new_size : natural; mailbox_id : mailbox_id_t) is
   begin
     if mailbox_id = inbox then
       check(num_of_messages(actor, inbox) <= new_size, insufficient_size_error);
-      actors(actor.id).inbox.size         := new_size;
+      actors(actor.p_id_number).inbox.size         := new_size;
     else
       check(num_of_messages(actor, outbox) <= new_size, insufficient_size_error);
-      actors(actor.id).outbox.size         := new_size;
+      actors(actor.p_id_number).outbox.size         := new_size;
     end if;
   end;
 
   impure function subscriber_inbox_is_full (
     publisher                  : actor_t;
     subscription_traffic_types : subscription_traffic_types_t) return boolean is
     variable result : boolean_vector(subscription_traffic_types'range) := (others => false);
@@ -525,40 +604,40 @@
       variable result      : out boolean) is
       variable item : subscriber_item_ptr_t := subscribers;
     begin
       result := false;
       while item /= null loop
         result := is_full(item.actor, inbox);
         exit when result;
-        has_full_inboxes(actors(item.actor.id).subscribers(inbound), result);
+        has_full_inboxes(actors(item.actor.p_id_number).subscribers(inbound), result);
         exit when result;
         item   := item.next_item;
       end loop;
     end;
   begin
     for t in subscription_traffic_types'range loop
-      has_full_inboxes(actors(publisher.id).subscribers(subscription_traffic_types(t)), result(t));
+      has_full_inboxes(actors(publisher.p_id_number).subscribers(subscription_traffic_types(t)), result(t));
     end loop;
 
     return or result;
   end function;
 
   impure function has_subscribers (
     actor                     : actor_t;
     subscription_traffic_type : subscription_traffic_type_t := published) return boolean is
   begin
-    return actors(actor.id).subscribers(subscription_traffic_type) /= null;
+    return actors(actor.p_id_number).subscribers(subscription_traffic_type) /= null;
   end;
 
   impure function mailbox_size (actor : actor_t; mailbox_id : mailbox_id_t) return natural is
   begin
     if mailbox_id = inbox then
-      return actors(actor.id).inbox.size;
+      return actors(actor.p_id_number).inbox.size;
     else
-      return actors(actor.id).outbox.size;
+      return actors(actor.p_id_number).outbox.size;
     end if;
   end function;
 
   -----------------------------------------------------------------------------
   -- Send related subprograms
   -----------------------------------------------------------------------------
   procedure send (
@@ -579,15 +658,15 @@
     envelope.message.sender     := sender;
     envelope.message.receiver   := receiver;
     envelope.message.id         := next_message_id;
     envelope.message.request_id := request_id;
     write(envelope.message.payload, payload);
     next_message_id             := next_message_id + 1;
 
-    mailbox                 := actors(receiver.id).inbox when mailbox_id = inbox else actors(receiver.id).outbox;
+    mailbox                 := actors(receiver.p_id_number).inbox when mailbox_id = inbox else actors(receiver.p_id_number).outbox;
     mailbox.num_of_messages := mailbox.num_of_messages + 1;
     if mailbox.last_envelope /= null then
       mailbox.last_envelope.next_envelope := envelope;
     else
       mailbox.first_envelope := envelope;
     end if;
     mailbox.last_envelope := envelope;
@@ -595,15 +674,15 @@
 
   procedure publish (sender : actor_t; payload : string) is
     variable receipt         : receipt_t;
     variable subscriber_item : subscriber_item_ptr_t;
   begin
     check(not unknown_actor(sender), unknown_publisher_error);
 
-    subscriber_item := actors(sender.id).subscribers(published);
+    subscriber_item := actors(sender.p_id_number).subscribers(published);
     while subscriber_item /= null loop
       send(sender, subscriber_item.actor, inbox, no_message_id, payload, receipt);
       subscriber_item := subscriber_item.next_item;
     end loop;
   end;
 
   impure function to_string(msg : msg_t) return string is
@@ -665,15 +744,15 @@
     envelope.message.id         := msg.id;
     envelope.message.msg_type   := msg.msg_type;
     envelope.message.sender     := msg.sender;
     envelope.message.receiver   := msg.receiver;
     envelope.message.request_id := msg.request_id;
     write(envelope.message.payload, encode(data));
 
-    mailbox                 := actors(receiver.id).inbox when mailbox_id = inbox else actors(receiver.id).outbox;
+    mailbox                 := actors(receiver.p_id_number).inbox when mailbox_id = inbox else actors(receiver.p_id_number).outbox;
     mailbox.num_of_messages := mailbox.num_of_messages + 1;
     if mailbox.last_envelope /= null then
       mailbox.last_envelope.next_envelope := envelope;
     else
       mailbox.first_envelope := envelope;
     end if;
     mailbox.last_envelope := envelope;
@@ -705,28 +784,28 @@
 
     msg.id     := next_message_id;
     next_message_id := next_message_id + 1;
     msg.status := ok;
     msg.sender := sender;
 
     for t in subscriber_traffic_types'range loop
-      put_subscriber_messages(actors(sender.id).subscribers(subscriber_traffic_types(t)),
+      put_subscriber_messages(actors(sender.p_id_number).subscribers(subscriber_traffic_types(t)),
                               msg, set_msg_receiver => true);
     end loop;
 
     msg.receiver := null_actor;
   end;
 
   procedure internal_publish (
     constant sender                   : in    actor_t;
     variable msg                      : inout msg_t;
     constant subscriber_traffic_types : in    subscription_traffic_types_t) is
   begin
     for t in subscriber_traffic_types'range loop
-      put_subscriber_messages(actors(sender.id).subscribers(subscriber_traffic_types(t)),
+      put_subscriber_messages(actors(sender.p_id_number).subscribers(subscriber_traffic_types(t)),
                               msg, set_msg_receiver => false);
     end loop;
   end;
 
   procedure send (
     constant receiver   : in    actor_t;
     constant mailbox_id : in    mailbox_id_t;
@@ -747,15 +826,15 @@
   end;
 
   -----------------------------------------------------------------------------
   -- Receive related subprograms
   -----------------------------------------------------------------------------
   impure function has_messages (actor : actor_t) return boolean is
   begin
-    return actors(actor.id).inbox.first_envelope /= null;
+    return actors(actor.p_id_number).inbox.first_envelope /= null;
   end function has_messages;
 
   impure function has_messages (actor_vec : actor_vec_t) return boolean is
   begin
     for i in actor_vec'range loop
       if has_messages(actor_vec(i)) then
         return true;
@@ -768,15 +847,15 @@
     actor      : actor_t;
     position   : natural;
     mailbox_id : mailbox_id_t;
     variable mailbox : inout mailbox_ptr_t;
     variable envelope : inout envelope_ptr_t;
     variable previous_envelope : inout envelope_ptr_t) is
   begin
-    mailbox  := actors(actor.id).inbox when mailbox_id = inbox else actors(actor.id).outbox;
+    mailbox  := actors(actor.p_id_number).inbox when mailbox_id = inbox else actors(actor.p_id_number).outbox;
     envelope := mailbox.first_envelope;
     previous_envelope := null;
 
     for i in 1 to position loop
       exit when envelope = null;
       previous_envelope := envelope;
       envelope := envelope.next_envelope;
@@ -921,64 +1000,64 @@
 
   impure function has_reply_stash_message (
     actor      : actor_t;
     request_id : message_id_t := no_message_id)
     return boolean is
   begin
     if request_id = no_message_id then
-      return actors(actor.id).reply_stash /= null;
-    elsif actors(actor.id).reply_stash /= null then
-      return actors(actor.id).reply_stash.message.request_id = request_id;
+      return actors(actor.p_id_number).reply_stash /= null;
+    elsif actors(actor.p_id_number).reply_stash /= null then
+      return actors(actor.p_id_number).reply_stash.message.request_id = request_id;
     else
       return false;
     end if;
   end function has_reply_stash_message;
 
   impure function get_reply_stash_message_payload (actor : actor_t) return string is
-    variable envelope : envelope_ptr_t := actors(actor.id).reply_stash;
+    variable envelope : envelope_ptr_t := actors(actor.p_id_number).reply_stash;
   begin
     if envelope /= null then
       return envelope.message.payload.all;
     else
       return "";
     end if;
   end;
 
   impure function get_reply_stash_message_sender (actor : actor_t) return actor_t is
-    variable envelope : envelope_ptr_t := actors(actor.id).reply_stash;
+    variable envelope : envelope_ptr_t := actors(actor.p_id_number).reply_stash;
   begin
     if envelope /= null then
       return envelope.message.sender;
     else
       return null_actor;
     end if;
   end;
 
   impure function get_reply_stash_message_receiver (actor     : actor_t) return actor_t is
-    variable envelope : envelope_ptr_t := actors(actor.id).reply_stash;
+    variable envelope : envelope_ptr_t := actors(actor.p_id_number).reply_stash;
   begin
     if envelope /= null then
       return envelope.message.receiver;
     else
       return null_actor;
     end if;
   end;
 
   impure function get_reply_stash_message_id (actor : actor_t) return message_id_t is
-    variable envelope : envelope_ptr_t := actors(actor.id).reply_stash;
+    variable envelope : envelope_ptr_t := actors(actor.p_id_number).reply_stash;
   begin
     if envelope /= null then
       return envelope.message.id;
     else
       return no_message_id;
     end if;
   end;
 
   impure function get_reply_stash_message_request_id (actor : actor_t) return message_id_t is
-    variable envelope : envelope_ptr_t := actors(actor.id).reply_stash;
+    variable envelope : envelope_ptr_t := actors(actor.p_id_number).reply_stash;
   begin
     if envelope /= null then
       return envelope.message.request_id;
     else
       return no_message_id;
     end if;
   end;
@@ -988,15 +1067,15 @@
     request_id : message_id_t;
     mailbox_id : mailbox_id_t;
     variable mailbox : inout mailbox_ptr_t;
     variable envelope : inout envelope_ptr_t;
     variable previous_envelope : out envelope_ptr_t;
     variable position : out natural) is
   begin
-    mailbox  := actors(actor.id).inbox when mailbox_id = inbox else actors(actor.id).outbox;
+    mailbox  := actors(actor.p_id_number).inbox when mailbox_id = inbox else actors(actor.p_id_number).outbox;
     envelope := mailbox.first_envelope;
     previous_envelope := null;
     position := 0;
 
     while envelope /= null loop
       if envelope.message.request_id = request_id then
         return;
@@ -1035,15 +1114,15 @@
     variable previous_envelope : envelope_ptr_t := null;
     variable mailbox           : mailbox_ptr_t;
     variable position : natural;
   begin
     find_reply_message(actor, request_id, mailbox_id, mailbox, envelope, previous_envelope, position);
 
     if envelope /= null then
-      actors(actor.id).reply_stash := envelope;
+      actors(actor.p_id_number).reply_stash := envelope;
 
       if previous_envelope /= null then
         previous_envelope.next_envelope := envelope.next_envelope;
       else
         mailbox.first_envelope := envelope.next_envelope;
       end if;
 
@@ -1057,16 +1136,16 @@
     end if;
 
     return false;
   end function find_and_stash_reply_message;
 
   procedure clear_reply_stash (actor : actor_t) is
   begin
-    deallocate(actors(actor.id).reply_stash.message.payload);
-    deallocate(actors(actor.id).reply_stash);
+    deallocate(actors(actor.p_id_number).reply_stash.message.payload);
+    deallocate(actors(actor.p_id_number).reply_stash);
   end procedure clear_reply_stash;
 
   procedure subscribe (
     subscriber   : actor_t;
     publisher    : actor_t;
     traffic_type : subscription_traffic_type_t := published) is
     variable new_subscriber : subscriber_item_ptr_t;
@@ -1077,22 +1156,22 @@
     if traffic_type = published then
       check(not is_subscriber(subscriber, publisher, outbound), already_a_subscriber_error);
     elsif traffic_type = outbound then
       check(not is_subscriber(subscriber, publisher, published), already_a_subscriber_error);
     end if;
 
     if traffic_type = published then
-      new_subscriber                              := new subscriber_item_t'(subscriber, actors(publisher.id).subscribers(published));
-      actors(publisher.id).subscribers(published) := new_subscriber;
+      new_subscriber                              := new subscriber_item_t'(subscriber, actors(publisher.p_id_number).subscribers(published));
+      actors(publisher.p_id_number).subscribers(published) := new_subscriber;
     elsif traffic_type = outbound then
-      new_subscriber                             := new subscriber_item_t'(subscriber, actors(publisher.id).subscribers(outbound));
-      actors(publisher.id).subscribers(outbound) := new_subscriber;
+      new_subscriber                             := new subscriber_item_t'(subscriber, actors(publisher.p_id_number).subscribers(outbound));
+      actors(publisher.p_id_number).subscribers(outbound) := new_subscriber;
     else
-      new_subscriber                            := new subscriber_item_t'(subscriber, actors(publisher.id).subscribers(inbound));
-      actors(publisher.id).subscribers(inbound) := new_subscriber;
+      new_subscriber                            := new subscriber_item_t'(subscriber, actors(publisher.p_id_number).subscribers(inbound));
+      actors(publisher.p_id_number).subscribers(inbound) := new_subscriber;
     end if;
   end procedure subscribe;
 
   procedure unsubscribe (
     subscriber   : actor_t;
     publisher    : actor_t;
     traffic_type : subscription_traffic_type_t := published) is
@@ -1152,30 +1231,30 @@
 
   impure function get_subscribers(publisher : actor_t) return subscription_vec_t is
     impure function num_of_subscriptions return natural is
       variable n_subscriptions : natural := 0;
       variable item : subscriber_item_ptr_t;
     begin
       for t in subscription_traffic_type_t'left to subscription_traffic_type_t'right loop
-        item := actors(publisher.id).subscribers(t);
+        item := actors(publisher.p_id_number).subscribers(t);
         while item /= null loop
           n_subscriptions := n_subscriptions + 1;
           item := item.next_item;
         end loop;
       end loop;
 
       return n_subscriptions;
     end;
     constant n_subscriptions : natural := num_of_subscriptions;
     variable subscriptions : subscription_vec_t(0 to n_subscriptions - 1);
     variable item : subscriber_item_ptr_t;
     variable idx : natural := 0;
   begin
     for t in subscription_traffic_type_t'left to subscription_traffic_type_t'right loop
-      item := actors(publisher.id).subscribers(t);
+      item := actors(publisher.p_id_number).subscribers(t);
       while item /= null loop
         subscriptions(idx).subscriber := item.actor;
         subscriptions(idx).publisher := publisher;
         subscriptions(idx).traffic_type := t;
         idx := idx + 1;
         item := item.next_item;
       end loop;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/src/com_string.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/src/com_string.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/src/com_support.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/src/com_support.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/src/com_types.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/src/com_types.vhd`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 use work.integer_vector_ptr_pkg.all;
 use work.integer_array_pkg.all;
 use work.string_ptr_pkg.all;
 use work.logger_pkg.all;
 use work.queue_pkg.all;
 use work.queue_2008p_pkg.all;
 use work.queue_pool_pkg.all;
+use work.dict_pkg.all;
+use work.event_private_pkg.all;
 
 package com_types_pkg is
 
   -- These status types are mostly internal to com and will cause runtime
   -- errors. Only ok and timeout will ever be returned to the user
   type com_status_t is (ok,
                         timeout,
@@ -39,24 +41,25 @@
                         already_a_subscriber_error,
                         not_a_subscriber_error,
                         full_inbox_error,
                         reply_missing_request_id_error,
                         unknown_request_id_error,
                         deprecated_interface_error,
                         insufficient_size_error,
-                        duplicate_actor_name_error);
+                        duplicate_actor_name_error,
+                        new_actor_from_root_id_error);
 
-  subtype com_error_t is com_status_t range timeout to duplicate_actor_name_error;
+  subtype com_error_t is com_status_t range timeout to new_actor_from_root_id_error;
 
   -- All fields of the actor type are private
   type actor_t is record
-    id : natural;
+    p_id_number : natural;
   end record actor_t;
   type actor_vec_t is array (integer range <>) of actor_t;
-  constant null_actor : actor_t := (id => 0);
+  constant null_actor : actor_t := (p_id_number => 0);
 
   -- Mailboxes owned by an actor
   type mailbox_id_t is (inbox, outbox);
 
   -- A message type (of type msg_type_t) can be used identify the type of a message
   -- (of type msg_t) such that it can be parsed correctly.
   type msg_type_t is record
@@ -140,17 +143,15 @@
     id : message_id_t;
   end record receipt_t;
 
   -- An event type representing the network over which actors communicate. An event in
   -- the network notifies connected actors which can determine the cause of the
   -- event by consulting the com messenger (com_messenger.vhd). Actors can be
   -- connected to different networks but there's only one global messenger.
-  subtype network_t is std_logic;
-  constant network_event : std_logic := '1';
-  constant idle_network : std_logic := 'Z';
+  alias network_t is basic_event_t;
 
   -- Default value for timeout parameters. ModelSim can't handle time'high
   constant max_timeout : time := 1 hr;
 
   -- Captures the state of a mailbox
   type mailbox_state_t is record
     id : mailbox_id_t;
@@ -390,14 +391,19 @@
   alias pop_msg_t is pop[msg_t return msg_t];
 
   procedure push_ref(constant msg : msg_t; value : inout integer_array_t);
   impure function pop_ref(msg : msg_t) return integer_array_t;
   alias push_integer_array_t_ref is push_ref[msg_t, integer_array_t];
   alias pop_integer_array_t_ref is pop_ref[msg_t return integer_array_t];
 
+  procedure push_ref(constant msg : msg_t; value : inout dict_t);
+  impure function pop_ref(msg : msg_t) return dict_t;
+  alias push_dict_t_ref is push_ref[msg_t, dict_t];
+  alias pop_dict_t_ref is pop_ref[msg_t return dict_t];
+
 end package;
 
 package body com_types_pkg is
 
   -----------------------------------------------------------------------------
   -- Handling of message types
   -----------------------------------------------------------------------------
@@ -515,29 +521,29 @@
   end;
 
   procedure push(queue : queue_t; variable value : inout msg_t) is
   begin
     push(queue, value.id);
     push(queue, value.msg_type.p_code);
     push(queue, com_status_t'pos(value.status));
-    push(queue, value.sender.id);
-    push(queue, value.receiver.id);
+    push(queue, value.sender.p_id_number);
+    push(queue, value.receiver.p_id_number);
     push(queue, value.request_id);
     push_queue_ref(queue, value.data);
     value := null_msg;
   end;
 
   impure function pop(queue : queue_t) return msg_t is
     variable ret_val : msg_t;
   begin
     ret_val.id := pop(queue);
     ret_val.msg_type := (p_code => pop(queue));
     ret_val.status := com_status_t'val(integer'(pop(queue)));
-    ret_val.sender.id := pop(queue);
-    ret_val.receiver.id := pop(queue);
+    ret_val.sender.p_id_number := pop(queue);
+    ret_val.receiver.p_id_number := pop(queue);
     ret_val.request_id := pop(queue);
     ret_val.data := pop_queue_ref(queue);
 
     return ret_val;
   end;
 
   -----------------------------------------------------------------------------
@@ -850,8 +856,19 @@
   end;
 
   impure function pop_ref(msg : msg_t) return integer_array_t is
   begin
     return pop_ref(msg.data);
   end;
 
+  procedure push_ref(constant msg : msg_t; value : inout dict_t) is
+  begin
+    push_ref(msg.data, value);
+  end;
+
+  impure function pop_ref(msg : msg_t) return dict_t is
+  begin
+    return pop_ref(msg.data);
+  end;
+
+
 end package body com_types_pkg;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/test/custom_types.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/test/custom_types.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/test/tb_com.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/test/tb_com.vhd`

 * *Files 4% similar despite different names*

```diff
@@ -54,69 +54,136 @@
     variable null_actor_state                                   : actor_state_t     := (null,
                                                                                         false,
                                                                                         null_mailbox_state,
                                                                                         null_mailbox_state,
                                                                                         null, null
                                                                                        );
     variable null_messenger_state                               : messenger_state_t := (null, null);
-
+    variable id : id_t;
   begin
     test_runner_setup(runner, runner_cfg);
 
     while test_suite loop
       reset_messenger;
       self := new_actor("test runner");
 
       -- Create
       if run("Test that named actors can be created") then
         n_actors := num_of_actors;
         actor    := new_actor("actor");
         check(actor /= null_actor, "Failed to create named actor");
         check_equal(name(actor), "actor");
+        check(get_id(actor) = get_id("actor"));
+        check_equal(num_of_actors, n_actors + 1, "Expected one extra actor");
+        check(new_actor("other actor").p_id_number /= new_actor("another actor").p_id_number, "Failed to create unique actors");
+        check_equal(num_of_actors, n_actors + 3, "Expected two extra actors");
+
+      elsif run("Test that actors can be created from identities") then
+        n_actors := num_of_actors;
+        id := get_id("actor");
+        actor := new_actor(id);
+        check(actor /= null_actor, "Failed to create actor from identity");
+        check_equal(name(actor), "actor");
+        check(get_id(actor) = id);
         check_equal(num_of_actors, n_actors + 1, "Expected one extra actor");
-        check(new_actor("other actor").id /= new_actor("another actor").id, "Failed to create unique actors");
+        check(new_actor(get_id("other actor")).p_id_number /= new_actor(get_id("another actor")).p_id_number, "Failed to create unique actors");
         check_equal(num_of_actors, n_actors + 3, "Expected two extra actors");
+
       elsif run("Test that no name actors can be created") then
         actor := new_actor;
         check(actor /= null_actor, "Failed to create no name actor");
-        check_equal(name(actor), "");
-      elsif run("Test that the null actor has no name") then
+        check_equal(name(actor)(1 to 7), "_actor_");
+        check(get_id(actor) /= null_id);
+
+      elsif run("Test that null_id actors can be created") then
+        actor := new_actor(null_id);
+        check(actor /= null_actor, "Failed to create no name actor");
+        check_equal(name(actor)(1 to 7), "_actor_");
+        check(get_id(actor) /= null_id);
+
+      elsif run("Test that the null actor has no name and identity") then
         check_equal(name(null_actor), "");
-      elsif run("Test that two actors of the same name cannot be created") then
+        check(get_id(actor) = null_id);
+
+      elsif run("Test that two actors with the same name/identity cannot be created") then
         actor := new_actor("actor2");
         mock(com_logger);
         actor := new_actor("actor2");
         check_only_log(com_logger, "DUPLICATE ACTOR NAME ERROR.", failure);
         unmock(com_logger);
-      elsif run("Test that multiple no-name actors can be created") then
+
+        actor := new_actor(get_id("actor3"));
+        mock(com_logger);
+        actor := new_actor(get_id("actor3"));
+        check_only_log(com_logger, "DUPLICATE ACTOR NAME ERROR.", failure);
+        unmock(com_logger);
+
+      elsif run("Test that no actor can be created for root_id") then
+        mock(com_logger);
+        actor := new_actor(root_id);
+        check_only_log(com_logger, "NEW ACTOR FROM ROOT ID ERROR.", failure);
+        unmock(com_logger);
+
+      elsif run("Test that multiple no-name actors can be created by name") then
         n_actors := num_of_actors;
         actor    := new_actor;
         actor2   := new_actor;
-        check(actor.id /= actor2.id, "The two actors must have different identities");
+        check(actor.p_id_number /= actor2.p_id_number, "The two actors must have different identities");
+        check_equal(num_of_actors, n_actors + 2);
+        check_equal(num_of_deferred_creations, 0);
+
+      elsif run("Test that multiple no-name actors can be created by id") then
+        n_actors := num_of_actors;
+        actor    := new_actor(null_id);
+        actor2   := new_actor(null_id);
+        check(actor.p_id_number /= actor2.p_id_number, "The two actors must have different identities");
         check_equal(num_of_actors, n_actors + 2);
         check_equal(num_of_deferred_creations, 0);
 
       -- Find
-      elsif run("Test that a created actor can be found") then
+      elsif run("Test that a created actor can be found by name") then
         actor := new_actor("actor to be found");
         check(find("actor to be found", false) /= null_actor, "Failed to find created actor");
         check_equal(num_of_deferred_creations, 0, "Expected no deferred creations");
         check_false(is_deferred(actor));
-      elsif run("Test that an actor not created is found and its creation is deferred") then
+
+      elsif run("Test that a created actor can be found by id") then
+        id := get_id("actor to be found");
+        actor := new_actor(id);
+        check(find(id, false) /= null_actor, "Failed to find created actor");
+        check_equal(num_of_deferred_creations, 0, "Expected no deferred creations");
+        check_false(is_deferred(actor));
+
+      elsif run("Test that an actor not created is found by name and its creation is deferred") then
         check_equal(num_of_deferred_creations, 0, "Expected no deferred creations");
         actor := find("actor with deferred creation");
         check(actor /= null_actor, "Failed to find actor with deferred creation");
         check_equal(num_of_deferred_creations, 1, "Expected one deferred creations");
         check(is_deferred(actor));
-      elsif run("Test that deferred creation can be suppressed when an actor is not found") then
+
+      elsif run("Test that an actor not created is found by id and its creation is deferred") then
+        check_equal(num_of_deferred_creations, 0, "Expected no deferred creations");
+        actor := find(get_id("actor with deferred creation"));
+        check(actor /= null_actor, "Failed to find actor with deferred creation");
+        check_equal(num_of_deferred_creations, 1, "Expected one deferred creations");
+        check(is_deferred(actor));
+
+      elsif run("Test that deferred creation can be suppressed when an actor is not found by name") then
         actor  := new_actor("actor");
         actor2 := find("actor with deferred creation", false);
         check(actor2 = null_actor, "Didn't expect to find any actor");
         check_equal(num_of_deferred_creations, 0, "Expected no deferred creations");
-      elsif run("Test that a created actor get the correct mailbox size") then
+
+      elsif run("Test that deferred creation can be suppressed when an actor is not found by id") then
+        actor  := new_actor("actor");
+        actor2 := find(get_id("actor with deferred creation"), false);
+        check(actor2 = null_actor, "Didn't expect to find any actor");
+        check_equal(num_of_deferred_creations, 0, "Expected no deferred creations");
+
+      elsif run("Test that a created actor by name gets the correct mailbox size") then
         actor := new_actor("actor with max inbox");
         check_equal(mailbox_size(actor), positive'high, result("for inbox size"));
         check_equal(mailbox_size(actor, outbox), positive'high, result("for outbox size"));
 
         actor2 := new_actor("actor with bounded inbox", 23, 17);
         check_equal(mailbox_size(actor2), 23, result("for inbox size"));
         check_equal(mailbox_size(actor2, outbox), 17, result("for outbox size"));
@@ -126,15 +193,30 @@
 
         check_equal(mailbox_size(find("actor to be created")), 1, result("for inbox size"));
         check_equal(mailbox_size(find("actor to be created"), outbox), positive'high, result("for outbox size"));
 
         check_equal(mailbox_size(new_actor("actor to be created", 42, 99)), 42, result("for inbox size"));
         check_equal(mailbox_size(find("actor to be created"), outbox), 99, result("for outbox size"));
 
-      elsif run("Test that mailboxes can be resize") then
+      elsif run("Test that a created actor by id gets the correct mailbox size") then
+        actor := new_actor(get_id("actor with max inbox"));
+        check_equal(mailbox_size(actor), positive'high, result("for inbox size"));
+        check_equal(mailbox_size(actor, outbox), positive'high, result("for outbox size"));
+
+        actor2 := new_actor(get_id("actor with bounded inbox"), 23, 17);
+        check_equal(mailbox_size(actor2), 23, result("for inbox size"));
+        check_equal(mailbox_size(actor2, outbox), 17, result("for outbox size"));
+
+        check_equal(mailbox_size(find(get_id("actor to be created"))), 1, result("for inbox size"));
+        check_equal(mailbox_size(find(get_id("actor to be created")), outbox), positive'high, result("for outbox size"));
+
+        check_equal(mailbox_size(new_actor(get_id("actor to be created"), 42, 99)), 42, result("for inbox size"));
+        check_equal(mailbox_size(find(get_id("actor to be created")), outbox), 99, result("for outbox size"));
+
+      elsif run("Test that mailboxes can be resized") then
         actor := new_actor("actor with max inbox");
 
         resize_mailbox(actor, 17);
         check_equal(mailbox_size(actor), 17, result("for inbox size"));
         check_equal(mailbox_size(actor, outbox), positive'high, result("for outbox size"));
 
         resize_mailbox(actor, 23, outbox);
@@ -166,31 +248,45 @@
 
       elsif run("Test that no-name actors can't be found") then
         actor  := new_actor;
         actor2 := new_actor;
         check(find("") = null_actor, "Must not find a no-name actor");
         check_equal(num_of_deferred_creations, 0);
 
+      elsif run("Test that null_id actors can't be found") then
+        actor  := new_actor(null_id);
+        actor2 := new_actor(null_id);
+        check(find(null_id) = null_actor, "Must not find a null_id actor");
+        check_equal(num_of_deferred_creations, 0);
+
+      elsif run("Test that root_id actors can't be found") then
+        actor  := new_actor(null_id);
+        actor2 := new_actor(null_id);
+        check(find(root_id) = null_actor, "Must not find a root_id actor");
+        check_equal(num_of_deferred_creations, 0);
+
       -- Destroy
       elsif run("Test that a created actor can be destroyed") then
         actor    := new_actor("actor to destroy");
         actor2   := new_actor("actor to keep");
         n_actors := num_of_actors;
         destroy(actor);
         check(num_of_actors = n_actors - 1, "Expected one less actor");
         check(actor = null_actor, "Destroyed actor should be nullified");
         check(find("actor to destroy", false) = null_actor, "A destroyed actor should not be found");
         check(find("actor to keep", false) /= null_actor,
               "Actors other than the one destroyed must not be affected");
+
       elsif run("Test that a non-existing actor cannot be destroyed") then
         actor := null_actor;
         mock(com_logger);
         destroy(actor);
         check_only_log(com_logger, "UNKNOWN ACTOR ERROR.", failure);
         unmock(com_logger);
+
       elsif run("Test that all actors can be destroyed") then
         reset_messenger;
         actor  := new_actor("actor to destroy");
         actor2 := new_actor("actor to destroy 2");
         check(num_of_actors = 2, "Expected two actors");
         reset_messenger;
         check(num_of_actors = 0, "Failed to destroy all actors");
@@ -262,115 +358,139 @@
 
       -- Send and receive
       elsif run("Test that data ownership is lost at send") then
         msg := new_msg;
         push_string(msg, "hello");
         send(net, self, msg);
         check(msg.data = null_queue);
+
       elsif run("Test that an actor can send a message to another actor") then
         start_receiver <= true;
         wait for 1 ns;
         my_receiver    := find("my_receiver");
         msg            := new_msg(sender => self);
         push_string(msg, "hello world");
         send(net, my_receiver, msg);
         check(msg.sender = self);
         check(msg.receiver = my_receiver);
         wait until hello_world_received for 1 ns;
         check(hello_world_received, "Expected ""hello world"" to be received at the server");
+
       elsif run("Test that an actor can send a reply to a message from an a priori unknown actor") then
         start_server <= true;
         wait for 1 ns;
         server       := find("server");
         request_msg  := new_msg(sender => self);
         push_string(request_msg, "request");
         send(net, server, request_msg);
         receive(net, self, reply_msg);
         check(reply_msg.status = ok, "Expected no receive problems");
         check_equal(pop_string(reply_msg), "request acknowledge");
+
       elsif run("Test that an actor can send a message to itself") then
         msg := new_msg;
         push_string(msg, "hello");
         send(net, self, msg);
         receive(net, self, msg2);
         check(msg2.status = ok, "Expected no receive problems");
         check_equal(pop_string(msg2), "hello");
+
       elsif run("Test that no-name actors can communicate") then
         actor := new_actor;
         msg   := new_msg;
         push_string(msg, "hello");
         send(net, actor, msg);
         receive(net, actor, msg2);
         check_equal(pop_string(msg2), "hello");
+
+      elsif run("Test that many back-to-back messages don't hit the simulator's delta cycle limit") then
+        actor := new_actor;
+        for iter in 1 to 10000 loop
+          msg   := new_msg;
+          push(msg, iter);
+          send(net, actor, msg);
+        end loop;
+        for iter in 1 to 10000 loop
+          receive(net, actor, msg2);
+          check_equal(pop_integer(msg2), iter);
+        end loop;
+
       elsif run("Test that an actor can poll for incoming messages") then
         wait_for_message(net, self, status, 0 ns);
         check(status = timeout, "Expected timeout");
         msg := new_msg(sender => self);
         push_string(msg, "hello again");
         send(net, self, msg);
         wait_for_message(net, self, status, 0 ns);
         check(status = ok, "Expected ok status");
         get_message(net, self, msg2);
         check(msg2.status = ok, "Expected no problems with receive");
         check_equal(pop_string(msg2), "hello again");
         check(msg2.sender = self, "Expected message from myself");
+
       elsif run("Test that sending to a non-existing actor results in an error") then
         msg := new_msg;
         push_string(msg, "hello");
         mock(com_logger);
         send(net, null_actor, msg);
         check_only_log(com_logger, "UNKNOWN RECEIVER ERROR.", failure);
         unmock(com_logger);
+
       elsif run("Test that an actor can send to an actor with deferred creation") then
         actor := find("deferred actor");
         msg   := new_msg;
         push_string(msg, "hello actor to be created");
         send(net, actor, msg);
         actor := new_actor("deferred actor");
         receive(net, actor, msg2);
         check(msg2.status = ok, "Expected no problems with receive");
         check_equal(pop_string(msg2), "hello actor to be created");
+
       elsif run("Test that receiving from an actor with deferred creation results in an error") then
         actor := find("deferred actor");
         mock(com_logger);
         receive(net, actor, msg);
         check_log(com_logger, "DEFERRED RECEIVER ERROR.", failure);
         check_only_log(com_logger, "DEFERRED RECEIVER ERROR.", failure);
         unmock(com_logger);
+
       elsif run("Test that empty messages can be sent") then
         msg := new_msg;
         send(net, self, msg);
         receive(net, self, msg2);
         check(msg2.status = ok, "Expected no problems with receive");
         check_equal(length(msg2.data), 0);
+
       elsif run("Test that each sent message gets an increasing message number") then
         msg := new_msg;
         send(net, self, msg);
         check(msg.id = 1, "Expected first receipt id to be 1");
         msg := new_msg;
         send(net, self, msg);
         check(msg.id = 2, "Expected first receipt id to be 2");
         receive(net, self, msg2);
         check(msg2.id = 1, "Expected first message id to be 1");
         receive(net, self, msg2);
         check(msg2.id = 2, "Expected first message id to be 2");
+
       elsif run("Test that each published message gets an increasing message number") then
         for i in actor_vec'range loop
           actor_vec(i) := new_actor;
           subscribe(actor_vec(i), self);
         end loop;
 
         for j in 1 to 3 loop
           msg := new_msg;
           publish(net, self, msg);
           for i in actor_vec'range loop
             receive(net, actor_vec(i), msg);
             check_equal(msg.id, j);
           end loop;
         end loop;
+
       elsif run("Test that a limited-inbox receiver can receive as expected without blocking") then
         start_limited_inbox <= true;
         actor               := find("limited inbox");
         t_start             := now;
         msg                 := new_msg;
         push_string(msg, "First message");
         send(net, actor, msg);
@@ -386,14 +506,15 @@
         msg                 := new_msg;
         push_string(msg, "Third message");
         send(net, actor, msg, 11 ns);
         t_stop              := now;
         check_equal(t_stop - t_start, 10 ns, "Expected a 10 ns blocking period on third message");
 
         wait until limited_inbox_actor_done;
+
       elsif run("Test that sending to a limited-inbox receiver times out as expected") then
         start_limited_inbox <= true;
         actor               := find("limited inbox");
         msg                 := new_msg;
         push_string(msg, "First message");
         send(net, actor, msg);
         msg                 := new_msg;
@@ -402,14 +523,15 @@
         msg                 := new_msg;
         push_string(msg, "Third message");
         mock(com_logger);
         send(net, actor, msg, 9 ns);
         check_log(com_logger, "FULL INBOX ERROR.", failure);
         check_only_log(com_logger, "[3:- - -> limited inbox (-)] => limited inbox inbox", trace);
         unmock(com_logger);
+
       elsif run("Test that messages can be awaited from several actors") then
         actor  := new_actor;
         actor2 := new_actor;
         msg    := new_msg;
         push_string(msg, "To actor");
         send(net, actor, msg);
         wait_for_message(net, actor_vec_t'(actor, actor2), status);
@@ -423,56 +545,60 @@
         send(net, actor2, msg);
         wait_for_message(net, actor_vec_t'(actor, actor2), status);
         check(status = ok, "Expected ok status");
         check_true(has_message(actor2));
         check_false(has_message(actor));
         get_message(net, actor2, msg);
         check_equal(pop_string(msg), "To actor2");
+
       elsif run("Test sending to several actors") then
         actor_vec := (new_actor, new_actor, new_actor);
         for n in 0 to 2 loop
           msg := new_msg;
           push_string(msg, "hello");
           send(net, actor_vec(1 to n), msg);
           check(msg.data = null_queue);
           for i in 1 to n loop
             receive(net, actor_vec(i), msg, 0 ns);
             check_equal(pop_string(msg), "hello");
           end loop;
         end loop;
+
       elsif run("Test sending to several actors with timeout") then
         actor_vec := (new_actor(inbox_size => 1), new_actor(inbox_size => 1), new_actor(inbox_size => 1));
         msg       := new_msg;
         push_string(msg, "hello");
         send(net, actor_vec, msg);
         mock(com_logger);
         msg       := new_msg;
         push_string(msg, "hello");
         t_start   := now;
         send(net, actor_vec, msg, 10 ns);
         check_equal(now - t_start, 10 ns);
         check_log(com_logger, "FULL INBOX ERROR.", failure);
-        check_log(com_logger, "[4:- - ->  (-)] =>  inbox", trace);
+        check_log(com_logger, "[4:- - -> _actor_" & to_string(actor_vec(0).p_id_number) & " (-)] => _actor_" & to_string(actor_vec(0).p_id_number) & " inbox", trace);
         check_log(com_logger, "FULL INBOX ERROR.", failure);
-        check_log(com_logger, "[5:- - ->  (-)] =>  inbox", trace);
+        check_log(com_logger, "[5:- - -> _actor_" & to_string(actor_vec(1).p_id_number) & " (-)] => _actor_" & to_string(actor_vec(1).p_id_number) & " inbox", trace);
         check_log(com_logger, "FULL INBOX ERROR.", failure);
-        check_log(com_logger, "[6:- - ->  (-)] =>  inbox", trace);
+        check_log(com_logger, "[6:- - -> _actor_" & to_string(actor_vec(2).p_id_number) & " (-)] => _actor_" & to_string(actor_vec(2).p_id_number) & " inbox", trace);
         unmock(com_logger);
+
       elsif run("Test receiving from several actors") then
         for i in 0 to 2 loop
           actor_vec(i) := new_actor;
           subscribe(actor_vec(i), find("publisher " & to_string(i)));
         end loop;
         start_publishers <= true;
         receive(net, actor_vec(0 to 0), msg);
         check_equal(name(msg.sender), pop_string(msg));
         for i in 1 to 2 loop
           receive(net, actor_vec(1 to 2), msg);
           check_equal(name(msg.sender), pop_string(msg));
         end loop;
+
       elsif run("Test that the sender and the receiver of a message can be retrieved") then
         actor  := new_actor;
         actor2 := new_actor;
         msg    := new_msg(sender => actor2);
         push_string(msg, "To actor");
         send(net, actor, msg);
         receive(net, actor, msg);
@@ -480,14 +606,15 @@
         check(receiver(msg) = actor);
         msg    := new_msg;
         push_string(msg, "To actor");
         send(net, actor, msg);
         receive(net, actor, msg);
         check(sender(msg) = null_actor);
         check(receiver(msg) = actor);
+
       elsif run("Test that get_message will wake up sender blocking on full inbox") then
         actor         := new_actor("actor", 1);
         start_server6 <= true;
         wait for 1 ns;
         server        := find("server6");
 
         request_msg := new_msg(sender => actor);
@@ -535,14 +662,15 @@
         msg               := new_msg;
         push_string(msg, "hello subscriber");
         publish(net, publisher, msg);
         check(msg.sender = publisher);
         check(msg.receiver = null_actor);
         wait until hello_subscriber_received = "11" for 1 ns;
         check(hello_subscriber_received = "11", "Expected ""hello subscribers"" to be received at the subscribers");
+
       elsif run("Test that subscribers receive messages sent on outbound subscription") then
         my_sender   := new_actor;
         my_receiver := new_actor;
         subscribe(self, my_sender, outbound);
 
         msg := new_msg(sender => my_sender);
         push_string(msg, "hello");
@@ -575,24 +703,26 @@
         push_string(msg, "hello");
         send(net, self, msg);
 
         receive(net, self, msg2, 0 ns);
         check(msg2.receiver = self);
         wait_for_message(net, self, status, 0 ns);
         check(status = timeout, "Expected only one message");
+
       elsif run("Test that actors don't get send messages on a publish subscription") then
         publisher := new_actor("publisher");
         subscribe(self, publisher);
 
         msg := new_msg(sender => publisher);
         push_string(msg, "hello");
         send(net, publisher, msg);
 
         wait_for_message(net, self, status, 0 ns);
         check(status = timeout, "Expected no message");
+
       elsif run("Test that actors can subscribe to inbound traffic") then
         my_receiver := new_actor;
         subscribe(self, my_receiver, inbound);
 
         msg := new_msg;
         push_string(msg, "hello");
         send(net, my_receiver, msg);
@@ -617,14 +747,15 @@
         actor := new_actor("actor");
         msg   := new_msg(sender => my_receiver);
         push_string(msg, "hello");
 
         send(net, actor, msg);
         wait_for_message(net, self, status, 0 ns);
         check(status = timeout, "Expected no message");
+
       elsif run("Test request/reply with actor having inbound subscribers") then
         subscriber    := new_actor("subscriber");
         start_server5 <= true;
         wait for 1 ns;
         server        := find("server5");
         subscribe(subscriber, server, inbound);
 
@@ -633,14 +764,15 @@
         send(net, server, request_msg);
 
         receive_reply(net, request_msg, reply_msg, 100 ns);
         check_equal(pop_string(reply_msg), "reply");
 
         receive(net, subscriber, reply_msg, 0 ns);
         check_equal(pop_string(reply_msg), "request");
+
       elsif run("Test chained subscribers") then
         my_sender   := new_actor;
         my_receiver := new_actor;
         subscriber  := new_actor;
         subscribe(self, my_sender, outbound);
         subscribe(subscriber, self, inbound);
 
@@ -688,31 +820,34 @@
         check_equal(pop_string(msg), "hello subscriber");
         unsubscribe(self, self, published);
         msg := new_msg;
         push_string(msg, "hello subscriber");
         publish(net, self, msg);
         wait_for_message(net, self, status, 0 ns);
         check(status = timeout, "Expected no message");
+
       elsif run("Test that a destroyed subscriber is not addressed by the publisher") then
         subscriber := new_actor("subscriber");
         subscribe(subscriber, self);
         msg        := new_msg;
         push_string(msg, "hello subscriber");
         publish(net, self, msg);
         receive(net, subscriber, msg, 0 ns);
         check_equal(pop_string(msg), "hello subscriber");
         destroy(subscriber);
         push_string(msg, "hello subscriber");
         publish(net, self, msg);
+
       elsif run("Test that an actor can only subscribe once to the same publisher") then
         subscribe(self, self);
         mock(com_logger);
         subscribe(self, self);
         check_only_log(com_logger, "ALREADY A SUBSCRIBER ERROR.", failure);
         unmock(com_logger);
+
       elsif run("Test that publishing to subscribers with full inboxes results is an error") then
         start_limited_inbox_subscriber <= true;
         wait for 1 ns;
         msg                            := new_msg;
         push_string(msg, "hello subscriber");
         publish(net, self, msg);
         msg                            := new_msg;
@@ -720,14 +855,15 @@
         mock(com_logger);
         publish(net, self, msg, 8 ns);
         check_log(com_logger, "FULL INBOX ERROR.", failure);
         check_only_log(com_logger,
                        "[2:- test runner -> limited inbox subscriber (-)] => limited inbox subscriber inbox",
                        trace);
         unmock(com_logger);
+
       elsif run("Test that publishing to subscribers with full inboxes results passes if waiting") then
         start_limited_inbox_subscriber <= true;
         wait for 1 ns;
         msg                            := new_msg;
         push_string(msg, "hello subscriber");
         publish(net, self, msg);
         msg                            := new_msg;
@@ -777,14 +913,15 @@
         request(net, server, request_msg, ack);
         check(ack, "Expected positive acknowledgement");
 
         request_msg := new_msg(sender => self);
         push_string(request_msg, "request3");
         request(net, server, request_msg, ack);
         check_false(ack, "Expected negative acknowledgement");
+
       elsif run("Test that waiting and getting a reply with timeout works") then
         start_server4 <= true;
         server        := find("server4");
 
         t_start     := now;
         request_msg := new_msg(sender => self);
         push_string(request_msg, "request1");
@@ -811,14 +948,15 @@
         t_start     := now;
         request_msg := new_msg;
         push_string(request_msg, "request4");
         send(net, server, request_msg);
         wait_for_reply(net, request_msg, status);
         get_reply(net, request_msg, reply_msg);
         check_equal(pop_string(reply_msg), "reply4");
+
       elsif run("Test waiting and getting a reply out-of-order") then
         start_server2 <= true;
         server        := find("server2");
 
         request_msg  := new_msg(sender => self);
         push_string(request_msg, "request1");
         send(net, server, request_msg);
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/test/tb_com_codec.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/test/tb_com_codec.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/test/tb_com_deprecated.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/test/tb_com_deprecated.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/com/test/tb_com_msg_building.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/com/test/tb_com_msg_building.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 library vunit_lib;
 context vunit_lib.vunit_context;
 context vunit_lib.com_context;
 use vunit_lib.queue_pkg.all;
 use vunit_lib.integer_vector_ptr_pkg.all;
 use vunit_lib.integer_array_pkg.all;
+use vunit_lib.dict_pkg.all;
 
 library ieee;
 use ieee.std_logic_1164.all;
 use ieee.numeric_std.all;
 use ieee.numeric_bit.all;
 use ieee.math_complex.all;
 use ieee.fixed_pkg.all;
@@ -35,14 +36,15 @@
     variable msg, msg2, msg2_copy : msg_t;
     variable queue, queue_copy : queue_t;
     variable bv : bit_vector(0 to 5);
     variable sulv : std_ulogic_vector(0 to 5);
     variable boolv : boolean_vector(0 to 1);
     variable integer_vector_ptr, integer_vector_ptr_copy : integer_vector_ptr_t;
     variable integer_array, integer_array_copy : integer_array_t;
+    variable dict : dict_t;
 
     constant my_msg_type : msg_type_t := new_msg_type("my msg type");
   begin
     test_runner_setup(runner, runner_cfg);
 
     while test_suite loop
       if run("Test that a message can be created") then
@@ -264,14 +266,21 @@
       elsif run("Test push and pop of integer_array_t") then
         msg := new_msg;
         integer_array := new_3d(1, 2, 3, 4);
         integer_array_copy := integer_array;
         push_integer_array_t_ref(msg, integer_array);
         check(integer_array = null_integer_array);
         check(pop_integer_array_t_ref(msg) = integer_array_copy);
+      elsif run("Test push and pop of dict_t") then
+        msg := new_msg;
+        dict := new_dict;
+        set_integer(dict, "key", 17);
+        push_dict_t_ref(msg, dict);
+        check(dict = null_dict);
+        check_equal(get_integer(pop_dict_t_ref(msg), "key"), 17);
       elsif run("Test push and pop of msg_t") then
         msg := new_msg;
         msg2 := new_msg;
         msg2_copy := msg2;
         push(msg, msg2);
         assert msg2 = null_msg report "Ownership was transfered";
         check(pop(msg) = msg2_copy);
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/core/src/core_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/core/src/core_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/core/src/stop_body_2008p.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/core/src/stop_body_2008p.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/api/external_integer_vector_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/api/external_integer_vector_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/api/external_string_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/api/external_string_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/byte_vector_ptr_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/byte_vector_ptr_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/codec-2008p.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/codec-2008p.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/codec.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/codec.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/codec_builder-2008p.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/codec_builder-2008p.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/codec_builder.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/codec_builder.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/data_types_context.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/data_types_context.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_array_pkg-body.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_array_pkg-body.vhd`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 -- This Source Code Form is subject to the terms of the Mozilla Public
 -- License, v. 2.0. If a copy of the MPL was not distributed with this file,
 -- You can obtain one at http://mozilla.org/MPL/2.0/.
 --
 -- Copyright (c) 2014-2023, Lars Asplund lars.anders.asplund@gmail.com
 
 use std.textio.all;
+use work.codec_pkg.all;
+use work.codec_builder_pkg.all;
 
 package body integer_array_pkg is
   type binary_file_t is file of character;
 
   procedure read_byte (
     file fread      : binary_file_t;
     variable result : out integer
@@ -449,8 +451,45 @@
                    bytes_per_word => (arr.bit_width+7)/8,
                    is_signed => arr.is_signed);
       append(arr, tmp);
     end loop;
     file_close(fread);
     return arr;
   end;
+
+  function encode (
+    data : integer_array_t
+  ) return string is
+  begin
+    return encode(data.length) & encode(data.width) & encode(data.height) &
+    encode(data.depth) & encode(data.bit_width) & encode(data.is_signed) &
+    encode(data.lower_limit) & encode(data.upper_limit) & encode(data.data);
+  end;
+
+  function decode (
+    code : string
+  ) return integer_array_t is
+    variable result : integer_array_t;
+    variable index : positive := code'left;
+  begin
+    decode(code, index, result);
+
+    return result;
+  end;
+
+  procedure decode (
+    constant code   : string;
+    variable index  : inout positive;
+    variable result : out integer_array_t
+  ) is
+  begin
+    decode(code, index, result.length);
+    decode(code, index, result.width);
+    decode(code, index, result.height);
+    decode(code, index, result.depth);
+    decode(code, index, result.bit_width);
+    decode(code, index, result.is_signed);
+    decode(code, index, result.lower_limit);
+    decode(code, index, result.upper_limit);
+    decode(code, index, result.data);
+  end;
 end package body;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_array_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_array_pkg.vhd`

 * *Files 7% similar despite different names*

```diff
@@ -174,8 +174,22 @@
     file_name : string
   );
 
   procedure save_raw (
     arr       : integer_array_t;
     file_name : string
   );
+
+  function encode (
+    data : integer_array_t
+  ) return string;
+
+  function decode (
+    code : string
+  ) return integer_array_t;
+
+  procedure decode (
+    constant code   : string;
+    variable index  : inout positive;
+    variable result : out integer_array_t
+  );
 end package;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_vector_ptr_pkg-body-2002p.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_vector_ptr_pkg-body-2002p.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_vector_ptr_pkg-body-93.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_vector_ptr_pkg-body-93.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_vector_ptr_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_vector_ptr_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/integer_vector_ptr_pool_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/integer_vector_ptr_pool_pkg.vhd`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,21 @@
 use ieee.std_logic_1164.all;
 
 use work.integer_vector_ptr_pkg.all;
 use work.queue_pkg.all;
 
 package integer_vector_ptr_pool_pkg is
   type integer_vector_ptr_pool_t is record
-    ptrs : queue_t;
+    p_data : integer_vector_ptr_t;
   end record;
-  constant null_integer_vector_ptr_pool : integer_vector_ptr_pool_t := (others => null_queue);
+  constant pool_idx : natural := 0;
+  constant length_idx : natural := 1;
+  constant max_length_idx : natural := 2;
+
+  constant null_integer_vector_ptr_pool : integer_vector_ptr_pool_t := (p_data => null_integer_vector_ptr);
 
   impure function new_integer_vector_ptr_pool
   return integer_vector_ptr_pool_t;
 
   impure function new_integer_vector_ptr (
     pool       : integer_vector_ptr_pool_t;
     min_length : natural := 0
@@ -27,43 +31,64 @@
   procedure recycle (
     pool         : integer_vector_ptr_pool_t;
     variable ptr : inout integer_vector_ptr_t
   );
 end package;
 
 package body integer_vector_ptr_pool_pkg is
+  constant pool_size_increment : positive := 2 ** 16;
+
   impure function new_integer_vector_ptr_pool
-  return integer_vector_ptr_pool_t is begin
-    return (ptrs => new_queue);
+  return integer_vector_ptr_pool_t is
+    variable pool : integer_vector_ptr_pool_t;
+  begin
+    pool.p_data := new_integer_vector_ptr(3);
+    set(pool.p_data, pool_idx, to_integer(new_integer_vector_ptr(pool_size_increment)));
+    set(pool.p_data, length_idx, 0);
+    set(pool.p_data, max_length_idx, pool_size_increment);
+
+    return pool;
   end;
 
   impure function new_integer_vector_ptr (
     pool       : integer_vector_ptr_pool_t;
     min_length : natural := 0
   ) return integer_vector_ptr_t is
     variable ptr : integer_vector_ptr_t;
+    constant len : natural := get(pool.p_data, length_idx);
   begin
-    if length(pool.ptrs) > 0 then
+    if len > 0 then
       -- Reuse
-      ptr := pop_integer_vector_ptr_ref(pool.ptrs);
+      ptr.ref := get(to_integer_vector_ptr(get(pool.p_data, pool_idx)), len - 1);
+      set(pool.p_data, length_idx, len - 1);
       if length(ptr) < min_length then
         reallocate(ptr, min_length);
       end if;
     else
       -- Allocate new
       ptr := new_integer_vector_ptr(min_length);
     end if;
     return ptr;
   end;
 
   procedure recycle (
     pool         : integer_vector_ptr_pool_t;
     variable ptr : inout integer_vector_ptr_t
-  ) is begin
+  ) is
+    constant len : natural := get(pool.p_data, length_idx);
+    constant max_len : natural := get(pool.p_data, max_length_idx);
+  begin
     if ptr = null_ptr then
       return;
     end if;
-    push_integer_vector_ptr_ref(pool.ptrs, ptr);
+
+    if len = max_len then
+      resize(to_integer_vector_ptr(get(pool.p_data, pool_idx)), max_len + pool_size_increment);
+      set(pool.p_data, max_length_idx, max_len + pool_size_increment);
+    end if;
+
+    set(to_integer_vector_ptr(get(pool.p_data, pool_idx)), len, ptr.ref);
+    set(pool.p_data, length_idx, len + 1);
     ptr := null_ptr;
   end;
 
 end package body;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/queue_pkg-2008p.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/queue_pkg-2008p.vhd`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 library ieee;
 use ieee.fixed_pkg.all;
 use ieee.float_pkg.all;
 
 use work.queue_pkg.all;
 use work.codec_2008p_pkg.all;
 use work.codec_builder_2008p_pkg.all;
+use work.data_types_private_pkg.all;
 
 package queue_2008p_pkg is
   procedure push (
     queue : queue_t;
     value : boolean_vector
   );
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/queue_pkg-body.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/queue_pkg-body.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -116,34 +116,34 @@
     data := get(queue.data, 1 + head);
     set(queue.p_meta, head_idx, head + 1);
     return data;
   end;
 
   procedure push_type (
     queue        : queue_t;
-    element_type : queue_element_type_t
+    element_type : data_type_t
   ) is begin
-    unsafe_push(queue, character'val(queue_element_type_t'pos(element_type)));
+    unsafe_push(queue, character'val(data_type_t'pos(element_type)));
   end;
 
   impure function pop_type (
     queue : queue_t
-  ) return queue_element_type_t is begin
-    return queue_element_type_t'val(character'pos(unsafe_pop(queue)));
+  ) return data_type_t is begin
+    return data_type_t'val(character'pos(unsafe_pop(queue)));
   end;
 
   procedure check_type (
     queue        : queue_t;
-    element_type : queue_element_type_t
+    element_type : data_type_t
   ) is
-    constant popped_type : queue_element_type_t := pop_type(queue);
+    constant popped_type : data_type_t := pop_type(queue);
   begin
     if popped_type /= element_type then
-      report "Got queue element of type " & queue_element_type_t'image(popped_type) &
-        ", expected " & queue_element_type_t'image(element_type) & "." severity error;
+      report "Got queue element of type " & to_string(popped_type) &
+        ", expected " & to_string(element_type) & "." severity error;
     end if;
   end;
 
   procedure push (
     queue : queue_t;
     value : character
   ) is begin
@@ -372,22 +372,22 @@
     return decode(pop_variable_string(queue));
   end;
 
   procedure push (
     queue : queue_t;
     value : std_ulogic_vector
   ) is begin
-    push_type(queue, vhdl_std_ulogic_vector);
+    push_type(queue, ieee_std_ulogic_vector);
     push_variable_string(queue, encode(value));
   end;
 
   impure function pop (
     queue : queue_t
   ) return std_ulogic_vector is begin
-    check_type(queue, vhdl_std_ulogic_vector);
+    check_type(queue, ieee_std_ulogic_vector);
     return decode(pop_variable_string(queue));
   end;
 
   procedure push (
     queue : queue_t;
     value : complex
   ) is begin
@@ -597,8 +597,9 @@
       bit_width   => unsafe_pop(queue),
       is_signed   => unsafe_pop(queue),
       lower_limit => unsafe_pop(queue),
       upper_limit => unsafe_pop(queue),
       data        => unsafe_pop(queue)
     );
   end;
+
 end package body;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/queue_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/queue_pkg.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 use ieee.std_logic_1164.all;
 use ieee.math_complex.all;
 use ieee.numeric_bit.all;
 use ieee.numeric_std.all;
 use work.integer_vector_ptr_pkg.all;
 use work.string_ptr_pkg.all;
 use work.integer_array_pkg.all;
+use work.data_types_private_pkg.all;
 
 package queue_pkg is
   type queue_t is record
     p_meta : integer_vector_ptr_t;
     data   : string_ptr_t;
   end record;
   type queue_vec_t is array(integer range <>) of queue_t;
@@ -322,24 +323,14 @@
   impure function pop_ref (
     queue : queue_t
   ) return integer_array_t;
 
   alias push_integer_array_t_ref is push_ref[queue_t, integer_array_t];
   alias pop_integer_array_t_ref is pop_ref[queue_t return integer_array_t];
 
-  -- Private
-  type queue_element_type_t is (
-    vhdl_character, vhdl_integer, vunit_byte, vhdl_string, vhdl_boolean, vhdl_real, vhdl_bit, ieee_std_ulogic,
-    vhdl_severity_level, vhdl_file_open_status, vhdl_file_open_kind, vhdl_bit_vector, vhdl_std_ulogic_vector,
-    ieee_complex, ieee_complex_polar, ieee_numeric_bit_unsigned, ieee_numeric_bit_signed,
-    ieee_numeric_std_unsigned, ieee_numeric_std_signed, vhdl_time, vunit_integer_vector_ptr_t,
-    vunit_string_ptr_t, vunit_queue_t, vunit_integer_array_t, vhdl_boolean_vector, vhdl_integer_vector,
-    vhdl_real_vector, vhdl_time_vector, ieee_ufixed, ieee_sfixed, ieee_float
-  );
-
   function encode (
     data : queue_t
   ) return string;
 
   function decode (
     code : string
   ) return queue_t;
@@ -351,20 +342,20 @@
   );
 
   alias encode_queue_t is encode[queue_t return string];
   alias decode_queue_t is decode[string return queue_t];
 
   procedure push_type (
     queue        : queue_t;
-    element_type : queue_element_type_t
+    element_type : data_type_t
   );
 
   procedure check_type (
     queue        : queue_t;
-    element_type : queue_element_type_t
+    element_type : data_type_t
   );
 
   procedure unsafe_push (
     queue : queue_t;
     value : character
   );
 
@@ -386,8 +377,18 @@
     value : string
   );
 
   impure function pop_fix_string (
     queue  : queue_t;
     length : natural
   ) return string;
+
+  -- Private
+  procedure unsafe_push (
+    queue : queue_t;
+    value : integer_vector_ptr_t
+  );
+
+  impure function unsafe_pop (
+    queue : queue_t
+  ) return integer_vector_ptr_t;
 end package;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/queue_pool_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/queue_pool_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/string_ptr_pkg-body-2002p.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/string_ptr_pkg-body-2002p.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/string_ptr_pkg-body-93.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/string_ptr_pkg-body-93.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/string_ptr_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/string_ptr_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/string_ptr_pool_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_string_ptr_pool.vhd`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,81 @@
 -- This Source Code Form is subject to the terms of the Mozilla Public
 -- License, v. 2.0. If a copy of the MPL was not distributed with this file,
 -- You can obtain one at http://mozilla.org/MPL/2.0/.
 --
 -- Copyright (c) 2014-2023, Lars Asplund lars.anders.asplund@gmail.com
 
-library ieee;
-use ieee.std_logic_1164.all;
+library vunit_lib;
+--context vunit_lib.vunit_context;
+use vunit_lib.check_pkg.all;
+use vunit_lib.run_pkg.all;
 
 use work.string_ptr_pkg.all;
-use work.queue_pkg.all;
+use work.string_ptr_pool_pkg.all;
 
-package string_ptr_pool_pkg is
-  type string_ptr_pool_t is record
-    ptrs : queue_t;
-  end record;
-  constant null_string_ptr_pool : string_ptr_pool_t := (others => null_queue);
-
-  impure function new_string_ptr_pool
-  return string_ptr_pool_t;
-
-  impure function new_string_ptr (
-    pool       : string_ptr_pool_t;
-    min_length : natural := 0
-  ) return string_ptr_t;
-
-  impure function new_string_ptr (
-    pool  : string_ptr_pool_t;
-    value : string
-  ) return string_ptr_t;
-
-  procedure recycle (
-    pool : string_ptr_pool_t;
-    variable ptr : inout string_ptr_t
-  );
-end package;
-
-package body string_ptr_pool_pkg is
-  impure function new_string_ptr_pool
-  return string_ptr_pool_t is begin
-    return (ptrs => new_queue);
-  end;
-
-  impure function new_string_ptr (
-    pool       : string_ptr_pool_t;
-    min_length : natural := 0
-  ) return string_ptr_t is
-    variable ptr : string_ptr_t;
+entity tb_string_ptr_pool is
+  generic(runner_cfg : string);
+end entity;
+
+architecture a of tb_string_ptr_pool is
+begin
+  main : process
+    variable pool : string_ptr_pool_t;
+    variable ptr, old_ptr, first_ptr : string_ptr_t;
   begin
-    if length(pool.ptrs) > 0 then
-      -- Reuse
-      ptr := to_string_ptr(pop(pool.ptrs));
-      if length(ptr) < min_length then
-        reallocate(ptr, min_length);
-      end if;
-    else
-      -- Allocate new
-      ptr := new_string_ptr(min_length);
-    end if;
-    return ptr;
-  end;
+    test_runner_setup(runner, runner_cfg);
 
-  impure function new_string_ptr (
-    pool  : string_ptr_pool_t;
-    value : string
-  ) return string_ptr_t is
-    variable ptr : string_ptr_t;
-  begin
-    if length(pool.ptrs) > 0 then
-      -- Reuse
-      ptr := to_string_ptr(pop(pool.ptrs));
-      reallocate(ptr, value);
-    else
-      -- Allocate new
-      ptr := new_string_ptr(value);
-    end if;
-    return ptr;
-  end;
+    if run("Test default pool is null") then
+      assert pool = null_string_ptr_pool report "Expected null pool";
 
-  procedure recycle (
-    pool : string_ptr_pool_t;
-    variable ptr : inout string_ptr_t
-  ) is begin
-    if ptr = null_string_ptr then
-      return;
+    elsif run("Test new ptr has length") then
+      pool := new_string_ptr_pool;
+      ptr := new_string_ptr(pool, 77);
+      assert ptr /= null_string_ptr report "Expected non null ptr";
+      check_equal(length(ptr), 77);
+      recycle(pool, ptr);
+
+    elsif run("Test allocate string recycled") then
+      pool := new_string_ptr_pool;
+      ptr := new_string_ptr(pool, "hello");
+      check_equal(to_string(ptr), "hello");
+      old_ptr := ptr;
+      recycle(pool, ptr);
+      ptr := new_string_ptr(pool, "foobar");
+      check_equal(to_string(ptr), "foobar");
+      assert ptr = old_ptr report "Was recycled";
+
+    elsif run("Test recycled ptr is null") then
+      pool := new_string_ptr_pool;
+      ptr := new_string_ptr(pool);
+      assert ptr /= null_string_ptr report "Expected non null ptr";
+      recycle(pool, ptr);
+      assert ptr = null_string_ptr report "Expected null ptr";
+
+    elsif run("Test ptr is recycled") then
+      pool := new_string_ptr_pool;
+      ptr := new_string_ptr(pool, 2);
+      old_ptr := ptr;
+      recycle(pool, ptr);
+      ptr := new_string_ptr(pool, 2);
+      assert ptr = old_ptr report "Was recycled";
+
+    elsif run("Test recycling beyond initial pool size") then
+      pool := new_string_ptr_pool;
+      first_ptr := new_string_ptr(pool);
+      for i in first_ptr.ref + 1 to first_ptr.ref + 1 + 2 ** 16 loop
+        ptr := new_string_ptr(pool);
+        assert ptr.ref = i;
+      end loop;
+      for i in first_ptr.ref + 1 to first_ptr.ref + 1 + 2 ** 16 loop
+        ptr.ref := i;
+        recycle(pool, ptr);
+      end loop;
+      for i in first_ptr.ref + 1 + 2 ** 16 downto first_ptr.ref + 1 loop
+        ptr := new_string_ptr(pool);
+        assert ptr.ref = i;
+      end loop;
     end if;
-    push(pool.ptrs, to_integer(ptr));
-    ptr := null_string_ptr;
-  end;
-end package body;
+
+    test_runner_cleanup(runner);
+  end process;
+end architecture;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/src/types.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/src/types.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_byte_vector_ptr.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_byte_vector_ptr.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_codec-2008p.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_codec-2008p.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_codec.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_codec.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_integer_array.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_integer_array.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_integer_vector_ptr.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_integer_vector_ptr.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_queue-2008p.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_queue-2008p.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_queue.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_queue.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_queue_pool.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_queue_pool.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/data_types/test/tb_string_ptr.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/data_types/test/tb_string_ptr.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/dictionary/src/dictionary.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/dictionary/src/dictionary.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/dictionary/test/tb_dictionary.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/dictionary/test/tb_dictionary.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/run.py` & `vunit_hdl-4.7.0/vunit/vhdl/logging/run.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/ansi_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/ansi_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/file_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/file_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/location_pkg-body-2008m.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/location_pkg-body-2008m.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/location_pkg-body-2019p.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/location_pkg-body-2019p.vhd`

 * *Files 1% similar despite different names*

```diff
@@ -22,11 +22,11 @@
       if call_path(path_offset + 1).file_line /= -1 then
         result.file_name := call_path(path_offset + 1).file_name;
         result.line_num := call_path(path_offset + 1).file_line;
         return result;
       end if;
     end if;
 
-    write(result.file_name, "");
+    swrite(result.file_name, "");
     return result;
   end;
 end package body;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/location_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/location_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/log_deprecated_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/log_deprecated_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/log_handler_pkg-body.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/log_handler_pkg-body.vhd`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 use work.ansi_pkg.all;
 use work.string_ops.upper;
 use work.file_pkg.all;
 
 package body log_handler_pkg is
 
-  constant display_handler_id : natural := 0;
-  constant next_log_handler_id : integer_vector_ptr_t := new_integer_vector_ptr(1, value => display_handler_id+1);
+  constant display_handler_id_number : natural := 0;
+  constant next_log_handler_id_number : integer_vector_ptr_t := new_integer_vector_ptr(1, value => display_handler_id_number+1);
 
-  constant id_idx : natural := 0;
+  constant id_number_idx : natural := 0;
   constant file_name_idx : natural := 1;
   constant format_idx : natural := 2;
   constant use_color_idx : natural := 3;
   constant file_id_idx : natural := 4;
   constant max_logger_name_idx : natural := 5;
   constant log_handler_length : natural := max_logger_name_idx + 1;
 
@@ -41,52 +41,52 @@
   begin
     if (file_name /= null_file_name) and (file_name /= stdout_file_name) then
       file_open_for_write(file_id, file_name);
     end if;
     set(log_handler.p_data, file_id_idx, to_integer(file_id));
   end procedure;
 
-  impure function new_log_handler(id : natural;
+  impure function new_log_handler(id_number : natural;
                                   file_name : string;
                                   format : log_format_t;
                                   use_color : boolean) return log_handler_t is
     constant log_handler : log_handler_t := (p_data => new_integer_vector_ptr(log_handler_length));
   begin
-    set(log_handler.p_data, id_idx, id);
+    set(log_handler.p_data, id_number_idx, id_number);
     set(log_handler.p_data, file_name_idx, to_integer(new_string_ptr(file_name)));
     set(log_handler.p_data, file_id_idx, to_integer(null_file_id));
     init_log_file(log_handler, file_name);
     set(log_handler.p_data, max_logger_name_idx, 0);
     set_format(log_handler, format, use_color);
     return log_handler;
   end;
 
   impure function new_log_handler(file_name : string;
                                   format : log_format_t := verbose;
                                   use_color : boolean := false) return log_handler_t is
-    constant id : natural := get(next_log_handler_id, 0);
+    constant id_number : natural := get(next_log_handler_id_number, 0);
   begin
-    set(next_log_handler_id, 0, id + 1);
-    return new_log_handler(id, file_name, format, use_color);
+    set(next_log_handler_id_number, 0, id_number + 1);
+    return new_log_handler(id_number, file_name, format, use_color);
   end;
 
   -- Display handler; Write to stdout
-  constant p_display_handler : log_handler_t := new_log_handler(display_handler_id,
+  constant p_display_handler : log_handler_t := new_log_handler(display_handler_id_number,
                                                                 stdout_file_name,
                                                                 format => verbose,
                                                                 use_color => true);
 
   impure function display_handler return log_handler_t is
   begin
     return p_display_handler;
   end function;
 
-  impure function get_id(log_handler : log_handler_t) return natural is
+  impure function get_id_number(log_handler : log_handler_t) return natural is
   begin
-    return get(log_handler.p_data, id_idx);
+    return get(log_handler.p_data, id_number_idx);
   end;
 
   impure function get_file_name (log_handler : log_handler_t) return string is
   begin
     return to_string(to_string_ptr(get(log_handler.p_data, file_name_idx)));
   end;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/log_handler_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/log_handler_pkg.vhd`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
   impure function new_log_handler(file_name : string;
                                   format : log_format_t := verbose;
                                   use_color : boolean := false) return log_handler_t;
 
   ---------------------------------------------
   -- Private parts not intended for public use
   ---------------------------------------------
-  impure function get_id(log_handler : log_handler_t) return natural;
+  impure function get_id_number(log_handler : log_handler_t) return natural;
   procedure update_max_logger_name_length(log_handler : log_handler_t; value : natural);
   impure function get_max_logger_name_length(log_handler : log_handler_t) return natural;
 
   procedure log_to_handler(log_handler : log_handler_t;
                            logger_name : string;
                            msg : string;
                            log_level : log_level_t;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/log_levels_pkg-body.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/log_levels_pkg-body.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/log_levels_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/log_levels_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/logger_pkg-body.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/logger_pkg-body.vhd`

 * *Files 6% similar despite different names*

```diff
@@ -9,32 +9,30 @@
 use work.queue_pkg.all;
 use work.core_pkg.core_failure;
 use std.textio.all;
 use work.string_ops.all;
 use work.print_pkg.print;
 use work.ansi_pkg.all;
 use work.location_pkg.all;
+use work.id_pkg.all;
 
 package body logger_pkg is
-  constant root_logger_id : natural := 0;
-  constant next_logger_id : integer_vector_ptr_t := new_integer_vector_ptr(1, value => root_logger_id + 1);
   constant global_log_count : integer_vector_ptr_t := new_integer_vector_ptr(1, value => 0);
   constant p_mock_queue_length : integer_vector_ptr_t := new_integer_vector_ptr(1, value => 0);
   constant mock_queue : queue_t := new_queue;
 
   constant id_idx : natural := 0;
-  constant name_idx : natural := 1;
-  constant parent_idx : natural := 2;
-  constant children_idx : natural := 3;
-  constant log_count_idx : natural := 4;
-  constant stop_counts_idx : natural := 5;
-  constant handlers_idx : natural := 6;
-  constant state_idx : natural := 7;
-  constant log_level_filters_idx : natural := 8;
-  constant logger_length : natural := 9;
+  constant parent_idx : natural := 1;
+  constant children_idx : natural := 2;
+  constant log_count_idx : natural := 3;
+  constant stop_counts_idx : natural := 4;
+  constant handlers_idx : natural := 5;
+  constant state_idx : natural := 6;
+  constant log_level_filters_idx : natural := 7;
+  constant logger_length : natural := 8;
 
   constant log_level_invisible : integer := 0;
   constant log_level_visible : integer := 1;
 
   constant stop_count_unset : integer := 0;
   constant stop_count_infinite : integer := integer'high;
 
@@ -52,23 +50,22 @@
   procedure add_child(logger : logger_t; child : logger_t) is
     constant children : integer_vector_ptr_t := to_integer_vector_ptr(get(logger.p_data, children_idx));
   begin
     resize(children, length(children)+1);
     set(children, length(children)-1, to_integer(child));
   end;
 
-  impure function new_logger(id : natural;
-                             name : string;
+  impure function new_logger(id : id_t;
                              parent : logger_t) return logger_t is
     variable logger : logger_t;
     variable log_handler : log_handler_t;
   begin
     logger := (p_data => new_integer_vector_ptr(logger_length));
-    set(logger.p_data, id_idx, id);
-    set(logger.p_data, name_idx, to_integer(new_string_ptr(name)));
+    set(logger.p_data, id_idx, to_integer(id));
+
     set(logger.p_data, parent_idx, to_integer(parent));
     set(logger.p_data, children_idx, to_integer(new_integer_vector_ptr));
     set(logger.p_data, log_count_idx, to_integer(new_integer_vector_ptr(log_level_t'pos(log_level_t'high)+1, value => 0)));
     set(logger.p_data, stop_counts_idx, to_integer(new_integer_vector_ptr(log_level_t'pos(log_level_t'high)+1, value => stop_count_unset)));
     set(logger.p_data, handlers_idx, to_integer(new_integer_vector_ptr));
     set(logger.p_data, state_idx, to_integer(new_integer_vector_ptr(log_level_t'pos(log_level_t'high)+1, value => enabled_state)));
     set(logger.p_data, log_level_filters_idx, to_integer(new_integer_vector_ptr));
@@ -108,35 +105,35 @@
   procedure set_log_level_filter(logger : logger_t;
                                  log_handler : log_handler_t;
                                  log_levels : log_level_vec_t;
                                  visible : boolean;
                                  include_children : boolean) is
     constant log_level_filters : integer_vector_ptr_t :=
       to_integer_vector_ptr(get(logger.p_data, log_level_filters_idx));
-    constant handler_id : natural := get_id(log_handler);
+    constant handler_id_number : natural := get_id_number(log_handler);
     variable log_level_filter : integer_vector_ptr_t;
     variable log_level_setting : natural;
 
   begin
-    if handler_id >= length(log_level_filters) then
-      resize(log_level_filters, handler_id + 1, value => to_integer(null_ptr));
+    if handler_id_number >= length(log_level_filters) then
+      resize(log_level_filters, handler_id_number + 1, value => to_integer(null_ptr));
     end if;
 
-    log_level_filter := to_integer_vector_ptr(get(log_level_filters, handler_id));
+    log_level_filter := to_integer_vector_ptr(get(log_level_filters, handler_id_number));
 
     if log_level_filter = null_ptr then
       -- Only show valid log levels by default
       log_level_filter := new_integer_vector_ptr(length => n_log_levels, value => log_level_invisible);
       for log_level in log_level_t'low to log_level_t'high loop
         if is_valid(log_level) then
           set(log_level_filter, log_level_t'pos(log_level), log_level_visible);
         end if;
       end loop;
 
-      set(log_level_filters, handler_id, to_integer(log_level_filter));
+      set(log_level_filters, handler_id_number, to_integer(log_level_filter));
     end if;
 
     if visible then
       log_level_setting := log_level_visible;
     else
       log_level_setting := log_level_invisible;
     end if;
@@ -149,122 +146,121 @@
       for i in 0 to num_children(logger)-1 loop
         set_log_level_filter(get_child(logger, i), log_handler, log_levels, visible,
                              include_children => true);
       end loop;
     end if;
   end;
 
-  impure function new_logger(name : string; parent : logger_t) return logger_t is
-    constant id : natural := get(next_logger_id, 0);
+  impure function get_id(logger : logger_t) return id_t is
   begin
-    set(next_logger_id, 0, id + 1);
-    return new_logger(id, name, parent);
+    return to_id(get(logger.p_data, id_idx));
   end;
 
-  impure function get_id(logger : logger_t) return natural is
+  impure function new_logger(name : string; parent : logger_t) return logger_t is
+    constant parent_id : id_t := get_id(parent);
+    constant id : id_t := get_id(name, parent_id);
   begin
-    return get(logger.p_data, id_idx);
+    if id = null_id then
+      return null_logger;
+    end if;
+
+    return new_logger(id, parent);
   end;
 
   impure function get_real_parent(parent : logger_t) return logger_t is
   begin
     if parent = null_logger then
       return root_logger;
     end if;
     return parent;
   end;
 
-  impure function head(name : string; dot_idx : natural) return string is
-  begin
-    if dot_idx = 0 then
-      return name;
-    else
-      return name(name'left to dot_idx-1);
-    end if;
-  end;
+  impure function has_logger(id : id_t) return boolean is
+    impure function has_logger(lineage : id_vec_t; search_root : logger_t) return boolean is
+      constant n_children : natural := num_children(search_root);
+      variable child : logger_t;
+      variable child_id : id_t;
+    begin
+      for idx in 0 to n_children - 1 loop
+        child := get_child(search_root, idx);
+        child_id := get_id(child);
+
+        if child_id = lineage(lineage'left) then
+          if lineage'length = 1 then
+            return true;
+          end if;
 
-  impure function tail(name : string; dot_idx : natural) return string is
+          return has_logger(lineage(lineage'left + 1 to lineage'right), child);
+        end if;
+      end loop;
+
+      return false;
+    end;
+
+    constant lineage : id_vec_t := get_lineage(id);
   begin
-    if dot_idx = 0 then
-      return "";
-    else
-      return name(dot_idx+1 to name'right);
+    if id = root_id then
+      return false;
     end if;
+
+    return has_logger(lineage(lineage'left + 1 to lineage'right), root_logger);
   end;
 
-  impure function validate_logger_name(name : string;
-                                       parent : logger_t) return boolean is
-    function join(s1, s2 : string) return string is
+  impure function get_logger(id : id_t) return logger_t is
+    impure function get_logger(lineage : id_vec_t; parent : logger_t) return logger_t is
+      constant n_children : natural := num_children(parent);
+      variable child : logger_t;
+      variable child_id : id_t;
+      variable logger : logger_t := null_logger;
     begin
-      if s1 = "" then
-        return s2;
-      else
-        return s1 & ":" & s2;
+      for idx in 0 to n_children - 1 loop
+        child := get_child(parent, idx);
+        child_id := get_id(child);
+        if child_id = lineage(lineage'left) then
+          logger := child;
+          exit;
+        end if;
+      end loop;
+
+      if logger = null_logger then
+        logger := new_logger(lineage(lineage'left), parent);
+        set_log_handlers(logger, get_log_handlers(parent));
+      end if;
+
+      if lineage'length > 1 then
+        return get_logger(lineage(lineage'left + 1 to lineage'right), logger);
       end if;
+
+      return logger;
     end;
 
-    constant full_name : string := join(get_name(parent), name);
+    constant lineage : id_vec_t := get_lineage(id);
   begin
-    if name = "" then
-      core_failure("Invalid logger name """ & full_name & """");
+    if id = null_id then
+      return null_logger;
     end if;
 
-    for i in full_name'range loop
-      if full_name(i) = ',' then
-        core_failure("Invalid logger name """ & full_name & """");
-        return false;
-      end if;
-    end loop;
-
-    return true;
+    return get_logger(lineage(lineage'left + 1 to lineage'right), root_logger);
   end;
 
   impure function get_logger(name : string;
                              parent : logger_t := null_logger) return logger_t is
     constant real_parent : logger_t := get_real_parent(parent);
-    variable child, logger : logger_t;
-    constant stripped_name : string := strip(name, ":");
-    constant dot_idx : integer := find(stripped_name, ':');
-    constant head_name : string := head(stripped_name, dot_idx);
-    constant tail_name : string := tail(stripped_name, dot_idx);
+    constant id : id_t := get_id(name, get_id(real_parent));
   begin
-    if not validate_logger_name(head_name, real_parent) then
+    if id = null_id then
       return null_logger;
     end if;
 
-    logger := null_logger;
-    for i in 0 to num_children(real_parent)-1 loop
-      child := get_child(real_parent, i);
-
-      if get_name(child) = head_name then
-        logger := child;
-        exit;
-      end if;
-    end loop;
-
-    if logger = null_logger then
-      logger := new_logger(head_name, real_parent);
-      set_log_handlers(logger, get_log_handlers(real_parent));
-    end if;
-
-    if dot_idx /= 0 then
-      return get_logger(tail_name, logger);
-    end if;
-
-    return logger;
+    return get_logger(id);
   end;
 
   impure function get_full_name(logger : logger_t) return string is
-    variable parent : logger_t := get_parent(logger);
   begin
-    if parent = null_logger or get_id(parent) = root_logger_id then
-      return get_name(logger);
-    else
-      return get_full_name(parent) & ":" & get_name(logger);
-    end if;
+    return full_name(get_id(logger));
   end;
 
   impure function get_max_name_length(logger : logger_t) return natural is
     constant full_name : string := get_full_name(logger);
     variable result : natural := 0;
     variable child_result : natural;
   begin
@@ -280,15 +276,15 @@
     end loop;
 
     return result;
   end;
 
   impure function get_name(logger : logger_t) return string is
   begin
-    return to_string(to_string_ptr(get(logger.p_data, name_idx)));
+    return name(get_id(logger));
   end;
 
   impure function get_parent(logger : logger_t) return logger_t is
   begin
     return (p_data => to_integer_vector_ptr(get(logger.p_data, parent_idx)));
   end;
 
@@ -389,15 +385,14 @@
   procedure set_stop_level(level : alert_log_level_t) is
   begin
     set_stop_level(root_logger, level);
   end;
 
   procedure set_stop_level(logger : logger_t;
                            log_level : alert_log_level_t) is
-    variable stop_count : natural;
   begin
     for level in log_level_t'low to log_level_t'high loop
       disable_stop(logger, level,
                               unset_children => true);
     end loop;
 
     for level in alert_log_level_t'low to alert_log_level_t'high loop
@@ -446,21 +441,21 @@
     return stop_count /= stop_count_unset;
   end;
 
   impure function get_log_level_filter(logger : logger_t;
                                        log_handler : log_handler_t) return integer_vector_ptr_t is
     constant log_level_filters : integer_vector_ptr_t :=
       to_integer_vector_ptr(get(logger.p_data, log_level_filters_idx));
-    constant handler_id : natural := get_id(log_handler);
+    constant handler_id_number : natural := get_id_number(log_handler);
   begin
-    if handler_id >= length(log_level_filters) then
-      resize(log_level_filters, handler_id + 1, value => to_integer(null_ptr));
+    if handler_id_number >= length(log_level_filters) then
+      resize(log_level_filters, handler_id_number + 1, value => to_integer(null_ptr));
     end if;
 
-    return to_integer_vector_ptr(get(log_level_filters, handler_id));
+    return to_integer_vector_ptr(get(log_level_filters, handler_id_number));
   end;
 
   impure function get_log_level_filter(logger : logger_t;
                                        log_handler : log_handler_t;
                                        visible : boolean) return log_level_vec_t is
     variable ret : log_level_vec_t(0 to n_log_levels - 1);
     variable idx : natural := 0;
@@ -671,22 +666,14 @@
       for i in 0 to num_children(logger)-1 loop
         set_log_handlers(get_child(logger, i), log_handlers,
                          include_children => true);
       end loop;
     end if;
   end;
 
-  procedure clear_log_count(logger : logger_t; idx : natural) is
-    constant log_counts : integer_vector_ptr_t := to_integer_vector_ptr(get(logger.p_data, idx));
-  begin
-    for lvl in log_level_t'low to log_level_t'high loop
-      set(log_counts, log_level_t'pos(lvl), 0);
-    end loop;
-  end;
-
   impure function get_log_count(logger : logger_t;
                                 idx : natural;
                                 log_level : log_level_t := null_log_level) return natural is
     constant log_counts : integer_vector_ptr_t := to_integer_vector_ptr(get(logger.p_data, idx));
     variable result : natural;
   begin
     if log_level = null_log_level then
@@ -836,15 +823,15 @@
                            file_name : string := "") is
   begin
     check_log(logger, msg, log_level, log_time, line_num, file_name);
     check_no_log;
   end;
 
   procedure check_no_log is
-    variable fail : boolean := length(mock_queue) > 0;
+    constant fail : boolean := length(mock_queue) > 0;
   begin
     while length(mock_queue) > 0 loop
       report "Got unexpected log item " & LF & LF & pop_log_item_string(true) & LF;
     end loop;
 
     if fail then
       core_failure("Got unexpected log items");
@@ -1024,15 +1011,15 @@
   begin
     if condition then
       failure(logger, msg, path_offset + 1, line_num => line_num, file_name => file_name);
     end if;
   end;
 
   impure function new_root_logger return logger_t is
-    variable logger : logger_t := new_logger(root_logger_id, "", null_logger);
+    constant logger : logger_t := new_logger(root_id, null_logger);
   begin
     p_set_log_handlers(logger, (0 => display_handler));
 
     for log_level in legal_log_level_t'low to legal_log_level_t'high loop
       case log_level is
         when error|failure =>
           set_stop_count(logger, log_level, 1);
@@ -1210,15 +1197,15 @@
             return "s";
           else
             return "";
           end if;
         end;
 
         variable count : natural;
-        variable level_is_disabled : boolean := is_disabled(logger, log_level);
+        constant level_is_disabled : boolean := is_disabled(logger, log_level);
       begin
         count := get_log_count(logger, log_level);
         if count > 0 and not (allow_disabled and level_is_disabled) then
           print(level_to_color(failure) & " - Logger " & source_to_color(get_full_name(logger)) &
                 " has " & integer'image(count) & disabled_str(level_is_disabled) & " " &
                 get_name(log_level) & plural_suffix(count > 1));
           return false;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/logger_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/logger_pkg.vhd`

 * *Files 0% similar despite different names*

```diff
@@ -3,30 +3,40 @@
 -- You can obtain one at http://mozilla.org/MPL/2.0/.
 --
 -- Copyright (c) 2014-2023, Lars Asplund lars.anders.asplund@gmail.com
 
 use work.log_levels_pkg.all;
 use work.log_handler_pkg.all;
 use work.integer_vector_ptr_pkg.all;
+use work.id_pkg.all;
 
 package logger_pkg is
 
   -- Logger record, all fields are private
   type logger_t is record
     p_data : integer_vector_ptr_t;
   end record;
   constant null_logger : logger_t := (p_data => null_ptr);
   type logger_vec_t is array (natural range <>) of logger_t;
   impure function root_logger return logger_t;
 
-  -- Get a logger with name.
-  -- Can also optionally be relative to a parent logger
+  -- Get a logger with name. A new one is created if it doesn't
+  -- already exist. Can also optionally be relative to a parent logger.
+  -- If a new logger is created then a new identity with the name/parent
+  -- is also created.
   impure function get_logger(name : string;
                              parent : logger_t := null_logger) return logger_t;
 
+  -- Get logger by identity. Create a new identity and/or logger if they
+  -- don't already exist.
+  impure function get_logger(id : id_t) return logger_t;
+
+  -- Return true if logger with id already exists, false otherwise.
+  impure function has_logger(id : id_t) return boolean;
+
   -------------------------------------
   -- Log procedures for each log level
   -------------------------------------
   procedure trace(logger : logger_t;
                   msg : string;
                   path_offset : natural := 0;
                   line_num : natural := 0;
@@ -165,14 +175,17 @@
 
   -- Get the name of this logger get_name(get_logger("parent:child")) = "child"
   impure function get_name(logger : logger_t) return string;
 
   -- Get the full name of this logger get_name(get_logger("parent:child")) = "parent:child"
   impure function get_full_name(logger : logger_t) return string;
 
+  -- Get identity for this logger.
+  impure function get_id(logger : logger_t) return id_t;
+
   -- Get the parent of this logger
   impure function get_parent(logger : logger_t) return logger_t;
 
   -- Get the number of children of this logger
   impure function num_children(logger : logger_t) return natural;
 
   -- Get the idx'th child of this logger
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/print_pkg-body.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/print_pkg-body.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/src/print_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/src/print_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/test/tb_deprecated.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/test/tb_deprecated.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/test/tb_location.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/test/tb_location.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/test/tb_log.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/test/tb_log.vhd`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 use work.log_levels_pkg.all;
 use work.logger_pkg.all;
 use work.log_handler_pkg.all;
 use work.core_pkg.all;
 use work.test_support_pkg.all;
 use work.print_pkg.all;
+use work.id_pkg.all;
 
 entity tb_log is
   generic (
     runner_cfg : string);
 end entity;
 
 architecture a of tb_log is
@@ -55,16 +56,16 @@
       assert status = open_ok
         report "Failed opening " & file_name & " (" & file_open_status'image(status) & ")."
         severity failure;
 
       if status = open_ok then
         for i in 0 to num_keys(entries)-1 loop
           readline(fptr, l);
-          assert l.all = get(entries, integer'image(i))
-            report "(" & integer'image(i) & ") " & LF & "Got:" & LF & l.all & LF & "expected:" & LF & get(entries, integer'image(i))
+          assert l.all = get_string(entries, integer'image(i))
+            report "(" & integer'image(i) & ") " & LF & "Got:" & LF & l.all & LF & "expected:" & LF & get_string(entries, integer'image(i))
             severity failure;
         end loop;
       end if;
     end;
 
     procedure check_log_file (file_handler : log_handler_t;
                               file_name : string;
@@ -145,20 +146,20 @@
 
     if run("raw format") then
       set_format(display_handler, format => raw);
       init_log_handler(file_handler, file_name => log_file_name, format => raw);
       disable_stop(logger, error);
       disable_stop(logger, failure);
       perform_logging(logger);
-      set(entries, "0", "message 1");
-      set(entries, "1", "message 2");
-      set(entries, "2", "message 3");
-      set(entries, "3", "message 4");
-      set(entries, "4", "message 5");
-      set(entries, "5", "message 6");
+      set_string(entries, "0", "message 1");
+      set_string(entries, "1", "message 2");
+      set_string(entries, "2", "message 3");
+      set_string(entries, "3", "message 4");
+      set_string(entries, "4", "message 5");
+      set_string(entries, "5", "message 6");
 
       check_log_file(file_handler, log_file_name, entries);
       reset_log_count(logger, error);
       reset_log_count(logger, failure);
 
     elsif run("Can get file name") then
       init_log_handler(file_handler, file_name => log_file_name, format => raw);
@@ -171,21 +172,21 @@
 
       file_open(status, fptr, print_file_name, append_mode);
       assert status = open_ok
         report "Failed to open file " & print_file_name & " - " & file_open_status'image(status) severity failure;
       print("message 3", fptr);
       file_close(fptr);
 
-      set(entries, "0", "message 1");
-      set(entries, "1", "message 2");
-      set(entries, "2", "message 3");
+      set_string(entries, "0", "message 1");
+      set_string(entries, "1", "message 2");
+      set_string(entries, "2", "message 3");
       check_file(print_file_name, entries);
 
       print("message 6", print_file_name, write_mode);
-      set(entries2, "0", "message 6");
+      set_string(entries2, "0", "message 6");
       check_file(print_file_name, entries2);
 
     elsif run("Can use 'instance_name") then
       tmp_logger := get_logger(tmp_logger'instance_name);
       assert_equal(get_name(tmp_logger), "tmp_logger");
       assert_equal(get_name(get_parent(tmp_logger)), "main");
       assert_equal(get_name(get_parent(get_parent(tmp_logger))), "tb_log(a)");
@@ -205,92 +206,92 @@
 
     elsif run("level format") then
       set_format(display_handler, format => level);
       init_log_handler(file_handler, file_name => log_file_name, format => level);
       disable_stop(logger, error);
       disable_stop(logger, failure);
       perform_logging(logger);
-      set(entries, "0", "  TRACE - message 1");
-      set(entries, "1", "  DEBUG - message 2");
-      set(entries, "2", "   INFO - message 3");
-      set(entries, "3", "WARNING - message 4");
-      set(entries, "4", "  ERROR - message 5");
-      set(entries, "5", "FAILURE - message 6");
+      set_string(entries, "0", "  TRACE - message 1");
+      set_string(entries, "1", "  DEBUG - message 2");
+      set_string(entries, "2", "   INFO - message 3");
+      set_string(entries, "3", "WARNING - message 4");
+      set_string(entries, "4", "  ERROR - message 5");
+      set_string(entries, "5", "FAILURE - message 6");
       check_log_file(file_handler, log_file_name, entries);
       reset_log_count(logger, error);
       reset_log_count(logger, failure);
 
     elsif run("level format aligns multi line logs") then
       set_format(display_handler, format => level);
       init_log_handler(file_handler, file_name => log_file_name, format => level);
       info(logger, "hello" & LF & "world" & LF & "    !");
-      set(entries, "0", "   INFO - hello");
-      set(entries, "1", "          world");
-      set(entries, "2", "              !");
+      set_string(entries, "0", "   INFO - hello");
+      set_string(entries, "1", "          world");
+      set_string(entries, "2", "              !");
       check_log_file(file_handler, log_file_name, entries);
 
     elsif run("csv format") then
       set_format(display_handler, format => csv);
       init_log_handler(file_handler, file_name => log_file_name, format => csv);
 
       wait for 3 ns;
       tmp := get_log_count;
       warning(nested_logger, "msg1");
       info(logger, "msg2", file_name => "file_name.vhd", line_num => 11);
-      set(entries, "0", integer'image(tmp+0) & "," & time'image(3 ns) & ",WARNING,,,logger:nested,msg1");
-      set(entries, "1", integer'image(tmp+1) & "," & time'image(3 ns) & ",INFO,file_name.vhd,11,logger,msg2");
+      set_string(entries, "0", integer'image(tmp+0) & "," & time'image(3 ns) & ",WARNING,,,logger:nested,msg1");
+      set_string(entries, "1", integer'image(tmp+1) & "," & time'image(3 ns) & ",INFO,file_name.vhd,11,logger,msg2");
       check_log_file(file_handler, log_file_name, entries);
 
     elsif run("verbose format") then
       set_format(display_handler, format => verbose);
       init_log_handler(file_handler, file_name => log_file_name, format => verbose);
       disable_stop(logger, error);
       disable_stop(logger, failure);
       perform_logging(logger);
-      set(entries, "0", format_time(0 ns) & " - logger               -   TRACE - message 1");
-      set(entries, "1", format_time(1 ns) & " - logger               -   DEBUG - message 2");
-      set(entries, "2", format_time(2 ns) & " - logger               -    INFO - message 3");
-      set(entries, "3", format_time(3 ns) & " - logger               - WARNING - message 4");
-      set(entries, "4", format_time(4 ns) & " - logger               -   ERROR - message 5");
-      set(entries, "5", format_time(5 ns) & " - logger               - FAILURE - message 6");
+      set_string(entries, "0", format_time(0 ns) & " - logger               -   TRACE - message 1");
+      set_string(entries, "1", format_time(1 ns) & " - logger               -   DEBUG - message 2");
+      set_string(entries, "2", format_time(2 ns) & " - logger               -    INFO - message 3");
+      set_string(entries, "3", format_time(3 ns) & " - logger               - WARNING - message 4");
+      set_string(entries, "4", format_time(4 ns) & " - logger               -   ERROR - message 5");
+      set_string(entries, "5", format_time(5 ns) & " - logger               - FAILURE - message 6");
       check_log_file(file_handler, log_file_name, entries);
       reset_log_count(logger, error);
       reset_log_count(logger, failure);
 
     elsif run("verbose format with file and line numbers") then
       set_format(display_handler, format => verbose);
       init_log_handler(file_handler, file_name => log_file_name, format => verbose);
       info(logger, "message", file_name => "tb_log.vhd", line_num => 188);
       info(logger, "hello" & LF & "world", file_name => "tb_log.vhd", line_num => 189);
-      set(entries, "0", format_time(0 ns) & " - logger               -    INFO - message (tb_log.vhd:188)");
-      set(entries, "1", format_time(0 ns) & " - logger               -    INFO - hello (tb_log.vhd:189)");
-      set(entries, "2", time_padding      & "                                    world");
+      set_string(entries, "0", format_time(0 ns) & " - logger               -    INFO - message (tb_log.vhd:188)");
+      set_string(entries, "1", format_time(0 ns) & " - logger               -    INFO - hello (tb_log.vhd:189)");
+      set_string(entries, "2", time_padding      & "                                    world");
       check_log_file(file_handler, log_file_name, entries);
 
     elsif run("verbose format aligns multi line logs") then
       set_format(display_handler, format => verbose);
       init_log_handler(file_handler, file_name => log_file_name, format => verbose);
       info(logger, "hello" & LF & "world" & LF & "    !");
-      set(entries, "0", format_time(0 ns) & " - logger               -    INFO - hello");
-      set(entries, "1", time_padding      & "                                    world");
-      set(entries, "2", time_padding      & "                                        !");
+      set_string(entries, "0", format_time(0 ns) & " - logger               -    INFO - hello");
+      set_string(entries, "1", time_padding      & "                                    world");
+      set_string(entries, "2", time_padding      & "                                        !");
       check_log_file(file_handler, log_file_name, entries);
 
     elsif run("hierarchical format") then
       set_format(display_handler, format => verbose);
       init_log_handler(file_handler, file_name => log_file_name, format => verbose);
       disable_stop(nested_logger, error);
       disable_stop(nested_logger, failure);
       perform_logging(nested_logger);
-      set(entries, "0", format_time(0 ns) & " - logger:nested        -   TRACE - message 1");
-      set(entries, "1", format_time(1 ns) & " - logger:nested        -   DEBUG - message 2");
-      set(entries, "2", format_time(2 ns) & " - logger:nested        -    INFO - message 3");
-      set(entries, "3", format_time(3 ns) & " - logger:nested        - WARNING - message 4");
-      set(entries, "4", format_time(4 ns) & " - logger:nested        -   ERROR - message 5");
-      set(entries, "5", format_time(5 ns) & " - logger:nested        - FAILURE - message 6");
+      set_string(entries, "0", format_time(0 ns) & " - logger:nested        -   TRACE - message 1");
+      set_string(entries, "1", format_time(1 ns) & " - logger:nested        -   DEBUG - message 2");
+      set_string(entries, "2", format_time(2 ns) & " - logger:nested        -    INFO - message 3");
+      set_string(entries, "3", format_time(3 ns) & " - logger:nested        - WARNING - message 4");
+      set_string(entries, "4", format_time(4 ns) & " - logger:nested        -   ERROR - message 5");
+      set_string(entries, "5", format_time(5 ns) & " - logger:nested        - FAILURE - message 6");
       check_log_file(file_handler, log_file_name, entries);
       reset_log_count(nested_logger, error);
       reset_log_count(nested_logger, failure);
 
     elsif run("can log to default logger") then
       init_log_handler(file_handler, file_name => log_file_name, format => level);
 
@@ -304,20 +305,20 @@
       wait for 1 ns;
       warning("message 4");
       wait for 1 ns;
       error("message 5");
       wait for 1 ns;
       failure("message 6");
 
-      set(entries, "0", "  DEBUG - message 1");
-      set(entries, "1", "  TRACE - message 2");
-      set(entries, "2", "   INFO - message 3");
-      set(entries, "3", "WARNING - message 4");
-      set(entries, "4", "  ERROR - message 5");
-      set(entries, "5", "FAILURE - message 6");
+      set_string(entries, "0", "  DEBUG - message 1");
+      set_string(entries, "1", "  TRACE - message 2");
+      set_string(entries, "2", "   INFO - message 3");
+      set_string(entries, "3", "WARNING - message 4");
+      set_string(entries, "4", "  ERROR - message 5");
+      set_string(entries, "5", "FAILURE - message 6");
       check_log_file(file_handler, log_file_name, entries);
       reset_log_count(default_logger, error);
       reset_log_count(default_logger, failure);
 
     elsif run("can show and hide from handler") then
       init_log_handler(file_handler, file_name => log_file_name, format => level);
       disable_stop(root_logger, error);
@@ -337,57 +338,57 @@
       for log_level in trace to failure loop
         assert_true(is_visible(default_logger, file_handler, log_level));
         assert_true(is_visible(logger, file_handler, log_level));
         assert_true(is_visible(nested_logger, file_handler, log_level));
       end loop;
 
       perform_logging(logger);
-      set(entries, "0", "  TRACE - message 1");
-      set(entries, "1", "  DEBUG - message 2");
-      set(entries, "2", "   INFO - message 3");
-      set(entries, "3", "WARNING - message 4");
-      set(entries, "4", "  ERROR - message 5");
-      set(entries, "5", "FAILURE - message 6");
+      set_string(entries, "0", "  TRACE - message 1");
+      set_string(entries, "1", "  DEBUG - message 2");
+      set_string(entries, "2", "   INFO - message 3");
+      set_string(entries, "3", "WARNING - message 4");
+      set_string(entries, "4", "  ERROR - message 5");
+      set_string(entries, "5", "FAILURE - message 6");
       check_log_file(file_handler, log_file_name, entries);
       reset_log_count(logger, error);
       reset_log_count(logger, failure);
 
     elsif run("can show individual levels") then
       init_log_handler(file_handler, file_name => log_file_name, format => level);
       hide_all(file_handler);
       show(file_handler, (warning, error, failure));
       disable_stop(root_logger, error);
       disable_stop(root_logger, failure);
       perform_logging(logger);
-      set(entries, "0", "WARNING - message 4");
-      set(entries, "1", "  ERROR - message 5");
-      set(entries, "2", "FAILURE - message 6");
+      set_string(entries, "0", "WARNING - message 4");
+      set_string(entries, "1", "  ERROR - message 5");
+      set_string(entries, "2", "FAILURE - message 6");
       check_log_file(file_handler, log_file_name, entries);
       reset_log_count(logger, error);
       reset_log_count(logger, failure);
 
     elsif run("can hide individual levels") then
       init_log_handler(file_handler, file_name => log_file_name, format => level);
       hide(file_handler, (trace, debug, info, error, failure));
       disable_stop(root_logger, error);
       disable_stop(root_logger, failure);
       perform_logging(logger);
-      set(entries, "0", "WARNING - message 4");
+      set_string(entries, "0", "WARNING - message 4");
       check_log_file(file_handler, log_file_name, entries);
       reset_log_count(logger, error);
       reset_log_count(logger, failure);
 
     elsif run("visibility also set for nested loggers") then
       init_log_handler(file_handler, file_name => log_file_name, format => level);
       hide_all(logger, file_handler);
       show(logger, file_handler, failure);
       info(logger, "message 1");
       info(nested_logger, "message 2");
       info("message 3");
-      set(entries, "0", "   INFO - message 3");
+      set_string(entries, "0", "   INFO - message 3");
       check_log_file(file_handler, log_file_name, entries);
 
     elsif run("can show and hide source") then
       init_log_handler(file_handler, file_name => log_file_name, format => level);
       hide_all(logger, file_handler);
 
       for log_level in trace to failure loop
@@ -395,31 +396,31 @@
         assert_false(is_visible(logger, file_handler, log_level));
         assert_false(is_visible(nested_logger, file_handler, log_level));
       end loop;
 
       info(logger, "message");
       info(nested_logger, "message");
       info("message");
-      set(entries, "0", "   INFO - message");
+      set_string(entries, "0", "   INFO - message");
       check_log_file(file_handler, log_file_name, entries);
 
       init_log_handler(file_handler, file_name => log_file_name, format => level);
       show_all(logger, file_handler);
       for log_level in trace to failure loop
         assert_true(is_visible(default_logger, file_handler, log_level));
         assert_true(is_visible(logger, file_handler, log_level));
         assert_true(is_visible(nested_logger, file_handler, log_level));
       end loop;
 
       info(logger, "message 1");
       info(nested_logger, "message 2");
       info("message 3");
-      set(entries, "0", "   INFO - message 1");
-      set(entries, "1", "   INFO - message 2");
-      set(entries, "2", "   INFO - message 3");
+      set_string(entries, "0", "   INFO - message 1");
+      set_string(entries, "1", "   INFO - message 2");
+      set_string(entries, "2", "   INFO - message 3");
       check_log_file(file_handler, log_file_name, entries);
 
     elsif run("mock and unmock") then
       mock(logger);
       unmock(logger);
 
     elsif run("mock check_only_log") then
@@ -582,15 +583,15 @@
     elsif run("new logger has unset stop counts") then
       tmp_logger := get_logger("new_logger");
 
       for log_level in legal_log_level_t'low to legal_log_level_t'high loop
         assert_false(has_stop_count(tmp_logger, log_level));
       end loop;
 
-    elsif run("Get logger") then
+    elsif run("Get logger by name") then
       tmp_logger := get_logger("logger:child");
       assert_equal(get_name(tmp_logger), "child");
       assert_equal(get_full_name(tmp_logger), "logger:child");
 
       tmp_logger := get_logger("logger:child:grandchild");
       assert_equal(get_name(tmp_logger), "grandchild");
       assert_equal(get_full_name(tmp_logger), "logger:child:grandchild");
@@ -600,14 +601,42 @@
 
       tmp_logger := get_logger("logger:nested");
       assert_true(tmp_logger = nested_logger);
 
       tmp_logger := get_logger("nested", parent => logger);
       assert_true(tmp_logger = nested_logger);
 
+    elsif run("Get logger by id") then
+      tmp_logger := get_logger(get_id("logger:child"));
+      assert_equal(get_name(tmp_logger), "child");
+      assert_equal(get_full_name(tmp_logger), "logger:child");
+
+      tmp_logger := get_logger(get_id("logger:child:grandchild"));
+      assert_equal(get_name(tmp_logger), "grandchild");
+      assert_equal(get_full_name(tmp_logger), "logger:child:grandchild");
+
+      tmp_logger := get_logger(get_id("default"));
+      assert_true(tmp_logger = default_logger);
+
+      tmp_logger := get_logger(get_id("logger:nested"));
+      assert_true(tmp_logger = nested_logger);
+
+      tmp_logger := get_logger(get_id("nested", parent => get_id(logger)));
+      assert_true(tmp_logger = nested_logger);
+
+    elsif run("Test has_logger") then
+      tmp_logger := get_logger("parent:child");
+      assert_true(has_logger(get_id("parent:child")));
+      assert_true(has_logger(get_id("parent")));
+
+      assert_false(has_logger(root_id));
+      assert_false(has_logger(get_id("id")));
+      assert_false(has_logger(get_id("parent:child2")));
+      assert_false(has_logger(get_id("parent:child:grandchild")));
+
     elsif run("Create hierarchical logger") then
       tmp_logger := get_logger("logger:child");
       assert_false(tmp_logger = null_logger, "logger not null");
       assert_equal(get_name(tmp_logger), "child", "nested logger name");
       assert_true(get_parent(tmp_logger) = logger, "parent logger");
 
     elsif run("Log counts") then
@@ -704,24 +733,27 @@
 
     elsif run("Test logger name validation") then
       tmp_logger := get_logger("foo:bar");
       assert_equal(get_name(get_logger("foo")), "foo");
 
       mock_core_failure;
       tmp_logger := get_logger("foo,bar");
-      check_core_failure("Invalid logger name ""foo,bar""");
+      check_core_failure("Invalid ID name ""foo,bar""");
 
       tmp_logger := get_logger("parent:foo,bar");
-      check_core_failure("Invalid logger name ""parent:foo,bar""");
+      check_core_failure("Invalid ID name ""parent:foo,bar""");
+
+      tmp_logger := get_logger("par,ent:foo");
+      check_core_failure("Invalid ID name ""par,ent""");
 
       tmp_logger := get_logger("");
-      check_core_failure("Invalid logger name """"");
+      check_core_failure("Invalid ID name """"");
 
       tmp_logger := get_logger(":");
-      check_core_failure("Invalid logger name """"");
+      check_core_failure("Invalid ID name """"");
 
       unmock_core_failure;
 
     elsif run("Test final log check fails for errors") then
       disable_stop(error);
       error(get_logger("parent:my_logger"), "message");
       mock_core_failure;
@@ -851,22 +883,22 @@
 
       -- But still be counted
       assert_equal(get_log_count(logger, warning), 1);
 
     elsif run("Disabled log is not visible") then
       init_log_handler(file_handler, file_name => log_file_name, format => raw);
       warning(logger, "message");
-      set(entries, "0", "message");
+      set_string(entries, "0", "message");
       check_log_file(file_handler, log_file_name, entries);
 
       init_log_handler(file_handler, file_name => log_file_name, format => raw);
       disable(logger, warning);
       assert_false(is_visible(logger, warning));
       warning(logger, "message");
-      set(entries, "0", "message");
+      set_string(entries, "0", "message");
       check_empty_log_file(log_file_name);
 
    elsif run("many log files") then
      set_format(display_handler, format => raw);
 
      for i in file_handlers'range loop
        file_handlers(i) := new_log_handler(log_file_name & integer'image(i),
@@ -880,17 +912,17 @@
      for i in file_handlers'range loop
        info(loggers(i), "a " & integer'image(i));
        info(loggers(i), "b " & integer'image(i));
        info(loggers(i), "c " & integer'image(i));
      end loop;
 
      for i in file_handlers'range loop
-       set(entries, "0", "a " & integer'image(i));
-       set(entries, "1", "b " & integer'image(i));
-       set(entries, "2", "c " & integer'image(i));
+       set_string(entries, "0", "a " & integer'image(i));
+       set_string(entries, "1", "b " & integer'image(i));
+       set_string(entries, "2", "c " & integer'image(i));
 
        check_log_file(file_handlers(i), log_file_name & integer'image(i), entries);
      end loop;
 
     end if;
 
     test_runner_cleanup(runner);
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/test/tb_log_levels.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/test/tb_log_levels.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/logging/test/test_support_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/logging/test/test_support_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/AUTHORS.md` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/AlertLogPkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/AlertLogPkg.vhd`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 --        SynthWorks Design Inc.
 --        VHDL Training Classes
 --        11898 SW 128th Ave.  Tigard, Or  97223
 --        http://www.SynthWorks.com
 --
 --  Revision History:
 --    Date      Version    Description
+--    10/2021   2021.10    Moved EndOfTestSummary to ReportPkg 
 --    09/2021   2021.09    Added EndOfTestSummary and CreateYamlReport - Experimental Release 
 --    07/2021   2021.07    When printing time value from GetOsvvmDefaultTimeUnits is used.
 --    06/2021   2021.06    FindAlertLogID updated to allow an ID name to match the name set by SetAlertLogName (ALERTLOG_BASE_ID) 
 --    12/2020   2020.12    Added MetaMatch to AffirmIfEqual and AffirmIfNotEqual for std_logic family to use MetaMatch
 --                         Added AffirmIfEqual for boolean
 --    10/2020   2020.10    Added MetaMatch.
 --                         Updated AlertIfEqual and AlertIfNotEqual for std_logic family to use MetaMatch
@@ -113,14 +114,15 @@
 
   constant  ALERTLOG_BASE_ID               : AlertLogIDType := 0 ;  -- Careful as some code may assume this is 0.
   constant  ALERTLOG_DEFAULT_ID            : AlertLogIDType := ALERTLOG_BASE_ID + 1 ;
   constant  OSVVM_ALERTLOG_ID              : AlertLogIDType := ALERTLOG_BASE_ID + 2 ; -- reporting for packages
   constant  REQUIREMENT_ALERTLOG_ID        : AlertLogIDType := ALERTLOG_BASE_ID + 3 ;
   -- May have its own ID or OSVVM_ALERTLOG_ID as default - most scoreboards allocate their own ID
   constant  OSVVM_SCOREBOARD_ALERTLOG_ID   : AlertLogIDType := OSVVM_ALERTLOG_ID ;
+  constant  OSVVM_COV_ALERTLOG_ID          : AlertLogIDType := OSVVM_ALERTLOG_ID ;
 
   -- Same as ALERTLOG_DEFAULT_ID
   constant  ALERT_DEFAULT_ID               : AlertLogIDType := ALERTLOG_DEFAULT_ID ;
   constant  LOG_DEFAULT_ID                 : AlertLogIDType := ALERTLOG_DEFAULT_ID ;
 
   constant  ALERTLOG_ID_NOT_FOUND          : AlertLogIDType := -1 ;  -- alternately integer'right
   constant  ALERTLOG_ID_NOT_ASSIGNED       : AlertLogIDType := -1 ;
@@ -302,19 +304,28 @@
     ReportAll      : Boolean         := FALSE 
   ) ;
   procedure ReportNonZeroAlerts ( 
     Name           : string          := OSVVM_STRING_INIT_PARM_DETECT ; 
     AlertLogID     : AlertLogIDType  := ALERTLOG_BASE_ID ; 
     ExternalErrors : AlertCountType  := (others => 0) 
   ) ;
-  procedure CreateYamlReport (ExternalErrors : AlertCountType := (0,0,0)) ;
-  procedure EndOfTestSummary (
-    ReportAll      : boolean        := FALSE ;
-    ExternalErrors : AlertCountType := (0,0,0) 
+  procedure WriteAlertYaml (
+    FileName       : string ;
+    ExternalErrors : AlertCountType := (0,0,0) ;
+    Prefix         : string := "" ;
+    PrintSettings  : boolean := TRUE ;
+    PrintChildren  : boolean := TRUE ;
+    OpenKind       : File_Open_Kind := WRITE_MODE
   ) ;
+  procedure WriteAlertSummaryYaml (FileName : string := "" ; ExternalErrors : AlertCountType := (0,0,0)) ;
+  procedure CreateYamlReport (ExternalErrors : AlertCountType := (0,0,0)) ;  -- Deprecated.  Use WriteAlertSummaryYaml.
+--  procedure EndOfTestSummary (
+--    ReportAll      : boolean        := FALSE ;
+--    ExternalErrors : AlertCountType := (0,0,0) 
+--  ) ;
   procedure WriteTestSummary   ( 
     FileName       : string ; 
     OpenKind       : File_Open_Kind := APPEND_MODE ; 
     Prefix         : string := "" ; 
     Suffix         : string := "" ; 
     ExternalErrors : AlertCountType := (0,0,0) ;
     WriteFieldName : boolean := FALSE 
@@ -595,14 +606,22 @@
     procedure ReportAlerts ( 
       Name           : string := OSVVM_STRING_INIT_PARM_DETECT ;
       AlertLogID     : AlertLogIDType := ALERTLOG_BASE_ID ;
       ExternalErrors : AlertCountType := (0,0,0) ;
       ReportAll      : boolean := FALSE ;
       ReportWhenZero : boolean := TRUE
     ) ;
+    procedure WriteAlertYaml (
+      FileName       : string ;
+      ExternalErrors : AlertCountType := (0,0,0) ;
+      Prefix         : string := "" ;
+      PrintSettings  : boolean := TRUE ;
+      PrintChildren  : boolean := TRUE ;
+      OpenKind       : File_Open_Kind := WRITE_MODE
+    ) ;
     procedure WriteTestSummary ( 
       FileName       : string ;
       OpenKind       : File_Open_Kind ;
       Prefix         : string ; 
       Suffix         : string ; 
       ExternalErrors : AlertCountType ;
       WriteFieldName : boolean 
@@ -778,16 +797,16 @@
       ParentID            : AlertLogIDType ;
       ParentIDSet         : Boolean ;
       SiblingID           : AlertLogIDType ;
       ChildID             : AlertLogIDType ;
       ChildIDLast         : AlertLogIDType ;
       AlertCount          : AlertCountType ;
       DisabledAlertCount  : AlertCountType ;
-      AffirmCount         : Integer ;
       PassedCount         : Integer ;
+      AffirmCount         : Integer ;
       PassedGoal          : Integer ;
       PassedGoalSet       : Boolean ;
       AlertStopCount      : AlertCountType ;
       AlertEnabled        : AlertEnableType ;
       LogEnabled          : LogEnableType ;
       DoNotReport         : Boolean ;
       -- Used only by ReadTestSummaries
@@ -1132,15 +1151,18 @@
       variable localAlertLogID : AlertLogIDType ;
     begin
       localAlertLogID := VerifyID(AlertLogID) ;
       return LocalGetDisabledAlertCount(localAlertLogID) ;
     end function GetDisabledAlertCount ;
 
     ------------------------------------------------------------
-    -- Local
+    -- Local  GetRequirementsCount
+    --    Each bin contains a separate requirement 
+    --    RequirementsGoal   = # of bins with PassedGoal > 0
+    --    RequirementsPassed = # bins with PassedGoal > 0 and PassedCount > PassedGoal 
     procedure GetRequirementsCount(
       AlertLogID              : AlertLogIDType;
       RequirementsPassed      : out integer ;
       RequirementsGoal        : out integer
     )  is
     ------------------------------------------------------------
       variable ChildRequirementsPassed, ChildRequirementsGoal  : integer ;
@@ -1161,14 +1183,15 @@
         RequirementsPassed := RequirementsPassed + ChildRequirementsPassed ;
         RequirementsGoal   := RequirementsGoal   + ChildRequirementsGoal ;
         CurID := AlertLogPtr(CurID).SiblingID ;
       end loop ;
     end procedure GetRequirementsCount ;
 
     ------------------------------------------------------------
+-- Only used at top level and superceded by variables PassedCountVar AffirmCheckCountVar
     -- Local
     procedure GetPassedAffirmCount(
       AlertLogID       : AlertLogIDType;
       PassedCount      : out integer ;
       AffirmCount      : out integer
     )  is
     ------------------------------------------------------------
@@ -1184,14 +1207,81 @@
         PassedCount := PassedCount + ChildPassedCount ;
         AffirmCount := AffirmCount + ChildAffirmCount ;
         CurID := AlertLogPtr(CurID).SiblingID ;
       end loop ;
     end procedure GetPassedAffirmCount ;
 
     ------------------------------------------------------------
+    -- Local
+    procedure CalcTopTotalErrors (
+    ------------------------------------------------------------
+      constant ExternalErrors           : in  AlertCountType ;
+      variable TotalErrors              : out integer ;
+      variable TotalAlertCount          : out AlertCountType ; 
+      variable TotalRequirementsPassed  : out integer ; 
+      variable TotalRequirementsCount   : out integer
+    ) is 
+      variable DisabledAlertCount : AlertCountType ;
+      variable TotalAlertErrors, TotalDisabledAlertErrors : integer ;
+      variable TotalRequirementErrors : integer ;
+    begin
+      TotalAlertCount        := AlertLogPtr(ALERTLOG_BASE_ID).AlertCount + ExternalErrors ;
+      TotalAlertErrors       := SumAlertCount( RemoveNonFailingWarnings(TotalAlertCount)) ;
+      TotalErrors            := TotalAlertErrors ;
+
+      DisabledAlertCount        := GetDisabledAlertCount(ALERTLOG_BASE_ID) ;
+      TotalDisabledAlertErrors  := SumAlertCount( RemoveNonFailingWarnings(DisabledAlertCount) ) ;
+      if FailOnDisabledErrorsVar then
+        TotalAlertCount := TotalAlertCount + DisabledAlertCount ; 
+        TotalErrors := TotalErrors + TotalDisabledAlertErrors ;
+      end if ;
+
+      -- Perspective, 1 requirement per bin
+      GetRequirementsCount(ALERTLOG_BASE_ID, TotalRequirementsPassed, TotalRequirementsCount) ;
+      TotalRequirementErrors := TotalRequirementsCount - TotalRequirementsPassed ;
+      if FailOnRequirementErrorsVar then
+        TotalErrors := TotalErrors + TotalRequirementErrors ;
+      end if ;
+      
+      -- Set AffirmCount for top level
+      AlertLogPtr(ALERTLOG_BASE_ID).PassedCount := PassedCountVar ;
+      AlertLogPtr(ALERTLOG_BASE_ID).AffirmCount := AffirmCheckCountVar ;
+    end procedure CalcTopTotalErrors ;
+
+    ------------------------------------------------------------
+    -- Local
+    impure function CalcTotalErrors (AlertLogID : AlertLogIDType) return integer is 
+    ------------------------------------------------------------
+      variable TotalErrors : integer ;
+      variable TotalAlertCount, DisabledAlertCount : AlertCountType ;
+      variable TotalAlertErrors, TotalDisabledAlertErrors : integer ;
+      variable TotalRequirementErrors : integer ;
+      variable TotalRequirementsPassed, TotalRequirementsCount : integer ;
+    begin
+      TotalAlertCount        := AlertLogPtr(AlertLogID).AlertCount ;
+      TotalAlertErrors       := SumAlertCount( RemoveNonFailingWarnings(TotalAlertCount)) ;
+      TotalErrors            := TotalAlertErrors ;
+
+      DisabledAlertCount        := GetDisabledAlertCount(AlertLogID) ;
+      TotalDisabledAlertErrors  := SumAlertCount( RemoveNonFailingWarnings(DisabledAlertCount) ) ;
+      if FailOnDisabledErrorsVar then
+        TotalErrors := TotalErrors + TotalDisabledAlertErrors ;
+      end if ;
+
+      -- Perspective, 1 requirement per bin
+      GetRequirementsCount(AlertLogID, TotalRequirementsPassed, TotalRequirementsCount) ;
+      TotalRequirementErrors := TotalRequirementsCount - TotalRequirementsPassed ;
+      if FailOnRequirementErrorsVar then
+        TotalErrors := TotalErrors + TotalRequirementErrors ;
+      end if ;
+      
+      return TotalErrors ;
+    end function CalcTotalErrors ;
+
+    ------------------------------------------------------------
     -- PT Local
     procedure PrintTopAlerts (
     ------------------------------------------------------------
       AlertLogID                  : AlertLogIDType ;
       Name                        : string ;
       ExternalErrors              : AlertCountType ;
       variable HasDisabledAlerts  : inout Boolean ;
@@ -1204,14 +1294,17 @@
       variable buf : line ;
       variable TotalErrors : integer ;
       variable TotalAlertErrors, TotalDisabledAlertErrors : integer ;
       variable TotalRequirementsPassed, TotalRequirementsGoal, TotalRequirementErrors : integer ;
       variable AlertCountVar, DisabledAlertCount : AlertCountType ;
       variable PassedCount, AffirmCheckCount : integer ;
     begin
+--!! 
+--!! Update to use CalcTopTotalErrors
+--!! 
       AlertCountVar     := AlertLogPtr(AlertLogID).AlertCount + ExternalErrors ;
       TotalAlertErrors  := SumAlertCount( RemoveNonFailingWarnings(AlertCountVar)) ;
 
       DisabledAlertCount        := GetDisabledAlertCount(AlertLogID) ;
       TotalDisabledAlertErrors  := SumAlertCount( RemoveNonFailingWarnings(DisabledAlertCount) ) ;
       HasDisabledAlerts         := TotalDisabledAlertErrors /= 0 ;
 
@@ -1337,15 +1430,15 @@
       CurID := AlertLogPtr(AlertLogID).ChildID ;
       while CurID > ALERTLOG_BASE_ID loop
         -- Don't print requirements if there no requirements
         if CurID = REQUIREMENT_ALERTLOG_ID and HasRequirementsVar = FALSE then
           CurID := AlertLogPtr(CurID).SiblingID ;
           next ;
         end if ;
-        if not AlertLogPtr(AlertLogID).DoNotReport then
+        if not AlertLogPtr(CurID).DoNotReport then
           PrintOneChild(
             AlertLogID         => CurID,
             Prefix             => Prefix,
             IndentAmount       => IndentAmount,
             ReportWhenZero     => ReportWhenZero,
             HasDisabledErrors  => HasDisabledErrors
           ) ;
@@ -1488,14 +1581,199 @@
         write(buf, "  Failures: "  & to_string(AlertCount(FAILURE)) ) ;
         write(buf, "  Errors: "    & to_string(AlertCount(ERROR) ) ) ;
         write(buf, "  Warnings: "  & to_string(AlertCount(WARNING) ) ) ;
         write(buf, "  at "  & to_string(NOW, 1 ns)) ;
         writeLine(buf) ;
       end if ;
     end procedure ReportAlerts ;
+    
+    ------------------------------------------------------------
+    --  pt local
+    procedure WriteOneAlertYaml (
+    ------------------------------------------------------------
+      file TestFile : text ;
+      AlertLogID           : AlertLogIDType ; 
+      TotalErrors          : integer ;
+      RequirementsPassed   : integer ; 
+      RequirementsGoal     : integer ;
+      FirstPrefix          : string := "" ;
+      Prefix               : string := ""
+    ) is
+      variable buf : line ;
+      constant DELIMITER : string := ", " ;
+    begin
+      Write(buf, 
+        FirstPrefix & "Name: " & '"' & AlertLogPtr(AlertLogID).Name.all & '"'  & LF  & 
+        Prefix & "Status: " & IfElse(TotalErrors=0, "PASSED", "FAILED")        & LF  &
+        Prefix & "Results: {" & 
+          "TotalErrors: "        & to_string( TotalErrors )          & DELIMITER & 
+          "AlertCount: {" & 
+            "Failure: "            & to_string( AlertLogPtr(AlertLogID).AlertCount(FAILURE) )  & DELIMITER & 
+            "Error: "              & to_string( AlertLogPtr(AlertLogID).AlertCount(ERROR) )    & DELIMITER & 
+            "Warning: "            & to_string( AlertLogPtr(AlertLogID).AlertCount(WARNING) )  & 
+          "}" & DELIMITER &
+          "PassedCount: "        & to_string( AlertLogPtr(AlertLogID).PassedCount )          & DELIMITER &
+          "AffirmCount: "        & to_string( AlertLogPtr(AlertLogID).AffirmCount )          & DELIMITER & 
+          "RequirementsPassed: " & to_string( RequirementsPassed )   & DELIMITER & 
+          "RequirementsGoal: "   & to_string( RequirementsGoal )     & DELIMITER & 
+          "DisabledAlertCount: {" & 
+            "Failure: "            & to_string( AlertLogPtr(AlertLogID).DisabledAlertCount(FAILURE) )  & DELIMITER & 
+            "Error: "              & to_string( AlertLogPtr(AlertLogID).DisabledAlertCount(ERROR) )    & DELIMITER & 
+            "Warning: "            & to_string( AlertLogPtr(AlertLogID).DisabledAlertCount(WARNING) )  &
+          "}" & 
+        "}"
+      ) ;        
+      WriteLine(TestFile, buf) ;
+    end procedure WriteOneAlertYaml ;
+
+    ------------------------------------------------------------
+    -- PT Local
+    procedure IterateAndWriteChildrenYaml(
+    ------------------------------------------------------------
+      file TestFile     : text ;
+      AlertLogID        : AlertLogIDType ;
+      Prefix            : string 
+    ) is
+      variable buf : line ;
+      variable CurID : AlertLogIDType ;
+      variable RequirementsPassed, RequirementsGoal : integer ; 
+    begin
+      CurID := AlertLogPtr(AlertLogID).ChildID ;
+      if CurID >= ALERTLOG_BASE_ID then 
+        -- Write "Children:" at current level
+        Write(buf, Prefix & "Children: " ) ;  
+        WriteLine(TestFile, buf) ;
+        while CurID > ALERTLOG_BASE_ID loop
+          -- Don't print requirements if there no requirements
+          if CurID = REQUIREMENT_ALERTLOG_ID and HasRequirementsVar = FALSE then
+            CurID := AlertLogPtr(CurID).SiblingID ;
+            next ;
+          end if ;
+          RequirementsGoal   := AlertLogPtr(CurID).PassedGoal ;
+          if AlertLogPtr(CurID).PassedGoalSet and (RequirementsGoal > 0) then 
+            RequirementsPassed := AlertLogPtr(CurID).PassedCount ;
+          else
+            RequirementsPassed := 0 ;
+            RequirementsGoal   := 0 ;
+          end if ; 
+          if not AlertLogPtr(CurID).DoNotReport then
+            WriteOneAlertYaml(
+              TestFile             => TestFile,
+              AlertLogID           => CurID,
+              TotalErrors          => CalcTotalErrors(CurID),
+              RequirementsPassed   => RequirementsPassed,
+              RequirementsGoal     => RequirementsGoal,
+              FirstPrefix          => Prefix & "  - ",
+              Prefix               => Prefix & "    "
+            ) ;
+            IterateAndWriteChildrenYaml(
+              TestFile             => TestFile,
+              AlertLogID           => CurID,
+              Prefix               => Prefix & "    "
+            ) ;
+          end if ; 
+          CurID := AlertLogPtr(CurID).SiblingID ;
+        end loop ;
+      else
+        -- No Children, Print Empty List
+        Write(buf, Prefix & "Children: {}" ) ;  
+        WriteLine(TestFile, buf) ;
+      end if ;
+    end procedure IterateAndWriteChildrenYaml ;  
+
+    ------------------------------------------------------------
+    --  pt local
+    procedure WriteSettingsYaml (
+    ------------------------------------------------------------
+      file TestFile  : text ;
+      ExternalErrors : AlertCountType ;
+      Prefix         : string := ""
+    ) is
+      variable buf : line ;
+      constant DELIMITER : string := ", " ;
+    begin
+      Write(buf, 
+        Prefix & "Settings: {" & 
+          "ExternalErrors: {" & 
+            "Failure: "                & '"' & to_string( ExternalErrors(FAILURE) )  & '"'  & DELIMITER & 
+            "Error: "                  & '"' & to_string( ExternalErrors(ERROR) )    & '"'  & DELIMITER & 
+            "Warning: "                & '"' & to_string( ExternalErrors(WARNING) )  & '"'  & 
+          "}" & DELIMITER &
+          "FailOnDisabledErrors: "     & '"' & to_string( FailOnDisabledErrorsVar )     & '"' & DELIMITER &
+          "FailOnRequirementErrors: "  & '"' & to_string( FailOnRequirementErrorsVar )  & '"' & DELIMITER & 
+          "FailOnWarning: "            & '"' & to_string( FailOnWarningVar )   & '"' &
+        "}"
+      ) ;        
+      WriteLine(TestFile, buf) ;
+    end procedure WriteSettingsYaml ;  
+
+    
+    ------------------------------------------------------------
+    --  pt local
+    procedure WriteAlertYaml (
+    ------------------------------------------------------------
+      file TestFile  : text ;
+      ExternalErrors : AlertCountType ;
+      Prefix         : string ;
+      PrintSettings  : boolean ;
+      PrintChildren  : boolean 
+    ) is
+      -- Format:  Action Count min1 max1 min2 max2
+      variable TotalErrors : integer ;
+      variable TotalAlertCount : AlertCountType ;
+      variable TotalRequirementsPassed, TotalRequirementsCount : integer ;
+    begin
+      CalcTopTotalErrors (
+        ExternalErrors           => ExternalErrors         ,
+        TotalErrors              => TotalErrors            ,
+        TotalAlertCount          => TotalAlertCount        ,
+        TotalRequirementsPassed  => TotalRequirementsPassed,
+        TotalRequirementsCount   => TotalRequirementsCount
+      ) ; 
+      
+      WriteOneAlertYaml (
+        TestFile                 => TestFile,
+        AlertLogID               => ALERTLOG_BASE_ID,
+        TotalErrors              => TotalErrors,
+        RequirementsPassed       => TotalRequirementsPassed,
+        RequirementsGoal         => TotalRequirementsCount,
+        FirstPrefix              => Prefix,
+        Prefix                   => Prefix
+      ) ;   
+      if PrintSettings then 
+        WriteSettingsYaml(
+          TestFile               => TestFile,
+          ExternalErrors         => ExternalErrors,
+          Prefix                 => Prefix
+        ) ; 
+      end if ; 
+      if PrintChildren then 
+        IterateAndWriteChildrenYaml(
+          TestFile             => TestFile,
+          AlertLogID           => ALERTLOG_BASE_ID,
+          Prefix               => Prefix
+        ) ;
+      end if ; 
+    end procedure WriteAlertYaml ;
+    
+    ------------------------------------------------------------
+    procedure WriteAlertYaml (
+    ------------------------------------------------------------
+      FileName       : string ;
+      ExternalErrors : AlertCountType := (0,0,0) ;
+      Prefix         : string := "" ;
+      PrintSettings  : boolean := TRUE ;
+      PrintChildren  : boolean := TRUE ;
+      OpenKind       : File_Open_Kind := WRITE_MODE
+    ) is
+      file TestFile : text open OpenKind is FileName ;
+    begin
+      WriteAlertYaml(TestFile, ExternalErrors, Prefix, PrintSettings, PrintChildren) ; 
+    end procedure WriteAlertYaml ;
+    
 
 --     ------------------------------------------------------------
 --     procedure EndOfTestSummary (
 --     ------------------------------------------------------------
 -- --      variable TestErrorsOut : out integer ; 
 --       constant ReportAll      : boolean        := FALSE ;
 --       constant ExternalErrors : AlertCountType := (0,0,0) 
@@ -1611,14 +1889,17 @@
       variable TotalRequirementsPassed, TotalRequirementsGoal : integer ;
       variable TotalRequirementErrors : integer ;
       variable TotalAlertCount, DisabledAlertCount : AlertCountType ;
       constant AlertLogID : AlertLogIDType := ALERTLOG_BASE_ID ;
       variable PassedCount, AffirmCount : integer ;
       constant DELIMITER : string := ", " ;
     begin
+--!! 
+--!! Update to use CalcTopTotalErrors
+--!!    
       TotalAlertCount        := AlertLogPtr(AlertLogID).AlertCount + ExternalErrors ;
       TotalAlertErrors     := SumAlertCount( RemoveNonFailingWarnings(TotalAlertCount)) ;
 
       DisabledAlertCount        := GetDisabledAlertCount(AlertLogID) ;
       TotalDisabledAlertErrors  := SumAlertCount( RemoveNonFailingWarnings(DisabledAlertCount) ) ;
 
       GetRequirementsCount(AlertLogID, TotalRequirementsPassed, TotalRequirementsGoal) ;
@@ -2467,15 +2748,15 @@
       end if ;
       NumAllocatedAlertLogIDsVar := NewNumAlertLogIDs ;
     end procedure GrowAlertStructure ;
 
     ------------------------------------------------------------
     -- Sets a AlertLogPtr to a particular size
     -- Use for small bins to save space or large bins to
-    -- suppress the resize and copy as a CovBin autosizes.
+    -- suppress the resize and copy in autosizes.
     procedure SetNumAlertLogIDs (NewNumAlertLogIDs : AlertLogIDType) is
     ------------------------------------------------------------
       variable oldAlertLogPtr : AlertLogArrayPtrType ;
     begin
       if NewNumAlertLogIDs > NumAllocatedAlertLogIDsVar then
         GrowAlertStructure(NewNumAlertLogIDs) ;
       end if;
@@ -3802,19 +4083,40 @@
     if L /= R then
       AlertLogStruct.Alert(ALERT_DEFAULT_ID, Message & " L /= R,  L = " & to_string(L, GetOsvvmDefaultTimeUnits) & 
                                                               "   R = " & to_string(R, GetOsvvmDefaultTimeUnits), Level) ;
     end if ;
     -- synthesis translate_on
   end procedure AlertIfNotEqual ;
 
+  ------------------------------------------------------------
+  -- Local
+  function LocalDiff (Line1, Line2 : string) return boolean is
+  -- Simple diff.  Move to string handling functions?
+  ------------------------------------------------------------
+    alias aLine1 : string (1 to Line1'length) is Line1 ;
+    alias aLine2 : string (1 to Line2'length) is Line2 ;
+    variable EndLine1 : integer := Line1'length; 
+    variable EndLine2 : integer := Line2'length; 
+  begin
+    -- Strip off any windows or unix end of line characters 
+    for i in Line1'length downto 1 loop
+      exit when aLine1(i) /= LF and aLine1(i) /= CR ;
+      EndLine1 := i - 1; 
+    end loop ;
+    for i in Line2'length downto 1 loop
+      exit when aLine2(i) /= LF and aLine2(i) /= CR ;
+      EndLine2 := i - 1; 
+    end loop ;
+    
+    return aLine1(1 to EndLine1) /= aLine2(1 to EndLine2) ;
+  end function LocalDiff ; 
 
   ------------------------------------------------------------
   -- Local
   procedure LocalAlertIfDiff (AlertLogID : AlertLogIDType ; file File1, File2 : text; Message : string ; Level : AlertType ; Valid : out boolean ) is
-  -- Simple diff.
   ------------------------------------------------------------
     variable Buf1, Buf2 : line ;
     variable File1Done, File2Done : boolean ;
     variable LineCount : integer := 0 ;
   begin
     -- synthesis translate_off
     ReadLoop : loop
@@ -3822,15 +4124,16 @@
       File2Done := EndFile(File2) ;
       exit ReadLoop when File1Done or File2Done ;
 
       ReadLine(File1, Buf1) ;
       ReadLine(File2, Buf2) ;
       LineCount := LineCount + 1 ;
 
-      if Buf1.all /= Buf2.all then
+--      if Buf1.all /= Buf2.all then  -- fails when use Windows file in Unix
+      if LocalDiff(Buf1.all, Buf2.all) then
         AlertLogStruct.Alert(AlertLogID , Message & " File miscompare on line " & to_string(LineCount), Level) ;
         exit ReadLoop ;
       end if ;
     end loop ReadLoop ;
     if File1Done /= File2Done then
       if not File1Done then
         AlertLogStruct.Alert(AlertLogID , Message & " File1 longer than File2 " & to_string(LineCount), Level) ;
@@ -4555,36 +4858,62 @@
   begin
     -- synthesis translate_off
     AlertLogStruct.ReportAlerts(Name, AlertLogID, ExternalErrors, FALSE, FALSE) ;
     -- synthesis translate_on
   end procedure ReportNonZeroAlerts ;
 
   ------------------------------------------------------------
-  procedure CreateYamlReport (ExternalErrors : AlertCountType := (0,0,0)) is
+  procedure WriteAlertYaml (
   ------------------------------------------------------------
+    FileName       : string ;
+    ExternalErrors : AlertCountType := (0,0,0) ;
+    Prefix         : string := "" ;
+    PrintSettings  : boolean := TRUE ;
+    PrintChildren  : boolean := TRUE ;
+    OpenKind       : File_Open_Kind := WRITE_MODE
+  ) is
   begin
     -- synthesis translate_off
-    --  WriteTestSummary(FileName => "OsvvmRun.yml", OpenKind => APPEND_MODE, Prefix => "      Results: {", Suffix => "}", ExternalErrors => ExternalErrors) ; 
-    WriteTestSummary(FileName => "OsvvmRun.yml", OpenKind => APPEND_MODE, Prefix => "      ", Suffix => "", ExternalErrors => ExternalErrors, WriteFieldName => TRUE) ; 
+    AlertLogStruct.WriteAlertYaml(FileName, ExternalErrors, Prefix, PrintSettings, PrintChildren, OpenKind) ;
     -- synthesis translate_on
-  end procedure CreateYamlReport ;
+  end procedure WriteAlertYaml ;
 
   ------------------------------------------------------------
-  procedure EndOfTestSummary (
+  procedure WriteAlertSummaryYaml (FileName : string := "" ; ExternalErrors : AlertCountType := (0,0,0)) is
   ------------------------------------------------------------
-    ReportAll      : boolean        := FALSE ;
-    ExternalErrors : AlertCountType := (0,0,0) 
-  ) is
+    constant RESOLVED_FILE_NAME : string := IfElse(FileName = "", "OsvvmRun.yml", FileName) ; 
   begin
     -- synthesis translate_off
-    ReportAlerts(ExternalErrors => ExternalErrors, ReportAll => ReportAll) ; 
-    CreateYamlReport(ExternalErrors => ExternalErrors) ; 
-    std.env.stop(SumAlertCount(GetAlertCount + ExternalErrors)) ;
+    WriteAlertYaml(FileName => RESOLVED_FILE_NAME, ExternalErrors => ExternalErrors, Prefix => "      ", PrintSettings => FALSE, PrintChildren => FALSE, OpenKind => APPEND_MODE) ; 
+    -- WriteTestSummary(FileName => "OsvvmRun.yml", OpenKind => APPEND_MODE, Prefix => "      ", Suffix => "", ExternalErrors => ExternalErrors, WriteFieldName => TRUE) ; 
     -- synthesis translate_on
-  end procedure EndOfTestSummary ;
+  end procedure WriteAlertSummaryYaml ;
+
+  ------------------------------------------------------------
+  -- Deprecated.  Use WriteAlertSummaryYaml Instead.
+  procedure CreateYamlReport (ExternalErrors : AlertCountType := (0,0,0)) is
+  begin
+    -- synthesis translate_off
+    WriteAlertSummaryYaml(ExternalErrors => ExternalErrors) ; 
+    -- synthesis translate_on
+  end procedure CreateYamlReport ;
+
+--  ------------------------------------------------------------
+--  procedure EndOfTestSummary (
+--  ------------------------------------------------------------
+--    ReportAll      : boolean        := FALSE ;
+--    ExternalErrors : AlertCountType := (0,0,0) 
+--  ) is
+--  begin
+--    -- synthesis translate_off
+--    ReportAlerts(ExternalErrors => ExternalErrors, ReportAll => ReportAll) ; 
+--    WriteAlertSummaryYaml(ExternalErrors => ExternalErrors) ; 
+--    std.env.stop(SumAlertCount(GetAlertCount + ExternalErrors)) ;
+--    -- synthesis translate_on
+--  end procedure EndOfTestSummary ;
 
   ------------------------------------------------------------
   procedure WriteTestSummary (
   ------------------------------------------------------------
     FileName       : string ; 
     OpenKind       : File_Open_Kind := APPEND_MODE ; 
     Prefix         : string := "" ;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/CHANGELOG.md` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # OSVVM Utility Library (aka OSVVM) Change Log 
 
 | Revision name | Revision  Date |  Summary |
 ----------------|----------------|----------- 
+| 2021.12  | December 2021   |  Added ReadCovYaml. 
+| 2021.11  | November 2021   |  Minor updates.  Print CovWeight first in WriteCovYaml. 
+|          |                 |     Update to usage of PercentCov in GetCov. 
+| 2021.10  | October 2021    |  Updates to generate HTML and JUnit XML for test suite information
+|          |                 |     Generate YAML and HTML for reporting Alert and Coverag information
+|          |                 |     Added ReportPkg. Uupdated CoveragePkg and AlertLogPkg 
 | 2021.09  | September 2021  |  Minor updates to support Synopsys and Cadence
 | 2021.08  | August 2021     |  Minor deprecations in CoveragePkg and ScoreboardGenericPkg
 | 2021.07  | July 2021       |  Updated Data Structure of CoveragePkg
 | 2021.06  | June 2021       |  Updated Data Structures
 | 2020.12  | December 2020   |  Minor Updates
 | 2020.10  | October 2020    |  Minor Updates
 | 2020.08  | August 2020     |  Specification Tracking
@@ -46,16 +52,15 @@
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
 
-## Revision 2021.09 September 2021
-
+## Revision 2021.10 October 2021
 
 ### Current Revision and Compile Order
 
 The following table lists the files and revision, starting with the
 files that need to be compiled first. Be sure to turn on the VHDL-2008
 compile switch. You may also use the OSVVM script - osvvm.pro -- details 
 how to run it are in the scripts directory as well as Scripts_user_guide.pdf.
@@ -66,32 +71,69 @@
   | NamePkg.vhd                                        | 2020.01  |  
   | NameStorePkg.vhd                                   | 2021.06  |  
   | OsvvmGlobalPkg.vhd                                 | 2020.01  |  
   | VendorCovApiPkg_Aldec.vhd (Aldec only)             | 2020.01  |
   | VendorCovApiPkg.vhd (All others)                   | 2020.01  |
   | TranscriptPkg.vhd                                  | 2020.12  |  
   | TextUtilPkg.vhd                                    | 2020.08  | 
-  | AlertLogPkg.vhd                                    | **2021.09**  | 
+  | AlertLogPkg.vhd                                    | 2021.10  | 
   | MessageListPkg.vhd                                 | 2021.07  | 
   | SortListPkg_int.vhd                                | 2020.01  |
   | RandomBasePkg.vhd                                  | 2021.06  |
   | RandomPkg.vhd                                      | 2021.06  |
   | RandomProcedurePkg.vhd                             | 2021.06  |
-  | CoveragePkg.vhd                                    | 2021.08  |
+  | CoveragePkg.vhd                                    | **2021.12**  |
   | MemoryPkg.vhd                                      | 2021.06  |
   | ScoreboardGenericPkg.vhd                           | 2021.08  |
   | ScoreboardPkg_slv.vhd                              | 2020.10  |
   | ScoreboardPkg_int.vhd                              | 2020.01  |
-  | ScoreboardPkg_slv_c.vhd                            | **2021.09**  |
-  | ScoreboardPkg_int_c.vhd                            | **2021.09**  |
+  | ScoreboardPkg_slv_c.vhd                            | 2021.09  |
+  | ScoreboardPkg_int_c.vhd                            | 2021.09  |
   | ResizePkg.vhd                                      | 2021.06  |
   | TbUtilPkg.vhd                                      | 2020.01  |
+  | ReportPkg.vhd                                      | 2021.10  | 
   | OsvvmContext.vhd                                   | 2020.01  |
 
+### CoveragePkg.vhd  2021.12 
+Added ReadCovYaml.
+
+
+## Revision 2021.11 November 2021
 
+### CoveragePkg.vhd  2021.11 
+Minor updates.  Print CovWeight first in WriteCovYaml. 
+Update to usage of PercentCov in GetCov. 
+
+## Revision 2021.10 October 2021
+
+### ReportPkg.vhd 2021.10 
+Implements EndOfTestReports (was called EndOfTestSummary in 2021.09).
+EndOfTestReports calls 
+   - ReportAlerts from AlertPkg,
+   - WriteAlertSummaryYaml from AlertPkg to generate Build Report <build>.yml,
+   - WriteAlertYaml from AlertPkg to generate ./reports/<test>_alerts.yml
+   - WriteCovYaml from CoveragePkg to generate ./reports/<test>_cov.yml
+See the OSVVM scripts as the above YAML files are all automatically converted to HTML.
+Make sure to name your tests with AlertLogPkg.SetAlertLogName as that is where the 
+above "<test>" comes from.   
+
+### AlertLogPkg.vhd 2021.10 
+Added WriteAlertYaml to create AlertLog reports in Yaml (which the scripts convert to HTML)
+WriteAlertSummaryYaml replaced the experimental CreateYamlReport.
+Both of the above are called by ReportPkg.EndOfTestReports.  See above.
+Deprecated Items:
+  - CreateYamlReport is deprecated.  Please use WriteAlertSummaryYaml.
+  - EndOfTestSummary was moved to ReportPkg and deprecated.   It is replaced by EndOfTestReports.
+    The move was necessary as it calls procedures from AlertLogPkg and CoveragePkg. 
+
+### CoveragePkg.vhd  2021.10 
+Added WriteCovYaml which is called by EndOfTestReports
+
+
+## Revision 2021.09 September 2021
 ### AlertLogPkg.vhd 2021.09 
 Experimental Release of EndOfTestSummary and CreateYamlReport
 
 ### CoveragePkg.vhd  2021.09 
 Minor update to WriteBin in CoveragePkg for setting parameters
 
 ### ScoreboardPkg_slv_c.vhd and ScoreboardPkg_int_c.vhd  2021.09
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/CONTRIBUTORS.md` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/CoveragePkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/CoveragePkg.vhd`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 --        SynthWorks Design Inc.
 --        VHDL Training Classes
 --        11898 SW 128th Ave.  Tigard, Or  97223
 --        http://www.SynthWorks.com
 --
 --  Revision History:
 --    Date      Version    Description
+--    11/2021   2021.11    Updated WriteCovYaml to write CovWeight first.   
+--                         Updated GetCov calculation with PercentCov.
+--    10/2021   2021.10    Added WriteCovYaml to write out coverage as a YAML file
 --    08/2021   2021.08    Removed SetAlertLogID from singleton public interface - set instead by NewID
 --                         Moved SetName, SetMessage to deprecated 
 --                         Moved AddBins, AddCross, GenBin, and GenCross with weight parameter to deprecated 
 --    07/2021   2021.07    Updated for new data structure
 --    07/2020   2020.07    Adjusted NextPointModeType:  Changed MIN to MODE_MINIMUM.
 --                         The preferred MINIMUM will not work in some tools
 --                         Added GetNext{Index, BinVal, Point}[(Mode => {RANDOM|INCREMENT|MODE_MINIMUM})]
@@ -75,15 +78,15 @@
 --      it was inappropriate to overload either textio write or to_string
 --      In the notes VHDL-2008 notes refers to
 --      composites with unconstrained elements
 --
 --
 --  This file is part of OSVVM.
 --
---  Copyright (c) 2010 - 2020 by SynthWorks Design Inc.
+--  Copyright (c) 2010 - 2021 by SynthWorks Design Inc.
 --
 --  Licensed under the Apache License, Version 2.0 (the "License");
 --  you may not use this file except in compliance with the License.
 --  You may obtain a copy of the License at
 --
 --      https://www.apache.org/licenses/LICENSE-2.0
 --
@@ -324,27 +327,40 @@
   impure function GetAlertLogID (ID : CoverageIDType) return AlertLogIDType ;
 
   ------------------------------------------------------------
 -- Name set by NewID
   impure function GetName         (ID : CoverageIDType) return String ;
   impure function GetCovModelName (ID : CoverageIDType) return String ;
   impure function GetNamePlus     (ID : CoverageIDType; prefix, suffix : string) return String ;
+  procedure SetItemBinNames (
+    ID         : CoverageIDType ;
+    Name1      : String ; 
+            Name2,  Name3,  Name4,  Name5, 
+    Name6,  Name7,  Name8,  Name9,  Name10, 
+    Name11, Name12, Name13, Name14, Name15, 
+    Name16, Name17, Name18, Name19, Name20 : string := ""
+  ) ;
+  alias SetFieldName is SetItemBinNames [CoverageIDType, 
+    string, string, string, string, string, string, string, string, string, string, 
+    string, string, string, string, string, string, string, string, string, string] ;                      
 
   procedure       SetCovTarget       (ID : CoverageIDType; Percent : real) ;
   impure function GetCovTarget       (ID : CoverageIDType) return real ;
   procedure       SetThresholding    (ID : CoverageIDType; A : boolean := TRUE ) ;
   procedure       SetCovThreshold    (ID : CoverageIDType; Percent : real) ;
   procedure       SetMerging         (ID : CoverageIDType; A : boolean := TRUE ) ;
   procedure       SetCountMode       (ID : CoverageIDType; A : CountModeType) ;
   procedure       SetIllegalMode     (ID : CoverageIDType; A : IllegalModeType) ;
   procedure       SetNextPointMode   (ID : CoverageIDType; A : NextPointModeType) ;
   -- 
   -- SetWeightMode with a WeightMode other than AT_LEAST or REMAIN is deprecated
   -- SetWeightMode with a WeightScale parameter is deprecated
   procedure       SetWeightMode      (ID : CoverageIDType; WeightMode : WeightModeType;  WeightScale : real := 1.0) ;
+  procedure       SetCovWeight       (ID : CoverageIDType; Weight : integer) ;
+  impure function GetCovWeight       (ID : CoverageIDType) return integer ;
 
   ------------------------------------------------------------
   -- Seeds are initialized by NewID.  
   procedure       InitSeed      (ID : CoverageIDType; S : string;  UseNewSeedMethods : boolean := TRUE) ;
   impure function InitSeed      (ID : CoverageIDType; S : string;  UseNewSeedMethods : boolean := TRUE ) return string ;
   procedure       InitSeed      (ID : CoverageIDType; I : integer; UseNewSeedMethods : boolean := TRUE ) ;
 
@@ -449,14 +465,16 @@
 
   impure function IsInitialized (ID : CoverageIDType) return boolean ;
 
   ------------------------------------------------------------
   impure function GetItemCount    (ID : CoverageIDType) return integer ;
   impure function GetCov          (ID : CoverageIDType; PercentCov : real ) return real ;
   impure function GetCov          (ID : CoverageIDType) return real ;
+  impure function GetTotalCovCount(ID : CoverageIDType; PercentCov : real ) return integer ;
+  impure function GetTotalCovCount(ID : CoverageIDType) return integer ;
   impure function GetTotalCovGoal (ID : CoverageIDType; PercentCov : real ) return integer ;
   impure function GetTotalCovGoal (ID : CoverageIDType) return integer ;
 
   ------------------------------------------------------------
   impure function GetMinCov   (ID : CoverageIDType) return real ;
   impure function GetMinCount (ID : CoverageIDType) return integer ;
   impure function GetMaxCov   (ID : CoverageIDType) return real ;
@@ -595,14 +613,26 @@
   --  Writing Out RAW Coverage Bin Information
   --  Note that read supports merging of coverage models
   -- /////////////////////////////////////////
   ------------------------------------------------------------
   procedure ReadCovDb  (ID : CoverageIDType; FileName : string; Merge : boolean := FALSE) ;
   procedure WriteCovDb (ID : CoverageIDType; FileName : string; OpenKind : File_Open_Kind := WRITE_MODE ) ;
   --     procedure WriteCovDb (ID : CoverageIDType) ;
+--  procedure WriteCovYaml (ID : CoverageIDType; FileName : string; OpenKind : File_Open_Kind := WRITE_MODE ) ;
+
+  ------------------------------------------------------------
+  -- /////////////////////////////////////////
+  --  Operations across all coverage models
+  -- /////////////////////////////////////////
+  ------------------------------------------------------------
+  procedure WriteCovYaml (FileName : string := ""; OpenKind : File_Open_Kind := WRITE_MODE) ;
+  procedure ReadCovYaml  (FileName : string := ""; Merge : boolean := FALSE) ;
+  impure function GotCoverage return boolean ;
+  impure function GetCov (PercentCov : real ) return real ;
+  impure function GetCov return real ;
 
 
   ------------------------------------------------------------
   -- Experimental.  Intended primarily for development.
   procedure CompareBins (
   ------------------------------------------------------------
     constant Bin1       : in    CoverageIDType ;
@@ -754,14 +784,15 @@
   --  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX  CovPType  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
   --  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX  CovPType  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
   --  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX  CovPType  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
   ------------------------------------------------------------------------------------------
   type CovPType is protected
     ------------------------------------------------------------
     impure function NewID (NameIn : String) return CoverageIDType ;
+    impure function GetNumIDs return integer ;
 
     ------------------------------------------------------------
     -- /////////////////////////////////////////
     --  Coverage Global Settings Common to All Coverage Models
     -- /////////////////////////////////////////
     ------------------------------------------------------------
     procedure FileOpenWriteBin (FileName : string; OpenKind : File_Open_Kind ) ;
@@ -789,28 +820,38 @@
     ------------------------------------------------------------
     procedure       SetName         (ID : CoverageIDType; Name : String) ;
     impure function SetName         (ID : CoverageIDType; Name : String) return string ;
     procedure       DeallocateName  (ID : CoverageIDType) ;
     impure function GetName         (ID : CoverageIDType) return String ;
     impure function GetCovModelName (ID : CoverageIDType) return String ;
     impure function GetNamePlus     (ID : CoverageIDType; prefix, suffix : string) return String ;
+    procedure SetItemBinNames (
+      ID         : CoverageIDType ;
+      Name1      : String ; 
+              Name2,  Name3,  Name4,  Name5, 
+      Name6,  Name7,  Name8,  Name9,  Name10, 
+      Name11, Name12, Name13, Name14, Name15, 
+      Name16, Name17, Name18, Name19, Name20 : string := ""
+    ) ;
 
     ------------------------------------------------------------
     procedure       SetMessage         (ID : CoverageIDType; Message : String) ;
     procedure       DeallocateMessage  (ID : CoverageIDType) ;
 
     procedure       SetCovTarget       (ID : CoverageIDType; Percent : real) ;
     impure function GetCovTarget       (ID : CoverageIDType) return real ;
     procedure       SetThresholding    (ID : CoverageIDType; A : boolean := TRUE ) ;
     procedure       SetCovThreshold    (ID : CoverageIDType; Percent : real) ;
     procedure       SetMerging         (ID : CoverageIDType; A : boolean := TRUE ) ;
     procedure       SetCountMode       (ID : CoverageIDType; A : CountModeType) ;
     procedure       SetIllegalMode     (ID : CoverageIDType; A : IllegalModeType) ;
     procedure       SetWeightMode      (ID : CoverageIDType; WeightMode : WeightModeType;  WeightScale : real := 1.0) ;
     procedure       SetNextPointMode   (ID : CoverageIDType; A : NextPointModeType) ;
+    procedure       SetCovWeight       (ID : CoverageIDType; Weight : integer) ;
+    impure function GetCovWeight       (ID : CoverageIDType) return integer ;
 
     ------------------------------------------------------------
     procedure       SetAlertLogID (ID : CoverageIDType; A : AlertLogIDType) ;
     procedure       SetAlertLogID (ID : CoverageIDType; Name : string ; ParentID : AlertLogIDType := ALERTLOG_BASE_ID ; CreateHierarchy : Boolean := TRUE) ;
     impure function GetAlertLogID (ID : CoverageIDType) return AlertLogIDType ;
 
     ------------------------------------------------------------
@@ -944,16 +985,20 @@
     impure function IsCovered     (ID : CoverageIDType; PercentCov : real ) return boolean ;
     impure function IsCovered     (ID : CoverageIDType) return boolean ;
 
     impure function IsInitialized (ID : CoverageIDType) return boolean ;
 
     ------------------------------------------------------------
     impure function GetItemCount    (ID : CoverageIDType) return integer ;
+    procedure GetTotalCovCountAndGoal     (ID : CoverageIDType; PercentCov : real; TotalCovCount : out integer; TotalCovGoal : out integer ) ;
+    procedure GetTotalCovCountAndGoal     (ID : CoverageIDType; TotalCovCount : out integer; TotalCovGoal : out integer ) ;
     impure function GetCov          (ID : CoverageIDType; PercentCov : real ) return real ;
     impure function GetCov          (ID : CoverageIDType) return real ;
+    impure function GetTotalCovCount(ID : CoverageIDType; PercentCov : real ) return integer ;
+    impure function GetTotalCovCount(ID : CoverageIDType) return integer ;
     impure function GetTotalCovGoal (ID : CoverageIDType; PercentCov : real ) return integer ;
     impure function GetTotalCovGoal (ID : CoverageIDType) return integer ;
 
     ------------------------------------------------------------
     impure function GetMinCov   (ID : CoverageIDType) return real ;
     impure function GetMinCount (ID : CoverageIDType) return integer ;
     impure function GetMaxCov   (ID : CoverageIDType) return real ;
@@ -1095,14 +1140,18 @@
     --  Writing Out RAW Coverage Bin Information
     --  Note that read supports merging of coverage models
     -- /////////////////////////////////////////
     ------------------------------------------------------------
     procedure ReadCovDb  (ID : CoverageIDType; FileName : string; Merge : boolean := FALSE) ;
     procedure WriteCovDb (ID : CoverageIDType; FileName : string; OpenKind : File_Open_Kind := WRITE_MODE ) ;
     --     procedure WriteCovDb (ID : CoverageIDType) ;
+--    procedure WriteCovYaml (ID : CoverageIDType; FileName : string; OpenKind : File_Open_Kind := WRITE_MODE ) ;
+    procedure WriteCovYaml (FileName : string := ""; Coverage : real ; OpenKind : File_Open_Kind := WRITE_MODE) ;
+    procedure ReadCovYaml  (FileName : string := ""; Merge : boolean := FALSE) ;
+    impure function GotCoverage return boolean ;
 
 
   ------------------------------------------------------------
   -- /////////////////////////////////////////
   -- /////////////////////////////////////////
   -- Compatibility Methods - Allows CoveragePkg to Work as a PT still
   -- /////////////////////////////////////////
@@ -1239,14 +1288,16 @@
     impure function IsCovered ( PercentCov : real ) return boolean ;
     impure function IsInitialized return boolean ;
 
     ------------------------------------------------------------
     impure function GetItemCount return integer ;
     impure function GetCov ( PercentCov : real ) return real ;
     impure function GetCov return real ; -- PercentCov of entire model/all bins
+    impure function GetTotalCovCount ( PercentCov : real ) return integer ;
+    impure function GetTotalCovCount return integer ;
     impure function GetTotalCovGoal ( PercentCov : real ) return integer ;
     impure function GetTotalCovGoal return integer ;
 
     ------------------------------------------------------------
     impure function GetMinCov return real ;       -- PercentCov
     impure function GetMinCount return integer ;  -- Count
     impure function GetMaxCov return real ;       -- PercentCov
@@ -1611,14 +1662,26 @@
 
 --- ///////////////////////////////////////////////////////////////////////////
 --- ///////////////////////////////////////////////////////////////////////////
 --- ///////////////////////////////////////////////////////////////////////////
 
 package body CoveragePkg is
   ------------------------------------------------------------
+  --  package local
+  function ActionToName(Action : integer) return string is 
+  ------------------------------------------------------------
+  begin 
+    case Action is
+      when 1 =>        return "COUNT" ;
+      when 0 =>        return "IGNORE"  ;
+      when others =>   return "ILLEGAL" ;
+    end case ; 
+  end function ActionToName ; 
+
+  ------------------------------------------------------------
   function inside (
   -- package local
   ------------------------------------------------------------
     CovPoint : integer_vector ;
     BinVal   : RangeArrayType
   ) return boolean is
     alias iCovPoint : integer_vector(BinVal'range) is CovPoint ;
@@ -2038,15 +2101,15 @@
 
   ------------------------------------------------------------------------------------------
   --  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX  CovPType  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
   --  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX  CovPType  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
   --  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX  CovPType  XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
   ------------------------------------------------------------------------------------------
   type CovPType is protected body
-
+    constant COV_READ_YAML_ALERT_LEVEL : AlertType := ERROR ;
 
     ------------------------------------------------------------
     -- Global Settings for Coverage Modeling
     -- Local WriteBin and WriteCovHoles formatting settings, defaults determined by CoverageGlobals
     variable WritePassFailVar   : OsvvmOptionsType := COV_OPT_INIT_PARM_DETECT ;
     variable WriteBinInfoVar    : OsvvmOptionsType := COV_OPT_INIT_PARM_DETECT ;
     variable WriteCountVar      : OsvvmOptionsType := COV_OPT_INIT_PARM_DETECT ;
@@ -2062,36 +2125,41 @@
 
     ------------------------------------------------------------
     -- /////////////////////////////////////////
     -- CoverageBin Data Structures
     -- /////////////////////////////////////////
     type RangeArrayPtrType is access RangeArrayType ;
 
-    type CovBinBaseTempType is record
+    type CovBinInternalBaseType is record
       BinVal        : RangeArrayPtrType ;
       Action        : integer ;
       Count         : integer ;
       AtLeast       : integer ;
       Weight        : integer ;
       PercentCov    : real ;
       Name          : line ;
-    end record CovBinBaseTempType ;
-    type CovBinTempType is array (natural range <>) of CovBinBaseTempType ;
-    type CovBinPtrType is access CovBinTempType ;
+    end record CovBinInternalBaseType ;
+    type CovBinInternalType is array (natural range <>) of CovBinInternalBaseType ;
+    type CovBinPtrType is access CovBinInternalType ;
+    
+    type FieldNameArrayType is array (natural range <>) of Line ;
+    type FieldNameArrayPtrType is access FieldNameArrayType ;
 
     ------------------------------------------------------------
     -- /////////////////////////////////////////
     -- Coverage Information and Settings Structure
     -- /////////////////////////////////////////
     type CovStructType is record
       --  Coverage Bin Structure
       CovBinPtr          : CovBinPtrType ;
       CovName            : line ;
       NumBins            : integer ;
       BinValLength       : integer ;
+      FieldName          : FieldNameArrayPtrType ; 
+      CovWeight          : integer ; -- Set GetCov for entire model
 
       CovMessage         : MessageStructPtrType ;
       VendorCovHandle    : VendorCovHandleType ;
 
       --  Statistics and History
       ItemCount          : integer ;  -- Count of randomizations
       LastIndex          : integer ;  -- Index of last Stimulus Gen or Coverage Collection
@@ -2121,14 +2189,16 @@
     variable COV_STRUCT_INIT : CovStructType :=
       (
         --  Coverage Bin Structure
         CovBinPtr          =>  NULL,
         CovName            =>  NULL,
         NumBins            =>  0,
         BinValLength       =>  1,
+        FieldName          =>  NULL,
+        CovWeight          =>  1,
 
         CovMessage         =>  NULL,
         VendorCovHandle    =>  0,
 
         --  Statistics and History
         ItemCount          =>  0,   -- Count of randomizations
         LastIndex          =>  1,   -- Index of last Stimulus Gen or Coverage Collection
@@ -2207,30 +2277,46 @@
     end procedure GrowNumberItems ;
 
     ------------------------------------------------------------
     impure function NewID (NameIn : String) return CoverageIDType is
     ------------------------------------------------------------
       variable NewNumItems : integer ;
       variable NewCoverageID : CoverageIDType ;
+      variable NameID : integer ; 
     begin
-      NewNumItems   := NumItems + 1 ;
-      GrowNumberItems(CovStructPtr, NewNumItems, NumItems, MIN_NUM_ITEMS) ;
-      NumItems      := NewNumItems ;
-      CovStructPtr(NumItems) := COV_STRUCT_INIT ;
-      NewCoverageID := (ID => NumItems) ;
-      InitSeed( NewCoverageID, NameIn) ;
-      SetName( NewCoverageID, NameIn) ;
-      SetAlertLogID(NewCoverageID, NameIn, OSVVM_COVERAGE_ALERTLOG_ID, FALSE) ; 
---      CovStructPtr(NumItems).AlertLogID := OSVVM_COVERAGE_ALERTLOG_ID ;
---!!
---!!  Set name for each Coverage Point.
---!!
-      return NewCoverageID ;
+      NameID := LocalNameStore.find(NameIn) ; 
+      if NameID /= ID_NOT_FOUND.ID then 
+        NewCoverageID := (ID => NameID) ;
+        SetName(NewCoverageID, NameIn) ;
+        return NewCoverageID ; 
+      else
+        NewNumItems   := NumItems + 1 ;
+        GrowNumberItems(CovStructPtr, NewNumItems, NumItems, MIN_NUM_ITEMS) ;
+        NumItems      := NewNumItems ;
+        NameID := LocalNameStore.NewID(NameIn) ;
+        CovStructPtr(NumItems) := COV_STRUCT_INIT ;
+        NewCoverageID := (ID => NumItems) ;
+        InitSeed( NewCoverageID, NameIn) ;
+        SetName( NewCoverageID, NameIn) ;
+        SetAlertLogID(NewCoverageID, NameIn, OSVVM_COVERAGE_ALERTLOG_ID, FALSE) ; 
+  --      CovStructPtr(NumItems).AlertLogID := OSVVM_COVERAGE_ALERTLOG_ID ;
+  --!!
+  --!!  Set name for each Coverage Point.
+  --!!
+        return NewCoverageID ;
+      end if ; 
     end function NewID ;
-
+    
+    ------------------------------------------------------------
+    impure function GetNumIDs return integer is
+    ------------------------------------------------------------
+    begin
+      return NumItems ;
+    end function GetNumIDs ;
+    
     ------------------------------------------------------------
     -- /////////////////////////////////////////
     --  Coverage Global Settings Common to All Coverage Models
     -- /////////////////////////////////////////
     ------------------------------------------------------------
     procedure FileOpenWriteBin (FileName : string; OpenKind : File_Open_Kind ) is
     ------------------------------------------------------------
@@ -2413,19 +2499,22 @@
     procedure SetName (ID : CoverageIDType; Name : String) is
     ------------------------------------------------------------
     begin
       if CovStructPtr(ID.ID).CovName /= NULL then
         deallocate (CovStructPtr(ID.ID).CovName) ;
       end if;
       CovStructPtr(ID.ID).CovName := new string'(Name) ;
+      
       -- Update if name updated after model created                      -- VendorCov
       if IsInitialized(ID) then                                          -- VendorCov
         VendorCovSetName(CovStructPtr(ID.ID).VendorCovHandle, Name) ;    -- VendorCov
       end if ;                                                           -- VendorCov
-      if not CovStructPtr(ID.ID).RvSeedInit then  -- Init seed if not initialized
+      
+      -- Init seed if not already initialized
+      if not CovStructPtr(ID.ID).RvSeedInit then  
         InitSeed(ID, Name) ;
         CovStructPtr(ID.ID).RvSeedInit := TRUE ;
       end if ;
     end procedure SetName ;
 
     ------------------------------------------------------------
     impure function SetName (ID : CoverageIDType; Name : String) return string is
@@ -2480,14 +2569,107 @@
         return prefix & GetWord(CovStructPtr(ID.ID).CovMessage.Name.all) & suffix ;
       else
         return "" ;
       end if ;
     end function GetNamePlus ;
 
     ------------------------------------------------------------
+    -- PT Local
+    impure function NewNamePtr(Name : string) return Line is 
+    ------------------------------------------------------------
+    begin
+      if Name /= "" then
+        return new string'(Name) ;
+      else
+        return NULL ;
+      end if; 
+    end function NewNamePtr ; 
+
+--    ------------------------------------------------------------
+--    -- pt local
+--    procedure CheckBinValLength(ID : CoverageIDType; CurBinValLength : integer ; Caller : string ) is
+--    ------------------------------------------------------------
+--    begin
+--      if CovStructPtr(ID.ID).NumBins = 0 then
+--        CovStructPtr(ID.ID).BinValLength := CurBinValLength ; -- number of points in cross
+--      else
+--        AlertIfNotEqual(CovStructPtr(ID.ID).AlertLogID, CovStructPtr(ID.ID).BinValLength, CurBinValLength, GetNamePlus(ID, prefix => "in ", suffix => ", ") & "CoveragePkg." & Caller & ":" &
+--        " Cross coverage bins of different dimensions prohibited", FAILURE) ;
+--      end if;
+--    end procedure CheckBinValLength ;
+
+    ------------------------------------------------------------
+    -- pt local
+    impure function BinValLengthNotEqual(ID : CoverageIDType; CurBinValLength : integer) return boolean is
+    ------------------------------------------------------------
+    begin
+      if CovStructPtr(ID.ID).NumBins = 0 then
+        CovStructPtr(ID.ID).BinValLength := CurBinValLength ; 
+        return FALSE ;
+      else
+        return CurBinValLength /= CovStructPtr(ID.ID).BinValLength ;
+      end if;
+    end function BinValLengthNotEqual ;
+
+    ------------------------------------------------------------
+    procedure SetItemBinNames (
+    ------------------------------------------------------------
+      ID         : CoverageIDType ;
+      Name1      : String ; 
+              Name2,  Name3,  Name4,  Name5, 
+      Name6,  Name7,  Name8,  Name9,  Name10, 
+      Name11, Name12, Name13, Name14, Name15, 
+      Name16, Name17, Name18, Name19, Name20 : string := ""
+    ) is
+      variable NamePtr : Line ; 
+      variable FieldNameArray : FieldNameArrayType(1 to 20) ; 
+      variable Dimensions : integer := 0 ;
+    begin
+      -- Support names for up to a cross of 20
+      for i in 1 to 20 loop 
+        if CovStructPtr(ID.ID).FieldName /= NULL then
+          for i in 1 to CovStructPtr(ID.ID).FieldName'length loop 
+            deallocate (CovStructPtr(ID.ID).FieldName(i)) ; 
+          end loop ;
+          deallocate (CovStructPtr(ID.ID).FieldName) ;
+        end if;
+        case i is
+          when  1 =>  NamePtr := NewNamePtr(Name1) ;
+          when  2 =>  NamePtr := NewNamePtr(Name2) ;
+          when  3 =>  NamePtr := NewNamePtr(Name3) ;
+          when  4 =>  NamePtr := NewNamePtr(Name4) ;
+          when  5 =>  NamePtr := NewNamePtr(Name5) ;
+          when  6 =>  NamePtr := NewNamePtr(Name6) ;
+          when  7 =>  NamePtr := NewNamePtr(Name7) ;
+          when  8 =>  NamePtr := NewNamePtr(Name8) ;
+          when  9 =>  NamePtr := NewNamePtr(Name9) ;
+          when 10 =>  NamePtr := NewNamePtr(Name10) ;
+          when 11 =>  NamePtr := NewNamePtr(Name11) ;
+          when 12 =>  NamePtr := NewNamePtr(Name12) ;
+          when 13 =>  NamePtr := NewNamePtr(Name13) ;
+          when 14 =>  NamePtr := NewNamePtr(Name14) ;
+          when 15 =>  NamePtr := NewNamePtr(Name15) ;
+          when 16 =>  NamePtr := NewNamePtr(Name16) ;
+          when 17 =>  NamePtr := NewNamePtr(Name17) ;
+          when 18 =>  NamePtr := NewNamePtr(Name18) ;
+          when 19 =>  NamePtr := NewNamePtr(Name19) ;
+          when 20 =>  NamePtr := NewNamePtr(Name20) ;
+        end case ; 
+        exit when NamePtr = NULL ; 
+        FieldNameArray(i) := NamePtr ; 
+        Dimensions := i ; 
+      end loop ;
+      CovStructPtr(ID.ID).FieldName := new FieldNameArrayType'(FieldNameArray(1 to Dimensions)) ;
+      -- Check that Dimensions match bin dimensions    
+      if BinValLengthNotEqual(ID, Dimensions) then 
+        Alert(CovStructPtr(ID.ID).AlertLogID, "CoveragePkg.SetItemBinNames: Coverage bins of different dimensions prohibited", FAILURE) ;
+      end if ;
+    end procedure SetItemBinNames ;
+
+    ------------------------------------------------------------
     procedure SetMessage (ID : CoverageIDType; Message : String) is
     ------------------------------------------------------------
     begin
       SetMessage(CovStructPtr(ID.ID).CovMessage, Message) ;
       -- VendorCov update if name updated after model created
       if IsInitialized(ID) then                                       -- VendorCov
         -- Refine this?   If CovName or AlertLogID is set,            -- VendorCov
@@ -2619,47 +2801,49 @@
       end if;
       if WeightScale <= 0.0 then
         Alert(CovStructPtr(ID.ID).AlertLogID, GetNamePlus(ID, prefix => "in ", suffix => ", ") & "CoveragePkg.SetWeightMode:" &
                       " WeightScale must be > 0.0", FAILURE) ;
         CovStructPtr(ID.ID).WeightScale := 1.0 ;
       end if;
     end procedure SetWeightMode ;
+    
+    ------------------------------------------------------------
+    procedure SetCovWeight (ID : CoverageIDType; Weight : integer) is
+    ------------------------------------------------------------
+    begin
+      CovStructPtr(ID.ID).CovWeight := Weight ;
+    end procedure SetCovWeight ;
+
+    ------------------------------------------------------------
+    impure function GetCovWeight (ID : CoverageIDType) return integer is
+    ------------------------------------------------------------
+    begin
+      return CovStructPtr(ID.ID).CovWeight ;
+    end function GetCovWeight ;
 
     ------------------------------------------------------------
     procedure SetBinSize (ID : CoverageIDType; NewNumBins : integer) is
     -- Sets a CovBin to a particular size
     -- Use for small bins to save space or large bins to
     -- suppress the resize and copy as a CovBin autosizes.
     ------------------------------------------------------------
       variable oldCovBinPtr : CovBinPtrType ;
     begin
       if CovStructPtr(ID.ID).CovBinPtr = NULL then
-        CovStructPtr(ID.ID).CovBinPtr := new CovBinTempType(1 to NewNumBins) ;
+        CovStructPtr(ID.ID).CovBinPtr := new CovBinInternalType(1 to NewNumBins) ;
       elsif NewNumBins > CovStructPtr(ID.ID).CovBinPtr'length then
         -- make message bigger
         oldCovBinPtr := CovStructPtr(ID.ID).CovBinPtr ;
-        CovStructPtr(ID.ID).CovBinPtr := new CovBinTempType(1 to NewNumBins) ;
+        CovStructPtr(ID.ID).CovBinPtr := new CovBinInternalType(1 to NewNumBins) ;
         CovStructPtr(ID.ID).CovBinPtr.all(1 to CovStructPtr(ID.ID).NumBins) := oldCovBinPtr.all(1 to CovStructPtr(ID.ID).NumBins) ;
         deallocate(oldCovBinPtr) ;
       end if ;
     end procedure SetBinSize ;
 
     ------------------------------------------------------------
-    -- pt local
-    procedure CheckBinValLength(ID : CoverageIDType; CurBinValLength : integer ; Caller : string ) is
-    begin
-      if CovStructPtr(ID.ID).NumBins = 0 then
-        CovStructPtr(ID.ID).BinValLength := CurBinValLength ; -- number of points in cross
-      else
-        AlertIfNotEqual(CovStructPtr(ID.ID).AlertLogID, CovStructPtr(ID.ID).BinValLength, CurBinValLength, GetNamePlus(ID, prefix => "in ", suffix => ", ") & "CoveragePkg." & Caller & ":" &
-        " Cross coverage bins of different dimensions prohibited", FAILURE) ;
-      end if;
-    end procedure CheckBinValLength ;
-
-    ------------------------------------------------------------
     --  pt local
     impure function NormalizeNumBins(ID : CoverageIDType; ReqNumBins : integer ) return integer is
       variable NormNumBins : integer := MIN_NUM_BINS ;
     begin
       while NormNumBins < ReqNumBins loop
         NormNumBins := NormNumBins + MIN_NUM_BINS ;
       end loop ;
@@ -2670,19 +2854,19 @@
     --  pt local
     procedure GrowBins (ID : CoverageIDType; ReqNumBins : integer) is
       variable oldCovBinPtr : CovBinPtrType ;
       variable NewNumBins   : integer ;
     begin
       NewNumBins := CovStructPtr(ID.ID).NumBins + ReqNumBins ;
       if CovStructPtr(ID.ID).CovBinPtr = NULL then
-        CovStructPtr(ID.ID).CovBinPtr := new CovBinTempType(1 to NormalizeNumBins(ID, NewNumBins)) ;
+        CovStructPtr(ID.ID).CovBinPtr := new CovBinInternalType(1 to NormalizeNumBins(ID, NewNumBins)) ;
       elsif NewNumBins > CovStructPtr(ID.ID).CovBinPtr'length then
         -- make message bigger
         oldCovBinPtr := CovStructPtr(ID.ID).CovBinPtr ;
-        CovStructPtr(ID.ID).CovBinPtr := new CovBinTempType(1 to NormalizeNumBins(ID, NewNumBins)) ;
+        CovStructPtr(ID.ID).CovBinPtr := new CovBinInternalType(1 to NormalizeNumBins(ID, NewNumBins)) ;
         CovStructPtr(ID.ID).CovBinPtr.all(1 to CovStructPtr(ID.ID).NumBins) := oldCovBinPtr.all(1 to CovStructPtr(ID.ID).NumBins) ;
         deallocate(oldCovBinPtr) ;
       end if ;
     end procedure GrowBins ;
 
     ------------------------------------------------------------
     --  pt local, called by InsertBin
@@ -2833,15 +3017,18 @@
       AtLeast : integer ;
       Weight  : integer ;
       CovBin  : CovBinType
     ) is
       variable vCalcAtLeast : integer ;
       variable vCalcWeight  : integer ;
     begin
-      CheckBinValLength(ID, 1, "AddBins") ;
+      if BinValLengthNotEqual(ID, 1) then 
+        Alert(CovStructPtr(ID.ID).AlertLogID, "CoveragePkg.AddBins: Coverage bins of different dimensions prohibited", FAILURE) ;
+        return ; 
+      end if ;
 
       GrowBins(ID, CovBin'length) ;
       for i in CovBin'range loop
         if CovBin(i).Action = COV_COUNT then
           vCalcAtLeast := maximum(AtLeast, CovBin(i).AtLeast) ;
           vCalcWeight  := maximum(Weight, CovBin(i).Weight) ;
         else
@@ -2913,15 +3100,18 @@
            ) ;
       constant NUM_NEW_BINS : integer := CalcNumCrossBins(BIN_LENS) ;
       variable BinIndex     : integer_vector(1 to BIN_LENS'length) := (others => 1) ;
       variable CrossBins    : CovBinType(BinIndex'range) ;
       variable vCalcAction, vCalcCount, vCalcAtLeast, vCalcWeight : integer ;
       variable vCalcBinVal   : RangeArrayType(BinIndex'range) ;
     begin
-      CheckBinValLength(ID, BIN_LENS'length, "AddCross") ;
+      if BinValLengthNotEqual(ID, BIN_LENS'length) then 
+        Alert(CovStructPtr(ID.ID).AlertLogID, "CoveragePkg.AddCross: Cross coverage bins of different dimensions prohibited", FAILURE) ;
+        return ; 
+      end if ;
 
       GrowBins(ID, NUM_NEW_BINS) ;
       vCalcCount := 0 ;
       for MatrixIndex in 1 to NUM_NEW_BINS loop
         CrossBins := ConcatenateBins(BinIndex,
              Bin1, Bin2, Bin3, Bin4, Bin5, Bin6, Bin7, Bin8, Bin9, Bin10, Bin11,
              Bin12, Bin13, Bin14, Bin15, Bin16, Bin17, Bin18, Bin19, Bin20
@@ -3013,59 +3203,69 @@
       AddCross(ID, "", 0, 0,
            Bin1, Bin2, Bin3, Bin4, Bin5, Bin6, Bin7, Bin8, Bin9, Bin10, Bin11,
            Bin12, Bin13, Bin14, Bin15, Bin16, Bin17, Bin18, Bin19, Bin20
         ) ;
     end procedure AddCross ;
 
     ------------------------------------------------------------
+    procedure DeallocateBins(CoverID : CoverageIDType) is
+    ------------------------------------------------------------
+      constant Index   : integer := CoverID.ID ; 
+    begin
+      -- Local for a particular CoverageModel
+      if CovStructPtr(Index).CovBinPtr /= NULL then
+        for i in 1 to CovStructPtr(Index).NumBins loop
+          deallocate(CovStructPtr(Index).CovBinPtr(i).BinVal) ;
+          deallocate(CovStructPtr(Index).CovBinPtr(i).Name) ;
+        end loop ;
+        deallocate(CovStructPtr(Index).CovBinPtr) ;
+      end if ; 
+      CovStructPtr(Index).NumBins := 0 ;
+    end procedure DeallocateBins ;
+    
+    ------------------------------------------------------------
     procedure Deallocate(ID : CoverageIDType) is
     ------------------------------------------------------------
+      constant Index   : integer := ID.ID ; 
     begin
 --!!?? These are only done when removing all coverage models.
 --      -- Globals - for all coverage models
 --      WritePassFailVar   := COV_OPT_INIT_PARM_DETECT ;
 --      WriteBinInfoVar    := COV_OPT_INIT_PARM_DETECT ;
 --      WriteCountVar      := COV_OPT_INIT_PARM_DETECT ;
 --      WriteAnyIllegalVar := COV_OPT_INIT_PARM_DETECT ;
 --      WritePrefixVar.deallocate ;
 --      PassNameVar.deallocate ;
 --      FailNameVar.deallocate ;
-
-      -- Local for a particular CoverageModel
-      for i in 1 to CovStructPtr(ID.ID).NumBins loop
-        deallocate(CovStructPtr(ID.ID).CovBinPtr(i).BinVal) ;
-        deallocate(CovStructPtr(ID.ID).CovBinPtr(i).Name) ;
-      end loop ;
-      deallocate(CovStructPtr(ID.ID).CovBinPtr) ;
+      DeallocateBins(ID) ; 
       DeallocateName(ID) ;
       DeallocateMessage(ID) ;
       -- Restore internal variables to their default values
---      CovStructPtr(ID.ID) := COV_STRUCT_INIT ;
+--      CovStructPtr(Index) := COV_STRUCT_INIT ;
 
-      CovStructPtr(ID.ID).NumBins            := 0 ;
-      CovStructPtr(ID.ID).BinValLength       := 1 ;
-      CovStructPtr(ID.ID).VendorCovHandle    := 0 ;
-      CovStructPtr(ID.ID).ItemCount          := 0 ;
-      CovStructPtr(ID.ID).LastIndex          := 1 ;
-      CovStructPtr(ID.ID).LastStimGenIndex   := 1 ;
+      CovStructPtr(Index).BinValLength       := 1 ;
+      CovStructPtr(Index).VendorCovHandle    := 0 ;
+      CovStructPtr(Index).ItemCount          := 0 ;
+      CovStructPtr(Index).LastIndex          := 1 ;
+      CovStructPtr(Index).LastStimGenIndex   := 1 ;
       
       -- Changing these is beyond what deallocate should do.
-      CovStructPtr(ID.ID).NextPointMode      := RANDOM ;
-      CovStructPtr(ID.ID).IllegalMode        := ILLEGAL_ON ;
-      CovStructPtr(ID.ID).IllegalModeLevel   := ERROR ;
-      CovStructPtr(ID.ID).WeightMode         := AT_LEAST ;
-      CovStructPtr(ID.ID).WeightScale        := 1.0 ;
-      CovStructPtr(ID.ID).ThresholdingEnable := FALSE ;
-      CovStructPtr(ID.ID).CovThreshold       := 45.0 ;
-      CovStructPtr(ID.ID).CovTarget          := 100.0 ;
-      CovStructPtr(ID.ID).MergingEnable      := FALSE ;
-      CovStructPtr(ID.ID).CountMode          := COUNT_FIRST ;
---      CovStructPtr(ID.ID).RV                 := (1, 7) ;
---      CovStructPtr(ID.ID).RvSeedInit         := FALSE ;
---      CovStructPtr(ID.ID).AlertLogID         := OSVVM_COVERAGE_ALERTLOG_ID ;
+      CovStructPtr(Index).NextPointMode      := RANDOM ;
+      CovStructPtr(Index).IllegalMode        := ILLEGAL_ON ;
+      CovStructPtr(Index).IllegalModeLevel   := ERROR ;
+      CovStructPtr(Index).WeightMode         := AT_LEAST ;
+      CovStructPtr(Index).WeightScale        := 1.0 ;
+      CovStructPtr(Index).ThresholdingEnable := FALSE ;
+      CovStructPtr(Index).CovThreshold       := 45.0 ;
+      CovStructPtr(Index).CovTarget          := 100.0 ;
+      CovStructPtr(Index).MergingEnable      := FALSE ;
+      CovStructPtr(Index).CountMode          := COUNT_FIRST ;
+--      CovStructPtr(Index).RV                 := (1, 7) ;
+--      CovStructPtr(Index).RvSeedInit         := FALSE ;
+--      CovStructPtr(Index).AlertLogID         := OSVVM_COVERAGE_ALERTLOG_ID ;
 
     end procedure deallocate ;
 
     ------------------------------------------------------------
     -- Local
     procedure ICoverIndex(ID : CoverageIDType; Index : integer ; CovPoint : integer_vector ) is
     ------------------------------------------------------------
@@ -3076,15 +3276,16 @@
       VendorCovBinInc(CovStructPtr(ID.ID).VendorCovHandle, Index);   -- VendorCov
       CovStructPtr(ID.ID).CovBinPtr(Index).PercentCov := CalcPercentCov(
           Count => CovStructPtr(ID.ID).CovBinPtr.all(Index).Count,
           AtLeast =>  CovStructPtr(ID.ID).CovBinPtr.all(Index).AtLeast
         ) ;
       if CovStructPtr(ID.ID).CovBinPtr(Index).action = COV_ILLEGAL then
         if CovStructPtr(ID.ID).IllegalMode /= ILLEGAL_OFF then
-          if CovPoint = NULL_INTV then
+--          if CovPoint = NULL_INTV then
+          if CovPoint'length = 0 then
             alert(CovStructPtr(ID.ID).AlertLogID, GetNamePlus(ID, prefix => "in ", suffix => ", ") & "CoveragePkg.ICoverLast:" &
                           " Value randomized is in an illegal bin.", CovStructPtr(ID.ID).IllegalModeLevel) ;
           else
             write(buf, CovPoint) ;
             alert(CovStructPtr(ID.ID).AlertLogID, GetNamePlus(ID, prefix => "in ", suffix => ", ") & "CoveragePkg.ICover:" &
                           " Value " & buf.all & " is in an illegal bin.", CovStructPtr(ID.ID).IllegalModeLevel) ;
             deallocate(buf) ;
@@ -3230,69 +3431,100 @@
     ------------------------------------------------------------
     begin
       -- AlertIf(CovStructPtr(ID.ID).NumBins < 1, OSVVM_COVERAGE_ALERTLOG_ID, "CoveragePkg.IsCovered: Empty Coverage Model", failure) ;
       return CountCovHoles(ID, CovStructPtr(ID.ID).CovTarget) = 0 ;
     end function IsCovered ;
 
     ------------------------------------------------------------
-    impure function GetCov (ID : CoverageIDType; PercentCov : real ) return real is
+    procedure GetTotalCovCountAndGoal (ID : CoverageIDType; PercentCov : real; TotalCovCount : out integer; TotalCovGoal : out integer ) is
     ------------------------------------------------------------
-      variable TotalCovGoal, TotalCovCount, ScaledCovGoal : integer := 0 ;
+      variable ScaledCovGoal : integer := 0 ;
     begin
+      TotalCovCount := 0 ; 
+      TotalCovGoal  := 0 ; 
       BinLoop : for i in 1 to CovStructPtr(ID.ID).NumBins loop
         if CovStructPtr(ID.ID).CovBinPtr(i).action = COV_COUNT then
           ScaledCovGoal := integer(ceil(PercentCov * real(CovStructPtr(ID.ID).CovBinPtr(i).AtLeast)/100.0)) ;
           TotalCovGoal := TotalCovGoal + ScaledCovGoal ;
           if CovStructPtr(ID.ID).CovBinPtr(i).Count <= ScaledCovGoal then
             TotalCovCount := TotalCovCount + CovStructPtr(ID.ID).CovBinPtr(i).Count ;
           else
             -- do not count the extra values that exceed their cov goal
             TotalCovCount := TotalCovCount + ScaledCovGoal ;
           end if ;
         end if ;
       end loop BinLoop ;
-      return 100.0 * real(TotalCovCount) / real(TotalCovGoal) ;
+    end procedure GetTotalCovCountAndGoal ;
+
+    ------------------------------------------------------------
+    procedure GetTotalCovCountAndGoal (ID : CoverageIDType; TotalCovCount : out integer; TotalCovGoal : out integer ) is
+    ------------------------------------------------------------
+    begin
+      GetTotalCovCountAndGoal(ID, CovStructPtr(ID.ID).CovTarget, TotalCovCount, TotalCovGoal) ; 
+    end procedure GetTotalCovCountAndGoal ;
+
+    ------------------------------------------------------------
+    impure function GetCov (ID : CoverageIDType; PercentCov : real ) return real is
+    ------------------------------------------------------------
+      variable TotalCovCount, TotalCovGoal : integer ;
+    begin
+      GetTotalCovCountAndGoal(ID, PercentCov, TotalCovCount, TotalCovGoal) ; 
+      if TotalCovGoal > 0 then 
+        return 100.0 * real(TotalCovCount) / real(TotalCovGoal) ;
+      else
+        return 0.0 ; 
+      end if ; 
     end function GetCov ;
 
     ------------------------------------------------------------
     impure function GetCov (ID : CoverageIDType) return real is
     ------------------------------------------------------------
-      variable TotalCovGoal, TotalCovCount : integer := 0 ;
     begin
       return GetCov(ID, CovStructPtr(ID.ID).CovTarget ) ;
     end function GetCov ;
 
     ------------------------------------------------------------
-    impure function GetItemCount (ID : CoverageIDType) return integer is
+    impure function GetTotalCovCount (ID : CoverageIDType; PercentCov : real ) return integer is
     ------------------------------------------------------------
+      variable TotalCovCount, TotalCovGoal : integer ;
     begin
-      return CovStructPtr(ID.ID).ItemCount ;
-    end function GetItemCount ;
+      GetTotalCovCountAndGoal(ID, PercentCov, TotalCovCount, TotalCovGoal) ; 
+      return TotalCovCount ; 
+    end function GetTotalCovCount ;
+
+    ------------------------------------------------------------
+    impure function GetTotalCovCount (ID : CoverageIDType) return integer is
+    ------------------------------------------------------------
+    begin
+      return GetTotalCovCount(ID, CovStructPtr(ID.ID).CovTarget) ;
+    end function GetTotalCovCount ;
 
     ------------------------------------------------------------
     impure function GetTotalCovGoal (ID : CoverageIDType; PercentCov : real ) return integer is
     ------------------------------------------------------------
-      variable TotalCovGoal, ScaledCovGoal : integer := 0 ;
+      variable TotalCovCount, TotalCovGoal : integer ;
     begin
-      BinLoop : for i in 1 to CovStructPtr(ID.ID).NumBins loop
-        if CovStructPtr(ID.ID).CovBinPtr(i).action = COV_COUNT then
-          ScaledCovGoal := integer(ceil(PercentCov * real(CovStructPtr(ID.ID).CovBinPtr(i).AtLeast)/100.0)) ;
-          TotalCovGoal := TotalCovGoal + ScaledCovGoal ;
-        end if ;
-      end loop BinLoop ;
+      GetTotalCovCountAndGoal(ID, PercentCov, TotalCovCount, TotalCovGoal) ; 
       return TotalCovGoal ;
     end function GetTotalCovGoal ;
 
     ------------------------------------------------------------
     impure function GetTotalCovGoal (ID : CoverageIDType) return integer is
     ------------------------------------------------------------
     begin
       return GetTotalCovGoal(ID, CovStructPtr(ID.ID).CovTarget) ;
     end function GetTotalCovGoal ;
 
+    ------------------------------------------------------------
+    impure function GetItemCount (ID : CoverageIDType) return integer is
+    ------------------------------------------------------------
+    begin
+      return CovStructPtr(ID.ID).ItemCount ;
+    end function GetItemCount ;
+
     -- Return Index Values
     ------------------------------------------------------------
     impure function GetNumBins (ID : CoverageIDType) return integer is
     ------------------------------------------------------------
     begin
       return CovStructPtr(ID.ID).NumBins ;
     end function GetNumBins ;
@@ -4660,27 +4892,783 @@
         WriteCovDb(ID, CovDbFile) ;
       else
         Alert(CovStructPtr(ID.ID).AlertLogID, GetNamePlus(ID, prefix => "in ", suffix => ", ") &
                        "CoveragePkg.WriteCovDb: no bins defined ", FAILURE) ;
       end if ;
       file_close(CovDbFile) ;
     end procedure WriteCovDb ;
-
+    
 --     ------------------------------------------------------------
 --     procedure WriteCovDb (ID : CoverageIDType) is
 --     ------------------------------------------------------------
 --     begin
 --       if WriteCovDbFileInit then
 --         WriteCovDb(ID, WriteCovDbFile) ;
 --       else
 --         report "CoveragePkg: WriteCovDb file not specified" severity failure ;
 --       end if ;
 --     end procedure WriteCovDb ;
 
     ------------------------------------------------------------
+    --  pt local
+    procedure WriteCovSettingsYaml (ID : CoverageIDType; variable buf : inout LINE; Prefix : string ) is
+    ------------------------------------------------------------
+      variable TotalCovCount, TotalCovGoal : integer ; 
+    begin
+      -- write bins to YAML file
+      write(buf, Prefix & "Settings: " & LF) ; 
+      write(buf, Prefix & "  CovWeight: "          & to_string(CovStructPtr(ID.ID).CovWeight)                    & LF) ; 
+      write(buf, Prefix & "  Goal: "               & to_string(CovStructPtr(ID.ID).CovTarget, 1)                 & LF) ; 
+      write(buf, Prefix & "  WeightMode: """       & to_upper(to_string(CovStructPtr(ID.ID).WeightMode))         & '"' & LF) ; 
+      write(buf, Prefix & "  Seeds: ["             & to_string(CovStructPtr(ID.ID).RV, ", ") & "]"               & LF) ; 
+      write(buf, Prefix & "  CountMode: """        & to_upper(to_string(CovStructPtr(ID.ID).CountMode))          & '"' & LF) ; 
+      write(buf, Prefix & "  IllegalMode: """      & to_upper(to_string(CovStructPtr(ID.ID).IllegalMode))        & '"' & LF) ; 
+      write(buf, Prefix & "  Threshold: "          & to_string(CovStructPtr(ID.ID).CovThreshold, 1)              & LF) ; 
+      write(buf, Prefix & "  ThresholdEnable: """  & to_upper(to_string(CovStructPtr(ID.ID).ThresholdingEnable)) & '"' & LF) ; 
+      GetTotalCovCountAndGoal (ID, TotalCovCount, TotalCovGoal) ;
+      write(buf, Prefix & "  TotalCovCount: "      & to_string(TotalCovCount)                                    & LF) ; 
+      write(buf, Prefix & "  TotalCovGoal: "       & to_string(TotalCovGoal)                                     & LF) ; 
+    end procedure WriteCovSettingsYaml ;
+    
+    ------------------------------------------------------------
+    --  pt local
+    procedure WriteCovFieldNameYaml (ID : CoverageIDType; variable buf : inout LINE; Prefix : string ) is
+    ------------------------------------------------------------
+      variable Dimensions : integer ;
+      variable FieldWidth : integer ; 
+      variable FieldName  : FieldNameArrayPtrType ;
+    begin
+      FieldName  := CovStructPtr(ID.ID).FieldName ; 
+      Dimensions := CovStructPtr(ID.ID).BinValLength ;
+      if FieldName = NULL then 
+        FieldWidth := 0 ; 
+      else 
+        FieldWidth := FieldName'length; 
+      end if; 
+      
+      write(buf, Prefix & "  FieldNames: " & LF) ; 
+      for i in 1 to Dimensions loop 
+        if i > FieldWidth then 
+          write(buf, Prefix & "    - ""Bin" & to_string(i)  & '"' & LF) ; 
+        else 
+          write(buf, Prefix & "    - """ & FieldName(i).all & '"' & LF) ; 
+        end if ; 
+      end loop ; 
+    end procedure WriteCovFieldNameYaml ;
+    
+    ------------------------------------------------------------
+    --  pt local
+    procedure WriteCovBinInfoYaml (ID : CoverageIDType; variable buf : inout LINE; Prefix : string ) is
+    ------------------------------------------------------------
+    begin
+      -- write bins to YAML file
+      write(buf, Prefix & "BinInfo: " & LF) ; 
+      write(buf, Prefix & "  Dimensions: " & to_string(CovStructPtr(ID.ID).BinValLength) & LF) ; 
+      WriteCovFieldNameYaml(ID, buf, Prefix) ; 
+      write(buf, Prefix & "  NumBins: " & to_string(CovStructPtr(ID.ID).NumBins) & LF) ; 
+    end procedure WriteCovBinInfoYaml ;
+    
+    ------------------------------------------------------------
+    procedure WriteBinValYaml (
+    -- package local for now
+    ------------------------------------------------------------
+      variable buf    : inout line ;
+      constant BinVal : in    RangeArrayType ;
+      constant Prefix : in    string
+    ) is
+    begin
+      for i in BinVal'range loop
+        write(buf, Prefix & 
+            "- {Min: " & to_string(BinVal(i).min) & 
+            ", Max: "  & to_string(BinVal(i).max) & "}" & LF) ; 
+      end loop ;
+    end procedure WriteBinValYaml ;
+
+    ------------------------------------------------------------
+    --  pt local
+    procedure WriteCovBinsYaml (ID : CoverageIDType; variable buf : inout LINE; Prefix : string ) is
+    ------------------------------------------------------------
+      variable Action : integer ; 
+      variable CovBin : CovBinInternalBaseType ;
+    begin
+      -- write bins to YAML file
+      write(buf, Prefix & "Bins: " & LF) ; 
+      
+      writeloop : for EachLine in 1 to CovStructPtr(ID.ID).NumBins loop
+        CovBin := CovStructPtr(ID.ID).CovBinPtr(EachLine) ;
+        write(buf, Prefix & "  - Name: """ & CovBin.Name.all             & '"' & LF) ;
+        write(buf, Prefix & "    Type: """ & ActionToName(CovBin.Action) & '"' & LF ) ;
+        write(buf, Prefix & "    Range: " & LF) ;
+        WriteBinValYaml(buf, CovBin.BinVal.all, Prefix & "      ") ; 
+        write(buf, Prefix & "    Count: "      & to_string(CovBin.Count) & LF) ;
+        write(buf, Prefix & "    AtLeast: "    & to_string(CovBin.AtLeast) & LF) ;
+        write(buf, Prefix & "    PercentCov: " & to_string(CovBin.PercentCov, 4) & LF) ;
+      end loop writeloop ; 
+    end procedure WriteCovBinsYaml ;
+    
+    ------------------------------------------------------------
+    --  pt local
+    procedure WriteCovYaml (ID : CoverageIDType; file CovYamlFile : text; TestCaseName : string ) is
+    ------------------------------------------------------------
+      variable buf       : line ;
+      constant NAME_PREFIX : string := "  " ; 
+    begin
+      -- If no bins, FAIL and return (if resumed)
+      if CovStructPtr(ID.ID).NumBins < 1 then
+        Alert(CovStructPtr(ID.ID).AlertLogID, GetNamePlus(ID, prefix => "in ", suffix => ", ") &
+                       "CoveragePkg.WriteCovDb: no bins defined ", FAILURE) ;
+        return ; 
+      end if ; 
+      
+      write(buf, NAME_PREFIX & "- Name: "     & '"' & GetName(ID) & '"' & LF) ; 
+      write(buf, NAME_PREFIX & "  TestCases: " & LF) ; 
+      write(buf, NAME_PREFIX & "    - " & '"' & TestCaseName & '"' & LF) ; 
+--!! Add code to list out merged tests      
+      write(buf, NAME_PREFIX & "  Coverage: " & to_string(GetCov(ID), 2) & LF) ; 
+      WriteCovSettingsYaml(ID, buf, NAME_PREFIX &  "  ") ; 
+      WriteCovBinInfoYaml (ID, buf, NAME_PREFIX &  "  ") ; 
+      WriteCovBinsYaml    (ID, buf, NAME_PREFIX &  "  ") ;
+      writeline(CovYamlFile, buf) ;
+    end procedure WriteCovYaml ;
+
+--     ------------------------------------------------------------
+--     procedure WriteCovYaml (ID : CoverageIDType; FileName : string; OpenKind : File_Open_Kind := WRITE_MODE ) is
+--     ------------------------------------------------------------
+--       file CovYamlFile : text open OpenKind is FileName ;
+--     begin
+--       WriteCovYaml(ID, CovYamlFile) ; 
+--       file_close(CovYamlFile) ;
+--     end procedure WriteCovYaml ;
+
+    ------------------------------------------------------------
+    procedure WriteCovYaml (FileName : string := ""; Coverage : real ; OpenKind : File_Open_Kind := WRITE_MODE) is
+    ------------------------------------------------------------
+      constant RESOLVED_FILE_NAME : string := IfElse(FileName = "", "./reports/" & GetAlertLogName & "_cov.yml", FileName) ; 
+      file CovYamlFile : text open OpenKind is RESOLVED_FILE_NAME ;
+      variable buf : line ;
+    begin
+      swrite(buf, "Version: 1.0" & LF) ; 
+      swrite(buf, "Coverage: " & to_string(Coverage, 2) & LF) ; 
+      swrite(buf, "Models: ") ; 
+      writeline(CovYamlFile, buf) ; 
+      for i in 1 to NumItems loop
+        if CovStructPtr(i).NumBins >= 1 then 
+          WriteCovYaml(CoverageIDType'(ID => i), CovYamlFile, GetAlertLogName) ; 
+        end if ; 
+      end loop ; 
+      file_close(CovYamlFile) ;
+    end procedure WriteCovYaml ;
+    
+    ------------------------------------------------------------
+    --  pt local.  Find a specific token potentially split across lines
+    procedure ReadFindToken (
+    ------------------------------------------------------------
+      file     ReadFile :       text ; 
+      constant Token    : in    string ;
+      variable buf      : inout line ;
+      variable Found    : out   boolean
+    ) is
+      variable Empty, MultiLineComment, ReadValid  : boolean ;
+      variable vToken     : string(1 to Token'length) ;
+    begin
+      Found := FALSE ; 
+      
+      ReadLoop : loop   
+        if buf = NULL or buf.all'length = 0  then 
+          -- return Good FALSE when file empty
+          exit ReadLoop when EndFile(ReadFile) ;
+          -- Get Next Line
+          ReadLine(ReadFile, buf) ;
+        end if ; 
+        -- Skip blank and multi-line comment lines
+        EmptyOrCommentLine(buf, Empty, MultiLineComment) ; 
+        next ReadLoop when Empty;
+
+        read(buf, vToken, ReadValid) ;
+        if not ReadValid then 
+          deallocate(buf) ; 
+          next ReadLoop ; 
+        end if ; 
+        next ReadLoop when vToken /= Token ;
+        Found := TRUE ; 
+        exit ReadLoop ;
+      end loop ReadLoop ;
+    end procedure ReadFindToken ;
+
+    ------------------------------------------------------------
+    --  pt local
+    procedure ReadQuotedString (
+    ------------------------------------------------------------
+      variable buf      : inout line ;
+      variable Name     : inout line 
+    ) is
+      variable char    : character ; 
+      variable vString : string(1 to buf'length) ; 
+      variable Index   : integer := 1 ; 
+      variable Found, Empty, ReadValid : boolean ; 
+    begin
+      Found := FALSE ; 
+      if Name /= NULL then 
+        deallocate(Name) ; 
+      end if ; 
+      
+      ReadLoop : loop   
+        SkipWhiteSpace(buf, Empty) ;  -- Skips white space at beginning of line
+        exit ReadLoop when Empty ;
+        
+        exit ReadLoop when buf.all(buf'left) /= '"' ;
+        Read(buf, Char, ReadValid) ;
+        exit ReadLoop when not ReadValid ;
+        
+        for i in vString'range loop
+          Read(buf, vString(i), ReadValid) ;
+          exit ReadLoop when not ReadValid ;
+          if vString(i) = '"' then 
+            Index := i - 1 ; 
+            Found := TRUE ; 
+            exit ; 
+          end if ; 
+          exit ReadLoop when buf.all'length = 0 ;
+        end loop ; 
+      end loop ReadLoop ;
+        
+      if Found then 
+        Name := new string'(vString(1 to Index)) ; 
+      end if ; 
+    end procedure ReadQuotedString ;
+    
+    ------------------------------------------------------------
+    --  pt local
+    procedure ReadCovModelNameYaml (
+    ------------------------------------------------------------
+      variable ID          : out CoverageIDType ;
+      file     CovYamlFile :     text ; 
+      variable Found       : out boolean
+    ) is
+      variable buf  : line ;
+      variable Name : line ; 
+    begin
+      Found := FALSE ; 
+      ReadLoop: loop
+        ReadFindToken (CovYamlFile, "- Name:", buf, Found) ; 
+        exit ReadLoop when not Found ; 
+        -- Get the Name
+        ReadQuotedString(buf, Name) ;
+        exit when AlertIf(OSVVM_COV_ALERTLOG_ID, Name = NULL, 
+            "CoveragePkg.ReadCovYaml: Unnamed Coverage Model.", COV_READ_YAML_ALERT_LEVEL);
+        ID := NewID(Name.all) ; 
+        deallocate(Name) ; 
+        Found := TRUE ; 
+        exit ; 
+      end loop ReadLoop ; 
+    end procedure ReadCovModelNameYaml ; 
+
+    ------------------------------------------------------------
+    --  pt local
+    procedure ReadCovSettingsYaml (
+    ------------------------------------------------------------
+      constant CovID       : in  CoverageIDType ;
+      file     CovYamlFile :     text ; 
+      variable Found       : out boolean
+    ) is
+      variable buf          : line ;
+      variable Name         : line ; 
+      constant ID           : integer := CovID.ID ; 
+      constant AlertLogID   : AlertLogIDType := CovStructPtr(ID).AlertLogID ;
+      variable vInteger     : integer ; 
+      variable vReal        : real ; 
+      variable Seed1, Seed2 : integer ; 
+      variable ReadValid    : boolean ; 
+    begin
+      Found := FALSE ; 
+      ReadLoop: loop
+        ReadFindToken (CovYamlFile, "Settings:", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""Settings:""", COV_READ_YAML_ALERT_LEVEL) ;
+
+        -- CovWeight
+        ReadFindToken (CovYamlFile, "CovWeight:", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""Settings:""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, vInteger, ReadValid) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading CovWeight value.", COV_READ_YAML_ALERT_LEVEL) ;
+        CovStructPtr(ID).CovWeight := vInteger ; 
+
+        -- Goal / CovTarget
+        ReadFindToken (CovYamlFile, "Goal:", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""Goal:""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, vReal, ReadValid) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading CovTarget value.", COV_READ_YAML_ALERT_LEVEL) ;
+        CovStructPtr(ID).CovTarget := vReal ; 
+
+       -- WeightMode
+        ReadFindToken (CovYamlFile, "WeightMode:", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""WeightMode:""", COV_READ_YAML_ALERT_LEVEL) ;
+        ReadQuotedString(buf, Name) ; 
+        exit ReadLoop when AlertIf(AlertLogID, Name = NULL, 
+            "CoveragePkg.ReadCovYaml Error while reading WeightMode value.", COV_READ_YAML_ALERT_LEVEL) ;
+        if Name.all = "REMAIN" then
+          CovStructPtr(ID).WeightMode := REMAIN ; 
+        else -- at_least
+          CovStructPtr(ID).WeightMode := AT_LEAST ; 
+        end if ; 
+        
+       -- Seeds
+        ReadFindToken (CovYamlFile, "Seeds:", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""Seeds:""", COV_READ_YAML_ALERT_LEVEL) ;
+            
+        -- [
+        ReadFindToken (CovYamlFile, "[", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find Seeds ""[""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, Seed1, ReadValid) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading Seed1 value.", COV_READ_YAML_ALERT_LEVEL) ;
+
+        -- ,
+        ReadFindToken (CovYamlFile, ",", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find Seed #2 "",""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, Seed2, ReadValid) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading Seed2 value.", COV_READ_YAML_ALERT_LEVEL) ;
+
+        CovStructPtr(ID).RV := (Seed1, Seed2) ; 
+            
+       -- CountMode
+        ReadFindToken (CovYamlFile, "CountMode:", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""CountMode:""", COV_READ_YAML_ALERT_LEVEL) ;
+        ReadQuotedString(buf, Name) ; 
+        exit ReadLoop when AlertIf(AlertLogID, Name = NULL, 
+            "CoveragePkg.ReadCovYaml Error while reading CountMode value.", COV_READ_YAML_ALERT_LEVEL) ;
+        if Name.all = "COUNT_ALL" then
+          CovStructPtr(ID).CountMode := COUNT_ALL ; 
+        else
+          CovStructPtr(ID).CountMode := COUNT_FIRST ; 
+        end if ; 
+
+       -- IllegalMode
+        ReadFindToken (CovYamlFile, "IllegalMode:", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""IllegalMode:""", COV_READ_YAML_ALERT_LEVEL) ;
+        ReadQuotedString(buf, Name) ; 
+        exit ReadLoop when AlertIf(AlertLogID, Name = NULL, 
+            "CoveragePkg.ReadCovYaml Error while reading IllegalMode value.", COV_READ_YAML_ALERT_LEVEL) ;
+        if Name.all = "ILLEGAL_OFF" then
+          CovStructPtr(ID).IllegalMode := ILLEGAL_OFF ; 
+        elsif Name.all = "ILLEGAL_FAILURE" then
+          CovStructPtr(ID).IllegalMode := ILLEGAL_FAILURE ; 
+        else
+          CovStructPtr(ID).IllegalMode := ILLEGAL_ON ; 
+        end if ; 
+
+       -- Threshold
+        ReadFindToken (CovYamlFile, "Threshold:", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""Threshold:""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, vReal, ReadValid) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading Threshold value.", COV_READ_YAML_ALERT_LEVEL) ;
+        CovStructPtr(ID).CovThreshold := vReal ; 
+
+       -- ThresholdEnable
+        ReadFindToken (CovYamlFile, "ThresholdEnable:", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""ThresholdEnable:""", COV_READ_YAML_ALERT_LEVEL) ;
+        ReadQuotedString(buf, Name) ; 
+        exit ReadLoop when AlertIf(AlertLogID, Name = NULL, 
+            "CoveragePkg.ReadCovYaml Error while reading IllegalMode value.", COV_READ_YAML_ALERT_LEVEL) ;
+        if Name.all = "TRUE" then
+          CovStructPtr(ID).ThresholdingEnable := TRUE ; 
+        else
+          CovStructPtr(ID).ThresholdingEnable := FALSE ; 
+        end if ; 
+
+       -- TotalCovCount - read and toss
+        ReadFindToken (CovYamlFile, "TotalCovCount:", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""TotalCovCount:""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, vInteger, ReadValid) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading TotalCovCount value.", COV_READ_YAML_ALERT_LEVEL) ;
+        -- Value not used
+
+       -- TotalCovGoal - read and toss
+        ReadFindToken (CovYamlFile, "TotalCovGoal:", buf, Found) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""TotalCovGoal:""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, vInteger, ReadValid) ; 
+        exit ReadLoop when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading TotalCovGoal value.", COV_READ_YAML_ALERT_LEVEL) ;
+
+        -- End
+        Found := TRUE ; 
+        exit ReadLoop ; 
+      end loop ReadLoop ; 
+      deallocate(Name) ; 
+    end procedure ReadCovSettingsYaml ; 
+    
+    ------------------------------------------------------------
+    --  pt local
+    procedure ReadCovBinInfoYaml (
+    ------------------------------------------------------------
+      constant CovID       : in  CoverageIDType ;
+      file     CovYamlFile :     text ; 
+      variable Dimensions  : out integer ; 
+      variable NumBins     : out integer ; 
+      variable Found       : out boolean
+    ) is
+      variable buf            : line ;
+      variable FieldNameArray : FieldNameArrayType(1 to 20) ;
+      constant ID             : integer := CovID.ID ; 
+      constant AlertLogID     : AlertLogIDType := CovStructPtr(ID).AlertLogID ;
+      variable ReadValid      : boolean ; 
+      variable FoundFieldName : boolean ; 
+    begin
+      Found := FALSE ; 
+      Dimensions := 0 ; 
+      NumBins := 0 ; 
+      ReadLoop: loop
+        ReadFindToken (CovYamlFile, "BinInfo:", buf, Found) ; 
+        exit when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""BinInfo:""", COV_READ_YAML_ALERT_LEVEL) ;
+        
+        -- Dimensions
+        ReadFindToken (CovYamlFile, "Dimensions:", buf, Found) ; 
+        exit when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""Dimensions:""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, Dimensions, ReadValid) ; 
+        exit when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading Dimensions value.", COV_READ_YAML_ALERT_LEVEL) ;
+        CovStructPtr(ID).BinValLength := Dimensions ;  
+        
+        -- FieldNames
+        ReadFindToken (CovYamlFile, "FieldNames:", buf, Found) ; 
+        exit when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""FieldNames:""", COV_READ_YAML_ALERT_LEVEL) ;
+
+        -- FieldNames Values
+        FoundFieldName := FALSE ; 
+        for i in 1 to Dimensions loop 
+          ReadFindToken (CovYamlFile, "-", buf, Found) ; 
+          exit when AlertIf(AlertLogID, not Found, 
+              "CoveragePkg.ReadCovYaml did not find Field Name deliminter '-'.", COV_READ_YAML_ALERT_LEVEL) ;
+          ReadQuotedString(buf, FieldNameArray(i)) ; 
+          exit ReadLoop when AlertIf(AlertLogID, FieldNameArray(i) = NULL, 
+              "CoveragePkg.ReadCovYaml Error while reading Field Name value # " & to_string(i), COV_READ_YAML_ALERT_LEVEL) ;
+          if FieldNameArray(i).all /= ("Bin" & to_string(i)) then 
+            FoundFieldName := TRUE ; 
+          end if ;
+        end loop ; 
+        if FoundFieldName then
+          CovStructPtr(ID).FieldName := new FieldNameArrayType'(FieldNameArray(1 to Dimensions)) ;
+        end if ;
+        
+        -- NumBins
+        ReadFindToken (CovYamlFile, "NumBins:", buf, Found) ; 
+        exit when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""NumBins:""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, NumBins, ReadValid) ; 
+        exit when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading NumBins value.", COV_READ_YAML_ALERT_LEVEL) ;
+        
+        -- End 
+        Found := TRUE ; 
+        exit ; 
+      end loop ReadLoop ;
+      if not Found or not FoundFieldName then 
+        -- clean up pointers
+        for i in 1 to Dimensions loop
+          deallocate(FieldNameArray(i)) ; 
+        end loop ;
+      end if ; 
+    end procedure ReadCovBinInfoYaml ; 
+
+    ------------------------------------------------------------
+    --  pt local
+    procedure ReadCovBinValYaml (
+    ------------------------------------------------------------
+      file     CovYamlFile :     text ; 
+      constant AlertLogID  : in  AlertLogIDType ;
+      variable BinVal      : out RangeArrayType ; 
+      variable Found       : out boolean
+    ) is
+      variable buf         : line ;
+      variable Min, Max    : integer ; 
+      variable ReadValid   : boolean ;
+    begin
+      Found := FALSE ; 
+      ReadLoop: loop
+        -- Range:
+        ReadFindToken (CovYamlFile, "Range:", buf, Found) ; 
+        exit when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""Range:""", COV_READ_YAML_ALERT_LEVEL) ;
+
+        -- RangeArrayType
+        for i in BinVal'range loop
+          -- - {Min:
+          ReadFindToken (CovYamlFile, "- {Min:", buf, Found) ; 
+          exit ReadLoop when AlertIf(AlertLogID, not Found, 
+              "CoveragePkg.ReadCovYaml did not find Bins ""Min:""", COV_READ_YAML_ALERT_LEVEL) ;
+          Read(buf, Min, ReadValid) ; 
+          exit ReadLoop when AlertIf(AlertLogID, not ReadValid, 
+              "CoveragePkg.ReadCovYaml Error while reading Min value.", COV_READ_YAML_ALERT_LEVEL) ;
+
+          -- , Max:
+          ReadFindToken (CovYamlFile, ", Max:", buf, Found) ; 
+          exit ReadLoop  when AlertIf(AlertLogID, not Found, 
+              "CoveragePkg.ReadCovYaml did not find Bins ""Max:""", COV_READ_YAML_ALERT_LEVEL) ;
+          Read(buf, Max, ReadValid) ; 
+          exit ReadLoop when AlertIf(AlertLogID, not ReadValid, 
+              "CoveragePkg.ReadCovYaml Error while reading Max value.", COV_READ_YAML_ALERT_LEVEL) ;
+
+          BinVal(i) := (Min => Min, Max => Max) ; 
+        end loop ; 
+        
+        Found := TRUE ; 
+        exit ReadLoop ;
+      end loop ; 
+    end procedure ReadCovBinValYaml ;
+
+    ------------------------------------------------------------
+    --  pt local
+    procedure ReadCovOneBinYaml (
+    ------------------------------------------------------------
+      file     CovYamlFile :     text ; 
+      constant CovID       : in  CoverageIDType ;
+      constant Merge       : in  boolean ; 
+      constant Dimensions  : in  integer ; 
+      variable Found       : out boolean
+    ) is
+      variable buf         : line ;
+      variable Name        : line ; 
+      constant ID          : integer := CovID.ID ; 
+      constant AlertLogID  : AlertLogIDType := CovStructPtr(ID).AlertLogID ;
+      variable NamePtr     : line ;
+      variable Action      : integer ;
+      variable BinVal      : RangeArrayType(1 to Dimensions) ;
+      variable Count       : integer ;
+      variable AtLeast     : integer ;
+      variable Weight      : integer ;
+      variable PercentCov  : real ;
+      variable Index       : integer ; 
+      variable ReadValid   : boolean ; 
+    begin
+      Found := FALSE ; 
+      ReadLoop: loop
+        -- - Name:
+        ReadFindToken (CovYamlFile, "- Name:", buf, Found) ; 
+        exit when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find Bins ""Name:""", COV_READ_YAML_ALERT_LEVEL) ;
+        ReadQuotedString(buf, NamePtr) ;
+        exit ReadLoop when AlertIf(AlertLogID, NamePtr = NULL, 
+            "CoveragePkg.ReadCovYaml Error while reading Name value.", COV_READ_YAML_ALERT_LEVEL) ;
+            
+        -- Type:
+        ReadFindToken (CovYamlFile, "Type:", buf, Found) ; 
+        exit when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""Type:""", COV_READ_YAML_ALERT_LEVEL) ;
+        ReadQuotedString(buf, Name) ; 
+        exit ReadLoop when AlertIf(AlertLogID, Name = NULL, 
+            "CoveragePkg.ReadCovYaml Error while reading Type value.", COV_READ_YAML_ALERT_LEVEL) ;
+        if Name.all = "COUNT" then
+          Action := 1 ; 
+        elsif Name.all = "IGNORE" then
+          Action := 0 ; 
+        else -- Illegal
+          Action := -1 ; 
+        end if ; 
+        deallocate(Name) ; 
+
+        -- BinVal
+        ReadCovBinValYaml(CovYamlFile, AlertLogID, BinVal, Found) ;
+        exit when not Found ; 
+        
+        -- Count: 
+        ReadFindToken (CovYamlFile, "Count:", buf, Found) ; 
+        exit when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""Count:""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, Count, ReadValid) ; 
+        exit when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading Count value.", COV_READ_YAML_ALERT_LEVEL) ;
+        
+        -- AtLeast: 
+        ReadFindToken (CovYamlFile, "AtLeast:", buf, Found) ; 
+        exit when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""AtLeast:""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, AtLeast, ReadValid) ; 
+        exit when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading AtLeast value.", COV_READ_YAML_ALERT_LEVEL) ;
+        Weight  := AtLeast ; 
+
+        -- PercentCov: 
+        ReadFindToken (CovYamlFile, "PercentCov:", buf, Found) ; 
+        exit when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""PercentCov:""", COV_READ_YAML_ALERT_LEVEL) ;
+        Read(buf, PercentCov, ReadValid) ; 
+        exit when AlertIf(AlertLogID, not ReadValid, 
+            "CoveragePkg.ReadCovYaml Error while reading PercentCov value.", COV_READ_YAML_ALERT_LEVEL) ;
+
+        -- Insert the Bin
+        Index := FindExactBin(CovID, Merge, BinVal, Action, AtLeast, Weight, NamePtr.all) ;
+        if Index > 0 then
+          -- Bin is an exact match so only merge the count values
+          CovStructPtr(ID).CovBinPtr(Index).Count := CovStructPtr(ID).CovBinPtr(Index).Count + Count ;
+          CovStructPtr(ID).CovBinPtr(Index).PercentCov := CalcPercentCov(
+              Count   =>  CovStructPtr(ID).CovBinPtr.all(Index).Count,
+              AtLeast =>  CovStructPtr(ID).CovBinPtr.all(Index).AtLeast ) ;
+        else
+          InsertNewBin(CovID, BinVal, Action, Count, AtLeast, Weight, NamePtr.all, PercentCov) ;
+        end if ;
+        deallocate(NamePtr) ;
+
+        -- End 
+        Found := TRUE ; 
+        exit ; 
+      end loop ReadLoop ;
+    end procedure ReadCovOneBinYaml ;     
+        
+    ------------------------------------------------------------
+    --  pt local
+    procedure ReadCovBinsYaml (
+    ------------------------------------------------------------
+      constant CovID       : in  CoverageIDType ;
+      file     CovYamlFile :     text ; 
+      constant Dimensions  : in  integer ; 
+      constant NumBins     : in  integer ; 
+      variable Found       : out boolean ;
+      constant Merge       : in  boolean := FALSE 
+    ) is
+      variable buf            : line ;
+      variable FieldNameArray : FieldNameArrayType(1 to 20) ;
+      constant ID             : integer := CovID.ID ; 
+      constant AlertLogID     : AlertLogIDType := CovStructPtr(ID).AlertLogID ;
+    begin
+      Found := FALSE ; 
+      ReadLoop: loop
+        ReadFindToken (CovYamlFile, "Bins:", buf, Found) ; 
+        exit when AlertIf(AlertLogID, not Found, 
+            "CoveragePkg.ReadCovYaml did not find ""Bins:""", COV_READ_YAML_ALERT_LEVEL) ;
+        
+        GrowBins(CovID, NumBins) ;
+        
+        for i in 1 to NumBins loop
+          ReadCovOneBinYaml(CovYamlFile, CovID, Merge, Dimensions, Found) ; 
+          exit ReadLoop when not Found ;
+        end loop ;
+
+        -- End 
+        Found := TRUE ; 
+        exit ; 
+      end loop ReadLoop ;
+    end procedure ReadCovBinsYaml ; 
+    
+    ------------------------------------------------------------
+    --  pt local
+    procedure ReadCovModelYaml (
+    ------------------------------------------------------------
+      file     CovYamlFile :     text ; 
+      variable Found       : out boolean ;
+      constant Merge       : in  boolean := FALSE 
+    ) is
+      variable CovID      : CoverageIDType ; 
+      variable Dimensions : integer ; 
+      variable NumBins    : integer ; 
+      variable FoundModelName : boolean ; 
+    begin
+      Found          := FALSE ;
+      FoundModelName := FALSE ;
+      
+      ReadLoop: loop
+        ReadCovModelNameYaml(CovID, CovYamlFile, Found) ;
+        exit when not Found ;
+        FoundModelName := TRUE ;
+
+        if not Merge then  -- remove any old bins
+          DeallocateBins(CovID) ;  
+        end if ;
+
+-- Nothing to do with this for now        
+--        ReadCovTestCasesYaml(CovID, CovYamlFile, Found) ;
+--        exit when not Found ;
+      
+-- On merge, new settings apply
+        ReadCovSettingsYaml(CovID, CovYamlFile, Found) ;
+        exit when not Found ;
+        
+-- On merge, new settings apply
+        ReadCovBinInfoYaml(CovID, CovYamlFile, Dimensions, NumBins, Found) ;
+        exit when not Found ;
+
+        -- On merge, matching bins are merged
+        ReadCovBinsYaml(CovID, CovYamlFile, Dimensions, NumBins, Found, Merge) ;
+        exit when not Found ;
+
+        -- End 
+        Found := TRUE ; 
+        exit ; 
+      end loop ReadLoop ; 
+      
+      if FoundModelName and not Found then
+        -- remove partially constructed model
+        Deallocate(CovID) ; 
+      end if ; 
+    end procedure ReadCovModelYaml ; 
+
+--     ------------------------------------------------------------
+--     procedure ReadCovYaml (ModelName : string; FileName : string) is
+--     ------------------------------------------------------------
+--       file CovYamlFile : text open READ_MODE is FileName ;
+--     begin
+--       ID := NewID("ModelName"
+--       ReadCovYaml(ID, CovYamlFile) ; 
+--       file_close(CovYamlFile) ;
+--     end procedure ReadCovYaml ;
+
+    ------------------------------------------------------------
+    procedure ReadCovYaml  (FileName : string := ""; Merge : boolean := FALSE) is
+    ------------------------------------------------------------
+      constant RESOLVED_FILE_NAME : string := IfElse(FileName = "", "./reports/" & GetAlertLogName & "_cov.yml", FileName) ; 
+      file CovYamlFile : text open READ_MODE is RESOLVED_FILE_NAME ;
+      variable buf     : line ;
+      variable Found   : boolean ; 
+    begin
+      ReadFindToken (CovYamlFile, "Models:", buf, Found) ; 
+      if not Found then 
+        Alert(OSVVM_COV_ALERTLOG_ID, 
+            "No Coverage Models found in " & RESOLVED_FILE_NAME, COV_READ_YAML_ALERT_LEVEL) ; 
+        return ; 
+      end if;
+      
+      loop
+        ReadCovModelYaml(CovYamlFile, Found, Merge) ; 
+        exit when not Found ; 
+      end loop ;
+      file_close(CovYamlFile) ;
+    end procedure ReadCovYaml ;
+    
+    ------------------------------------------------------------
+    impure function GotCoverage return boolean is
+    ------------------------------------------------------------
+    begin
+      for i in 1 to NumItems loop 
+        if CovStructPtr(i).NumBins >= 1 then 
+          return TRUE ; 
+        end if; 
+      end loop ; 
+      return FALSE ;     
+    end function GotCoverage ;
+
+    ------------------------------------------------------------
     impure function GetErrorCount (ID : CoverageIDType) return integer is
     ------------------------------------------------------------
       variable ErrorCnt : integer := 0 ;
     begin
       if CovStructPtr(ID.ID).NumBins < 1 then
         return 1 ;  -- return error if model empty
       else
@@ -4697,113 +5685,137 @@
     -- These support usage of cross coverage constants
     -- Also support the older AddCross(GenCross(...)) methodology
     -- which has been replaced by AddCross(GenBin, GenBin, ...)
     ------------------------------------------------------------
     procedure AddCross (ID : CoverageIDType; CovBin : CovMatrix2Type ; Name : String := "") is
     ------------------------------------------------------------
     begin
-      CheckBinValLength(ID, 2, "AddCross") ;
+      if BinValLengthNotEqual(ID, 2) then 
+        Alert(CovStructPtr(ID.ID).AlertLogID, "CoveragePkg.AddCross: Cross coverage bins of different dimensions prohibited", FAILURE) ;
+        return ; 
+      end if ;
       GrowBins(ID, CovBin'length) ;
       for i in CovBin'range loop
         InsertBin(ID,
           CovBin(i).BinVal, CovBin(i).Action, CovBin(i).Count,
           CovBin(i).AtLeast, CovBin(i).Weight, Name
         ) ;
       end loop ;
     end procedure AddCross ;
 
     ------------------------------------------------------------
     procedure AddCross (ID : CoverageIDType; CovBin : CovMatrix3Type ; Name : String := "") is
     ------------------------------------------------------------
     begin
-      CheckBinValLength(ID, 3, "AddCross") ;
+      if BinValLengthNotEqual(ID, 3) then 
+        Alert(CovStructPtr(ID.ID).AlertLogID, "CoveragePkg.AddCross: Cross coverage bins of different dimensions prohibited", FAILURE) ;
+        return ; 
+      end if ;
       GrowBins(ID, CovBin'length) ;
       for i in CovBin'range loop
         InsertBin(ID,
           CovBin(i).BinVal, CovBin(i).Action, CovBin(i).Count,
           CovBin(i).AtLeast, CovBin(i).Weight, Name
         ) ;
       end loop ;
     end procedure AddCross ;
 
     ------------------------------------------------------------
     procedure AddCross (ID : CoverageIDType; CovBin : CovMatrix4Type ; Name : String := "") is
     ------------------------------------------------------------
     begin
-      CheckBinValLength(ID, 4, "AddCross") ;
+      if BinValLengthNotEqual(ID, 4) then 
+        Alert(CovStructPtr(ID.ID).AlertLogID, "CoveragePkg.AddCross: Cross coverage bins of different dimensions prohibited", FAILURE) ;
+        return ; 
+      end if ;
       GrowBins(ID, CovBin'length) ;
       for i in CovBin'range loop
         InsertBin(ID,
           CovBin(i).BinVal, CovBin(i).Action, CovBin(i).Count,
           CovBin(i).AtLeast, CovBin(i).Weight, Name
         ) ;
       end loop ;
     end procedure AddCross ;
 
     ------------------------------------------------------------
     procedure AddCross (ID : CoverageIDType; CovBin : CovMatrix5Type ; Name : String := "") is
     ------------------------------------------------------------
     begin
-      CheckBinValLength(ID, 5, "AddCross") ;
+      if BinValLengthNotEqual(ID, 5) then 
+        Alert(CovStructPtr(ID.ID).AlertLogID, "CoveragePkg.AddCross: Cross coverage bins of different dimensions prohibited", FAILURE) ;
+        return ; 
+      end if ;
       GrowBins(ID, CovBin'length) ;
       for i in CovBin'range loop
         InsertBin(ID,
           CovBin(i).BinVal, CovBin(i).Action, CovBin(i).Count,
           CovBin(i).AtLeast, CovBin(i).Weight, Name
         ) ;
       end loop ;
     end procedure AddCross ;
 
     ------------------------------------------------------------
     procedure AddCross (ID : CoverageIDType; CovBin : CovMatrix6Type ; Name : String := "") is
     ------------------------------------------------------------
     begin
-      CheckBinValLength(ID, 6, "AddCross") ;
+      if BinValLengthNotEqual(ID, 6) then 
+        Alert(CovStructPtr(ID.ID).AlertLogID, "CoveragePkg.AddCross: Cross coverage bins of different dimensions prohibited", FAILURE) ;
+        return ; 
+      end if ;
       GrowBins(ID, CovBin'length) ;
       for i in CovBin'range loop
         InsertBin(ID,
           CovBin(i).BinVal, CovBin(i).Action, CovBin(i).Count,
           CovBin(i).AtLeast, CovBin(i).Weight, Name
         ) ;
       end loop ;
     end procedure AddCross ;
 
     ------------------------------------------------------------
     procedure AddCross (ID : CoverageIDType; CovBin : CovMatrix7Type ; Name : String := "") is
     ------------------------------------------------------------
     begin
-      CheckBinValLength(ID, 7, "AddCross") ;
+      if BinValLengthNotEqual(ID, 7) then 
+        Alert(CovStructPtr(ID.ID).AlertLogID, "CoveragePkg.AddCross: Cross coverage bins of different dimensions prohibited", FAILURE) ;
+        return ; 
+      end if ;
       GrowBins(ID, CovBin'length) ;
       for i in CovBin'range loop
         InsertBin(ID,
           CovBin(i).BinVal, CovBin(i).Action, CovBin(i).Count,
           CovBin(i).AtLeast, CovBin(i).Weight, Name
         ) ;
       end loop ;
     end procedure AddCross ;
 
     ------------------------------------------------------------
     procedure AddCross (ID : CoverageIDType; CovBin : CovMatrix8Type ; Name : String := "") is
     ------------------------------------------------------------
     begin
-      CheckBinValLength(ID, 8, "AddCross") ;
+      if BinValLengthNotEqual(ID, 8) then 
+        Alert(CovStructPtr(ID.ID).AlertLogID, "CoveragePkg.AddCross: Cross coverage bins of different dimensions prohibited", FAILURE) ;
+        return ; 
+      end if ;
       GrowBins(ID, CovBin'length) ;
       for i in CovBin'range loop
         InsertBin(ID,
           CovBin(i).BinVal, CovBin(i).Action, CovBin(i).Count,
           CovBin(i).AtLeast, CovBin(i).Weight, Name
         ) ;
       end loop ;
     end procedure AddCross ;
 
     ------------------------------------------------------------
     procedure AddCross (ID : CoverageIDType; CovBin : CovMatrix9Type ; Name : String := "") is
     ------------------------------------------------------------
     begin
-      CheckBinValLength(ID, 9, "AddCross") ;
+      if BinValLengthNotEqual(ID, 9) then 
+        Alert(CovStructPtr(ID.ID).AlertLogID, "CoveragePkg.AddCross: Cross coverage bins of different dimensions prohibited", FAILURE) ;
+        return ; 
+      end if ;
       GrowBins(ID, CovBin'length) ;
       for i in CovBin'range loop
         InsertBin(ID,
           CovBin(i).BinVal, CovBin(i).Action, CovBin(i).Count,
           CovBin(i).AtLeast, CovBin(i).Weight, Name
         ) ;
       end loop ;
@@ -5549,14 +6561,28 @@
     impure function GetItemCount return integer is
     ------------------------------------------------------------
     begin
       return GetItemCount(COV_STRUCT_ID_DEFAULT) ;
     end function GetItemCount ;
 
     ------------------------------------------------------------
+    impure function GetTotalCovCount ( PercentCov : real ) return integer is
+    ------------------------------------------------------------
+    begin
+      return GetTotalCovCount(COV_STRUCT_ID_DEFAULT, PercentCov) ;
+    end function GetTotalCovCount ;
+
+    ------------------------------------------------------------
+    impure function GetTotalCovCount return integer is
+    ------------------------------------------------------------
+    begin
+      return GetTotalCovCount(COV_STRUCT_ID_DEFAULT) ;
+    end function GetTotalCovCount ;
+
+    ------------------------------------------------------------
     impure function GetTotalCovGoal ( PercentCov : real ) return integer is
     ------------------------------------------------------------
     begin
       return GetTotalCovGoal(COV_STRUCT_ID_DEFAULT, PercentCov) ;
     end function GetTotalCovGoal ;
 
     ------------------------------------------------------------
@@ -6546,15 +7572,15 @@
     ) ;
   end procedure SetReportOptions ;
 
   procedure ResetReportOptions is
   begin
     CoverageStore.ResetReportOptions ;
   end procedure ResetReportOptions ;
-
+  
 
   ------------------------------------------------------------
   -- /////////////////////////////////////////
   --  Coverage Model Settings
   -- /////////////////////////////////////////
   ------------------------------------------------------------
   procedure SetName (ID : CoverageIDType; Name : String) is
@@ -6583,14 +7609,32 @@
   end function GetCovModelName ;
 
   impure function GetNamePlus (ID : CoverageIDType; prefix, suffix : string) return String is
   begin
     return CoverageStore.GetNamePlus (ID, prefix, suffix) ;
   end function GetNamePlus ;
 
+  procedure SetItemBinNames (
+    ID         : CoverageIDType ;
+    Name1      : String ; 
+            Name2,  Name3,  Name4,  Name5, 
+    Name6,  Name7,  Name8,  Name9,  Name10, 
+    Name11, Name12, Name13, Name14, Name15, 
+    Name16, Name17, Name18, Name19, Name20 : string := ""
+  ) is
+  begin
+    CoverageStore.SetItemBinNames (
+      ID,
+      Name1,  Name2,  Name3,  Name4,  Name5, 
+      Name6,  Name7,  Name8,  Name9,  Name10, 
+      Name11, Name12, Name13, Name14, Name15, 
+      Name16, Name17, Name18, Name19, Name20
+    ) ;
+  end procedure SetItemBinNames ;
+
 
   ------------------------------------------------------------
   procedure SetMessage (ID : CoverageIDType; Message : String) is
   begin
     CoverageStore.SetMessage(ID, Message) ;
   end procedure SetMessage ;
 
@@ -6636,14 +7680,24 @@
   end procedure SetIllegalMode ;
 
   procedure SetWeightMode (ID : CoverageIDType; WeightMode : WeightModeType;  WeightScale : real := 1.0) is
   begin
     CoverageStore.SetWeightMode(ID, WeightMode, WeightScale) ;
   end procedure SetWeightMode ;
 
+  procedure SetCovWeight (ID : CoverageIDType; Weight : integer) is
+  begin
+    CoverageStore.SetCovWeight(ID, Weight) ;
+  end procedure SetCovWeight ;
+
+  impure function GetCovWeight (ID : CoverageIDType) return integer is
+  begin
+    return CoverageStore.GetCovWeight(ID) ;
+  end function GetCovWeight ;
+
   procedure SetNextPointMode (ID : CoverageIDType; A : NextPointModeType) is
   begin
     CoverageStore.SetNextPointMode(ID, A) ;
   end procedure SetNextPointMode ;
 
 
   ------------------------------------------------------------
@@ -6957,14 +8011,24 @@
   end function GetCov ;
 
   impure function GetCov (ID : CoverageIDType) return real is
   begin
     return CoverageStore.GetCov (ID) ;
   end function GetCov ;
 
+  impure function GetTotalCovCount (ID : CoverageIDType; PercentCov : real ) return integer is
+  begin
+    return CoverageStore.GetTotalCovCount (ID, PercentCov) ;
+  end function GetTotalCovCount ;
+
+  impure function GetTotalCovCount (ID : CoverageIDType) return integer is
+  begin
+    return CoverageStore.GetTotalCovCount (ID) ;
+  end function GetTotalCovCount ;
+
   impure function GetTotalCovGoal (ID : CoverageIDType; PercentCov : real ) return integer is
   begin
     return CoverageStore.GetTotalCovGoal (ID, PercentCov) ;
   end function GetTotalCovGoal ;
 
   impure function GetTotalCovGoal (ID : CoverageIDType) return integer is
   begin
@@ -7426,14 +8490,78 @@
 
   procedure WriteCovDb (ID : CoverageIDType; FileName : string; OpenKind : File_Open_Kind := WRITE_MODE ) is
   begin
     CoverageStore.WriteCovDb (ID, FileName, OpenKind) ;
   end procedure WriteCovDb ;
 
   --     procedure WriteCovDb (ID : CoverageIDType) is
+  
+--  ------------------------------------------------------------
+--  procedure WriteCovYaml (ID : CoverageIDType; FileName : string; OpenKind : File_Open_Kind := WRITE_MODE ) is
+--  ------------------------------------------------------------
+--    file CovYamlFile : text open OpenKind is FileName ;
+--  begin
+--    CoverageStore.WriteCovYaml (ID, FileName, OpenKind) ;
+--  end procedure WriteCovYaml ;
+
+  ------------------------------------------------------------
+  procedure WriteCovYaml (FileName : string := ""; OpenKind : File_Open_Kind := WRITE_MODE) is
+  ------------------------------------------------------------
+  begin
+    CoverageStore.WriteCovYaml(FileName, GetCov, OpenKind) ;
+  end procedure WriteCovYaml ;
+  
+  ------------------------------------------------------------
+  procedure ReadCovYaml  (FileName : string := ""; Merge : boolean := FALSE) is
+  ------------------------------------------------------------
+  begin
+    CoverageStore.ReadCovYaml(FileName, Merge) ;
+  end procedure ReadCovYaml ;
+
+  ------------------------------------------------------------
+  impure function GotCoverage return boolean is
+  ------------------------------------------------------------
+  begin
+    return CoverageStore.GotCoverage ; 
+  end function GotCoverage ;
+
+  ------------------------------------------------------------
+  impure function GetCov (PercentCov : real ) return real is
+  ------------------------------------------------------------
+    variable ID : CoverageIDType ; 
+    variable ItemCovCount, ItemCovGoal   : integer ; 
+    variable TotalCovCount, TotalCovGoal : integer := 0; 
+    variable CovWeight : integer ; 
+    variable ScaledCovGoal, rTotalCovCount : real ; 
+  begin
+    for i in 1 to CoverageStore.GetNumIDs loop 
+      ID := (ID => i) ; 
+      CoverageStore.GetTotalCovCountAndGoal(ID, ItemCovCount, ItemCovGoal) ; 
+      CovWeight     := GetCovWeight(ID) ;    
+      TotalCovCount := TotalCovCount + (ItemCovCount * CovWeight) ;
+      TotalCovGoal  := TotalCovGoal  + (ItemCovGoal  * CovWeight) ;
+    end loop ;
+    ScaledCovGoal  := PercentCov * real(TotalCovGoal) / 100.0 ;
+    rTotalCovCount := real(TotalCovCount) ;
+    
+    if rTotalCovCount >= ScaledCovGoal then 
+      return 100.0 ;
+    elsif ScaledCovGoal > 0.0 then 
+      return (100.0 * rTotalCovCount) / ScaledCovGoal ;
+    else
+      return 0.0 ;
+    end if; 
+  end function GetCov ;
+
+  ------------------------------------------------------------
+  impure function GetCov return real is
+  ------------------------------------------------------------
+  begin
+    return GetCov (100.0) ;
+  end function GetCov ;
 
 
   ------------------------------------------------------------
   -- Experimental.  Intended primarily for development.
   procedure CompareBins (
   ------------------------------------------------------------
     variable Bin1       : inout CovPType ;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/LICENSE.md` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/MemoryPkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/MemoryPkg.vhd`

 * *Files 1% similar despite different names*

```diff
@@ -267,18 +267,20 @@
     -- Usage:  At the end of the simulation to remove all 
     -- memory used by data structure.  
     -- Note, a normal simulator does this for you.  
     -- You only need this if the simulator is broken.
     procedure deallocate ; 
 
     ------------------------------------------------------------
+    -- /////////////////////////////////////////
     -- Historical Interface
     --   In the new implementation, these use index 1. 
     --   These are for backward compatibility support
     -- 
+    -- /////////////////////////////////////////
     ------------------------------------------------------------
     procedure MemInit ( AddrWidth, DataWidth  : in  integer ) ;
     
     ------------------------------------------------------------
     procedure MemWrite ( Addr, Data  : in  std_logic_vector ) ; 
 
     ------------------------------------------------------------
@@ -759,19 +761,24 @@
               "MemoryPkg.FileReadB: Error while reading data on line: " & to_string(LineNum) &
               "  Item number: " & to_string(ItemNum), FAILURE) ;
             log(MemStructPtr(ID).AlertLogID, "MemoryPkg.FileReadX:  MemWrite(Addr => " & to_hstring(Addr) & ", Data => " & to_string(Data) & ")", DEBUG) ; 
             MemWrite(ID, Addr, data) ; 
             Addr := Addr + AddrInc ; 
           
           else
-          -- Invalid Text, Issue Warning and skip it
-            Alert(MemStructPtr(ID).AlertLogID,  
-              "MemoryPkg.FileReadX: Invalid text on line: " & to_string(LineNum) &
-              "  Item: " & to_string(ItemNum) & ".  Skipping text: " & buf.all) ;
-            exit ItemLoop ; 
+            if NextChar = LF or NextChar = CR then 
+              -- If LF or CR, silently skip the character (DOS file in Unix)
+              read(buf, NextChar) ; 
+            else
+              -- invalid Text, issue warning and skip rest of line
+              Alert(MemStructPtr(ID).AlertLogID,  
+                "MemoryPkg.FileReadX: Invalid text on line: " & to_string(LineNum) &
+                "  Item: " & to_string(ItemNum) & ".  Skipping text: " & buf.all) ;
+              exit ItemLoop ; 
+            end if ; 
           end if ; 
           
         end loop ItemLoop ; 
       end loop ReadLineLoop ; 
       
 --      -- must read EndAddr-StartAddr number of words if both start and end specified
 --      if (StartAddr /= 0 or (not EndAddr) /= 0) and (Addr /= EndAddr) then
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/MessageListPkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/MessageListPkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/MessagePkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/MessagePkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/NamePkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/NamePkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/NameStorePkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/NameStorePkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/OsvvmContext.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/OsvvmContext.vhd`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 --        SynthWorks Design Inc.
 --        VHDL Training Classes
 --        11898 SW 128th Ave.  Tigard, Or  97223
 --        http://www.SynthWorks.com
 --
 --  Revision History:      
 --    Date      Version    Description
+--    10/2021   2021.10    Added ReportPkg
 --    06/2021   2021.06    Updated for release
 --    01/2020   2020.01    Updated Licenses to Apache
 --    11/2016   2016.11    Added TbUtilPkg and ResolutionPkg
 --    06/2015   2015.06    Added MemoryPkg
 --    01/2015   2015.01    Initial Revision
 --
 --
@@ -53,10 +54,11 @@
   use OSVVM.RandomBasePkg.all ;
   use OSVVM.RandomPkg.all ;
   use OSVVM.CoveragePkg.all ;
   use OSVVM.MemoryPkg.all ;
   use OSVVM.ResolutionPkg.all ;
   use OSVVM.ResizePkg.all ;
   use OSVVM.TbUtilPkg.all ;
+  use OSVVM.ReportPkg.all ;
 
 end context OsvvmContext ;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/OsvvmGlobalPkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/OsvvmGlobalPkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/README.md` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/README.md`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/RandomBasePkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/RandomBasePkg.vhd`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
   impure function  GenRandSeed   (I  : integer) return RandomSeedType ;
   impure function  OldGenRandSeed(I  : integer) return RandomSeedType ;
   impure function  GenRandSeed   (S  : string)  return RandomSeedType ;
   impure function  OldGenRandSeed(S  : string)  return RandomSeedType ;
   
   -----------------------------------------------------------------
   --- RandomSeedType IO
-  function  to_string(A : RandomSeedType) return string ;
+  function  to_string(A : RandomSeedType; Separator : string := " ") return string ;
   procedure write(variable L: inout line ; A : RandomSeedType ) ;
   procedure read (variable L: inout line ; A : out RandomSeedType ; good : out boolean ) ;
   procedure read (variable L: inout line ; A : out RandomSeedType ) ;
 
   -----------------------------------------------------------------
   --- Distribution Types and read/write procedures
   type RandomDistType is (NONE, UNIFORM, FAVOR_SMALL, FAVOR_BIG, NORMAL, POISSON) ;
@@ -317,18 +317,18 @@
   end function OldGenRandSeed ;
 
 
   -----------------------------------------------------------------
   --  RandomSeedType IO
   -- 
   -----------------------------------------------------------------
-  function to_string(A : RandomSeedType) return string is
+  function to_string(A : RandomSeedType; Separator : string := " ") return string is
   -----------------------------------------------------------------
   begin
-    return to_string(A(A'left)) & " " & to_string(A(A'right)) ;
+    return to_string(A(A'left)) & Separator & to_string(A(A'right)) ;
   end function to_string ;
 
   -----------------------------------------------------------------
   procedure write(variable L: inout line ; A : RandomSeedType ) is
   -----------------------------------------------------------------
   begin
     write(L, to_string(A)) ;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/RandomPkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/RandomPkg.vhd`

 * *Files 1% similar despite different names*

```diff
@@ -1811,23 +1811,36 @@
     impure function RandSigned (Size : natural) return signed is
     ------------------------------------------------------------
     begin
       return signed(RandUnsigned(Size)) ;
     end function RandSigned ;
 
     ------------------------------------------------------------
+    impure function SizeByLeftMostBit (A : unsigned) return integer is
+    ------------------------------------------------------------
+      alias normA : unsigned (A'length downto 1) is A ;
+    begin
+      for i in normA'range loop 
+        if normA(i) = '1' then 
+          return i ; 
+        end if ; 
+      end loop ;
+      return -1 ; 
+    end function SizeByLeftMostBit ; 
+
+    ------------------------------------------------------------
     impure function RandUnsigned (Max : unsigned) return unsigned is
     ------------------------------------------------------------
       alias normMax : unsigned (Max'length downto 1) is Max ;
       variable Result : unsigned(Max'range) := (others => '0') ;
       alias normResult : unsigned(normMax'range) is Result ;
       variable Size : integer ;
     begin
       -- Size = -1 if not found or Max'length = 0
-      Size := find_leftmost(normMax, '1') ;
+      Size := SizeByLeftMostBit(Max) ;
 
       if Size > 0 then
         loop
           normResult(Size downto 1) := RandUnsigned(Size) ;
           exit when normResult <= Max ;
         end loop ;
         return Result ; -- = normResult with range same as Max
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/RandomProcedurePkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/RandomProcedurePkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/ResizePkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/ResizePkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/ResolutionPkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/ResolutionPkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/ScoreboardGenericPkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/ScoreboardGenericPkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/ScoreboardPkg_int.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/ScoreboardPkg_int.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/ScoreboardPkg_int_c.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/ScoreboardPkg_int_c.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/ScoreboardPkg_slv.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/ScoreboardPkg_slv.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/ScoreboardPkg_slv_c.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/ScoreboardPkg_slv_c.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/SortListPkg_int.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/SortListPkg_int.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/TbUtilPkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/TbUtilPkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/TextUtilPkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/TextUtilPkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/TranscriptPkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/TranscriptPkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/VendorCovApiPkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/VendorCovApiPkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/VendorCovApiPkg_Aldec.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/VendorCovApiPkg_Aldec.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/demo/AlertLog_Demo_Global.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/demo/AlertLog_Demo_Global.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/demo/AlertLog_Demo_Hierarchy.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/demo/AlertLog_Demo_Hierarchy.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/demo/Demo_Rand.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/demo/Demo_Rand.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/osvvm.pro` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/osvvm.pro`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #        SynthWorks Design Inc.
 #        VHDL Training Classes
 #        11898 SW 128th Ave.  Tigard, Or  97223
 #        http://www.SynthWorks.com
 #
 #  Revision History:
 #    Date      Version    Description
+#    10/2021   2021.10    Added ReportPkg
 #     6/2021   2021.06    Updated for release
 #     1/2020   2020.01    Updated Licenses to Apache
 #    11/2016   2016.11    Compile Script for OSVVM
 #
 #
 #  This file is part of OSVVM.
 #  
@@ -41,15 +42,15 @@
 library osvvm
 analyze ResolutionPkg.vhd
 analyze NamePkg.vhd
 analyze NameStorePkg.vhd
 analyze OsvvmGlobalPkg.vhd
 
 # Compile VendorCovApiPkg_Aldec.vhd for RivieraPro and ActiveHDL, otherwise compile VendorCovApiPkg.vhd
-if {[info exists aldec]} {
+if {$::osvvm::ToolVendor eq "Aldec"}  {
   analyze VendorCovApiPkg_Aldec.vhd
 } else {
   analyze VendorCovApiPkg.vhd
 }
 
 analyze TranscriptPkg.vhd
 analyze TextUtilPkg.vhd
@@ -75,8 +76,10 @@
 } else {
   analyze ScoreboardPkg_slv_c.vhd
   analyze ScoreboardPkg_int_c.vhd
 }
 analyze ResizePkg.vhd
 analyze TbUtilPkg.vhd
 
+analyze ReportPkg.vhd
+
 analyze OsvvmContext.vhd
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/osvvm/osvvm_old.tcl` & `vunit_hdl-4.7.0/vunit/vhdl/osvvm/osvvm_old.tcl`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/path/src/path.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/path/src/path.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/path/test/tb_path.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/path/test/tb_path.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/random/src/random_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/random/src/random_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/random/test/tb_random_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/random/test/tb_random_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/run/src/run.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/run/src/run.vhd`

 * *Files 11% similar despite different names*

```diff
@@ -11,60 +11,49 @@
 use work.log_handler_pkg.all;
 use work.ansi_pkg.enable_colors;
 use work.string_ops.all;
 use work.dictionary.all;
 use work.path.all;
 use work.core_pkg;
 use std.textio.all;
+use work.event_common_pkg.all;
+use work.event_private_pkg.all;
+use work.checker_pkg.all;
 
 package body run_pkg is
-  procedure notify(signal runner : inout runner_sync_t;
-                   idx : natural := runner_event_idx) is
-  begin
-    if runner(idx) /= runner_event then
-      runner(idx) <= runner_event;
-      wait until runner(idx) = runner_event;
-      runner(idx) <= idle_runner;
-    end if;
-  end procedure notify;
-
-  procedure test_runner_setup (
+  procedure test_runner_setup(
     signal runner : inout runner_sync_t;
     constant runner_cfg : in string := runner_cfg_default) is
     variable test_case_candidates : lines_t;
     variable selected_enabled_test_cases : line;
   begin
 
     -- fake active python runner key is only used during testing in tb_run.vhd
     -- to avoid creating vunit_results file
     set_active_python_runner(runner_state,
                              (active_python_runner(runner_cfg) and not has_key(runner_cfg, "fake active python runner")));
 
     if has_active_python_runner(runner_state) then
       core_pkg.setup(output_path(runner_cfg) & "vunit_results");
-    end if;
-
-
-    if has_active_python_runner(runner_state) then
       hide(runner_trace_logger, display_handler, info);
     end if;
 
     if has_key(runner_cfg, "use_color") and boolean'value(get(runner_cfg, "use_color")) then
       enable_colors;
     end if;
 
     if not active_python_runner(runner_cfg) then
       set_stop_level(failure);
     end if;
 
     set_phase(runner_state, test_runner_setup);
     runner(runner_exit_status_idx) <= runner_exit_with_errors;
-    notify(runner);
-
     trace(runner_trace_logger, "Entering test runner setup phase.");
+    notify(runner(runner_phase_idx to runner_phase_idx + basic_event_length - 1));
+
     entry_gate(runner);
 
     if selected_enabled_test_cases /= null then
       deallocate(selected_enabled_test_cases);
     end if;
 
     if has_key(runner_cfg, "enabled_test_cases") then
@@ -74,80 +63,86 @@
     end if;
     test_case_candidates := split(replace(selected_enabled_test_cases.all, ",,", "__comma__"), ",");
 
     set_cfg(runner_state, runner_cfg);
 
     set_run_all(runner_state, strip(test_case_candidates(0).all) = "__all__");
     if get_run_all(runner_state) then
-      set_num_of_test_cases(runner_state, unknown_num_of_test_cases_c);
+      set_num_of_test_cases(runner_state, unknown_num_of_test_cases);
     else
       set_num_of_test_cases(runner_state, 0);
       for i in 1 to test_case_candidates'length loop
         if strip(test_case_candidates(i - 1).all) /= "" then
           inc_num_of_test_cases(runner_state);
 
           set_test_case_name(runner_state,
                              get_num_of_test_cases(runner_state),
                              replace(strip(test_case_candidates(i - 1).all), "__comma__", ","));
         end if;
       end loop;
     end if;
     exit_gate(runner);
     set_phase(runner_state, test_suite_setup);
-    notify(runner);
     trace(runner_trace_logger, "Entering test suite setup phase.");
+    notify(runner(runner_phase_idx to runner_phase_idx + basic_event_length - 1));
     entry_gate(runner);
   end test_runner_setup;
 
-  procedure test_runner_cleanup (
-    signal runner: inout runner_sync_t;
+  procedure test_runner_cleanup(
+    signal runner : inout runner_sync_t;
     external_failure : boolean := false;
     allow_disabled_errors : boolean := false;
     allow_disabled_failures : boolean := false;
     fail_on_warning : boolean := false) is
   begin
-    failure_if(runner_trace_logger, external_failure, "External failure.");
-
     set_phase(runner_state, test_runner_cleanup);
-    notify(runner);
+    set_gate_status(runner_state, false);
     trace(runner_trace_logger, "Entering test runner cleanup phase.");
+    notify(runner(runner_phase_idx to runner_phase_idx + basic_event_length - 1));
     entry_gate(runner);
+    failure_if(runner_trace_logger, external_failure, "External failure.");
+
+    if p_has_unhandled_checks then
+      core_pkg.core_failure("Unhandled checks.");
+      return;
+    end if;
+
     exit_gate(runner);
     set_phase(runner_state, test_runner_exit);
-    notify(runner);
     trace(runner_trace_logger, "Entering test runner exit phase.");
+    notify(runner(runner_phase_idx to runner_phase_idx + basic_event_length - 1));
 
     if not final_log_check(allow_disabled_errors => allow_disabled_errors,
-                           allow_disabled_failures => allow_disabled_failures,
-                           fail_on_warning => fail_on_warning) then
+                             allow_disabled_failures => allow_disabled_failures,
+                             fail_on_warning => fail_on_warning) then
       return;
     end if;
 
     runner(runner_exit_status_idx) <= runner_exit_without_errors;
-    notify(runner);
+    notify(runner(runner_phase_idx to runner_phase_idx + basic_event_length - 1));
 
     if has_active_python_runner(runner_state) then
       core_pkg.test_suite_done;
     end if;
 
     if not p_simulation_exit_is_disabled(runner_state) then
       core_pkg.stop(0);
     end if;
 
   end procedure test_runner_cleanup;
 
   impure function num_of_enabled_test_cases
-    return integer is
+  return integer is
   begin
     return get_num_of_test_cases(runner_state);
   end;
 
-  impure function enabled (
+  impure function enabled(
     constant name : string)
-    return boolean is
+  return boolean is
     variable i : natural := 1;
   begin
     if get_run_all(runner_state) then
       return true;
     end if;
 
     for i in 1 to get_num_of_test_cases(runner_state) loop
@@ -156,15 +151,15 @@
       end if;
     end loop;
 
     return false;
   end;
 
   impure function test_suite
-    return boolean is
+  return boolean is
     variable ret_val : boolean;
   begin
     init_test_case_iteration(runner_state);
 
     if get_test_suite_completed(runner_state) then
       ret_val := false;
     elsif get_run_all(runner_state) then
@@ -189,15 +184,15 @@
       trace(runner_trace_logger, "Entering test suite cleanup phase.");
     end if;
 
     return ret_val;
   end;
 
   impure function test_case
-    return boolean is
+  return boolean is
   begin
     if get_test_case_iteration(runner_state) = 0 then
       set_phase(runner_state, test_case);
       trace(runner_trace_logger, "Entering test case phase.");
       inc_test_case_iteration(runner_state);
       clear_test_case_exit_after_error(runner_state);
       clear_test_suite_exit_after_error(runner_state);
@@ -206,31 +201,31 @@
     else
       set_phase(runner_state, test_case_cleanup);
       trace(runner_trace_logger, "Entering test case cleanup phase.");
       return false;
     end if;
   end function test_case;
 
-  impure function run (
+  impure function run(
     constant name : string)
-    return boolean is
+  return boolean is
 
-    impure function has_run (
+    impure function has_run(
       constant name : string)
-      return boolean is
+    return boolean is
     begin
       for i in 1 to get_num_of_run_test_cases(runner_state) loop
         if get_run_test_case(runner_state, i) = name then
           return true;
         end if;
       end loop;
       return false;
     end function has_run;
 
-    procedure register_run (
+    procedure register_run(
       constant name : in string) is
     begin
       inc_num_of_run_test_cases(runner_state);
       set_has_run_since_last_loop_check(runner_state);
       set_run_test_case(runner_state, get_num_of_run_test_cases(runner_state), name);
     end procedure register_run;
 
@@ -258,244 +253,268 @@
     end if;
 
     set_running_test_case(runner_state, "");
     return false;
   end;
 
   impure function active_test_case
-    return string is
+  return string is
   begin
     if get_run_all(runner_state) then
       return "";
     end if;
     return get_test_case_name(runner_state, get_active_test_case_index(runner_state));
   end;
 
   impure function running_test_case
-    return string is
+  return string is
   begin
     return get_running_test_case(runner_state);
   end;
 
   procedure set_timeout(signal runner : inout runner_sync_t;
                         constant timeout : in time) is
   begin
     set_timeout(runner_state, timeout);
-    notify(runner, runner_timeout_update_idx);
+    notify(runner(runner_timeout_update_idx to runner_timeout_update_idx + basic_event_length - 1));
   end;
 
-  procedure test_runner_watchdog (
-    signal runner                    : inout runner_sync_t;
-    constant timeout                 : in    time;
-    constant do_runner_cleanup : boolean := true) is
+  procedure test_runner_watchdog(
+    signal runner : inout runner_sync_t;
+    constant timeout : in time;
+    constant do_runner_cleanup : boolean := true;
+    constant line_num : in natural := 0;
+    constant file_name : in string := "") is
 
     variable current_timeout : time := timeout;
   begin
 
     loop
-      wait until (runner(runner_exit_status_idx) = runner_exit_without_errors or
-                  runner(runner_timeout_update_idx) = runner_event) for current_timeout;
+      wait until (runner(runner_exit_status_idx) = runner_exit_without_errors) or is_active(runner_timeout_update) for current_timeout;
 
-      if runner(runner_timeout_update_idx) = runner_event then
+      if is_active(runner_timeout_update) then
         debug(runner_trace_logger, "Update watchdog timeout " & time'image(current_timeout) & ".");
         current_timeout := get_timeout(runner_state);
       else
         exit;
       end if;
     end loop;
 
     if not (runner(runner_exit_status_idx) = runner_exit_without_errors) then
-      notify(runner, runner_timeout_idx);
-      wait until runner(runner_timeout_idx) = idle_runner;
-      error(runner_trace_logger, "Test runner timeout after " & time'image(current_timeout) & ".");
+      -- TODO: Only stop if error count is 1
+      notify(
+        runner(runner_timeout_idx to runner_timeout_idx + basic_event_length - 1),
+        runner(vunit_error_idx to vunit_error_idx + basic_event_length - 1)
+      );
+      error(runner_trace_logger,
+            "Test runner timeout after " & time'image(current_timeout) & ".",
+            path_offset => 1, line_num => line_num, file_name => file_name);
       if do_runner_cleanup then
         test_runner_cleanup(runner);
       end if;
     end if;
   end;
 
-  function timeout_notification (
+  function timeout_notification(
     signal runner : runner_sync_t
   ) return boolean is
   begin
-    return runner(runner_timeout_idx) = runner_event;
+    -- Cannot use better logging functions since timeout_notification is pure
+    report "timeout_notification(runner) is deprecated and will be removed in future releases. Use is_active(test_runner_timeout) instead.";
+    return runner(runner_timeout_idx to runner_timeout_idx + 1) /= p_inactive_event;
   end;
 
-  impure function test_suite_error (
+  impure function test_suite_error(
     constant err : boolean)
-    return boolean is
+  return boolean is
   begin
     if err then
       set_test_suite_completed(runner_state);
       set_phase(runner_state, test_case_cleanup);
       trace(runner_trace_logger, "Entering test case cleanup phase.");
       set_test_suite_exit_after_error(runner_state);
     end if;
 
     return err;
   end function test_suite_error;
 
-  impure function test_case_error (
+  impure function test_case_error(
     constant err : boolean)
-    return boolean is
+  return boolean is
   begin
     if err then
       set_phase(runner_state, test_case_cleanup);
       trace(runner_trace_logger, "Entering test case cleanup phase.");
       set_test_case_exit_after_error(runner_state);
     end if;
 
     return err;
   end function test_case_error;
 
   impure function test_suite_exit
-    return boolean is
+  return boolean is
   begin
     return get_test_suite_exit_after_error(runner_state);
   end function test_suite_exit;
 
   impure function test_case_exit
-    return boolean is
+  return boolean is
   begin
     return get_test_case_exit_after_error(runner_state);
   end function test_case_exit;
 
   impure function test_exit
-    return boolean is
+  return boolean is
   begin
     return test_suite_exit or test_case_exit;
   end function test_exit;
 
-  procedure lock_entry (
-    signal runner : inout runner_sync_t;
-    constant phase : in runner_legal_phase_t;
-    constant logger : in logger_t := runner_trace_logger;
-    constant path_offset : in natural := 0;
-    constant line_num  : in natural := 0;
-    constant file_name : in string := "") is
+  impure function get_entry_key(phase : runner_legal_phase_t) return key_t is
   begin
-    lock_entry(runner_state, phase);
-    log(logger, "Locked " & replace(runner_phase_t'image(phase), "_", " ") & " phase entry gate.", trace, path_offset + 1, line_num, file_name);
-    notify(runner);
+    return get_entry_key(runner_state, phase);
   end;
 
-  procedure unlock_entry (
-    signal runner : inout runner_sync_t;
-    constant phase : in runner_legal_phase_t;
-    constant logger : in logger_t := runner_trace_logger;
-    constant path_offset : in natural := 0;
-    constant line_num  : in natural := 0;
-    constant file_name : in string := "") is
+  impure function get_exit_key(phase : runner_legal_phase_t) return key_t is
   begin
-    unlock_entry(runner_state, phase);
-    log(logger, "Unlocked " & replace(runner_phase_t'image(phase), "_", " ") & " phase entry gate.", trace, path_offset + 1, line_num, file_name);
-    notify(runner);
+    return get_exit_key(runner_state, phase);
   end;
 
-  procedure lock_exit (
+  impure function is_locked(key : key_t) return boolean is
+  begin
+    return is_locked(runner_state, key);
+  end;
+
+  procedure lock(
     signal runner : inout runner_sync_t;
-    constant phase : in runner_legal_phase_t;
-    constant logger : in logger_t := runner_trace_logger;
+    constant key : in key_t;
+    constant logger : in logger_t := null_logger;
     constant path_offset : in natural := 0;
-    constant line_num  : in natural := 0;
+    constant line_num : in natural := 0;
     constant file_name : in string := "") is
   begin
-    lock_exit(runner_state, phase);
-    log(logger, "Locked " & replace(runner_phase_t'image(phase), "_", " ") & " phase exit gate.", trace, path_offset + 1, line_num, file_name);
-    notify(runner);
+    lock(runner_state, key);
+    if logger /= null_logger then
+      if key.p_is_entry_key then
+        log(logger, "Locked " & replace(runner_phase_t'image(key.p_phase), "_", " ") & " phase entry gate.", trace, path_offset + 1, line_num, file_name);
+      else
+        log(logger, "Locked " & replace(runner_phase_t'image(key.p_phase), "_", " ") & " phase exit gate.", trace, path_offset + 1, line_num, file_name);
+      end if;
+    end if;
   end;
 
-  procedure unlock_exit (
+  procedure unlock(
     signal runner : inout runner_sync_t;
-    constant phase : in runner_legal_phase_t;
-    constant logger : in logger_t := runner_trace_logger;
+    constant key : in key_t;
+    constant logger : in logger_t := null_logger;
     constant path_offset : in natural := 0;
-    constant line_num  : in natural := 0;
+    constant line_num : in natural := 0;
     constant file_name : in string := "") is
   begin
-    unlock_exit(runner_state, phase);
-    log(logger, "Unlocked " & replace(runner_phase_t'image(phase), "_", " ") & " phase exit gate.", trace, path_offset + 1, line_num, file_name);
-    notify(runner);
+    unlock(runner_state, key);
+    if logger /= null_logger then
+      if key.p_is_entry_key then
+        log(logger, "Unlocked " & replace(runner_phase_t'image(key.p_phase), "_", " ") & " phase entry gate.", trace, path_offset + 1, line_num, file_name);
+      else
+        log(logger, "Unlocked " & replace(runner_phase_t'image(key.p_phase), "_", " ") & " phase exit gate.", trace, path_offset + 1, line_num, file_name);
+      end if;
+    end if;
+    notify(runner(runner_phase_idx to runner_phase_idx + basic_event_length - 1));
   end;
 
-  procedure wait_until (
+  procedure wait_until(
     signal runner : in runner_sync_t;
     constant phase : in runner_legal_phase_t;
-    constant logger : in logger_t := runner_trace_logger;
+    constant logger : in logger_t := null_logger;
     constant path_offset : in natural := 0;
-    constant line_num  : in natural := 0;
+    constant line_num : in natural := 0;
     constant file_name : in string := "") is
   begin
     if get_phase(runner_state) /= phase then
-      log(logger, "Waiting for phase = " & replace(runner_phase_t'image(phase), "_", " ") & ".", trace, path_offset + 1, line_num, file_name);
-      wait on runner until get_phase(runner_state) = phase;
-      log(logger, "Waking up. Phase is " & replace(runner_phase_t'image(phase), "_", " ") & ".", trace, path_offset + 1, line_num, file_name);
+      if logger /= null_logger then
+        log(logger, "Waiting for phase = " & replace(runner_phase_t'image(phase), "_", " ") & ".", trace, path_offset + 1, line_num, file_name);
+      end if;
+      wait until is_active(runner_phase) and get_phase(runner_state) = phase;
+      if logger /= null_logger then
+        log(logger, "Waking up. Phase is " & replace(runner_phase_t'image(phase), "_", " ") & ".", trace, path_offset + 1, line_num, file_name);
+      end if;
     end if;
   end;
 
-  procedure entry_gate (
+  impure function get_phase return runner_phase_t is
+  begin
+    return get_phase(runner_state);
+  end;
+
+  impure function is_within_gates_of(phase : runner_legal_phase_t) return boolean is
+  begin
+    return is_within_gates(runner_state, phase);
+  end;
+
+  procedure entry_gate(
     signal runner : inout runner_sync_t) is
   begin
     if entry_is_locked(runner_state, get_phase(runner_state)) then
       trace(runner_trace_logger, "Halting on " & replace(runner_phase_t'image(get_phase(runner_state)), "_", " ") & " phase entry gate.");
       wait on runner until not entry_is_locked(runner_state, get_phase(runner_state)) for max_locked_time;
     end if;
-    notify(runner);
+    set_gate_status(runner_state, true);
     trace(runner_trace_logger, "Passed " & replace(runner_phase_t'image(get_phase(runner_state)), "_", " ") & " phase entry gate.");
+    notify(runner(runner_phase_idx to runner_phase_idx + basic_event_length - 1));
   end procedure entry_gate;
 
-  procedure exit_gate (
-    signal runner : in runner_sync_t) is
+  procedure exit_gate(
+    signal runner : inout runner_sync_t) is
   begin
     if exit_is_locked(runner_state, get_phase(runner_state)) then
       trace(runner_trace_logger, "Halting on " & replace(runner_phase_t'image(get_phase(runner_state)), "_", " ") & " phase exit gate.");
       wait on runner until not exit_is_locked(runner_state, get_phase(runner_state)) for max_locked_time;
     end if;
+    set_gate_status(runner_state, false);
     trace(runner_trace_logger, "Passed " & replace(runner_phase_t'image(get_phase(runner_state)), "_", " ") & " phase exit gate.");
+    notify(runner(runner_phase_idx to runner_phase_idx + basic_event_length - 1));
   end procedure exit_gate;
 
-  impure function active_python_runner (
+  impure function active_python_runner(
     constant runner_cfg : string)
-    return boolean is
+  return boolean is
   begin
     if has_key(runner_cfg, "active python runner") then
       return get(runner_cfg, "active python runner") = "true";
     else
       return false;
     end if;
   end;
 
-  impure function output_path (
+  impure function output_path(
     constant runner_cfg : string)
-    return string is
+  return string is
   begin
     if has_key(runner_cfg, "output path") then
       return get(runner_cfg, "output path");
     else
       return "";
     end if;
   end;
 
-  impure function enabled_test_cases (
+  impure function enabled_test_cases(
     constant runner_cfg : string)
-    return test_cases_t is
+  return test_cases_t is
   begin
     if has_key(runner_cfg, "enabled_test_cases") then
       return get(runner_cfg, "enabled_test_cases");
     else
       return "__all__";
     end if;
   end;
 
-  impure function tb_path (
+  impure function tb_path(
     constant runner_cfg : string)
-    return string is
+  return string is
   begin
     if has_key(runner_cfg, "tb path") then
       return get(runner_cfg, "tb path");
     else
       return "";
     end if;
   end;
 
-
 end package body run_pkg;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/run/src/run_deprecated_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/run/src/run_deprecated_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/run/src/run_types.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/run/src/run_types.vhd`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 -- License, v. 2.0. If a copy of the MPL was not distributed with this file,
 -- You can obtain one at http://mozilla.org/MPL/2.0/.
 --
 -- Copyright (c) 2014-2023, Lars Asplund lars.anders.asplund@gmail.com
 
 use std.textio.all;
 use work.dictionary.all;
+use work.event_private_pkg.all;
 
 library ieee;
 use ieee.std_logic_1164.all;
 
 package run_types_pkg is
   constant max_locked_time : time := 1 ms;
   constant max_n_test_cases : natural := 1024;
@@ -32,23 +33,20 @@
   type phase_locks_t is record
     entry_is_locked : boolean;
     exit_is_locked : boolean;
   end record;
 
   type boolean_array_t is array (integer range <>) of boolean;
 
-  constant runner_event_idx : natural := 0;
-  constant runner_exit_status_idx : natural := 1;
-  constant runner_timeout_update_idx : natural := 2;
-  constant runner_timeout_idx : natural := 3;
-
-  constant runner_event : std_logic := '1';
-  constant idle_runner  : std_logic := 'Z';
-
   constant runner_exit_with_errors : std_logic := 'Z';
   constant runner_exit_without_errors : std_logic := '1';
 
-  subtype runner_sync_t is std_logic_vector(runner_event_idx to runner_timeout_idx);
+  subtype runner_sync_t is std_logic_vector(0 to 4 * basic_event_length - 1 + 1);
+  constant runner_phase_idx : natural := 0;
+  constant runner_timeout_update_idx : natural := basic_event_length;
+  constant runner_timeout_idx : natural := 2 * basic_event_length;
+  constant vunit_error_idx : natural := 3 * basic_event_length;
+  constant runner_exit_status_idx : natural :=4 * basic_event_length;
 end package;
 
 package body run_types_pkg is
 end package body run_types_pkg;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/run/src/runner_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/run/src/runner_pkg.vhd`

 * *Files 11% similar despite different names*

```diff
@@ -18,45 +18,52 @@
 package runner_pkg is
   constant runner_trace_logger : logger_t := get_logger("runner");
 
   type runner_t is record
     p_data : integer_vector_ptr_t;
   end record;
 
+  type key_t is record
+    p_is_entry_key : boolean;
+    p_phase : runner_legal_phase_t;
+    p_key_id : natural;
+  end record;
+
   constant null_runner : runner_t := (p_data => null_ptr);
   constant unknown_num_of_test_cases : integer := integer'left;
 
   -- Deprecated
   constant unknown_num_of_test_cases_c : integer := unknown_num_of_test_cases;
 
   impure function new_runner return runner_t;
 
   procedure runner_init(runner : runner_t);
   procedure set_active_python_runner(runner : runner_t; value : boolean);
   impure function has_active_python_runner(runner : runner_t) return boolean;
 
-  procedure lock_entry(runner : runner_t; phase : runner_legal_phase_t);
-
-  procedure unlock_entry(runner : runner_t; phase : runner_legal_phase_t);
+  impure function get_entry_key(runner : runner_t; phase : runner_legal_phase_t) return key_t;
+  impure function get_exit_key(runner : runner_t; phase : runner_legal_phase_t) return key_t;
+  impure function is_locked(runner : runner_t; key : key_t) return boolean;
+  procedure lock(runner : runner_t; key : key_t);
+  procedure unlock(runner : runner_t; key : key_t);
 
   impure function entry_is_locked(runner : runner_t; phase : runner_legal_phase_t) return boolean;
-
-  procedure lock_exit(runner : runner_t; phase : runner_legal_phase_t);
-
-  procedure unlock_exit(runner : runner_t; phase : runner_legal_phase_t);
-
   impure function exit_is_locked(runner : runner_t; phase : runner_legal_phase_t) return boolean;
 
   procedure set_phase(runner : runner_t; new_phase : runner_phase_t);
 
   impure function get_phase(runner : runner_t) return runner_phase_t;
 
+  procedure set_gate_status(runner : runner_t; is_within_gates : boolean);
+
+  impure function is_within_gates(runner : runner_t; phase : runner_legal_phase_t) return boolean;
+
   procedure set_test_case_name(runner : runner_t; index : positive; new_name : string);
 
-  impure function get_test_case_name(runner : runner_t; index : positive) return string ;
+  impure function get_test_case_name(runner : runner_t; index : positive) return string;
 
   procedure set_num_of_test_cases(runner : runner_t; new_value : integer);
 
   procedure inc_num_of_test_cases(runner : runner_t);
 
   impure function get_num_of_test_cases(runner : runner_t) return integer;
 
@@ -72,15 +79,15 @@
 
   procedure inc_test_suite_iteration(runner : runner_t);
 
   procedure set_run_test_case(runner : runner_t; index : positive; new_name : string);
 
   impure function get_run_test_case(runner : runner_t; index : positive) return string;
 
-  procedure set_running_test_case(runner : runner_t; new_name  : string);
+  procedure set_running_test_case(runner : runner_t; new_name : string);
 
   impure function get_running_test_case(runner : runner_t) return string;
 
   impure function get_num_of_run_test_cases(runner : runner_t) return natural;
 
   procedure inc_num_of_run_test_cases(runner : runner_t);
 
@@ -144,15 +151,23 @@
   constant test_case_exit_after_error_idx : natural := 13;
   constant test_suite_exit_after_error_idx : natural := 14;
   constant runner_cfg_idx : natural := 15;
   constant disable_simulation_exit_idx : natural := 16;
   constant entry_locks_idx : natural := 17;
   constant exit_locks_idx : natural := 18;
   constant timeout_idx : natural := 19;
-  constant runner_length : natural := 20;
+  constant is_within_gates_idx : natural := 20;
+  constant runner_length : natural := 21;
+
+  constant n_locks : positive := 254;
+  constant n_locked_idx : natural := 0;
+  constant n_used_locks_idx : natural := 1;
+  constant lock_idx : natural := 2;
+  constant lock_is_unlocked : natural := 0;
+  constant lock_is_locked : natural := 1;
 
   function to_integer(value : boolean) return natural is
   begin
     if value then
       return 1;
     else
       return 0;
@@ -195,91 +210,162 @@
     set(runner.p_data, run_all_idx, to_integer(true));
     set(runner.p_data, test_case_iteration_idx, 0);
     set(runner.p_data, test_case_exit_after_error_idx, to_integer(false));
     set(runner.p_data, test_suite_exit_after_error_idx, to_integer(false));
     set(runner.p_data, runner_cfg_idx, to_integer(new_string_ptr(str_pool, runner_cfg_default)));
 
     set(runner.p_data, disable_simulation_exit_idx, to_integer(false));
+
     set(runner.p_data, entry_locks_idx, to_integer(integer_vector_ptr_t'(new_integer_vector_ptr(n_legal_phases))));
+    for idx in 0 to n_legal_phases - 1 loop
+      set(to_integer_vector_ptr(get(runner.p_data, entry_locks_idx)), idx, to_integer(integer_vector_ptr_t'(new_integer_vector_ptr(lock_idx + n_locks))));
+    end loop;
+
     set(runner.p_data, exit_locks_idx, to_integer(integer_vector_ptr_t'(new_integer_vector_ptr(n_legal_phases))));
+    for idx in 0 to n_legal_phases - 1 loop
+      set(to_integer_vector_ptr(get(runner.p_data, exit_locks_idx)), idx, to_integer(integer_vector_ptr_t'(new_integer_vector_ptr(lock_idx + n_locks))));
+    end loop;
+
     set(runner.p_data, timeout_idx, to_integer(new_string_ptr(str_pool, encode(0 ns))));
+    set(runner.p_data, is_within_gates_idx, 0);
   end;
 
   procedure set_active_python_runner(runner : runner_t; value : boolean) is
   begin
     set(runner.p_data, active_python_runner_idx, to_integer(value));
   end;
 
   impure function has_active_python_runner(runner : runner_t) return boolean is
   begin
     return get(runner.p_data, active_python_runner_idx) = 1;
   end function;
 
-  procedure lock_entry(runner : runner_t; phase : runner_legal_phase_t) is
+  impure function get_entry_key(runner : runner_t; phase : runner_legal_phase_t) return key_t is
+    variable key : key_t;
     constant entry_locks : integer_vector_ptr_t := to_integer_vector_ptr(get(runner.p_data, entry_locks_idx));
     constant idx : natural := runner_legal_phase_t'pos(phase) - runner_legal_phase_t'pos(runner_legal_phase_t'low);
-    constant n_locks : natural := get(entry_locks, idx);
+    constant lock_data : integer_vector_ptr_t := to_integer_vector_ptr(get(entry_locks, idx));
+    constant n_used_locks : natural := get(lock_data, n_used_locks_idx);
   begin
-    set(entry_locks, idx, n_locks + 1);
+    key.p_is_entry_key := true;
+    key.p_key_id := n_used_locks;
+    key.p_phase := phase;
+
+    set(lock_data, n_used_locks_idx, n_used_locks + 1);
+
+    return key;
   end;
 
-  procedure unlock_entry(runner : runner_t; phase : runner_legal_phase_t) is
-    constant entry_locks : integer_vector_ptr_t := to_integer_vector_ptr(get(runner.p_data, entry_locks_idx));
+  impure function get_exit_key(runner : runner_t; phase : runner_legal_phase_t) return key_t is
+    variable key : key_t;
+    constant exit_locks : integer_vector_ptr_t := to_integer_vector_ptr(get(runner.p_data, exit_locks_idx));
     constant idx : natural := runner_legal_phase_t'pos(phase) - runner_legal_phase_t'pos(runner_legal_phase_t'low);
-    constant n_locks : natural := get(entry_locks, idx);
+    constant lock_data : integer_vector_ptr_t := to_integer_vector_ptr(get(exit_locks, idx));
+    constant n_used_locks : natural := get(lock_data, n_used_locks_idx);
   begin
-    failure_if(runner_trace_logger, n_locks = 0,
-               "No locks to unlock on " & replace(runner_legal_phase_t'image(phase), "_", " ") & " entry gate.");
-    set(entry_locks, idx, n_locks - 1);
+    key.p_is_entry_key := false;
+    key.p_key_id := n_used_locks;
+    key.p_phase := phase;
+
+    set(lock_data, n_used_locks_idx, n_used_locks + 1);
+
+    return key;
   end;
 
-  impure function entry_is_locked(runner : runner_t; phase : runner_legal_phase_t) return boolean is
-    constant entry_locks : integer_vector_ptr_t := to_integer_vector_ptr(get(runner.p_data, entry_locks_idx));
-    constant idx : natural := runner_legal_phase_t'pos(phase) - runner_legal_phase_t'pos(runner_legal_phase_t'low);
-    constant n_locks : natural := get(entry_locks, idx);
+  impure function is_locked(runner : runner_t; key : key_t) return boolean is
+    constant idx : natural := runner_legal_phase_t'pos(key.p_phase) - runner_legal_phase_t'pos(runner_legal_phase_t'low);
+    variable lock_data : integer_vector_ptr_t;
   begin
-    return n_locks > 0;
+    if key.p_is_entry_key then
+      lock_data := to_integer_vector_ptr(get(to_integer_vector_ptr(get(runner.p_data, entry_locks_idx)), idx));
+    else
+      lock_data := to_integer_vector_ptr(get(to_integer_vector_ptr(get(runner.p_data, exit_locks_idx)), idx));
+    end if;
+
+    return get(lock_data, lock_idx + key.p_key_id) = lock_is_locked;
   end;
 
-  procedure lock_exit(runner : runner_t; phase : runner_legal_phase_t) is
-    constant exit_locks : integer_vector_ptr_t := to_integer_vector_ptr(get(runner.p_data, exit_locks_idx));
-    constant idx : natural := runner_legal_phase_t'pos(phase) - runner_legal_phase_t'pos(runner_legal_phase_t'low);
-    constant n_locks : natural := get(exit_locks, idx);
+  procedure lock(runner : runner_t; key : key_t) is
+    constant idx : natural := runner_legal_phase_t'pos(key.p_phase) - runner_legal_phase_t'pos(runner_legal_phase_t'low);
+    variable lock_data : integer_vector_ptr_t;
   begin
-    set(exit_locks, idx, n_locks + 1);
+    if key.p_is_entry_key then
+      lock_data := to_integer_vector_ptr(get(to_integer_vector_ptr(get(runner.p_data, entry_locks_idx)), idx));
+    else
+      lock_data := to_integer_vector_ptr(get(to_integer_vector_ptr(get(runner.p_data, exit_locks_idx)), idx));
+    end if;
+
+    if get(lock_data, lock_idx + key.p_key_id) = lock_is_unlocked then
+      set(lock_data, lock_idx + key.p_key_id, lock_is_locked);
+      set(lock_data, n_locked_idx, get(lock_data, n_locked_idx) + 1);
+    end if;
   end;
 
-  procedure unlock_exit(runner : runner_t; phase : runner_legal_phase_t) is
-    constant exit_locks : integer_vector_ptr_t := to_integer_vector_ptr(get(runner.p_data, exit_locks_idx));
+  procedure unlock(runner : runner_t; key : key_t) is
+    constant idx : natural := runner_legal_phase_t'pos(key.p_phase) - runner_legal_phase_t'pos(runner_legal_phase_t'low);
+    variable lock_data : integer_vector_ptr_t;
+  begin
+    if key.p_is_entry_key then
+      lock_data := to_integer_vector_ptr(get(to_integer_vector_ptr(get(runner.p_data, entry_locks_idx)), idx));
+    else
+      lock_data := to_integer_vector_ptr(get(to_integer_vector_ptr(get(runner.p_data, exit_locks_idx)), idx));
+    end if;
+
+    if get(lock_data, lock_idx + key.p_key_id) = lock_is_locked then
+      set(lock_data, lock_idx + key.p_key_id, lock_is_unlocked);
+      set(lock_data, n_locked_idx, get(lock_data, n_locked_idx) - 1);
+    end if;
+  end;
+
+  impure function entry_is_locked(runner : runner_t; phase : runner_legal_phase_t) return boolean is
+    constant entry_locks : integer_vector_ptr_t := to_integer_vector_ptr(get(runner.p_data, entry_locks_idx));
     constant idx : natural := runner_legal_phase_t'pos(phase) - runner_legal_phase_t'pos(runner_legal_phase_t'low);
-    constant n_locks : natural := get(exit_locks, idx);
+    constant lock_data : integer_vector_ptr_t := to_integer_vector_ptr(get(entry_locks, idx));
+    constant n_locked : natural := get(lock_data, n_locked_idx);
   begin
-    failure_if(runner_trace_logger, n_locks = 0,
-               "No locks to unlock on " & replace(runner_legal_phase_t'image(phase), "_", " ") & " exit gate.");
-    set(exit_locks, idx, n_locks - 1);
+    return n_locked > 0;
   end;
 
   impure function exit_is_locked(runner : runner_t; phase : runner_legal_phase_t) return boolean is
     constant exit_locks : integer_vector_ptr_t := to_integer_vector_ptr(get(runner.p_data, exit_locks_idx));
     constant idx : natural := runner_legal_phase_t'pos(phase) - runner_legal_phase_t'pos(runner_legal_phase_t'low);
-    constant n_locks : natural := get(exit_locks, idx);
+    constant lock_data : integer_vector_ptr_t := to_integer_vector_ptr(get(exit_locks, idx));
+    constant n_locked : natural := get(lock_data, n_locked_idx);
   begin
-    return n_locks > 0;
+    return n_locked > 0;
   end;
 
   procedure set_phase(runner : runner_t; new_phase : runner_phase_t) is
   begin
     set(runner.p_data, runner_phase_idx, runner_phase_t'pos(new_phase));
   end;
 
   impure function get_phase(runner : runner_t) return runner_phase_t is
   begin
     return runner_phase_t'val(get(runner.p_data, runner_phase_idx));
   end;
 
+  procedure set_gate_status(runner : runner_t; is_within_gates : boolean) is
+  begin
+    if is_within_gates then
+      set(runner.p_data, is_within_gates_idx, 1);
+    else
+      set(runner.p_data, is_within_gates_idx, 0);
+    end if;
+  end;
+
+  impure function is_within_gates(runner : runner_t; phase : runner_legal_phase_t) return boolean is
+  begin
+    if get_phase(runner) /= phase then
+      return false;
+    end if;
+
+    return get(runner.p_data, is_within_gates_idx) = 1;
+  end;
+
   procedure set_test_case_name(runner : runner_t; index : positive; new_name : string) is
     constant test_case_names : integer_vector_ptr_t := to_integer_vector_ptr(get(runner.p_data, test_case_names_idx));
     variable test_case_name : string_ptr_t;
   begin
     if index-1 >= length(test_case_names) then
       resize(test_case_names, index, value => to_integer(null_string_ptr));
     end if;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/run/test/run_tests.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/run/test/run_tests.vhd`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 use vunit_lib.checker_pkg.all;
 use vunit_lib.check_pkg.all;
 use std.textio.all;
 use vunit_lib.run_types_pkg.all;
 use vunit_lib.run_pkg.all;
 use vunit_lib.runner_pkg.all;
 use vunit_lib.core_pkg;
+use vunit_lib.event_common_pkg.all;
 
 library ieee;
 use ieee.std_logic_1164.all;
 
 entity run_tests is
   generic (output_path : string);
 end entity;
@@ -54,83 +55,100 @@
     end if;
     check_equal(now - t_start, 9 ns, "Expected wait on test_case_setup phase to be 9 ns.");
     test_process_completed <= true;
     wait;
   end process;
 
   test_process2 : process is
+    constant test_suite_setup_entry_key : key_t := get_entry_key(test_suite_setup);
+    constant test_suite_setup_exit_key : key_t := get_exit_key(test_suite_setup);
   begin
     wait until start_test_process2;
-    lock_entry(runner, test_suite_setup);
-    lock_exit(runner, test_suite_setup);
+    lock(runner, test_suite_setup_entry_key);
+    lock(runner, test_suite_setup_exit_key);
     wait for 7 ns;
-    unlock_entry(runner, test_suite_setup);
+    unlock(runner, test_suite_setup_entry_key);
     wait for 4 ns;
-    unlock_exit(runner, test_suite_setup);
+    unlock(runner, test_suite_setup_exit_key);
     wait;
   end process;
 
   locking_proc1: process is
+    constant test_runner_setup_entry_key : key_t := get_entry_key(test_runner_setup);
+    constant test_runner_setup_exit_key : key_t := get_exit_key(test_runner_setup);
+    constant test_suite_setup_entry_key : key_t := get_entry_key(test_suite_setup);
+    constant test_suite_setup_exit_key : key_t := get_exit_key(test_suite_setup);
+    constant test_case_setup_entry_key : key_t := get_entry_key(test_case_setup);
+    constant test_case_setup_exit_key : key_t := get_exit_key(test_case_setup);
+    constant test_case_entry_key : key_t := get_entry_key(test_case);
+    constant test_case_exit_key : key_t := get_exit_key(test_case);
+    constant test_case_cleanup_entry_key : key_t := get_entry_key(test_case_cleanup);
+    constant test_case_cleanup_exit_key : key_t := get_exit_key(test_case_cleanup);
+    constant test_suite_cleanup_entry_key : key_t := get_entry_key(test_suite_cleanup);
+    constant test_suite_cleanup_exit_key : key_t := get_exit_key(test_suite_cleanup);
+    constant test_runner_cleanup_entry_key : key_t := get_entry_key(test_runner_cleanup);
+    constant test_runner_cleanup_exit_key : key_t := get_exit_key(test_runner_cleanup);
   begin
     wait until start_locking_process = true;
-    lock_entry(runner, test_runner_setup, locking_proc1_logger);
-    lock_exit(runner, test_runner_setup, locking_proc1_logger);
-    lock_entry(runner, test_suite_setup, locking_proc1_logger);
-    lock_exit(runner, test_suite_setup, locking_proc1_logger);
+    lock(runner, test_runner_setup_entry_key, locking_proc1_logger);
+    lock(runner, test_runner_setup_exit_key, locking_proc1_logger);
+    lock(runner, test_suite_setup_entry_key, locking_proc1_logger);
+    lock(runner, test_suite_setup_exit_key, locking_proc1_logger);
     wait for 2 ns;
-    unlock_entry(runner, test_runner_setup, locking_proc1_logger);
+    unlock(runner, test_runner_setup_entry_key, locking_proc1_logger);
     wait for 1 ns;
-    unlock_exit(runner, test_runner_setup, locking_proc1_logger);
+    unlock(runner, test_runner_setup_exit_key, locking_proc1_logger);
     wait for 1 ns;
-    unlock_entry(runner, test_suite_setup, locking_proc1_logger);
+    unlock(runner, test_suite_setup_entry_key, locking_proc1_logger);
     wait for 3 ns;
 
-    lock_entry(runner, test_case_setup, locking_proc1_logger);
-    lock_exit(runner, test_case_setup, locking_proc1_logger);
-    lock_entry(runner, test_case, locking_proc1_logger);
-    lock_exit(runner, test_case, locking_proc1_logger);
-    lock_entry(runner, test_case_cleanup, locking_proc1_logger);
-    lock_exit(runner, test_case_cleanup, locking_proc1_logger);
-    lock_entry(runner, test_suite_cleanup, locking_proc1_logger);
-    lock_exit(runner, test_suite_cleanup, locking_proc1_logger);
-    lock_entry(runner, test_runner_cleanup, locking_proc1_logger);
-    lock_exit(runner, test_runner_cleanup, locking_proc1_logger);
+    lock(runner, test_case_setup_entry_key, locking_proc1_logger);
+    lock(runner, test_case_setup_exit_key, locking_proc1_logger);
+    lock(runner, test_case_entry_key, locking_proc1_logger);
+    lock(runner, test_case_exit_key, locking_proc1_logger);
+    lock(runner, test_case_cleanup_entry_key, locking_proc1_logger);
+    lock(runner, test_case_cleanup_exit_key, locking_proc1_logger);
+    lock(runner, test_suite_cleanup_entry_key, locking_proc1_logger);
+    lock(runner, test_suite_cleanup_exit_key, locking_proc1_logger);
+    lock(runner, test_runner_cleanup_entry_key, locking_proc1_logger);
+    lock(runner, test_runner_cleanup_exit_key, locking_proc1_logger);
 
     wait for 1 ns;
-    unlock_exit(runner, test_suite_setup, locking_proc1_logger);
+    unlock(runner, test_suite_setup_exit_key, locking_proc1_logger);
     wait for 1 ns;
-    unlock_entry(runner, test_case_setup, locking_proc1_logger);
+    unlock(runner, test_case_setup_entry_key, locking_proc1_logger);
     wait for 2 ns;
-    unlock_exit(runner, test_case_setup, locking_proc1_logger);
+    unlock(runner, test_case_setup_exit_key, locking_proc1_logger);
     wait for 1 ns;
-    unlock_entry(runner, test_case, locking_proc1_logger);
+    unlock(runner, test_case_entry_key, locking_proc1_logger);
     wait for 2 ns;
-    unlock_exit(runner, test_case, locking_proc1_logger);
+    unlock(runner, test_case_exit_key, locking_proc1_logger);
     wait for 1 ns;
-    unlock_entry(runner, test_case_cleanup, locking_proc1_logger);
+    unlock(runner, test_case_cleanup_entry_key, locking_proc1_logger);
     wait for 2 ns;
-    unlock_exit(runner, test_case_cleanup, locking_proc1_logger);
+    unlock(runner, test_case_cleanup_exit_key, locking_proc1_logger);
     wait for 4 ns;
-    unlock_entry(runner, test_suite_cleanup, locking_proc1_logger);
+    unlock(runner, test_suite_cleanup_entry_key, locking_proc1_logger);
     wait for 2 ns;
-    unlock_exit(runner, test_suite_cleanup, locking_proc1_logger);
+    unlock(runner, test_suite_cleanup_exit_key, locking_proc1_logger);
     wait for 1 ns;
-    unlock_entry(runner, test_runner_cleanup, locking_proc1_logger);
+    unlock(runner, test_runner_cleanup_entry_key, locking_proc1_logger);
     wait for 1 ns;
-    unlock_exit(runner, test_runner_cleanup, locking_proc1_logger);
+    unlock(runner, test_runner_cleanup_exit_key, locking_proc1_logger);
     wait;
   end process locking_proc1;
 
   locking_proc2: process is
+    constant key : key_t := get_exit_key(test_runner_cleanup);
   begin
     wait until start_locking_process = true;
     wait for 6 ns;
-    lock_exit(runner, test_runner_cleanup, locking_proc2_logger);
+    lock(runner, key, locking_proc2_logger);
     wait for 21 ns;
-    unlock_exit(runner, test_runner_cleanup, locking_proc2_logger);
+    unlock(runner, key, locking_proc2_logger);
     wait;
   end process locking_proc2;
 
   watchdog: process is
   begin
     wait until start_test_runner_watchdog;
     test_runner_watchdog(runner, 10 ns);
@@ -151,19 +169,15 @@
       return integer'image(value);
     end;
 
     procedure test_case_setup is
     begin
       runner_init(runner_state);
       runner(runner_exit_status_idx) <= runner_exit_with_errors;
-      if runner(runner_event_idx) /= runner_event then
-        runner(runner_event_idx) <= runner_event;
-        wait until runner(runner_event_idx) = runner_event;
-        runner(runner_event_idx) <= idle_runner;
-      end if;
+      notify(runner_phase);
     end;
 
     constant c : checker_t := new_checker("checker_t", default_log_level => failure);
 
     procedure test_case_cleanup is
       variable stat : checker_stat_t;
     begin
@@ -183,14 +197,18 @@
     constant test_checker : checker_t := new_checker("test_checker");
     variable runner_cfg : line;
     variable passed : boolean;
     variable level : log_level_t;
     variable my_checker : checker_t;
     variable error_counter : natural := 0;
     constant test_runner_logger : logger_t := get_logger("test_runner");
+    constant test_runner_setup_entry_key : key_t := get_entry_key(test_runner_setup);
+    constant test_runner_setup_exit_key : key_t := get_exit_key(test_runner_setup);
+    constant test_case_setup_entry_key : key_t := get_entry_key(test_case_setup);
+    constant test_case_setup_exit_key : key_t := get_exit_key(test_case_setup);
 
   begin
     banner("Should extract single enabled test case from input string");
     test_case_setup;
     test_runner_setup(runner, "enabled_test_cases : Should foo");
     check(c, num_of_enabled_test_cases = 1, "Expected 1 enabled test case but got " & integer'image(num_of_enabled_test_cases) & ".");
     check(c, enabled("Should foo"), "Expected ""Should foo"" test case to be enabled");
@@ -528,27 +546,14 @@
     test_runner_cleanup(runner);
     if not test_process_completed then
       wait until test_process_completed;
     end if;
     test_case_cleanup;
 
     ---------------------------------------------------------------------------
-    banner("Test that unlocking an unlocked phase will trigger a failure");
-    test_case_setup;
-    mock(runner_trace_logger);
-    unlock_entry(runner, test_runner_setup);
-    unlock_exit(runner, test_runner_setup);
-    check_log(runner_trace_logger, "No locks to unlock on test runner setup entry gate.", failure);
-    check_log(runner_trace_logger, "Unlocked test runner setup phase entry gate.", trace);
-    check_log(runner_trace_logger, "No locks to unlock on test runner setup exit gate.", failure);
-    check_log(runner_trace_logger, "Unlocked test runner setup phase exit gate.", trace);
-    unmock(runner_trace_logger);
-    test_case_cleanup;
-
-    ---------------------------------------------------------------------------
     banner("Should be possible to read current test case name");
     test_case_setup;
     test_runner_setup(runner, "enabled_test_cases : test a,, test b");
     i := 0;
     while test_suite loop
       while in_test_case loop
         if i = 0 then
@@ -737,18 +742,18 @@
 
     ---------------------------------------------------------------------------
     banner("Should be possible to track (un)lock commands to file and line number");
     test_case_setup;
 
     test_runner_setup(runner, "enabled_test_cases : test a");
     mock(runner_trace_logger);
-    lock_entry(runner, test_case_setup, line_num => 17, file_name => "foo1.vhd");
-    lock_exit(runner, test_case_setup, line_num => 18, file_name => "foo2.vhd");
-    unlock_entry(runner, test_case_setup, line_num => 19, file_name => "foo3.vhd");
-    unlock_exit(runner, test_case_setup, line_num => 20, file_name => "foo4.vhd");
+    lock(runner, test_case_setup_entry_key, runner_trace_logger, line_num => 17, file_name => "foo1.vhd");
+    lock(runner, test_case_setup_exit_key, runner_trace_logger, line_num => 18, file_name => "foo2.vhd");
+    unlock(runner, test_case_setup_entry_key, runner_trace_logger, line_num => 19, file_name => "foo3.vhd");
+    unlock(runner, test_case_setup_exit_key, runner_trace_logger, line_num => 20, file_name => "foo4.vhd");
     check_log(runner_trace_logger, "Locked test case setup phase entry gate.", trace,
               line_num => 17, file_name => "foo1.vhd");
     check_log(runner_trace_logger, "Locked test case setup phase exit gate.", trace,
               line_num => 18, file_name => "foo2.vhd");
     check_log(runner_trace_logger, "Unlocked test case setup phase entry gate.", trace,
               line_num => 19, file_name => "foo3.vhd");
     check_log(runner_trace_logger, "Unlocked test case setup phase exit gate.", trace,
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/run/test/tb_run.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/run/test/tb_run.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/run/test/tb_watchdog.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/run/test/tb_watchdog.vhd`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 library vunit_lib;
 use vunit_lib.log_levels_pkg.all;
 use vunit_lib.logger_pkg.all;
 use vunit_lib.check_pkg.all;
 use vunit_lib.run_types_pkg.all;
 use vunit_lib.run_pkg.all;
 use vunit_lib.runner_pkg.all;
+use vunit_lib.event_pkg.all;
 
 entity tb_watchdog is
   generic (
     runner_cfg : string);
 end entity;
 
 architecture tb of tb_watchdog is
@@ -26,15 +27,15 @@
     test_runner_setup(runner, runner_cfg);
 
     if run("test watchdog no timeout") then
       wait for 1 ns;
 
     elsif run("Test watchdog timeout") then
       mock(runner_trace_logger, error);
-      wait until timeout_notification(runner);
+      wait until is_active_msg(runner_timeout);
       check_equal(now, 2 ns);
       wait for 1 ps;
       check_only_log(runner_trace_logger, "Test runner timeout after " & time'image(2 ns) & ".", error, 2 ns);
       unmock(runner_trace_logger);
 
     elsif run("test setting timeout") then
       mock(runner_trace_logger, error);
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/string_ops/src/string_ops.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/string_ops/src/string_ops.vhd`

 * *Files 16% similar despite different names*

```diff
@@ -109,14 +109,46 @@
     return string;
   function to_nibble_string (
     constant value : std_logic_vector)
     return string;
   function to_nibble_string (
     constant value : signed)
     return string;
+
+  -- Initial tag in subprogram string input parameters. If supported, the tag is
+  -- used to indicate that the subprogram shall take the remainder of the string
+  -- and decorate it with information internal to the subprogram. The resulting
+  -- string as the actual parameter to be used. The decoration to be performed
+  -- is specific to the subprogram being called.
+  constant decorate_tag : string := "<+/->";
+
+  -- Used by caller of a subprogram supporting string decoration. The function
+  -- returns:
+  -- 1. decorate_tag if input is the empty string. The called subprogram is in
+  --    full control of the string used. For example, the decorate_tag may
+  --    be translated to "BFM has performed 5 transactions"
+  -- 2. decorate_tag & str if str starts with one of the punctuation marks '.', ',',
+  --    ':', ';', '?', or '!'. For example, if the provided string is
+  --    ". Completed init sequence." the subprogram may translate the decorated string
+  --    to "BFM has performed 5 transactions. Completed init sequence."
+  -- 3. decorate_tag & " " & str if str doesn't start with one of the punctuation marks.
+  --    If str = "after completing init sequence." the subprogram may translate
+  --    the decorated string to "BFM has performed 5 transactions after completing init
+  --    sequence."
+  --
+  -- Note: The function is very specific to VUnit and is not recommended for external use.
+  function decorate(
+  str : string := "") return string;
+
+  -- Return true if str is decorated with decorate_tag, false otherwise.
+  function is_decorated(str : string) return boolean;
+
+  -- Remove decorate_tag from str if str is decorated
+  function undecorate(str : string := "") return string;
+
 end package;
 
 package body string_ops is
   function offset (
     constant s     : string;
     constant index : natural)
     return natural is
@@ -701,8 +733,37 @@
   function to_nibble_string (
     constant value : signed)
     return string is
   begin
     return to_nibble_string(unsigned(value));
   end function to_nibble_string;
 
+  function decorate(str : string := "") return string is
+  begin
+    if str = "" then
+      return decorate_tag;
+    elsif str(str'left) = '.' or str(str'left) = ',' or str(str'left) = ':' or str(str'left) = ';' or str(str'left) = '?' or str(str'left) = '!' then
+      return decorate_tag & str;
+    else
+      return decorate_tag & " " & str;
+    end if;
+  end;
+
+  function is_decorated(str : string) return boolean is
+  begin
+    if str'length < decorate_tag'length then
+      return false;
+    else
+      return str(str'left to str'left + decorate_tag'length - 1) = decorate_tag;
+    end if;
+  end;
+
+  function undecorate(str : string := "") return string is
+  begin
+    if is_decorated(str) then
+      return str(str'left + decorate_tag'length to str'right);
+    else
+      return str;
+    end if;
+  end;
+
 end package body;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/string_ops/test/tb_string_ops.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/string_ops/test/tb_string_ops.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/run.py` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/run.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_master.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_master.vhd`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
 architecture a of avalon_master is
   constant av_master_read_actor : actor_t := new_actor;
   constant avmm_burst_rd_actor : actor_t := new_actor;
   constant acknowledge_queue : queue_t := new_queue;
   constant burst_acknowledge_queue : queue_t := new_queue;
   constant burstlen_queue : queue_t := new_queue;
-  signal burst_read_flag : boolean := false;
 begin
 
   main : process
     variable request_msg : msg_t;
     variable msg_type : msg_type_t;
     variable rnd : RandomPType;
     variable msgs : natural;
@@ -124,15 +123,15 @@
             wait until rising_edge(clk) and waitrequest = '0';
             write <= '0';
             address(address'range) <= (others => 'U');
             burstcount(burstcount'range) <= (others => 'U');
           end loop;
 
         elsif msg_type = wait_until_idle_msg then
-          wait until not burst_read_flag and is_empty(burst_acknowledge_queue) and rising_edge(clk);
+          wait until is_empty(burst_acknowledge_queue) and rising_edge(clk);
           handle_wait_until_idle(net, msg_type, request_msg);
 
         else
           unexpected_msg_type(msg_type);
         end if;
       else
         wait until rising_edge(clk);
@@ -162,24 +161,22 @@
   end process;
 
   burst_read_capture : process
     variable request_msg, reply_msg : msg_t;
     variable burst : positive;
   begin
     wait until readdatavalid = '1' and not is_empty(burst_acknowledge_queue) and rising_edge(clk);
-    burst_read_flag <= true;
-    request_msg := pop(burst_acknowledge_queue);
     burst := pop(burstlen_queue);
     reply_msg := new_msg(sender => avmm_burst_rd_actor);
     push_integer(reply_msg, burst);
     push_std_ulogic_vector(reply_msg, readdata);
     for i in 1 to burst-1 loop
       wait until readdatavalid = '1' and rising_edge(clk) for 1 us;
       check_true(readdatavalid = '1', "avalon master burst readdatavalid timeout");
       push_std_ulogic_vector(reply_msg, readdata);
     end loop;
+    request_msg := pop(burst_acknowledge_queue);
     reply(net, request_msg, reply_msg);
     delete(request_msg);
-    burst_read_flag <= false;
   end process;
 
 end architecture;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_sink.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_sink.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_slave.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_slave.vhd`

 * *Files 6% similar despite different names*

```diff
@@ -42,28 +42,35 @@
   constant slave_read_msg   : msg_type_t := new_msg_type("avmm slave read");
 
 begin
 
   write_handler : process
     variable pending_writes : positive := 1;
     variable addr : natural;
+    variable word_i : std_logic_vector(writedata'length-1 downto 0);
+    variable byteenable_i : std_logic_vector(byteenable'length-1 downto 0);
   begin
     loop
       wait until write = '1' and waitrequest = '0' and rising_edge(clk);
+      word_i := writedata;
+      byteenable_i := byteenable;
       -- Burst write in progress
       if pending_writes > 1 then
         addr := addr + byteenable'length;
         pending_writes := pending_writes -1;
-        write_word(avalon_slave.p_memory, addr, writedata);
       -- Burst start or single burst
       else
         addr := to_integer(unsigned(address));
         pending_writes := to_integer(unsigned(burstcount));
-        write_word(avalon_slave.p_memory, addr, writedata);
       end if;
+      for idx in 0 to word_i'length/8-1 loop
+        if byteenable_i(idx) then
+          write_byte(avalon_slave.p_memory, addr + idx, to_integer(unsigned(word_i(8*idx+7 downto 8*idx))));
+        end if;
+      end loop;
     end loop;
   end process;
 
   read_request : process
     variable rd_request_msg : msg_t;
   begin
     wait until read = '1' and waitrequest = '0' and rising_edge(clk);
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_source.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_source.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/avalon_stream_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/avalon_stream_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_lite_master.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_lite_master.vhd`

 * *Files 6% similar despite different names*

```diff
@@ -46,40 +46,45 @@
     bvalid : in std_logic;
     bready : out std_logic := '0';
     bresp : in axi_resp_t := axi_resp_okay);
 end entity;
 
 architecture a of axi_lite_master is
   constant reply_queue, message_queue : queue_t := new_queue;
+  signal idle : boolean := true;
 begin
   main : process
     variable request_msg : msg_t;
     variable msg_type : msg_type_t;
   begin
     receive(net, bus_handle.p_actor, request_msg);
     msg_type := message_type(request_msg);
 
     if is_read(msg_type) or is_write(msg_type) then
       push(message_queue, request_msg);
     elsif msg_type = wait_until_idle_msg then
-      wait until ((bvalid and bready) = '1' or (rvalid and rready) = '1') and is_empty(message_queue) and rising_edge(aclk);
+      if not idle or not is_empty(message_queue) then
+        wait until idle and is_empty(message_queue) and rising_edge(aclk);
+      end if;
       handle_wait_until_idle(net, msg_type, request_msg);
     else
       unexpected_msg_type(msg_type);
     end if;
   end process;
 
   -- Use separate process to always align to rising edge of clock
   bus_process : process
     variable request_msg : msg_t;
     variable msg_type : msg_type_t;
     variable w_done, aw_done : boolean;
     variable expected_resp : axi_resp_t;
   begin
     wait until rising_edge(aclk) and not is_empty(message_queue);
+    idle <= false;
+    wait for 0 ps;
 
     request_msg := pop(message_queue);
     msg_type := message_type(request_msg);
 
     if is_read(msg_type) then
       araddr <= pop_std_ulogic_vector(request_msg);
       expected_resp := pop_std_ulogic_vector(request_msg) when is_axi_lite_msg(msg_type) else axi_resp_okay;
@@ -133,14 +138,16 @@
 
       if is_visible(bus_handle.p_logger, debug) then
         debug(bus_handle.p_logger,
               "Wrote 0x" & to_hstring(wdata) &
                 " to address 0x" & to_hstring(awaddr));
       end if;
     end if;
+
+    idle <= true;
   end process;
 
   -- Reply in separate process do not destroy alignment with the clock
   read_reply : process
     variable request_msg, reply_msg : msg_t;
   begin
     wait until (rvalid and rready) = '1' and rising_edge(aclk);
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_lite_master_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_lite_master_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_read_slave.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_read_slave.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_slave_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_slave_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_slave_private_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_slave_private_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_statistics_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_statistics_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_master.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_master.vhd`

 * *Files 1% similar despite different names*

```diff
@@ -93,20 +93,23 @@
   begin
     rnd.InitSeed(rnd'instance_name);
     loop
       if drive_invalid then
         drive_invalid_output(tdata, tkeep, tstrb, tid, tdest, tuser);
       end if;
 
-      -- Wait for messages to arrive on the queue, posted by the process above
-      wait until rising_edge(aclk) and (not is_empty(message_queue) or areset_n = '0');
-
       if (areset_n = '0') then
         tvalid <= '0';
+        wait until areset_n = '1' and rising_edge(aclk);
       else
+        if is_empty(message_queue) then
+          -- Wait for messages to arrive on the queue, posted by the process above
+          wait until (not is_empty(message_queue) or areset_n = '0') and rising_edge(aclk);
+        end if;
+
         while not is_empty(message_queue) loop
           msg := pop(message_queue);
           msg_type := message_type(msg);
 
           if msg_type = wait_for_time_msg then
             handle_sync_message(net, msg_type, msg);
             -- Re-align with the clock when a wait for time message was handled, because this breaks edge alignment.
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_monitor.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_monitor.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_private_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_private_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_protocol_checker.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_protocol_checker.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -145,16 +145,15 @@
         set(active_streams, to_integer(tid), value);
       end if;
     end process;
 
     check_that_streams_have_ended : process
       variable incomplete_streams : line;
     begin
-      lock_entry(runner, test_runner_cleanup);
-      wait_until(runner, test_runner_cleanup);
+      wait until is_active(runner_phase) and is_within_gates_of(test_runner_cleanup);
 
       if tid'length = 0 then
         check(rule9_checker, get(active_streams, 0) = 0, result("for packet completion."));
       else
         for i in 0 to 2 * tid'length - 1 loop
           if get(active_streams, i) /= 0 then
             if incomplete_streams = null then
@@ -169,15 +168,14 @@
           check_failed(rule9_checker, result("for packet completion for the following streams: " &
             incomplete_streams.all & "."));
         else
           check_passed(rule9_checker, result("for packet completion."));
         end if;
       end if;
 
-      unlock_entry(runner, test_runner_cleanup);
       wait;
     end process;
   end block;
 
   -- AXI4STREAM_ERRM_TUSER_X A value of X on TUSER is not permitted when not in reset
   -- is HIGH
   check_not_unknown(rule10_checker, aclk, areset_n, tuser, result("for tuser when areset_n is high"));
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_stream_slave.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_stream_slave.vhd`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 context work.vunit_context;
 context work.com_context;
 use work.stream_slave_pkg.all;
 use work.axi_stream_pkg.all;
 use work.axi_stream_private_pkg.all;
 use work.sync_pkg.all;
 use work.string_ptr_pkg.all;
+use work.event_common_pkg.all;
+use work.event_pkg.all;
 
 library osvvm;
 use osvvm.RandomPkg.RandomPType;
 
 entity axi_stream_slave is
   generic (
     slave : axi_stream_slave_t);
@@ -34,17 +36,19 @@
     tdest    : in std_logic_vector(dest_length(slave)-1 downto 0)   := (others => '0');
     tuser    : in std_logic_vector(user_length(slave)-1 downto 0)   := (others => '0')
  );
 end entity;
 
 architecture a of axi_stream_slave is
 
-  constant notify_request_msg      : msg_type_t := new_msg_type("notify request");
-  constant message_queue           : queue_t    := new_queue;
-  signal   notify_bus_process_done : std_logic  := '0';
+  constant notify_request_msg       : msg_type_t := new_msg_type("notify request");
+  constant message_queue            : queue_t    := new_queue;
+  constant bus_process_done_base_id : id_t       := get_id("vunit_lib:axi_stream_slave:bus_process_done");
+  constant bus_process_done_id      : id_t       := get_id(to_string(num_children(bus_process_done_base_id)), parent => bus_process_done_base_id);
+  signal bus_process_done           : event_t    := new_event(bus_process_done_id);
 
 begin
 
   main : process
     variable request_msg    : msg_t;
     variable notify_msg     : msg_t;
     variable msg_type       : msg_type_t;
@@ -57,15 +61,15 @@
     elsif msg_type = check_axi_stream_msg then
       push(message_queue, request_msg);
     elsif msg_type = wait_for_time_msg then
       push(message_queue, request_msg);
     elsif msg_type = wait_until_idle_msg then
       notify_msg := new_msg(notify_request_msg);
       push(message_queue, notify_msg);
-      wait on notify_bus_process_done until is_empty(message_queue);
+      wait until is_active(bus_process_done) and is_empty(message_queue);
       handle_wait_until_idle(net, msg_type, request_msg);
     else
       unexpected_msg_type(msg_type);
     end if;
   end process;
 
   bus_process : process
@@ -88,16 +92,18 @@
       tdest(tdest'range),
       tuser(tuser'range)
     );
     variable rnd : RandomPType;
   begin
     rnd.InitSeed(rnd'instance_name);
     loop
+      if is_empty(message_queue) then
         -- Wait for messages to arrive on the queue, posted by the process above
-      wait until rising_edge(aclk) and (not is_empty(message_queue));
+        wait until rising_edge(aclk) and (not is_empty(message_queue));
+      end if;
 
       while not is_empty(message_queue) loop
         msg := pop(message_queue);
         msg_type := message_type(msg);
 
         if msg_type = wait_for_time_msg then
           handle_sync_message(net, msg_type, msg);
@@ -136,19 +142,19 @@
             check_field(tdest, pop_std_ulogic_vector(msg), "TDEST mismatch, " & to_string(report_msg));
             check_field(tuser, pop_std_ulogic_vector(msg), "TUSER mismatch, " & to_string(report_msg));
           end if;
 
         else
           unexpected_msg_type(msg_type);
         end if;
+
+        delete(msg);
       end loop;
 
-      notify_bus_process_done <= '1';
-      wait until notify_bus_process_done = '1';
-      notify_bus_process_done <= '0';
+      notify(bus_process_done);
     end loop;
   end process;
 
   axi_stream_monitor_generate : if slave.p_monitor /= null_axi_stream_monitor generate
     axi_stream_monitor_inst : entity work.axi_stream_monitor
       generic map(
         monitor => slave.p_monitor
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/axi_write_slave.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/axi_write_slave.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/bus2memory.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/bus2memory.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/bus_master_pkg-body.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/bus_master_pkg-body.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/bus_master_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/bus_master_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/memory_pkg-body.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/memory_pkg-body.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/memory_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/memory_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/memory_utils_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/memory_utils_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/ram_master.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/ram_master.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/signal_checker_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/signal_checker_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/std_logic_checker.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/std_logic_checker.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/stream_master_pkg-body.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/stream_master_pkg-body.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/stream_master_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/stream_master_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/stream_slave_pkg-body.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/stream_slave_pkg-body.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/stream_slave_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/stream_slave_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/sync_pkg-body.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/sync_pkg-body.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/sync_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/sync_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/uart_master.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/uart_master.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/uart_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/uart_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/uart_slave.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/uart_slave.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/vc_context.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/vc_context.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/wishbone_master.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/wishbone_master.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/wishbone_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/wishbone_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/src/wishbone_slave.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/src/wishbone_slave.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_master.gtkw` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_master.gtkw`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_master.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_master.vhd`

 * *Files 5% similar despite different names*

```diff
@@ -114,18 +114,18 @@
     variable rndburst : positive;
     variable i : natural;
     variable addr : natural range 0 to tb_cfg.transfers*byteenable'length;
   begin
     rnd.InitSeed(rnd'instance_name);
     test_runner_setup(runner, runner_cfg);
     set_format(display_handler, verbose, true);
-    show(tb_logger, display_handler, verbose);
-    show(default_logger, display_handler, verbose);
-    show(master_logger, display_handler, verbose);
-    show(com_logger, display_handler, verbose);
+    show(tb_logger, display_handler, trace);
+    show(default_logger, display_handler, trace);
+    show(master_logger, display_handler, trace);
+    show(com_logger, display_handler, trace);
 
     wait until rising_edge(clk);
 
     if run("wr single rd single") then
       info(tb_logger, "Writing...");
       write_bus(net, bus_handle, 0, value);
       wait until rising_edge(clk);
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_slave.gtkw` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_slave.gtkw`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_slave.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_slave.vhd`

 * *Files 13% similar despite different names*

```diff
@@ -73,17 +73,17 @@
 
   main_stim : process
     variable tmp : std_logic_vector(writedata'range);
     variable value : std_logic_vector(writedata'range) := (others => '1');
   begin
     test_runner_setup(runner, runner_cfg);
     set_format(display_handler, verbose, true);
-    show(tb_logger, display_handler, verbose);
-    show(default_logger, display_handler, verbose);
-    show(com_logger, display_handler, verbose);
+    show(tb_logger, display_handler, trace);
+    show(default_logger, display_handler, trace);
+    show(com_logger, display_handler, trace);
     burstcount <= std_logic_vector(to_unsigned(1, burstcount'length));
     wait until rising_edge(clk);
 
 
     if run("wr block rd block") then
       info(tb_logger, "Writing...");
       for i in 0 to tb_cfg.num_cycles-1 loop
@@ -132,27 +132,65 @@
       read <= '1';
       burstcount <= std_logic_vector(to_unsigned(tb_cfg.num_cycles, burstcount'length));
       address <= std_logic_vector(to_unsigned(0, address'length));
       wait until rising_edge(clk) and waitrequest = '0';
       read <= '0';
 
       wait until rising_edge(clk) and rd_ack_cnt = tb_cfg.num_cycles-1;
+
+    elsif run("byte enable") then
+      info(tb_logger, "Writing with byte enable...");
+      address <= (others => 'U');
+      burstcount(0) <= '1';
+
+      for i in 0 to tb_cfg.num_cycles-1 loop
+        if i = 0 then
+          address <= std_logic_vector(to_unsigned(0, address'length));
+          burstcount <= std_logic_vector(to_unsigned(tb_cfg.num_cycles, burstcount'length));
+        end if;
+        -- set byte enable for last word
+        if i=tb_cfg.num_cycles-1 then
+          byteenable <= std_logic_vector(to_unsigned(1,byteenable'length));
+        end if;
+        write <= '1';
+        writedata <= std_logic_vector(to_unsigned(256+i, writedata'length));
+        wait until rising_edge(clk) and waitrequest = '0';
+      end loop;
+      write <= '0';
+
+      wait until rising_edge(clk);
+      info(tb_logger, "Reading with byte enable...");
+      wait until rising_edge(clk);
+      read <= '1';
+      burstcount <= std_logic_vector(to_unsigned(tb_cfg.num_cycles, burstcount'length));
+      address <= std_logic_vector(to_unsigned(0, address'length));
+      wait until rising_edge(clk) and waitrequest = '0';
+      read <= '0';
+
+      wait until rising_edge(clk) and rd_ack_cnt = tb_cfg.num_cycles-1;
     end if;
 
     wait for 50 ns;
     test_runner_cleanup(runner);
     wait;
   end process;
   test_runner_watchdog(runner, 100 us);
 
   rd_ack: process
   begin
     wait until rising_edge(clk) and readdatavalid = '1';
-    check_equal(readdata, std_logic_vector(to_unsigned(rd_ack_cnt,
-          readdata'length)), "readdata");
+    if active_test_case = "byte enable" then
+      if rd_ack_cnt = tb_cfg.num_cycles-1 then
+        check_equal(readdata, std_logic_vector(to_unsigned(rd_ack_cnt,readdata'length)), "readdata");
+      else
+        check_equal(readdata, std_logic_vector(to_unsigned(256+rd_ack_cnt,readdata'length)), "readdata");
+      end if;
+    else
+      check_equal(readdata, std_logic_vector(to_unsigned(rd_ack_cnt,readdata'length)), "readdata");
+    end if;
     rd_ack_cnt <= rd_ack_cnt +1;
   end process;
 
   dut_slave : entity work.avalon_slave
     generic map (
       avalon_slave => avalon_slave
     )
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_stream.gtkw` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_stream.gtkw`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_stream.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_stream.vhd`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     variable is_sop  : std_logic;
     variable is_eop  : std_logic;
     variable sop_tmp : std_logic;
     variable eop_tmp : std_logic;
   begin
     test_runner_setup(runner, runner_cfg);
     set_format(display_handler, verbose, true);
-    show(avalon_sink_stream.p_logger, display_handler, verbose);
+    show(avalon_sink_stream.p_logger, display_handler, trace);
 
     wait until rising_edge(clk);
     if run("test single push and pop") then
       push_stream(net, master_stream, x"77");
       pop_stream(net, slave_stream, tmp);
       check_equal(tmp, std_logic_vector'(x"77"), "pop stream data");
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_avalon_stream_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_avalon_stream_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_lite_master.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_lite_master.vhd`

 * *Files 9% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
   signal start, done : boolean := false;
 begin
 
   main : process
     variable tmp : std_logic_vector(rdata'range);
     variable rnd : RandomPType;
+    variable timestamp : time;
   begin
     test_runner_setup(runner, runner_cfg);
     rnd.InitSeed("common_seed");
     start <= true;
     wait for 0 ns;
 
     if run("Test single write") then
@@ -115,14 +116,32 @@
           read_axi_lite(net, bus_handle, rnd.RandSlv(araddr'length), rnd.RandSlv(axi_resp_t'length), tmp);
           check_equal(tmp, rnd.RandSlv(rdata'length), "read data");
         else
           write_axi_lite(net, bus_handle, rnd.RandSlv(awaddr'length), rnd.RandSlv(wdata'length),
                          rnd.RandSlv(axi_resp_t'length));
         end if;
       end loop;
+
+    elsif run("Test idle when idle") then
+      wait until rising_edge(clk);
+      write_bus(net, bus_handle, x"01234567", x"1122");
+      wait for 0 ps;
+      timestamp := now;
+      wait_until_idle(net, bus_handle);
+      check(now > timestamp, "Write: First wait did not have to wait");
+      timestamp := now;
+      wait_until_idle(net, bus_handle);
+      check_equal(timestamp, now, "Write: Second wait had to wait");
+
+      wait until rising_edge(clk);
+      read_bus(net, bus_handle, x"01234567", tmp);
+      timestamp := now;
+      wait_until_idle(net, bus_handle);
+      check_equal(timestamp, now, "Read: Second wait had to wait");
+
     end if;
 
     wait for 100 ns;
 
     if not done then
       wait until done;
     end if;
@@ -363,14 +382,50 @@
           bvalid <= '1';
           bresp <= rnd.RandSlv(axi_resp_t'length);
           wait until (bready and bvalid) = '1' and rising_edge(clk);
           bvalid <= '0';
         end if;
       end loop;
       done <= true;
+
+    elsif enabled("Test idle when idle") then
+      wait until rising_edge(clk);
+      awready <= '1';
+      wait until (awready and awvalid) = '1' and rising_edge(clk);
+      awready <= '0';
+      check_equal(awaddr, std_logic_vector'(x"01234567"), "awaddr");
+
+      wait until rising_edge(clk);
+      wready <= '1';
+      wait until (wready and wvalid) = '1' and rising_edge(clk);
+      wready <= '0';
+      check_equal(wdata, std_logic_vector'(x"1122"), "wdata");
+      check_equal(wstrb, std_logic_vector'("11"), "wstrb");
+
+      wait until rising_edge(clk);
+      bvalid <= '1';
+      bresp <= axi_resp_okay;
+      wait until (bready and bvalid) = '1' and rising_edge(clk);
+      bvalid <= '0';
+
+      wait until rising_edge(clk);
+      arready <= '1';
+      wait until (arready and arvalid) = '1' and rising_edge(clk);
+      arready <= '0';
+      check_equal(araddr, std_logic_vector'(x"01234567"), "araddr");
+
+      wait until rising_edge(clk);
+      rvalid <= '1';
+      rresp <= axi_resp_okay;
+      rdata <= x"5566";
+      wait until (rready and rvalid) = '1' and rising_edge(clk);
+      rvalid <= '0';
+
+      done <= true;
+
     end if;
   end process;
 
   dut : entity work.axi_lite_master
     generic map (
       bus_handle => bus_handle)
     port map (
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_read_slave.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_read_slave.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_slave_private_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_slave_private_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_statistics_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_statistics_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_stream.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_stream.vhd`

 * *Files 0% similar despite different names*

```diff
@@ -499,18 +499,20 @@
                        tuser => std_logic_vector(to_unsigned(8, g_user_length)),
                        msg => "check non-blocking",
                        blocking  => false);
 
       check_equal(now, timestamp, result(" setting up transaction stalled"));
 
       wait until rising_edge(aclk);
+      wait for 1 ps;
       mocklogger := get_logger("check");
       mock(mocklogger);
 
       wait until rising_edge(aclk) and tvalid = '1';
+      wait for 1 ps;
 
       check_log(mocklogger, "TDATA mismatch, check non-blocking - Got 0000_0011 (3). Expected 0000_0110 (6).", error);
       check_log(mocklogger, "TKEEP mismatch, check non-blocking - Got 0 (0). Expected 1 (1).", error);
       check_log(mocklogger, "TSTRB mismatch, check non-blocking - Got 0 (0). Expected 1 (1).", error);
       check_log(mocklogger, "TLAST mismatch, check non-blocking - Got 1. Expected 0.", error);
       if id'length > 0 then
         check_log(mocklogger, "TID mismatch, check non-blocking - Got 0010_1010 (42). Expected 0010_1100 (44).", error);
@@ -520,15 +522,15 @@
       end if;
       if user'length > 0 then
         check_log(mocklogger, "TUSER mismatch, check non-blocking - Got 0000_0111 (7). Expected 0000_1000 (8).", error);
       end if;
 
       unmock(mocklogger);
 
-      check_equal(now, timestamp + 20 ns, " transaction time incorrect");
+      check_equal(now, timestamp + 20 ns + 1 ps, " transaction time incorrect");
 
     elsif run("test random stall on master") or run("test random pop stall on slave") then
       wait until rising_edge(aclk);
       for i in 0 to 100 loop
         pop_stream(net, slave_stream, reference);
         push(reference_queue, reference);
       end loop;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_stream_protocol_checker.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_stream_protocol_checker.vhd`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,14 @@
       tlast  <= '0';
       tready <= '1';
       wait until rising_edge(aclk);
       tlast  <= '0';
       wait until rising_edge(aclk);
 
       set_phase(runner_state, test_runner_cleanup);
-      notify(runner);
       entry_gate(runner);
 
       check_only_log(rule_logger, "Unconditional check failed for packet completion for the following streams: 0.", error);
 
       unmock(rule_logger);
 
     elsif run("Test passing check of that tuser must not be unknown unless in reset") then
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_axi_write_slave.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_axi_write_slave.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_bus_master_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_bus_master_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_memory.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_memory.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_memory_utils_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_memory_utils_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_ram_master.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_ram_master.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_std_logic_checker.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_std_logic_checker.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_sync_pkg.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_sync_pkg.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_uart.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_uart.vhd`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_wishbone_master.gtkw` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_wishbone_master.gtkw`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_wishbone_master.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_wishbone_master.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,18 @@
     variable bus_rd_ref1 : bus_reference_t;
     variable bus_rd_ref2 : bus_reference_t;
     type bus_reference_arr_t is array (0 to tb_cfg.num_cycles-1) of bus_reference_t;
     variable rd_ref : bus_reference_arr_t;
   begin
     test_runner_setup(runner, runner_cfg);
     set_format(display_handler, verbose, true);
-    show(tb_logger, display_handler, verbose);
-    show(default_logger, display_handler, verbose);
-    show(master_logger, display_handler, verbose);
-    show(com_logger, display_handler, verbose);
+    show(tb_logger, display_handler, trace);
+    show(default_logger, display_handler, trace);
+    show(master_logger, display_handler, trace);
+    show(com_logger, display_handler, trace);
 
     wait until rising_edge(clk);
 
     if run("wr single rd single") then
       info(tb_logger, "Writing...");
       write_bus(net, bus_handle, 0, value);
       wait until ack = '1' and rising_edge(clk);
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_wishbone_slave.gtkw` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_wishbone_slave.gtkw`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/verification_components/test/tb_wishbone_slave.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/verification_components/test/tb_wishbone_slave.vhd`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,17 @@
 
   main_stim : process
     variable tmp : std_logic_vector(dat_i'range);
     variable value : std_logic_vector(dat_i'range) := (others => '1');
   begin
     test_runner_setup(runner, runner_cfg);
     set_format(display_handler, verbose, true);
-    show(tb_logger, display_handler, verbose);
-    show(default_logger, display_handler, verbose);
-    show(com_logger, display_handler, verbose);
+    show(tb_logger, display_handler, trace);
+    show(default_logger, display_handler, trace);
+    show(com_logger, display_handler, trace);
     wait until rising_edge(clk);
 
 
     if run("wr block rd block") then
       info(tb_logger, "Writing...");
       for i in 0 to tb_cfg.num_cycles-1 loop
         cyc <= '1';
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/vunit_context.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/vunit_context.vhd`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,19 @@
   use vunit_lib.dictionary.all;
   use vunit_lib.path.all;
   use vunit_lib.print_pkg.all;
   use vunit_lib.log_levels_pkg.all;
   use vunit_lib.logger_pkg.all;
   use vunit_lib.log_handler_pkg.all;
   use vunit_lib.log_deprecated_pkg.all;
+  use vunit_lib.id_pkg.all;
   use vunit_lib.ansi_pkg.all;
   use vunit_lib.checker_pkg.all;
   use vunit_lib.check_pkg.all;
   use vunit_lib.check_deprecated_pkg.all;
   use vunit_lib.run_types_pkg.all;
   use vunit_lib.run_pkg.all;
   use vunit_lib.run_deprecated_pkg.all;
+  use vunit_lib.runner_pkg.key_t;
+  use vunit_lib.event_common_pkg.all;
+  use vunit_lib.event_pkg.all;
 end context;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl/vunit_run_context.vhd` & `vunit_hdl-4.7.0/vunit/vhdl/vunit_run_context.vhd`

 * *Files 14% similar despite different names*

```diff
@@ -8,8 +8,9 @@
   library vunit_lib;
   use vunit_lib.dictionary.all;
   use vunit_lib.path.all;
   use vunit_lib.checker_pkg.checker_stat_t;
   use vunit_lib.run_types_pkg.all;
   use vunit_lib.run_pkg.all;
   use vunit_lib.run_deprecated_pkg.all;
+  use vunit_lib.runner_pkg.key_t;
 end context;
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl_parser.py` & `vunit_hdl-4.7.0/vunit/vhdl_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,28 +504,31 @@
 
         # Split the interface elements
         interface_elements = cls._split_not_in_par(generic_list_string, ";")
 
         generic_list = []
         # Add interface elements to the generic list
         for interface_element in interface_elements:
+            if len(interface_element.strip()) == 0:
+                # Ignore space after a trailing comma
+                continue
 
             if cls._package_generic_re.match(interface_element) is not None:
                 # Ignore package generics
                 continue
 
             if cls._type_generic_re.match(interface_element) is not None:
                 # Ignore type generics
                 continue
 
             if cls._function_generic_re.match(interface_element) is not None:
                 # Ignore function generics
                 continue
 
-            generic_list.append(VHDLInterfaceElement.parse(interface_element))
+            generic_list.append(VHDLInterfaceElement.parse(interface_element, is_constant=True))
 
         return generic_list
 
     @classmethod
     def _parse_port_clause(cls, code):
         """
         Parse the port clause and return a list of interface elements
@@ -535,14 +538,17 @@
 
         # Split the interface elements
         interface_elements = port_list_string.split(";")
 
         port_list = []
         # Add interface elements to the port list
         for interface_element in interface_elements:
+            if len(interface_element.strip()) == 0:
+                # Ignore space after a trailing comma
+                continue
             port_list.append(VHDLInterfaceElement.parse(interface_element, is_signal=True))
 
         return port_list
 
 
 class VHDLContext(object):
     """
@@ -627,21 +633,27 @@
     def without_mode(self):
         """
         @returns A copy of this interface element without a mode
         """
         return VHDLInterfaceElement(self.identifier, self.subtype_indication, init_value=self.init_value)
 
     @classmethod
-    def parse(cls, code, is_signal=False):
+    def parse(cls, code, is_signal=False, is_constant=False):
         """
         Returns a new instance by parsing the code
         """
         if is_signal:
-            # Remove 'signal' string if a signal is beeing parsed
-            code = code.replace("signal", "")
+            # Remove 'signal' string if a signal is being parsed
+            # Note, the string must be a raw string for the word boundary '\b' to work properly
+            # see documentation https://docs.python.org/3/howto/regex.html#more-metacharacters
+            code = re.sub(r"\bsignal\b", "", code)
+
+        if is_constant:
+            # Remove 'constant' string if a constant is being parsed
+            code = re.sub(r"\bconstant\b", "", code)
 
         interface_element_string = code
 
         # Extract the identifier
         identifier = interface_element_string.split(":")[0].strip()
 
         # Extract subtype indication and mode (if any)
```

### Comparing `vunit_hdl-4.6.2/vunit/vhdl_standard.py` & `vunit_hdl-4.7.0/vunit/vhdl_standard.py`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vivado/tcl/extract_compile_order.tcl` & `vunit_hdl-4.7.0/vunit/vivado/tcl/extract_compile_order.tcl`

 * *Files identical despite different names*

### Comparing `vunit_hdl-4.6.2/vunit/vivado/vivado.py` & `vunit_hdl-4.7.0/vunit/vivado/vivado.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 """
 
 from subprocess import check_call
 from os import makedirs
 from pathlib import Path
 
 
-def add_from_compile_order_file(vunit_obj, compile_order_file, dependency_scan_defaultlib=True):
+def add_from_compile_order_file(
+    vunit_obj, compile_order_file, dependency_scan_defaultlib=True, fail_on_non_hdl_files=True
+):  # pylint: disable=too-many-locals
     """
     Add Vivado IP:s from a compile order file
     """
-    compile_order, libraries, include_dirs = _read_compile_order(compile_order_file)
+    compile_order, libraries, include_dirs = _read_compile_order(compile_order_file, fail_on_non_hdl_files)
 
     # Create libraries
     for library_name in libraries:
         vunit_obj.add_library(library_name, vhdl_standard="93")
 
     # Add all source files to VUnit
     source_files = []
@@ -73,28 +75,33 @@
     run_vivado(
         str(Path(__file__).parent / "tcl" / "extract_compile_order.tcl"),
         tcl_args=[project_file, compile_order_file],
         vivado_path=vivado_path,
     )
 
 
-def _read_compile_order(file_name):
+def _read_compile_order(file_name, fail_on_non_hdl_files):
     """
     Read the compile order file and filter out duplicate files
     """
     compile_order = []
     unique = set()
     include_dirs = set()
     libraries = set()
 
     with Path(file_name).open("r", encoding="utf-8") as ifile:
-
         for line in ifile.readlines():
             library_name, file_type, file_name = line.strip().split(",", 2)
-            assert file_type in ("Verilog", "VHDL", "Verilog Header")
+
+            if file_type not in ("Verilog", "VHDL", "Verilog Header"):
+                if fail_on_non_hdl_files:
+                    raise RuntimeError(f"Unsupported compile order file: {file_name}")
+                print(f"Compile order file ignored: {file_name}")
+                continue
+
             libraries.add(library_name)
 
             # Vivado generates duplicate files for different IP:s
             # using the same underlying libraries. We remove duplicates here
             key = (library_name, Path(file_name).name)
             if key in unique:
                 continue
```

### Comparing `vunit_hdl-4.6.2/vunit/vunit_cli.py` & `vunit_hdl-4.7.0/vunit/vunit_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,15 +145,23 @@
     parser.add_argument(
         "--elaborate",
         action="store_true",
         default=False,
         help="Only elaborate test benches without running",
     )
 
-    parser.add_argument("--clean", action="store_true", default=False, help="Remove output path first")
+    parser.add_argument(
+        "--clean",
+        action="store_true",
+        default=False,
+        help="Remove output path first. "
+        "This is useful, for example, to force a complete "
+        "recompile when compilation artifacts are obsolete "
+        "due to a simulator version update.",
+    )
 
     parser.add_argument(
         "-o",
         "--output-path",
         default=default_output_path,
         help="Output path for compilation and simulation artifacts",
     )
```

### Comparing `vunit_hdl-4.6.2/vunit_hdl.egg-info/PKG-INFO` & `vunit_hdl-4.7.0/vunit_hdl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: vunit-hdl
-Version: 4.6.2
+Version: 4.7.0
 Summary: VUnit is an open source unit testing framework for VHDL/SystemVerilog.
 Home-page: https://github.com/VUnit/vunit
 Author: Lars Asplund
 Author-email: lars.anders.asplund@gmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
@@ -32,23 +33,23 @@
 `Website <https://vunit.github.io>`__
 
 Contributing in the form of code, feedback, ideas or bug reports are
 welcome. Read our `contribution guide
 <https://vunit.github.io/contributing.html>`__ to get started.
 
 **VUnit**, except for the projects below, is released under the terms of `Mozilla Public License, v. 2.0`_.
-|copy| 2014-2021 Lars Asplund, lars.anders.asplund@gmail.com.
+|copy| 2014-2023 Lars Asplund, lars.anders.asplund@gmail.com.
 
 The following libraries are `redistributed`_ with VUnit for convenience:
 
 * **OSVVM** (``vunit/vhdl/osvvm``): these files are licensed under the terms of `Apache License, v 2.0`_,
-  |copy| 2010 - 2021 by `SynthWorks Design Inc`_. All rights reserved.
+  |copy| 2010 - 2023 by `SynthWorks Design Inc`_. All rights reserved.
 
 * **JSON-for-VHDL** (``vunit/vhdl/JSON-for-VHDL``): these files are licensed under the terms of `Apache License,
-  v 2.0`_, |copy| 2015 - 2021 Patrick Lehmann.
+  v 2.0`_, |copy| 2015 - 2023 Patrick Lehmann.
 
 The font used in VUnit's logo and illustrations is 'Tratex', the traffic sign typeface used on swedish road signs:
 
 - `transportstyrelsen.se: Teckensnitt <https://transportstyrelsen.se/sv/vagtrafik/Trafikregler/Om-vagmarken/Teckensnitt/>`__
 - `Wikipedia: Tratex <https://en.wikipedia.org/wiki/Tratex>`__
```

### Comparing `vunit_hdl-4.6.2/vunit_hdl.egg-info/SOURCES.txt` & `vunit_hdl-4.7.0/vunit_hdl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -87,28 +87,30 @@
 vunit/sim_if/activehdl.py
 vunit/sim_if/cds_file.py
 vunit/sim_if/common.py
 vunit/sim_if/factory.py
 vunit/sim_if/ghdl.py
 vunit/sim_if/incisive.py
 vunit/sim_if/modelsim.py
+vunit/sim_if/nvc.py
 vunit/sim_if/rivierapro.py
 vunit/sim_if/tcl_read_eval_loop.tcl
 vunit/sim_if/vsim_simulator_mixin.py
 vunit/test/__init__.py
 vunit/test/bench.py
 vunit/test/bench_list.py
 vunit/test/list.py
 vunit/test/report.py
 vunit/test/runner.py
 vunit/test/suites.py
 vunit/ui/__init__.py
 vunit/ui/common.py
 vunit/ui/library.py
 vunit/ui/packagefacade.py
+vunit/ui/preprocessor.py
 vunit/ui/results.py
 vunit/ui/source.py
 vunit/ui/test.py
 vunit/ui/testbench.py
 vunit/verilog/vunit_pkg.sv
 vunit/verilog/check/test/check_tb.sv
 vunit/verilog/include/vunit_defines.svh
@@ -540,15 +542,22 @@
 vunit/vhdl/data_types/run.py
 vunit/vhdl/data_types/src/byte_vector_ptr_pkg.vhd
 vunit/vhdl/data_types/src/codec-2008p.vhd
 vunit/vhdl/data_types/src/codec.vhd
 vunit/vhdl/data_types/src/codec_builder-2008p.vhd
 vunit/vhdl/data_types/src/codec_builder.vhd
 vunit/vhdl/data_types/src/data_types_context.vhd
+vunit/vhdl/data_types/src/data_types_private_pkg.vhd
+vunit/vhdl/data_types/src/dict_pkg-2008p.vhd
+vunit/vhdl/data_types/src/dict_pkg-body.vhd
 vunit/vhdl/data_types/src/dict_pkg.vhd
+vunit/vhdl/data_types/src/event_common_pkg.vhd
+vunit/vhdl/data_types/src/event_pkg.vhd
+vunit/vhdl/data_types/src/event_private_pkg.vhd
+vunit/vhdl/data_types/src/id_pkg.vhd
 vunit/vhdl/data_types/src/integer_array_pkg-body.vhd
 vunit/vhdl/data_types/src/integer_array_pkg.vhd
 vunit/vhdl/data_types/src/integer_vector_ptr_pkg-body-2002p.vhd
 vunit/vhdl/data_types/src/integer_vector_ptr_pkg-body-93.vhd
 vunit/vhdl/data_types/src/integer_vector_ptr_pkg.vhd
 vunit/vhdl/data_types/src/integer_vector_ptr_pool_pkg.vhd
 vunit/vhdl/data_types/src/queue_pkg-2008p.vhd
@@ -561,23 +570,28 @@
 vunit/vhdl/data_types/src/string_ptr_pool_pkg.vhd
 vunit/vhdl/data_types/src/types.vhd
 vunit/vhdl/data_types/src/api/external_integer_vector_pkg.vhd
 vunit/vhdl/data_types/src/api/external_string_pkg.vhd
 vunit/vhdl/data_types/test/tb_byte_vector_ptr.vhd
 vunit/vhdl/data_types/test/tb_codec-2008p.vhd
 vunit/vhdl/data_types/test/tb_codec.vhd
+vunit/vhdl/data_types/test/tb_dict-2008p.vhd
 vunit/vhdl/data_types/test/tb_dict.vhd
+vunit/vhdl/data_types/test/tb_event_pkg.vhd
+vunit/vhdl/data_types/test/tb_event_private_pkg.vhd
+vunit/vhdl/data_types/test/tb_id.vhd
 vunit/vhdl/data_types/test/tb_integer_array.vhd
 vunit/vhdl/data_types/test/tb_integer_vector_ptr.vhd
 vunit/vhdl/data_types/test/tb_integer_vector_ptr_pool.vhd
 vunit/vhdl/data_types/test/tb_queue-2008p.vhd
 vunit/vhdl/data_types/test/tb_queue.vhd
 vunit/vhdl/data_types/test/tb_queue_pool.vhd
 vunit/vhdl/data_types/test/tb_string_ptr.vhd
 vunit/vhdl/data_types/test/tb_string_ptr_pool.vhd
+vunit/vhdl/data_types/tools/generate_dict.py
 vunit/vhdl/dictionary/run.py
 vunit/vhdl/dictionary/src/dictionary.vhd
 vunit/vhdl/dictionary/test/tb_dictionary.vhd
 vunit/vhdl/logging/run.py
 vunit/vhdl/logging/src/ansi_pkg.vhd
 vunit/vhdl/logging/src/file_pkg.vhd
 vunit/vhdl/logging/src/location_pkg-body-2008m.vhd
@@ -612,14 +626,15 @@
 vunit/vhdl/osvvm/NameStorePkg.vhd
 vunit/vhdl/osvvm/OsvvmContext.vhd
 vunit/vhdl/osvvm/OsvvmGlobalPkg.vhd
 vunit/vhdl/osvvm/README.md
 vunit/vhdl/osvvm/RandomBasePkg.vhd
 vunit/vhdl/osvvm/RandomPkg.vhd
 vunit/vhdl/osvvm/RandomProcedurePkg.vhd
+vunit/vhdl/osvvm/ReportPkg.vhd
 vunit/vhdl/osvvm/ResizePkg.vhd
 vunit/vhdl/osvvm/ResolutionPkg.vhd
 vunit/vhdl/osvvm/ScoreboardGenericPkg.vhd
 vunit/vhdl/osvvm/ScoreboardPkg_int.vhd
 vunit/vhdl/osvvm/ScoreboardPkg_int_c.vhd
 vunit/vhdl/osvvm/ScoreboardPkg_slv.vhd
 vunit/vhdl/osvvm/ScoreboardPkg_slv_c.vhd
```

