# Comparing `tmp/ksfctl-0.2.1.tar.gz` & `tmp/ksfctl-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksfctl-0.2.1.tar", last modified: Mon Apr 17 17:58:02 2023, max compression
+gzip compressed data, was "ksfctl-0.2.3.tar", last modified: Sun Apr 23 15:55:57 2023, max compression
```

## Comparing `ksfctl-0.2.1.tar` & `ksfctl-0.2.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 17:58:02.471414 ksfctl-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-17 17:57:51.000000 ksfctl-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/cmd/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/generate/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/generate/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87289 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/generate/cpp/orm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/orm/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/generate/cpp/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/parser/ksf_lex.py
--rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/parser/ksf_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    34226 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/parser/ksf_yacc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-17 17:57:51.000000 ksfctl-0.2.1/ksfctl/parser/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:58:02.471414 ksfctl-0.2.1/ksfctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 17:58:02.000000 ksfctl-0.2.1/ksfctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:58:02.471414 ksfctl-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-17 17:57:51.000000 ksfctl-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-23 15:55:47.000000 ksfctl-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-23 15:55:57.789500 ksfctl-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-23 15:55:47.000000 ksfctl-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/cmd/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/cmd/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/generate/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81038 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/cpp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/cpp/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27554 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/cpp/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/generate/ksf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/ksf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/ksf/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/ksf/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22610 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/parser/ksf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34410 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/parser/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/parser/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 15:55:57.789500 ksfctl-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-23 15:55:47.000000 ksfctl-0.2.3/setup.py
```

### Comparing `ksfctl-0.2.1/README.md` & `ksfctl-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ksfctl-0.2.1/ksfctl/cmd/cmd.py` & `ksfctl-0.2.3/ksfctl/cmd/cmd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,222 +1,304 @@
-import os
+import enum
 
-import click
-import yaml
-
-from ksfctl.generate.cpp.generator import cpp_gen, cpp_sdk_gen
+from ksfctl.cmd.options import *
+from ksfctl.generate.cpp.generator import cpp_gen
 
 
 @click.group(context_settings={'help_option_names': ['-h', '--help']})
 @click.pass_context
 def cli(ctx):
     pass
 
 
 help_str = f'''\
 ksf文件解析器\n
-解析ksf文件到其他语言，目前支持[c++(cpp), python(py), java, node.js(node), go]\n
+解析ksf文件到其他语言，目前支持[ksf(自转译), c++(cpp), python(py), java, node.js(node), go]\n
 关键字: \n
 module, struct, enum, interface, const, bool, int, long, short, byte, double, float, string, map, vector, using, import, export, require, optional, key, out, false, true\n
 基础元素: 以模块(module)为核心，文件包含关系为树状结构，模块包含接口interface，结构struct，枚举enum，常量const等元素\n
 适合场景: 用于定义协议，生成对应的代码，用于服务端和客户端的通信\n
 '''
 
 
-@cli.group(name='parse', help=help_str,
-           context_settings={'help_option_names': ['-h', '--help']})
+@cli.group(name='trans', help=help_str,
+           context_settings={'help_option_names': ['-h', '--help']}
+           )
 @click.pass_context
-def parse(ctx):
+def ksf_trans(ctx):
     pass
 
 
-@parse.command(name='cpp', context_settings={'help_option_names': ['-h', '--help']})
+class ModeType(enum.Enum):
+    FILE = 'file'
+    ALL_IN_ONE = 'all_in_one'
+    EXPORT_IMPORT = 'export_import'
+
+
+class VisibilityType(enum.Enum):
+    PUBLIC = 'public'
+    PRIVATE = 'private'
+
+
+@ksf_trans.command(name='cxx', context_settings={'help_option_names': ['-h', '--help']})
 @click.pass_context
-@click.argument('ksf_files', nargs=-1, required=True, type=str)
-@click.option('-i', '--include', '--include-path', multiple=True, help='ksf协议文件搜索路径')
-@click.option('-d', '--dir', '--dest', 'destination_dir', multiple=False, help='生成的头文件存放的路径')
-@click.option('--sdk-export', 'sdk_export', multiple=False, default="ksf_export.h",
-              help='[sdk模式生效]生成的sdk导出符号头文件名(默认为ksf_export.h)')
-@click.option('--sdk-invoke', 'sdk_invoke', multiple=False, default="ksf_invoke.h",
-              help='[sdk模式生效]生成的sdk调用头文件名(默认为ksf_invoke.h)')
-@click.option('-f', '--config-file', 'config_file', multiple=False, help='注入的脚本文件yaml')
-@click.option('-c', '--config', 'config', multiple=False, help='注入的脚本yaml')
+@click.argument('files', nargs=-1, required=True, type=str, metavar='...<file>')
+@click.option('--mode', 'mode', default=ModeType.FILE.value, type=click.Choice([mode.value for mode in ModeType]),
+              help=f'''\
+生成器模式选择.
+
+file=单文件(每一个.ksf对应生成一个文件)
+all_in_one=合并文件(只生成一个聚合文件)
+export_import=导出导入模式(sdk模式), 默认为file)
+'''
+              )
+@click.option('--dispatch-mode', 'dispatch_mode', default='array', type=click.Choice(('array', 'set', 'hash')),
+              metavar='<dispatch-mode>', help='分发模式, 支持(array, set, hash)'
+              )
+@click.option('--visibility', 'visibility', default=VisibilityType.PUBLIC.value,
+              type=click.Choice([visibility.value for visibility in VisibilityType]), help='生成的符号的可见性'
+              )
+@click.option('-f', '--config-file', 'config_file', multiple=False, type=str, metavar='<config-file>',
+              help='注入的脚本文件yaml(优先级低于其他选项，即其他命令行参数可以覆盖文件定义的内容)'
+              )
+@click.option('-i', '--include', '--include-path', 'include_path', multiple=True, type=str, help='ksf协议文件搜索路径',
+              metavar='[<include-path> or @pwd]'
+              )
+@click.option('-d', '--dir', '--dest', 'destination_path', multiple=False, help='生成的头文件存放的路径',
+              metavar='<destination-path>'
+              )
+@click.option('-o', '--output-file', 'output_file', multiple=False, default="ksf_out.h",
+              help='[聚合模式]生成的聚合头文件名', metavar='<output-file>'
+              )
+@click.option('--export-file', 'export_file', multiple=False, default="ksf_export.h",
+              help='[导入导出模式生效]生成的导出符号头文件名(默认为ksf_export.h)', metavar='<export-file>'
+              )
+@click.option('--invoke-file', 'invoke_file', multiple=False, default="ksf_invoke.h",
+              help='[导入导出模式生效]生成的调用头文件名(默认为ksf_invoke.h)', metavar='<invoke-file>'
+              )
 @click.option('--export', 'export_symbols', multiple=True, help='需要导出的结构体或者函数体')
+@click.option('--hidden', 'hidden_symbols', multiple=True, help='需要隐藏的结构体或者函数体(TODO)')
 @click.option('--replace_ns', '--replace-ns', multiple=False, help='(将被废弃)替换namespace')
 @click.option('--replace-namespace', nargs=2, multiple=True, type=str, help='(推荐)将指定命名空间替换为另一个命名空间')
 @click.option('--replace-include-path', nargs=2, multiple=True, type=str, help='(推荐)替换头文件路径')
 @click.option('--push-function', multiple=True,
-              help='携带push模式的函数名, 用于生成push函数，参数形式为module.interface.operator')
+              help='携带push模式的函数名, 用于生成push函数，参数形式为module.interface.operator'
+              )
 @click.option('--ignore-relative-path', 'ignore_relative_path', is_flag=True, flag_value=True, default=False,
-              help='忽略依赖目录')
-@click.option('--check-default/--no-check-default', default=True, help='是否打包默认值')
-@click.option('--ksf/--no-ksf', 'ksf', is_flag=True, default=False, help='是否ksf内部模块')
-@click.option('--json/--no-json', 'json', is_flag=True, default=True, help='是否生成Json格式')
-@click.option('--sql/--no-sql', 'sql', is_flag=True, default=False, help='是否生成Sql接口')
-@click.option('--rpc/--no-rpc', 'rpc', is_flag=True, default=True, help='是否生成RPC接口')
-@click.option('--current-priority/--no-current-priority', 'current_priority', is_flag=True, default=True,
-              help='是否优先使用当前目录')
-@click.option('--trace/--no-trace', 'trace', is_flag=True, default=False, help='是否需要调用链追踪逻辑')
-@click.option('--push/--no-push', 'push', is_flag=True, default=True, help='是否需要推送接口')
-@click.option('--param-rvalue-ref/--no-param-rvalue-ref', 'param_rvalue_ref', is_flag=True, default=False,
-              help='是否参数使用右值引用')
-@click.option('--sdk-mode', 'sdk_mode', is_flag=True, default=False,
-              help='启动sdk模式，会生成一个纯结构体的头文件和一个纯rpc的头文件')
+              help='忽略依赖目录'
+              )
 @click.option('--verbose', 'verbose', is_flag=True, flag_value=True, default=False, help='是否打印详细信息')
-@click.option('--with-ksf', 'ksf', is_flag=True, flag_value=True, default=False, help='ksf内部模块')
-@click.option('--unjson', 'json', is_flag=True, flag_value=False, default=True, help='不生成Json格式')
-@click.option('--os', 'rpc', is_flag=True, default=True, flag_value=False, help='不生成RPC接口')
-@click.option('--currentPriority', 'current_priority', is_flag=True, flag_value=True, default=True,
-              help='优先使用当前目录')
-@click.option('--without-trace', 'trace', is_flag=True, flag_value=False, default=False, help='不需要调用链追踪')
-@click.option('--with-push', 'push', is_flag=True, flag_value=True, default=True, help='需要推送接口')
-@click.option('--with-param-rvalue-ref', 'param_rvalue_ref', is_flag=True, flag_value=True, default=False,
-              help='参数使用右值引用')
-def parse_cpp(ctx, ksf_files, include, destination_dir, replace_ns, replace_namespace, replace_include_path,
-              push_function, sdk_mode, verbose, sdk_export, sdk_invoke, export_symbols, config_file,
-              config, **kwargs):
+# 可选优化选项
+@click.option('--enable-check-default/--disable-check-default',
+              'check_default',
+              default=True,
+              help='是否打包默认值'
+              )
+@click.option('--enable-json/--disable-json', 'json', is_flag=True, default=True, help='是否生成Json格式')
+@click.option('--enable-rpc/--disable-rpc', 'rpc', is_flag=True, default=True, help='是否生成RPC接口')
+@click.option('--enable-current-priority/--disable-current-priority',
+              'current_priority',
+              is_flag=True,
+              default=True,
+              help='是否优先使用当前目录'
+              )
+@click.option('--enable-trace/--disable-trace',
+              'trace',
+              is_flag=True,
+              default=False,
+              help='是否需要调用链追踪逻辑'
+              )
+@click.option('--enable-push/--disable-push', 'push', is_flag=True, default=True, help='是否需要推送接口')
+@click.option('--enable-invoke-client/--disable-invoke-client',
+              'invoke_client',
+              is_flag=True,
+              default=True,
+              help='是否有客户端调用实现'
+              )
+@click.option('--enable-promise/--disable-promise',
+              'promise',
+              is_flag=True,
+              default=True,
+              help='是否使用客户端Promise调用实现'
+              )
+@click.option('--enable-coroutine/--disable-coroutine',
+              'coroutine',
+              is_flag=True,
+              default=True,
+              help='是否使用客户端Coroutine调用实现'
+              )
+@click.option('--enable-invoke-server/--disable-invoke-server',
+              'invoke_server',
+              is_flag=True,
+              default=True,
+              help='是否有客户端调用实现'
+              )
+@click.option('--enable-rvalue-ref/--disable-rvalue-ref', 'rvalue_ref', is_flag=True, default=False,
+              help='是否参数使用右值引用'
+              )
+@click.option('--enable-cxx17/--disable-cxx17',
+              'cxx17',
+              is_flag=True,
+              flag_value=True,
+              default=False,
+              help='使用C++17'
+              )
+def cxx(ctx, files, mode, **kwargs):
+    """c++(cpp)语言解析器"""
     ctx.help_option_names += ['-h']
-    repl_ns_dict = {}
 
-    def print_verbose(msg):
-        if verbose:
-            click.echo(msg)
+    parsed_kwargs = {}
+
+    print_verbose = flag_verbose(kwargs)
+
+    """解析配置文件"""
+    if "config_file" in kwargs:
+        """解析配置文件"""
+        parse_config_file_to_parsed_args(kwargs, parsed_kwargs)
 
     """命令的描述"""
-    print_verbose(f'文件列表: {ksf_files}')
+    if len(files) == 0:
+        raise click.BadParameter('未指定任何文件。')
+    print_verbose(f'文件列表: {files}')
+
+    """模式"""
+    print_verbose(f"""模式: {mode}""")
 
     """将指定命名空间替换为另一个命名空间"""
-    if replace_namespace:
-        for origin, actual in replace_namespace:
-            repl_ns_dict[origin] = actual
-            print_verbose(f'将命名空间 {origin} 替换为 {actual}。')
-    elif replace_ns:
-        for replace_namespace_str in replace_ns.split(";"):
-            origin, actual = replace_namespace_str.split("/")
-            repl_ns_dict[origin] = actual
-            print_verbose(f'将命名空间 {origin} 替换为 {actual}。')
-    else:
-        print_verbose('未指定任何命名空间的置换。')
+    print_verbose(list_replace_namespace(kwargs, parsed_kwargs))
 
     """替换头文件路径"""
-    repl_inc_dict = {}
-    if replace_include_path:
-        for origin, actual in replace_include_path:
-            repl_inc_dict[origin] = actual
-            print_verbose(f'将头文件路径 {origin} 替换为 {actual}。')
-    else:
-        print_verbose('未指定任何头文件路径的置换。')
+    print_verbose(list_replace_include_path(kwargs, parsed_kwargs))
 
     """生成文件位置"""
-    if destination_dir:
-        print_verbose(f'生成文件位置: {destination_dir}')
-    else:
-        destination_dir = os.getcwd()
-        print_verbose(f'生成文件位置: {destination_dir}')
+    print_verbose(var_destination_path(kwargs, parsed_kwargs))
 
     """头文件包含路径"""
-    if include:
-        print_verbose(f'包含路径: {include}')
-    else:
-        print_verbose(f'未指定包含路径，将只在当前路径搜索')
+    print_verbose(list_include_path(kwargs, parsed_kwargs))
+
+    """忽略依赖目录"""
+    print_verbose(f"忽略依赖目录：{kwargs['ignore_relative_path']}")
+
+    """是否优先搜索当前目录"""
+    print_verbose(f"是否优先搜索当前目录：{kwargs['current_priority']}")
 
     """携带push模式的函数名, 用于生成push函数，参数形式为module.interface.operator"""
-    if push_function:
-        print_verbose(f'推送模式的函数名: {push_function}')
-    else:
-        print_verbose(f'无指定推送模式的函数')
+    print_verbose(list_push_function(kwargs, parsed_kwargs))
 
-    """解析配置文件"""
-    if config_file:
-        with open(config_file, 'r') as f:
-            export_symbols = set()
-            configs = yaml.safe_load(f.read())
-            # print(configs)
-            for config in configs:
-                module = config['module']
-                if 'namespace' in config:
-                    repl_ns_dict[module] = config['namespace']
-
-                for element_type, elements in config['export'].items():
-                    if element_type == 'interface':
-                        for element in elements:
-                            if isinstance(element, dict):
-                                for interface, functions in element.items():
-                                    if functions is None or len(functions) == 0:
-                                        export_symbols.add(f'{module}.{interface}')
-                                    else:
-                                        for function in functions:
-                                            export_symbols.add(f'{module}.{interface}.{function}')
-                            else:
-                                export_symbols.add(f'{module}.{element}')
-                    else:
-                        for element in elements:
-                            export_symbols.add(f'{module}.{element}')
+    """是否只导出部分符号"""
+    print_verbose(list_export_symbol(kwargs, parsed_kwargs))
+
+    """分发模式"""
+    print_verbose(var_dispatch_mode(kwargs, parsed_kwargs))
+
+    """是否启动c++17风格"""
+    print_verbose(f"是否启动c++17风格：{kwargs['cxx17']}")
 
     """是否检测默认值"""
     print_verbose(f"是否检测默认值：{kwargs['check_default']}")
 
-    """是否ksf内部模块"""
-    print_verbose(f"是否ksf内部模块：{kwargs['ksf']}")
-
     """是否生成Json序列化接口"""
     print_verbose(f"是否生成Json序列化接口：{kwargs['json']}")
 
-    """是否生成Sql接口"""
-    print_verbose(f"是否生成Sql接口：{kwargs['sql']}")
-
     """是否生成RPC接口"""
     print_verbose(f"是否生成RPC接口：{kwargs['rpc']}")
 
-    """是否优先使用当前目录"""
-    print_verbose(f"是否优先使用当前目录：{kwargs['current_priority']}")
-
     """是否需要调用链追踪逻辑"""
     print_verbose(f"是否需要调用链追踪逻辑：{kwargs['trace']}")
 
     """是否参数使用右值引用"""
-    print_verbose(f"是否参数使用右值引用：{kwargs['param_rvalue_ref']}")
-
-    """忽略依赖目录"""
-    print_verbose(f"忽略依赖目录：{kwargs['ignore_relative_path']}")
+    print_verbose(f"是否参数使用右值引用：{kwargs['rvalue_ref']}")
 
     """解析所有的flags，携带with_头"""
-    kwargs_with_prefix = {}
+    parsed_kwargs['flags'] = {}
     for k, v in kwargs.items():
-        kwargs_with_prefix.update({f'with_{k}': v})
+        if isinstance(v, bool):
+            parsed_kwargs['flags'].update({f'with_{k}': v})
 
-    if sdk_mode:
-        """启动sdk模式，会生成一个纯结构体的头文件和一个纯rpc的头文件"""
-        if sdk_export:
-            print_verbose(f"生成纯结构体头文件：{sdk_export}")
-
-        if sdk_invoke:
-            print_verbose(f"生成纯rpc头文件：{sdk_invoke}")
-
-        if export_symbols:
-            print_verbose(f"导出头文件：{export_symbols}")
-
-        cpp_sdk_gen(files=ksf_files,
-                    repl_ns_dict=repl_ns_dict,
-                    repl_inc_dir=repl_inc_dict,
-                    include_dirs=include,
-                    destination_dir=destination_dir,
-                    push_functions=push_function,
-                    export_symbols=export_symbols,
-                    sdk_invoke=sdk_invoke,
-                    sdk_export=sdk_export,
-                    flags=kwargs_with_prefix)
+    if mode == ModeType.EXPORT_IMPORT.value:
+        """启动sdk模式，会生成一个export的头文件和一个内部invoke的头文件"""
+        print_verbose(var_invoke_file(kwargs, parsed_kwargs))
+        print_verbose(var_export_file(kwargs, parsed_kwargs))
+    elif mode == ModeType.FILE.value:
+        pass
     else:
-        cpp_gen(files=ksf_files,
-                repl_ns_dict=repl_ns_dict,
-                repl_inc_dir=repl_inc_dict,
-                include_dirs=include,
-                destination_dir=destination_dir,
-                push_functions=push_function,
-                flags=kwargs_with_prefix)
+        """启动all_one模式，会生成一个聚合的头文件"""
+        print_verbose(var_output_file(kwargs, parsed_kwargs))
+    cpp_gen(mode, files=files, **parsed_kwargs)
+
+
+# @ksf_trans.command(name='ksf', help="抽取元素并合并成新的ksf文件",
+#                    context_settings={'help_option_names': ['-h', '--help']}
+#                    )
+# @click.pass_context
+# @click.argument('ksf_files', nargs=-1, required=True, type=str)
+# @click.option('-d', '--destination', type=str, help='输出文件夹')
+# @click.option('-o', '--output', type=str, help='输出文件名')
+# @click.option('-i', '--include', type=str, multiple=True, help='头文件包含路径')
+# @click.option('--export', 'export_symbols', type=str, multiple=True, help='导出的接口')
+# @click.option('--verbose', 'verbose', is_flag=True, flag_value=True, default=False, help='是否打印详细信息')
+# @click.option('--special-container', 'special_container', is_flag=True, flag_value=True, default=False,
+#               help='是否启用特殊容器(默认不启用)，特殊容器为(vector[set], vector[hashset], map[hashmap])，不启用时退化为vector和map'
+#               )
+# def merge_ksf(ctx, **kwargs):
+#     verbose = False
+#
+#     def print_verbose(msg):
+#         if verbose:
+#             click.echo(msg)
+#
+#     if 'verbose' in kwargs:
+#         verbose = kwargs['verbose']
+#         del kwargs['verbose']
+#
+#     if 'ksf_files' in kwargs:
+#         ksf_files = kwargs['ksf_files']
+#         del kwargs['ksf_files']
+#     else:
+#         print_verbose('未指定ksf文件')
+#         exit(1)
+#
+#     if 'destination' in kwargs:
+#         destination_dir = kwargs['destination']
+#         del kwargs['destination']
+#     else:
+#         destination_dir = '.'
+#
+#     if 'output' in kwargs:
+#         output = kwargs['output']
+#         del kwargs['output']
+#     else:
+#         print_verbose('未指定输出文件名')
+#         exit(1)
+#
+#     if 'include' in kwargs:
+#         include = kwargs['include']
+#         del kwargs['include']
+#     else:
+#         include = []
+#
+#     if 'export_symbols' in kwargs:
+#         export_symbols = kwargs['export_symbols']
+#         del kwargs['export_symbols']
+#     else:
+#         print_verbose('未指定导出的接口')
+#         exit(1)
+#
+#     """解析所有的flags，携带with_头"""
+#     kwargs_with_prefix = {}
+#     for k, v in kwargs.items():
+#         kwargs_with_prefix.update({f'with_{k}': v})
+
+    # case_gen(files=ksf_files,
+    #          include_dirs=include,
+    #          destination_dir=destination_dir,
+    #          out_file=output,
+    #          export_symbols=export_symbols,
+    #          **kwargs_with_prefix
+    #          )
 
 
 if __name__ == '__main__':
     cli()
     exit(0)
 
     runner = CliRunner()
```

### Comparing `ksfctl-0.2.1/ksfctl/generate/cpp/generator.py` & `ksfctl-0.2.3/ksfctl/generate/cpp/generator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1554 +1,1138 @@
 from datetime import datetime
 from hashlib import md5
 
 from ksfctl.generate.cpp.parser import CppParser
-from ksfctl.parser.ksf_parser import *
-from ksfctl.parser.ksf_yacc import generate
+from ksfctl.generate.cpp.template import *
+from ksfctl.parser.ksf import *
+from ksfctl.parser.parser import generate
 
 
 class CppGenerator(CppParser):
-    def __init__(self, ast, filename, repl_ns_dict, repl_inc_dir, destination, push_functions,
-                 **kwargs):
-        super().__init__(ast, repl_ns_dict, repl_inc_dir, destination, push_functions, [], **kwargs)
-        file = Path(filename)
-        real_name = file.name
-        self.ast_in_file = ast.files[real_name]
-        self.generated_file = (Path(destination) / (real_name[:-4] + '.h'))
-
-        self.file_str = ''
-        self.curr_tab = ''
-
-        self.to_file()
-
-    def parse_enum(self, curr_module, ksf_enum: KsfEnum):
-        enum_str = f"{self.parse_comment_above(ksf_enum.comment)}{self.curr_tab}enum {ksf_enum.name} \n{{\n"
-        enum_member_str_list = []
-        enum_member_tostr = []
-        enum_member_strto = []
+    def __init__(self, ast, repl_ns_dict, repl_inc_dir, destination, push_functions, input_file, output_file,
+                 dispatch_mode,
+                 **kwargs
+                 ):
+        super().__init__(ast, repl_ns_dict, repl_inc_dir, destination, push_functions, [], dispatch_mode, **kwargs)
+        self.input_file = input_file
+        self.output_file = Path(destination) / output_file  # 生成的头文件
+
+    def parse_enum(self, ksf_enum: KsfEnum):
+        enum_members = []
+        function_etos = []
+        function_stoe = []
         for m in ksf_enum.member:
-            enum_member_str_list.append(self.parse_enum_member(m))
-            enum_member_tostr.append(self.parse_enum_to_str(curr_module, m))
-            enum_member_strto.append(self.parse_str_to_enum(curr_module, m))
-
-        enum_str += self.add_lines(',\n'.join(enum_member_str_list), 1)
-
-        enum_str += f"\n}};\n\n"
-
-        etos_member = '\n'.join(enum_member_tostr)
-        enum_str += f"""\
-inline std::string etos(const {ksf_enum.name} &e) {{
-    switch (e) {{
-{self.add_lines(etos_member, 2)}
-        default: return "";
-    }}
-}}
-
-"""
-
-        stoe_member = self.endl().join(enum_member_strto)
-        enum_str += f"""\
-inline int stoe(const std::string &s, {ksf_enum.name} &e) {{
-{self.add_lines(stoe_member, 1)}
-    return -1;
-}}
-
-"""
-        return enum_str
+            enum_members.append(self.parse_enum_member(m))
+            function_etos.append(self.parse_enum_to_str(m))
+            function_stoe.append(self.parse_str_to_enum(m))
+
+        return [fstr(template_enum,
+                     comment=self.parse_comment_above(ksf_enum.comment),
+                     enum_name=ksf_enum.name,
+                     enum_members=enum_members,
+                     ),
+                fstr(template_etos, enum_name=ksf_enum.name, etos_member=function_etos),
+                fstr(template_stoe, enum_name=ksf_enum.name, stoe_member=function_stoe)]
 
-    def parse_resetDefault(self, curr_module, ksf_struct: KsfStruct):
-        return self.add_lines(f'''\
-    ///重新赋值为初始构造的结构
-    void resetDefault() {{
-        *this = {ksf_struct.name}{{}}; 
-    }}\n''')
+    def parse_resetDefault(self, ksf_struct: KsfStruct):
+        return fstr(template_resetDefault, struct_name=ksf_struct.name)
 
     def parse_variable_writeTo(self, ksf_field: KsfField):
         value_type = ksf_field.value_type
         if self.with_check_default:
             if isinstance(value_type, KsfBuildInType):
-                if value_type.name != 'bool':
-                    return f"""{self.parse_default_var(ksf_field.name, value_type, ksf_field.default)} {{_os.write({ksf_field.name}, {ksf_field.tag});}}"""
+                if isinstance(value_type, KsfBoolType):
+                    check_default = f"""{'!' if not ksf_field.has_default() or ksf_field.default['value'] else ''}{ksf_field.name}"""
                 else:
-                    if ksf_field.default is None or ksf_field.default['value']:
-                        return f"""if (!{ksf_field.name}) {{_os.write({ksf_field.name}, {ksf_field.tag});}}"""
-                    else:
-                        return f"""if ({ksf_field.name}) {{_os.write({ksf_field.name}, {ksf_field.tag});}}"""
+                    check_default = self.parse_default_var(f'{ksf_field.name}',
+                                                           value_type,
+                                                           ksf_field.default,
+                                                           is_equal=False
+                                                           )
             elif isinstance(value_type, KsfStructType):
+                return fstr(template_writeTo_variable,
+                            variable_name=ksf_field.name,
+                            variable_tag=ksf_field.tag, )
+            elif isinstance(value_type, KsfEnumType):
+                module_name = f"{value_type.module}::" if self.curr_module != value_type.module else ""
+
                 # 如果是枚举类型
-                if value_type.name in self.ast.enums:
-                    return f"_os.write((int32_t){ksf_field.name}, {ksf_field.tag});"
+                if ksf_field.has_default():
+                    # 有枚举默认值的，使用默认值
+                    check_default = f"""{ksf_field.name} != {module_name}{value_type.name}::{ksf_field.default['value']}"""
                 else:
-                    return f"_os.write({ksf_field.name}, {ksf_field.tag});"
+                    # 没有默认值的，使用第一个枚举值
+                    check_default = f"""{ksf_field.name} != {module_name}{value_type.name}::{ksf_field.value_type.obj_type.member[0].name}"""
             elif isinstance(value_type, KsfVectorType):
-                return f"""if (!{ksf_field.name}.empty()) {{_os.write({ksf_field.name}, {ksf_field.tag});}}"""
+                check_default = f"""!{ksf_field.name}.empty()"""
             elif isinstance(value_type, KsfMapType):
-                return f"""if (!{ksf_field.name}.empty()) {{_os.write({ksf_field.name}, {ksf_field.tag});}}"""
+                check_default = f"""!{ksf_field.name}.empty()"""
             else:
                 raise SyntaxError(f"不能被解析的字段类型[{value_type}]")
+
+            return fstr(template_writeTo_variable_with_check,
+                        check_default=check_default,
+                        variable_declare=fstr(template_writeTo_variable,
+                                              variable_name=ksf_field.name,
+                                              variable_tag=ksf_field.tag, ),
+                        )
         else:
-            return f"_os.write({ksf_field.name}, {ksf_field.tag});"
+            return fstr(template_writeTo_variable,
+                        variable_name=ksf_field.name,
+                        variable_tag=ksf_field.tag, )
 
-    def parse_writeTo(self, curr_module, ksf_struct: KsfStruct):
-        var_list = ""
+    def parse_writeTo(self, ksf_struct: KsfStruct):
+        var_list = []
         for var in ksf_struct.variable:
-            var_list += self.parse_variable_writeTo(ksf_struct.variable[var]) + '\n'
+            var_list.append(self.parse_variable_writeTo(ksf_struct.variable[var]))
 
-        return self.add_lines(f'''\
-    ///序列化为二进制流
-    template<typename WriterT>
-    void writeTo(ksf::KsfOutputStream<WriterT>& _os) const {{
-{self.add_lines(var_list, 2)}
-    }}\n''')
+        return fstr(template_writeTo, variables=var_list)
 
-    def parse_variable_writeToJson(self, curr_module, ksf_field: KsfField):
+    def parse_variable_writeToJson(self, ksf_field: KsfField):
         return f"""p->value["{ksf_field.name}"] = ksf::JsonOutput::writeJson({ksf_field.name});"""
 
-    def parse_writeToJson(self, curr_module, ksf_struct: KsfStruct):
-        var_list = ""
+    def parse_writeToJson(self, ksf_struct: KsfStruct):
+        var_list = []
         for var in ksf_struct.variable:
-            var_list += self.parse_variable_writeToJson(curr_module, ksf_struct.variable[var]) + '\n'
+            var_list.append(self.parse_variable_writeToJson(ksf_struct.variable[var]))
 
-        return self.add_lines(f'''\
-    ///序列化为Json
-    ksf::JsonValueObjPtr writeToJson() const {{
-        ksf::JsonValueObjPtr p = new ksf::JsonValueObj();
-{self.add_lines(var_list, 2)}
-        return p;
-    }}
-    
-    ///序列化为Json字符串
-    std::string writeToJsonString() const {{
-        return ksf::KS_Json::writeValue(writeToJson());
-    }}\n''')
+        return fstr(template_writeToJson, variables=var_list)
 
-    def parse_variable_readFrom(self, curr_module, ksf_field: KsfField):
-        value_type = ksf_field.value_type
-        if isinstance(value_type, KsfBuildInType):
-            return f"""_is.read({ksf_field.name}, {ksf_field.tag}, false);"""
-        elif isinstance(value_type, KsfStructType):
-            return f"""_is.read({ksf_field.name}, {ksf_field.tag}, false);"""
-        elif isinstance(value_type, KsfVectorType):
-            return f"""_is.read({ksf_field.name}, {ksf_field.tag}, false);"""
-        elif isinstance(value_type, KsfMapType):
-            return f"""_is.read({ksf_field.name}, {ksf_field.tag}, false);"""
-        else:
-            raise SyntaxError(f"不能被解析的字段类型[{value_type}]")
+    def parse_variable_readFrom(self, ksf_field: KsfField):
+        return f"""_is.read({ksf_field.name}, {ksf_field.tag}, false);"""
 
-    def parse_readFrom(self, curr_module, ksf_struct: KsfStruct):
-        var_list = ""
+    def parse_readFrom(self, ksf_struct: KsfStruct):
+        var_list = []
         for var in ksf_struct.variable:
-            var_list += self.parse_variable_readFrom(curr_module, ksf_struct.variable[var]) + '\n'
+            var_list.append(self.parse_variable_readFrom(ksf_struct.variable[var]))
 
-        return self.add_lines(f'''\
-    ///二进制反序列化为结构体
-    template<typename ReaderT>
-    void readFrom(ksf::KsfInputStream<ReaderT>& _is)
-    {{
-        resetDefault();
-{self.add_lines(var_list, 2)}
-    }}
-
-''')
+        return fstr(template_readFrom, variables=var_list)
 
-    def parse_variable_readFromJson(self, curr_module, ksf_field: KsfField):
+    def parse_variable_readFromJson(self, ksf_field: KsfField):
         return f"""ksf::JsonInput::readJson({ksf_field.name}, pObj->value["{ksf_field.name}"], false);"""
 
-    def parse_readFromJson(self, curr_module, ksf_struct: KsfStruct):
-        var_list = ""
+    def parse_readFromJson(self, ksf_struct: KsfStruct):
+        var_list = []
         for var in ksf_struct.variable:
-            var_list += self.parse_variable_readFromJson(curr_module, ksf_struct.variable[var]) + '\n'
-
-        return self.add_lines(f'''\
-    ///Json反序列化为结构体
-    void readFromJson(const ksf::JsonValuePtr &p, bool isRequire = true) {{
-        resetDefault();
-        if(NULL == p.get() || p->getType() != ksf::eJsonTypeObj)
-        {{
-            char s[128];
-            snprintf(s, sizeof(s), "read 'struct' type mismatch, get type: %d.", (p.get() ? p->getType() : 0));
-            throw ksf::KS_Json_Exception(s);
-        }}
-    
-        ksf::JsonValueObjPtr pObj=ksf::JsonValueObjPtr::dynamicCast(p);
-{self.add_lines(var_list, 2)}
-    }}
-
-    ///Json字符串反序列化为结构体
-    void readFromJsonString(const std::string &str) {{
-        readFromJson(ksf::KS_Json::getValue(str));
-    }}
+            var_list.append(self.parse_variable_readFromJson(ksf_struct.variable[var]))
 
-''')
+        return fstr(template_readFromJson, variables=var_list)
 
-    def parse_display(self, curr_module, ksf_struct: KsfStruct):
+    def parse_display(self, ksf_struct: KsfStruct):
         var_list = ""
         for var in ksf_struct.variable:
             field = ksf_struct.variable[var]
-            if field.value_type['type'] == "class" and self.get_type_id(curr_module,
-                                                                        field.value_type) in self.ast.enums:
+            if isinstance(field.value_type, KsfEnumType):
                 var_list += f'_ds.display(static_cast<int32_t>({ksf_struct.variable[var].name}),"{ksf_struct.variable[var].name}");\n'
             else:
                 var_list += f'_ds.display({ksf_struct.variable[var].name},"{ksf_struct.variable[var].name}");\n'
 
-        return self.add_lines(f'''\
-    ///打印
-    std::ostream& display(std::ostream& _os, int _level=0) const
-    {{
-        ksf::KsfDisplayer _ds(_os, _level);
-{self.add_lines(var_list, 2)}
-        return _os;
-    }}\n''')
+        return fstr(template_display, variables=var_list)
 
-    def parse_displaySimple(self, curr_module, ksf_struct: KsfStruct):
+    def parse_displaySimple(self, ksf_struct: KsfStruct):
         var_list = ""
         for var in ksf_struct.variable:
             field = ksf_struct.variable[var]
-            if field.value_type['type'] == "class" and self.get_type_id(curr_module,
-                                                                        field.value_type) in self.ast.enums:
+            if isinstance(field.value_type, KsfEnumType):
                 var_list += f'_ds.displaySimple(static_cast<int32_t>({ksf_struct.variable[var].name}), true);\n'
             else:
                 var_list += f'_ds.displaySimple({ksf_struct.variable[var].name}, true);\n'
 
-        return self.add_lines(f'''\
-    ///简单打印
-    std::ostream& displaySimple(std::ostream& _os, int _level=0) const
-    {{
-        ksf::KsfDisplayer _ds(_os, _level);
-{self.add_lines(var_list, 2)}
-        return _os;
-    }}\n''')
+        return fstr(template_displaySimple, variables=var_list)
 
-    def parse_equal(self, curr_module, ksf_struct: KsfStruct):
+    def parse_equal(self, ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             field = ksf_struct.variable[var]
-            if field.value_type['type'] == "native" and field.value_type.name in {'float', 'double'}:
+            if isinstance(field.value_type, KsfFloatType):
                 var_list.append(f'ksf::KS_Common::equal(l.{field.name}, r.{field.name})')
             else:
-                var_list.append(f'l.{field.name} == r.{field.name}')
+                var_list.append(f'(l.{field.name} == r.{field.name})')
 
-        in_list = ' && '
-        var_eq = in_list.join(var_list)
-        return self.add_lines(f'''\
-inline bool operator==(const {ksf_struct.name} &l, const {ksf_struct.name} &r) {{
-    return {var_eq};
-}}\n''')
-
-    def parse_struct(self, curr_module, ksf_struct: KsfStruct):
-        self.add_include("<kup/Ksf.h>")
-
-        struct_str = f"{self.parse_comment_above(ksf_struct.comment)}"  # 注释(可能没有)
-
-        # struct XXX : public ksf::KsfStructBase
-        # {
-        struct_str += self.add_lines(f"struct {ksf_struct.name} : public ksf::KsfStructBase\n{{\n")
+        return fstr(template_operator_equal,
+                    struct_name=ksf_struct.name,
+                    variables=' && '.join(var_list)
+                    )
 
+    def parse_struct_variables(self, ksf_struct: KsfStruct):
+        text_lines = []
         # 解析字段
         var_list = []
         for var in ksf_struct.variable:
-            var_list.append(self.parse_variable(curr_module, ksf_struct.variable[var]))
+            var_list.append(self.parse_variable(ksf_struct.variable[var]))
 
         var_widths = self.get_column_widths(var_list)
         for comment, var_type, var_name, var_value in var_list:
             if comment:
-                struct_str += self.add_lines(f"{comment:<{var_widths[0]}}", 1) + self.endl()
-            struct_str += self.add_lines(f"{var_type:<{var_widths[1]}} {var_name:<{var_widths[2]}}{var_value}",
-                                         1) + self.endl()
-
-        # public:
-        struct_str += '\n'
-        struct_str += self.add_lines(f"public:\n")
-        #     static std::string className()
-        #     {
-        #         return "xx.xxx";
-        #     }
-        #     static std::string MD5()
-        #     {
-        #         return "a123123123213";
-        #     }
-        struct_str += self.add_lines(f'''\
-    static std::string className() {{
-        return "{ksf_struct.module}.{ksf_struct.name}";
-    }}
-    
-    static std::string MD5() {{
-        return "{md5(ksf_struct.id.encode('utf-8')).hexdigest()}";
-    }}
+                text_lines.append(self.add_lines(f"{comment:<{var_widths[0]}}", 1))
+            text_lines.append(self.add_lines(f"{var_type:<{var_widths[1]}} {var_name:<{var_widths[2]}}{var_value}",
+                                             1
+                                             )
+                              )
 
-''')
-        # public:
-        struct_str += self.add_lines(f"public:\n")
-        struct_str += self.parse_resetDefault(curr_module, ksf_struct)  # resetDefault
+        return self.endl().join(text_lines)
 
-        struct_str += '\n'
-        struct_str += self.parse_writeTo(curr_module, ksf_struct)  # writeTo
+    def parse_struct(self, ksf_struct: KsfStruct):
+        self.add_include("<kup/Ksf.h>")
+
+        comment = self.parse_comment_above(ksf_struct.comment)
+        variables = self.parse_struct_variables(ksf_struct)
+        struct_functions = [
+            self.parse_resetDefault(ksf_struct),
+            self.parse_writeTo(ksf_struct),
+            self.parse_readFrom(ksf_struct)
+        ]
 
-        struct_str += '\n'
-        struct_str += self.parse_readFrom(curr_module, ksf_struct)  # readFrom
+        struct_operators = []
 
         if self.with_json:
             self.add_include("<kup/KsfJson.h>")
-            struct_str += '\n'
-            struct_str += self.parse_writeToJson(curr_module, ksf_struct)  # writeToJson
-
-            struct_str += '\n'
-            struct_str += self.parse_readFromJson(curr_module, ksf_struct)  # readFromJson
+            struct_functions.append(self.parse_writeToJson(ksf_struct))
+            struct_functions.append(self.parse_readFromJson(ksf_struct))
 
-        struct_str += '\n'
-        struct_str += self.parse_display(curr_module, ksf_struct)  # display
+        struct_functions.append(self.parse_display(ksf_struct))
+        struct_functions.append(self.parse_displaySimple(ksf_struct))
+        struct_operators.append(self.parse_equal(ksf_struct))
 
-        struct_str += '\n'
-        struct_str += self.parse_displaySimple(curr_module, ksf_struct)  # displaySimple
-
-        # };
-        struct_str += f"}};\n"
-
-        # inline bool operator==(const {ksf_struct.name}&l, const {ksf_struct.name}&r)
-        struct_str += '\n'
-        # operator==
-        struct_str += self.parse_equal(curr_module, ksf_struct)
-
-        struct_str += '\n'
-        # operator!=
-        struct_str += f"""\
-inline bool operator!=(const {ksf_struct.name} &l, const {ksf_struct.name} &r) {{
-    return !(l == r);
-}}
-
-"""
         if len(ksf_struct.key_fields) != 0:
-            struct_str += f"""\
-inline bool operator<(const {ksf_struct.name} &l, const {ksf_struct.name} &r) {{\n"""
+            key_vars = []
             for key_field in ksf_struct.key_fields:
-                struct_str += f"""\
-    if(l.{key_field} != r.{key_field})  return (l.{key_field} < r.{key_field});\n"""
-            struct_str += f"""\
-    return false;
-}}
-
-inline bool operator<=(const {ksf_struct.name} &l, const {ksf_struct.name} &r) {{
-    return !(r < l);
-}}
-
-inline bool operator>(const {ksf_struct.name} &l, const {ksf_struct.name} &r) {{
-    return r < l;
-}}
-
-inline bool operator>=(const {ksf_struct.name} &l, const {ksf_struct.name} &r) {{
-    return !(l < r);
-}}
-
-"""
+                key_vars.append(f"""if(l.{key_field} != r.{key_field})  return (l.{key_field} < r.{key_field});""")
+            struct_operators.append(fstr(template_operator_compare, struct_name=ksf_struct.name, variables=key_vars))
 
         if self.with_json:
-            # operator<<
-            struct_str += f"""\
-inline std::ostream &operator<<(std::ostream &os, const {ksf_struct.name} &r) {{
-    os << r.writeToJsonString();
-    return os;
-}}
-
-inline std::istream &operator>>(std::istream &is, {ksf_struct.name} &l) {{
-    std::istreambuf_iterator<char> eos;
-    std::string s(std::istreambuf_iterator<char>(is), eos);
-    l.readFromJsonString(s);
-    return is;
-}}
+            struct_operators.append(fstr(template_operator_stream_with_json,
+                                         wrap_mode=False,
+                                         struct_name=ksf_struct.name
+                                         )
+                                    )
+
+        return fstr(template_struct,
+                    comment=comment,
+                    module_name=self.curr_module,
+                    struct_name=ksf_struct.name,
+                    md5sum=md5(ksf_struct.id.encode('utf8')).hexdigest(),
+                    variables=variables,
+                    struct_functions=struct_functions,
+                    struct_operators=struct_operators
+                    )
+
+    def parse_output_var(self, value_type, name, with_type):
+        if not isinstance(value_type, KsfVoidType):
+            if not self.is_movable_type(value_type):
+                return f"{self.parse_type(value_type)} {name}" if with_type else name
+            elif self.with_rvalue_ref:
+                return f"{self.parse_type(value_type)} &&{name}" if with_type else f"std::move({name})"
+            else:
+                return f"const {self.parse_type(value_type)} &{name}" if with_type else name
 
-"""
-        return struct_str
+    def parse_output_vars(self, ksf_operator, with_type=True):
+        vars_list = []
+        if ksf_operator.has_return():
+            vars_list.append(self.parse_output_var(ksf_operator.return_type, '_ret', with_type))
+
+        for arg in ksf_operator.output.values():
+            vars_list.append(self.parse_output_var(arg.value_type,
+                                                   arg.name,
+                                                   with_type
+                                                   )
+                             )
+
+        return ', '.join(vars_list)
+
+    def parse_InterfacePrxCallBack(self, ksf_interface: KsfInterface):
+        func_case_list = []
+        function_handles = []
+        dispatch_str = []
 
-    def parse_InterfacePrxCallBack(self, curr_module, ksf_interface: KsfInterface):
-        prx_str = f"""\
-class {ksf_interface.name}PrxCallback : public ksf::AgentCallback
-{{
-public:
-    virtual ~{ksf_interface.name}PrxCallback() = default;
-    
-public:
-\n"""
+        def parse_func_dispatch(index, operator):
+            """处理函数的分发"""
+            output_args = []
 
-        index = 0
-        func_case_str = ""
-        for item in ksf_interface.operator:
-            operator = ksf_interface.operator[item]
+            if operator.has_return():
+                output_args.append(fstr(template_output_argument_parse,
+                                        typename=self.parse_type(operator.return_type),
+                                        argument_name='_ret',
+                                        index=0
+                                        )
+                                   )
+
+            for var in operator.output.values():
+                output_args.append(fstr(template_output_argument_parse,
+                                        typename=self.parse_type(var.value_type),
+                                        argument_name=var.name,
+                                        index=var.index
+                                        )
+                                   )
+
+            func_case_list.append(fstr(template_dispatch_case_at_client,
+                                       case=index,
+                                       function_name=operator.name,
+                                       output_params=self.parse_output_vars(operator, False),
+                                       output_arguments=output_args
+                                       )
+                                  )
+
+            function_handles.append(fstr(template_function_call,
+                                         function_name=operator.name,
+                                         arguments=self.parse_output_vars(operator, True)
+                                         )
+                                    )
+
+        get_response_context = template_getResponseContext
+
+        def dispatch(function_names):
+            dispatch_str.append(fstr(template_array_style_onDispatch_at_client,
+                                     dispatch_case_str=func_case_list,
+                                     interface_name=ksf_interface.name,
+                                     function_names=function_names
+                                     )
+                                )
+
+        self.parse_DispatchOperatorCallBack(ksf_interface, dispatch, parse_func_dispatch)
+
+        return fstr(template_callback,
+                    interface_name=ksf_interface.name,
+                    function_handles=function_handles,
+                    get_response_context=get_response_context,
+                    dispatch_str=dispatch_str
+                    )
+
+    def parse_InterfacePrxCallbackPromise(self, ksf_interface: KsfInterface):
+        dispatch_case_str = []
+        interface_promises = []
+        on_dispatch = []
+
+        def parse_func_dispatch(index, operator):
+            output_parsed_list = []
+            if operator.has_return():
+                output_parsed_list.append(f"{self.parse_type(operator.return_type)} _ret;")
+
+            for var in operator.output.values():
+                output_parsed_list.append(f"{self.parse_type(var.value_type)} {var.name};")
+
+            interface_promises.append(fstr(template_callback_promise_class,
+                                           interface_name=ksf_interface.name,
+                                           function_name=operator.name,
+                                           output_parsed_list=output_parsed_list
+                                           )
+                                      )
+
+            func_case_list = []
+            if operator.has_return():
+                func_case_list.append(f"""_is.read(ptr->_ret, 0, true);""")
+
+            for var2 in operator.output.values():
+                func_case_list.append(f"""_is.read(ptr->{var2.name}, {var2.index}, true);""")
+
+            dispatch_case_str.append(fstr(template_parse_func_dispatch_promise,
+                                          case=index,
+                                          interface_name=ksf_interface.name,
+                                          function_name=operator.name,
+                                          output_arguments=func_case_list
+                                          )
+                                     )
+
+        def dispatch(function_names):
+            on_dispatch.append(fstr(template_onDispatch_promise,
+                                    dispatch_case_str=dispatch_case_str,
+                                    interface_name=ksf_interface.name,
+                                    function_names=function_names
+                                    )
+                               )
+
+        self.parse_DispatchOperatorCallBack(ksf_interface, dispatch, parse_func_dispatch)
+
+        return fstr(template_callback_promise,
+                    interface_name=ksf_interface.name,
+                    function_names=ksf_interface.operator.keys(),
+                    interface_promises=interface_promises,
+                    on_dispatch=on_dispatch
+                    )
+
+    def parse_InterfaceCoroPrxCallback(self, ksf_interface: KsfInterface):
+        func_case_str = []
+        on_dispatch = []
+
+        def parse_case_dispatch(index, operator):
+            func_case_list = []
+            if operator.has_return():
+                func_case_list.append(
+                    f"""{self.parse_type(operator.return_type)} _ret;\n_is.read(_ret, 0, true);"""
+                )
+
+            for var2 in operator.output.values():
+                func_case_list.append(
+                    f"""{self.parse_type(var2.value_type)} {var2.name};\n_is.read({var2.name}, {var2.index}, true);"""
+                )
 
             def parse_output_vars(with_type=True):
                 def parse_output_var(value_type, name, with_type):
                     if value_type.name != 'void':
-                        if not self.is_movable_type(curr_module, value_type):
-                            return f"{self.parse_type(curr_module, value_type)} {name}" if with_type else name
-                        elif self.with_param_rvalue_ref:
-                            return f"{self.parse_type(curr_module, value_type)} &&{name}" if with_type else f"std::move({name})"
+                        if not self.is_movable_type(value_type):
+                            return f"{self.parse_type(value_type)} {name}" if with_type else name
+                        elif self.with_rvalue_ref:
+                            return f"{self.parse_type(value_type)} &&{name}" if with_type else f"std::move({name})"
                         else:
-                            return f"const {self.parse_type(curr_module, value_type)} &{name}" if with_type else name
+                            return f"const {self.parse_type(value_type)} &{name}" if with_type else name
 
                 vars_list = []
-                if operator.return_type['name'] != 'void':
+                if operator.has_return():
                     vars_list.append(parse_output_var(operator.return_type, '_ret', with_type))
 
-                for i in operator.output:
-                    vars_list.append(
-                        parse_output_var(operator.output[i].value_type, operator.output[i].name, with_type))
-
-                return ', '.join(vars_list)
-
-            prx_str += f"""\
-    virtual void callback_{operator.name}({parse_output_vars(True)}) \
-{{ throw std::runtime_error("callback_{operator.name} override incorrect."); }}
-    
-    virtual void callback_{operator.name}_exception(int32_t ret) \
-{{ throw std::runtime_error("callback_{operator.name}_exception override incorrect."); }}
-                
-"""
-
-            def parse_var_dispatch(var, name, index):
-                if var['name'] == 'void':
-                    return ""
-
-                return f"""\
-                {self.parse_type(curr_module, var)} {name};
-                _is.read({name}, {index}, true);\n\n"""
-
-            def parse_func_dispatch():
-                """处理函数的分发"""
-                func_case_str = f"""
-            case {index}: {{
-                if (msg->response->iRet != ksf::KSFSERVERSUCCESS) {{
-                    callback_{operator.name}_exception(msg->response->iRet);
-                    return msg->response->iRet;
-                }}
-                
-                ksf::KsfInputStream<ksf::BufferReader> _is;
-                
-                _is.setBuffer(msg->response->sBuffer);\n\n"""
-
-                func_case_str += parse_var_dispatch(operator.return_type, '_ret', 0)
-
-                for i in operator.output:
-                    var = operator.output[i]
-                    func_case_str += parse_var_dispatch(var.value_type, var.name, var.index)
-
-                func_case_str += f"""\
-                
-                ksf::CallbackThreadData *pCbtd = ksf::CallbackThreadData::getData();
-                assert(pCbtd != NULL);
-                
-                pCbtd->setResponseContext(msg->response->context);
-                
-                callback_{operator.name}({parse_output_vars(False)});
-                
-                pCbtd->delResponseContext();
-                
-                return ksf::KSFSERVERSUCCESS;
-            }}"""
-                return func_case_str
-
-            func_case_str += parse_func_dispatch()
-            index += 1
-
-        # 函数列表
-        prx_str += f"""\
-public:
-    virtual const std::map<std::string, std::string> &getResponseContext() const {{
-        ksf::CallbackThreadData *pCbtd = ksf::CallbackThreadData::getData();
-        assert(pCbtd != NULL);
-        
-        if (!pCbtd->getContextValid()) {{
-            throw ksf::KS_Exception("cann't get response context");
-        }}
-        return pCbtd->getResponseContext();
-    }}\n\n"""
-
-        prx_str += f"""\
-public:
-    int onDispatch(ksf::ReqMessagePtr msg) override
-    {{
-        static std::string __{ksf_interface.name}_all[] = {{"{'", "'.join(ksf_interface.operator.keys())}"}};
-                                            
-        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + 9, std::string(msg->request.sFuncName));
-        
-        if (r.first == r.second) {{
-            return ksf::KSFSERVERNOFUNCERR;
-        }}
-        
-        switch (r.first - __{ksf_interface.name}_all) {{
-{func_case_str}
-        }} //end switch
-        
-        return ksf::KSFSERVERNOFUNCERR;
-    }} //end onDispatch\n"""
-
-        prx_str += f"""}}; //end {ksf_interface.name}PrxCallback
-
-using {ksf_interface.name}PrxCallbackPtr = ksf::KS_AutoPtr<{ksf_interface.name}PrxCallback>;\n\n"""
-
-        return prx_str
-
-    def parse_InterfacePrxCallbackPromise(self, curr_module, ksf_interface: KsfInterface):
-        parsed_str = f"""\
-class {ksf_interface.name}PrxCallbackPromise: public ksf::AgentCallback
-{{
-public:
-    virtual ~{ksf_interface.name}PrxCallbackPromise() = default;
-\n"""
-
-        dispatch_case_str = ""
-        case_index = 0
-        for item in ksf_interface.operator:
-            operator = ksf_interface.operator[item]
-            parsed_str += f"""\
-public:
-    struct Promise{operator.name}: virtual public KS_HandleBase 
-    {{
-        std::map<std::string, std::string> _mRspContext;\n"""
-
-            if operator.return_type['name'] != 'void':
-                parsed_str += f"        {self.parse_type(curr_module, operator.return_type)} _ret;\n"
-
-            for item in operator.output:
-                var = operator.output[item]
-                parsed_str += f"        {self.parse_type(curr_module, var.value_type)} {var.name};\n"
-
-            parsed_str += f"""\
-    }};
-        
-    using Promise{operator.name}Ptr = ksf::KS_AutoPtr<{ksf_interface.name}PrxCallbackPromise::Promise{operator.name}>;
-    
-    {ksf_interface.name}PrxCallbackPromise(const ksf::Promise<{ksf_interface.name}PrxCallbackPromise::Promise{operator.name}Ptr> &promise): _promise_{operator.name}(promise) {{}}
-    
-    virtual void callback_{operator.name}(const {ksf_interface.name}PrxCallbackPromise::Promise{operator.name}Ptr &ptr) {{
-        _promise_{operator.name}.setValue(ptr);
-    }}
-    
-    virtual void callback_{operator.name}_exception(ksf::Int32 ret) {{
-        std::stringstream oss;
-        oss << "Function:{operator.name}_exception|Ret:";
-        oss << ret;
-        _promise_{operator.name}.setException(ksf::copyException(oss.str(), ret));
-    }}
-    
-protected:
-    ksf::Promise<{ksf_interface.name}PrxCallbackPromise::Promise{operator.name}Ptr > _promise_{operator.name};\n\n"""
-
-            def parse_var_dispatch(var, name, index):
-                if var['name'] == 'void':
-                    return ""
-
-                return f"""\
-                    _is.read(ptr->{name}, {index}, true);\n"""
-
-            def parse_func_dispatch():
-                """处理函数的分发"""
-                func_case_str = f"""\
-            case {case_index}: {{
-                if (msg->response->iRet != ksf::KSFSERVERSUCCESS) {{
-                    callback_{operator.name}_exception(msg->response->iRet);
-                    return msg->response->iRet;
-                }}
-
-                ksf::KsfInputStream<ksf::BufferReader> _is;
-                _is.setBuffer(msg->response->sBuffer);
-                {ksf_interface.name}PrxCallbackPromise::Promise{operator.name}Ptr ptr = new {ksf_interface.name}PrxCallbackPromise::Promise{operator.name}();
-                
-                try {{\n"""
-
-                func_case_list = []
-                ret = parse_var_dispatch(operator.return_type, '_ret', 0)
-                if ret != "":
-                    func_case_list.append(ret)
-
-                for item2 in operator.output:
-                    var2 = operator.output[item2]
-                    func_case_list.append(parse_var_dispatch(var2.value_type, var2.name, var2.index))
-
-                func_case_str += ''.join(func_case_list)
-                return func_case_str
-
-            case_index += 1
-            dispatch_case_str += parse_func_dispatch()
-            dispatch_case_str += f"""\
-                }} catch (std::exception &ex) {{
-                    callback_{operator.name}_exception(ksf::KSFCLIENTDECODEERR);
-                    return ksf::KSFCLIENTDECODEERR;
-                }} catch (...) {{
-                    callback_{operator.name}_exception(ksf::KSFCLIENTDECODEERR);
-                    return ksf::KSFCLIENTDECODEERR;
-                }}
-                
-                ptr->_mRspContext = msg->response->context;
-                callback_{operator.name}(ptr);
-                return ksf::KSFSERVERSUCCESS;
-            }}\n"""
-
-        parsed_str += f"""\
-public:
-    int onDispatch(ksf::ReqMessagePtr msg) override
-    {{
-        static std::string __{ksf_interface.name}_all[] = {{"{'", "'.join(ksf_interface.operator.keys())}"}};
-
-        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + 9, std::string(msg->request.sFuncName));
-
-        if (r.first == r.second) {{
-            return ksf::KSFSERVERNOFUNCERR;
-        }}
-
-        switch (r.first - __{ksf_interface.name}_all) {{\n"""
-        parsed_str += dispatch_case_str
-        parsed_str += f"""\
-        }} //end switch
-        
-        return ksf::KSFSERVERNOFUNCERR;
-    }} //end onDispatch\n"""
-
-        parsed_str += f"\n}}; //end {ksf_interface.name}PrxCallbackPromise\n\n" \
-                      f"using {ksf_interface.name}PrxCallbackPromisePtr = ksf::KS_AutoPtr<{ksf_interface.name}PrxCallbackPromise>;\n" \
-                      f"\n"
-        return parsed_str
-
-    def parse_InterfaceCoroPrxCallback(self, curr_module, ksf_interface: KsfInterface):
-        def parse_var_dispatch(var, name, index):
-            if var['name'] == 'void':
-                return ""
-
-            return f"""\
-                    {self.parse_type(curr_module, var)} {name};
-                    _is.read({name}, {index}, true);\n\n"""
-
-        def parse_func_dispatch():
-            """处理函数的分发"""
-            func_case_str = ""
-            index = 0
-            for item in ksf_interface.operator:
-                operator = ksf_interface.operator[item]
-
-                def parse_output_vars(with_type=True):
-                    def parse_output_var(value_type, name, with_type):
-                        if value_type.name != 'void':
-                            if not self.is_movable_type(curr_module, value_type):
-                                return f"{self.parse_type(curr_module, value_type)} {name}" if with_type else name
-                            elif self.with_param_rvalue_ref:
-                                return f"{self.parse_type(curr_module, value_type)} &&{name}" if with_type else f"std::move({name})"
-                            else:
-                                return f"const {self.parse_type(curr_module, value_type)} &{name}" if with_type else name
-
-                    vars_list = []
-                    if operator.return_type.name != 'void':
-                        vars_list.append(parse_output_var(operator.return_type, '_ret', with_type))
-
-                    for item in operator.output:
-                        vars_list.append(
-                            parse_output_var(operator.output[item].value_type, operator.output[item].name, with_type))
-
-                    return ', '.join(vars_list)
-
-                func_case_str += f"""
-            case {index}: {{
-                if (msg->response->iRet != ksf::KSFSERVERSUCCESS) {{
-                    callback_{operator.name}_exception(msg->response->iRet);
-                    return msg->response->iRet;
-                }}
-    
-                ksf::KsfInputStream<ksf::BufferReader> _is;
-                _is.setBuffer(msg->response->sBuffer);
-    
-                try {{\n"""
-                func_case_list = []
-                ret = parse_var_dispatch(operator.return_type, '_ret', 0)
-                if ret != "":
-                    func_case_list.append(ret)
-
-                for item2 in operator.output:
-                    var2 = operator.output[item2]
-                    func_case_list.append(parse_var_dispatch(var2.value_type, var2.name, var2.index))
-
-                func_case_str += ''.join(func_case_list)
-
-                func_case_str += f"""\
-                    callback_{operator.name}({parse_output_vars(with_type=False)});
-                }} catch (std::exception &ex) {{
-                    callback_{operator.name}_exception(ksf::KSFCLIENTDECODEERR);
-                    return ksf::KSFCLIENTDECODEERR;
-                }} catch (...) {{
-                    callback_{operator.name}_exception(ksf::KSFCLIENTDECODEERR);
-                    return ksf::KSFCLIENTDECODEERR;
-                }}
-    
-                return ksf::KSFSERVERSUCCESS;
-            }}\n"""
-
-                index += 1
-
-            return func_case_str
-
-        parsed_str = f"""\
-class {ksf_interface.name}CoroPrxCallback : public {ksf_interface.name}PrxCallback
-{{
-public:
-    virtual ~{ksf_interface.name}CoroPrxCallback() = default;
-
-public:
-    const std::map<std::string, std::string> &getResponseContext() const override {{ return _mRspContext; }}
-    
-    virtual void setResponseContext(const std::map<std::string, std::string> &mContext) {{ _mRspContext = mContext; }}
-"""
-        parsed_str += f"""\
-public:
-    int onDispatch(ksf::ReqMessagePtr msg) override
-    {{
-        static std::string __{ksf_interface.name}_all[] = {{"{'", "'.join(ksf_interface.operator.keys())}"}};
-
-        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + 9, std::string(msg->request.sFuncName));
-
-        if (r.first == r.second) {{
-            return ksf::KSFSERVERNOFUNCERR;
-        }}
-
-        switch (r.first - __{ksf_interface.name}_all) {{
-{parse_func_dispatch()}
-        }} //end switch
-        
-        return ksf::KSFSERVERNOFUNCERR;
-    }} //end onDispatch
-
-protected:
-    std::map<std::string, std::string> _mRspContext;
-}}; //end {ksf_interface.name}CoroPrxCallback
-
-typedef ksf::KS_AutoPtr<{ksf_interface.name}CoroPrxCallback> {ksf_interface.name}CoroPrxCallbackPtr;\n"""
-        return parsed_str
-
-    def parse_InterfaceProxy(self, curr_module, ksf_interface: KsfInterface):
-        def parse_operators():
-            parsed_oper_str = ""
-            for item in ksf_interface.operator:
-                operator = ksf_interface.operator[item]
-
-                def has_return():
-                    return operator.return_type['name'] != 'void'
-
-                def parse_input_vars():
-                    parsed_list = []
-                    for name in operator.input:
-                        var = operator.input[name]
-                        parsed_list.append(f"""\
-        _os.write({name}, {var.index});\n""")
-                    return parsed_list
-
-                def parse_output_vars():
-                    parsed_list = []
-                    if operator.return_type['name'] != 'void':
-                        parsed_list.append(f"""\
-        {self.parse_type(curr_module, operator.return_type)} _ret;
-        _is.read(_ret, 0, true);\n""")
-
-                    for name in operator.output:
-                        var = operator.output[name]
-                        parsed_list.append(f"""\
-        _is.read({name}, {var.index}, true);\n""")
-                    return parsed_list
+                for argument in operator.output.values():
+                    vars_list.append(parse_output_var(argument.value_type, argument.name, with_type))
 
-                def parse_all_vars(with_output=False):
-                    parsed_list = []
-                    for var_name, is_output in operator.ordered_var:
-                        if is_output:
-                            if with_output:
-                                parsed_list.append(
-                                    f"{self.parse_type(curr_module, operator.output[var_name].value_type)} &{var_name}, ")
-                        else:
-                            parsed_list.append(
-                                f"const {self.parse_type(curr_module, operator.input[var_name].value_type)} &{var_name}, ")
+                return vars_list
 
-                    return parsed_list
+            func_case_str.append(fstr(template_parse_func_dispatch_coroutine,
+                                      case=index,
+                                      output_arguments=parse_output_vars(with_type=False),
+                                      function_name=operator.name,
+                                      func_case_list=func_case_list
+                                      )
+                                 )
+
+        def dispatch(function_names):
+            on_dispatch.append(fstr(template_onDispatch_coroutine,
+                                    interface_name=ksf_interface.name,
+                                    function_names=function_names,
+                                    func_case_str=func_case_str
+                                    )
+                               )
+
+        self.parse_DispatchOperatorCallBack(ksf_interface, dispatch, parse_case_dispatch)
+        return fstr(template_callback_coroutine_class,
+                    interface_name=ksf_interface.name,
+                    on_dispatch=on_dispatch
+                    )
+
+    def parse_InterfaceProxyOperator(self, ksf_interface: KsfInterface):
+        functions = []
+        for operator in ksf_interface.operator.values():
+            input_arguments = []
+            output_arguments = []
+            for var in operator.input.values():
+                input_arguments.append(f"""_os.write({var.name}, {var.index});""")
+
+            if operator.has_return():
+                output_arguments.append(
+                    f"""{self.parse_type(operator.return_type)} _ret;\n_is.read(_ret, 0, true);"""
+                )
+
+            for name in operator.output:
+                var = operator.output[name]
+                output_arguments.append(f"""_is.read({name}, {var.index}, true);""")
 
-                parsed_oper_str += f"""\
-public:
-{self.parse_comment_above(operator.comment, tab='    ')}\
-    {self.parse_type(curr_module, operator.return_type) if has_return() else 'void'} {operator.name}({''.join(parse_all_vars(True))}const std::map<std::string, std::string> &mapReqContext = KSF_CONTEXT(), std::map<std::string, std::string> *pResponseContext = NULL) {{
-        ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
-{''.join(parse_input_vars())}
-        std::map<std::string, std::string>   _mStatus;
-        std::shared_ptr<ksf::ResponsePacket> rep = ksf_invoke(ksf::KSFNORMAL, "{operator.name}", _os, mapReqContext, _mStatus);
-        if (pResponseContext) {{
-            pResponseContext->swap(rep->context);
-        }}
-        
-        ksf::KsfInputStream<ksf::BufferReader> _is;
-        _is.setBuffer(rep->sBuffer);
-{''.join(parse_output_vars())}
-        {'return _ret;' if has_return() else ''}
-    }}
-    
-    void async_{operator.name}({ksf_interface.name}PrxCallbackPtr callback, {''.join(parse_all_vars())}const std::map<std::string, std::string> &context = KSF_CONTEXT()) {{
-        ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
-{''.join(parse_input_vars())}
-        std::map<std::string, std::string> _mStatus;
-        ksf_invoke_async(ksf::KSFNORMAL, "{operator.name}", _os, context, _mStatus, callback);
-    }}
-    
-    ksf::Future<{ksf_interface.name}PrxCallbackPromise::Promise{operator.name}Ptr> promise_async_{operator.name}({''.join(parse_all_vars())}const std::map<std::string, std::string> &context) {{
-        ksf::Promise<{ksf_interface.name}PrxCallbackPromise::Promise{operator.name}Ptr> promise;
-        {ksf_interface.name}PrxCallbackPromisePtr callback = new {ksf_interface.name}PrxCallbackPromise(promise);
-        
-        ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
-{''.join(parse_input_vars())}
-        std::map<std::string, std::string> _mStatus;
-        ksf_invoke_async(ksf::KSFNORMAL, "{operator.name}", _os, context, _mStatus, callback);
-        
-        return promise.getFuture();
-    }}
-    
-    void coro_{operator.name}({ksf_interface.name}CoroPrxCallbackPtr callback, {''.join(parse_all_vars())}const std::map<std::string, std::string> &context = KSF_CONTEXT())
-    {{
-        ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
-{''.join(parse_input_vars())}
-        std::map<std::string, std::string> _mStatus;
-        ksf_invoke_async(ksf::KSFNORMAL, "{operator.name}", _os, context, _mStatus, callback, true);
-    }}\n\n"""
-            return parsed_oper_str
-
-        parsed_str = f"""\
-class {ksf_interface.name}Proxy : public ksf::Agent
-{{
-public:
-    typedef std::map<std::string, std::string> KSF_CONTEXT;
-    
-public:
-    {ksf_interface.name}Proxy* ksf_hash(uint32_t key) {{
-        return ({ksf_interface.name}Proxy*)Agent::ksf_hash(key);
-    }}
-
-    {ksf_interface.name}Proxy* ksf_consistent_hash(uint32_t key) {{
-        return ({ksf_interface.name}Proxy*)Agent::ksf_consistent_hash(key);
-    }}
-
-    {ksf_interface.name}Proxy* ksf_open_trace(bool traceParam = false) {{
-        return ({ksf_interface.name}Proxy*)Agent::ksf_open_trace(traceParam);
-    }}
-
-    {ksf_interface.name}Proxy* ksf_set_timeout(int msecond) {{
-        return ({ksf_interface.name}Proxy*)Agent::ksf_set_timeout(msecond);
-    }}
-
-    static const char* ksf_prxname() {{ return "{ksf_interface.name}Proxy"; }}
-    
-{parse_operators()}
-}}; //end {ksf_interface.name}Proxy
-
-using {ksf_interface.name}Prx = ksf::KS_AutoPtr<{ksf_interface.name}Proxy>;\n\n"""
-
-        return parsed_str
-
-    def parse_InterfaceObj(self, curr_module, ksf_interface: KsfInterface):
-        parsed_str = f"""\
-class {ksf_interface.name} : public ksf::Servant
-{{
-public:
-    ~{ksf_interface.name}() override = default;
-    
-public:
-/*必须继承并实现的函数*/
-"""
-        parsed_async_str = ''
-        parsed_push_str = ''
-        dispatch_case_str = ""
-        index = 0
-        for item in ksf_interface.operator:
-            operator = ksf_interface.operator[item]
-
-            def has_return():
-                return operator.return_type['name'] != 'void'
-
-            def parse_invoke_vars():
-                parsed_list = []
-                for name, is_output in operator.ordered_var:
-                    if not is_output:
-                        var = operator.input[name]
-                        if self.with_param_rvalue_ref and self.is_movable_type(curr_module, var.value_type):
-                            parsed_list.append(f"""std::move({var.name}), """)
-                        else:
-                            parsed_list.append(f"""{var.name}, """)
-                    else:
-                        var = operator.output[name]
-                        parsed_list.append(f"""{var.name}, """)
-
-                return ''.join(parsed_list)
-
-            def parse_vars_list(tab=None):
-                parsed_list = []
-                for name, is_output in operator.ordered_var:
-                    if not is_output:
-                        var = operator.input[name]
-                    else:
-                        var = operator.output[name]
-                    parsed_list.append(f"""{self.parse_type(curr_module, var.value_type)} {var.name};""")
-
-                return '\n'.join([' ' * (4 * tab) + line for line in parsed_list])
-
-            def parse_output_vars(mode='ksf', tab=None):
-                if tab is None:
-                    tab = 0
-
-                parsed_list = []
-                if operator.return_type['name'] != 'void':
-                    if mode == 'ksf':
-                        parsed_list.append(f"""_os.write(_ret, 0);""")
-                    elif mode == 'kup':
-                        parsed_list.append(f"""_ksfAttr_.put("", _ret);""")
-                        parsed_list.append(f"""_ksfAttr_.put("ksf_ret", _ret);""")
-                    elif mode == 'json':
-                        parsed_list.append(f"""_p->value["ksf_ret"] = ksf::JsonOutput::writeJson(_ret);""")
-
-                for name in operator.output:
-                    var = operator.output[name]
-                    if mode == 'ksf':
-                        parsed_list.append(f"""_os.write({name}, {var.index});""")
-                    elif mode == 'kup':
-                        parsed_list.append(f"""_ksfAttr_.put("{name}", {name});""")
-                    elif mode == 'json':
-                        parsed_list.append(f"""_p->value["{name}"] = ksf::JsonOutput::writeJson({name});""")
-                return '\n'.join([' ' * (4 * tab) + line for line in parsed_list])
-
-            def parse_all_vars(with_input=False):
+            def parse_all_vars(with_output=False):
                 parsed_list = []
-                if not with_input and has_return():
-                    parsed_list.append(f", const {self.parse_type(curr_module, operator.return_type)} &_ret")
-
                 for var_name, is_output in operator.ordered_var:
                     if is_output:
-                        if with_input:
-                            parsed_list.append(
-                                f"{self.parse_type(curr_module, operator.output[var_name].value_type)} &{var_name}, ")
-                        else:
-                            parsed_list.append(
-                                f", const {self.parse_type(curr_module, operator.output[var_name].value_type)} &{var_name}")
-                    elif with_input:
-                        if self.is_movable_type(curr_module, operator.input[var_name].value_type):
-                            if self.with_param_rvalue_ref:
-                                parsed_list.append(
-                                    f"{self.parse_type(curr_module, operator.input[var_name].value_type)} &&{var_name}, ")
-                            else:
-                                parsed_list.append(
-                                    f"const {self.parse_type(curr_module, operator.input[var_name].value_type)} &{var_name}, ")
-                        else:
+                        if with_output:
                             parsed_list.append(
-                                f"{self.parse_type(curr_module, operator.input[var_name].value_type)} {var_name}, ")
-
-                return parsed_list
-
-            if self.enable_async_rsp(f"{curr_module}.{ksf_interface.name}.{operator.name}"):
-                parsed_str += f"""\
-{self.parse_comment_above(operator.comment, tab='    ')}\
-    virtual {self.parse_type(curr_module, operator.return_type) if has_return() else 'void'} {operator.name}({''.join(parse_all_vars(True))}ksf::KsfCurrentPtr _current_) = 0;\n\n"""
-
-                parsed_async_str += f"""\
-    static void async_response_{operator.name}(ksf::KsfCurrentPtr _current_{''.join(parse_all_vars())})
-    {{
-        switch (_current_->getRequestVersion()) {{
-            case ksf::KUPVERSION: {{
-                ksf::kup::UniAttribute<ksf::BufferWriterVector, ksf::BufferReader> _ksfAttr_;
-                _ksfAttr_.setVersion(_current_->getRequestVersion());
-{parse_output_vars(mode='kup', tab=4)}
-                std::vector<char> sKupResponseBuffer;
-                _ksfAttr_.encode(sKupResponseBuffer);
-                _current_->sendResponse(ksf::KSFSERVERSUCCESS, sKupResponseBuffer);
-                break;
-            }}\n"""
-
-                # 增加json支持
-                if self.with_json:
-                    parsed_async_str += f"""\
-            case ksf::JSONVERSION: {{
-                ksf::JsonValueObjPtr _p = new ksf::JsonValueObj();
-{parse_output_vars(mode='json', tab=4)}
-                std::vector<char> sJsonResponseBuffer;
-                ksf::KS_Json::writeValue(_p, sJsonResponseBuffer);
-                _current_->sendResponse(ksf::KSFSERVERSUCCESS, sJsonResponseBuffer);
-                break;
-            }}\n"""
-
-                parsed_async_str += f"""\
-            case ksf::KSFVERSION: {{
-                ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
-{parse_output_vars(mode='ksf', tab=4)}
-                _current_->sendResponse(ksf::KSFSERVERSUCCESS, _os);
-                break;
-            }}
-            default: {{std::runtime_error("unsupport ksf packet version");}}
-        }} // end switch\n"""
-                parsed_async_str += f"""\
-    }}
+                                f"{self.parse_type(operator.output[var_name].value_type)} &{var_name}"
+                            )
+                    else:
+                        parsed_list.append(
+                            f"const {self.parse_type(operator.input[var_name].value_type)} &{var_name}"
+                        )
+
+                return ', '.join(parsed_list)
+
+            arguments = parse_all_vars(with_output=True)
+            comment = self.parse_comment_above(operator.comment)
+            return_type = self.parse_type(operator.return_type) if operator.has_return() else 'void'
+
+            return_line = self.add_lines(f"\nreturn _ret;", 1) if operator.has_return() else ""
+
+            functions.append(fstr(template_proxy_function,
+                                  interface_name=ksf_interface.name,
+                                  function_name=operator.name,
+                                  arguments=arguments,
+                                  argument_async_callback=f'{ksf_interface.name}PrxCallbackPtr callback',
+                                  argument_coroutine_callback=f'{ksf_interface.name}CoroPrxCallbackPtr callback',
+                                  argument_request_context=f'const _Context_ &_context_ = _Context_()',
+                                  argument_response_context=f'_Context_ *_rsp_context_ = nullptr',
+                                  input_arguments=input_arguments,
+                                  output_arguments=output_arguments,
+                                  return_type=return_type,
+                                  return_line=return_line,
+                                  comment=comment
+                                  )
+                             )
+        return functions
+
+    def parse_InterfaceProxy(self, ksf_interface: KsfInterface):
+        return fstr(template_proxy_class,
+                    interface_name=ksf_interface.name,
+                    functions=self.parse_InterfaceProxyOperator(ksf_interface)
+                    )
+
+    def parse_OperatorParamsList(self, operator: KsfOperator, mode: str):
+        """mode: json, ksf, kup"""
+        parsed_list = []
+        for index, (name, is_output) in enumerate(operator.ordered_var):
+            if mode == 'json':
+                parsed_list.append(
+                    f"""ksf::JsonInput::readJson({name}, _jsonPtr->value["{name}"], {"false" if is_output else "true"});"""
+                )
+            elif mode == 'kup':
+                if is_output:
+                    parsed_list.append(f"""_ksfAttr_.getByDefault("{name}", {name}, {name});""")
+                else:
+                    parsed_list.append(f"""_ksfAttr_.get("{name}", {name});""")
+            elif mode == 'ksf':
+                parsed_list.append(f"""_is.read({name}, {index + 1}, {"false" if is_output else "true"});""")
+
+        return parsed_list
+
+    def parse_DispatchOperatorCallBack(self, ksf_interface: KsfInterface, interface_callback,
+                                       *operator_callbacks
+                                       ):
+        if self.dispatch_mode in ['array', 'set']:
+            operators = dict(sorted(ksf_interface.operator.items()))
+        else:
+            operators = ksf_interface.operator
 
-"""
-            # 链路追踪
-            if self.with_trace:
-                if not self.with_json:
-                    raise SyntaxError("如果需要链路追踪，需要打开生成Json序列化支持(--json)")
-
-                parsed_async_str += f"""\
-        if (_current_->isTraced()) {{
-            std::string _trace_param_;
-            int _trace_param_flag_ = ksf::ServantProxyThreadData::needTraceParam(ksf::ServantProxyThreadData::TraceContext::EST_SS, _current_->getTraceKey(), _rsp_len_);
-            if (ksf::ServantProxyThreadData::TraceContext::ENP_NORMAL == _trace_param_flag_) {{
-                ksf::JsonValueObjPtr _p_ = new ksf::JsonValueObj();
-                {'_p_->value[""] = ksf::JsonOutput::writeJson(_ret);' if has_return() else ''}
-                _trace_param_ = ksf::KS_Json::writeValue(_p_);
-            }} else if(ksf::ServantProxyThreadData::TraceContext::ENP_OVERMAXLEN == _trace_param_flag_) {{
-                _trace_param_ = "{{\"trace_param_over_max_len\":true}}";
-            }}
-            
-            KSF_TRACE(_current_->getTraceKey(), TRACE_ANNOTATION_SS, "", ksf::ServerConfig::Application + "." + ksf::ServerConfig::ServerName, "test", 0, _trace_param_, "");
-        }}\n"""
-
-            if self.enable_push(f"{curr_module}.{ksf_interface.name}.{operator.name}"):
-                dispatch_case_str += f"""\
-            case {index}: return ksf::KSFSERVERNOFUNCERR;\n"""
+        for index, operator in enumerate(operators.values()):
+            for cb in operator_callbacks:
+                cb(index, operator)
+
+        interface_callback(operators.keys())
+
+    def parse_OperatorInvokeVars(self, index, operator: KsfOperator):
+        parsed_list = []
+        for name, is_output in operator.ordered_var:
+            if not is_output:
+                var = operator.input[name]
+                if self.with_rvalue_ref and self.is_movable_type(var.value_type):
+                    parsed_list.append(f"""std::move({var.name}), """)
+                else:
+                    parsed_list.append(f"""{var.name}, """)
             else:
-                dispatch_case_str += f"""\
-            case {index}: {{
-                ksf::KsfInputStream<ksf::BufferReader> _is;
-                _is.setBuffer(_current->getRequestBuffer());
-{parse_vars_list(tab=4)}
-                switch (_current->getRequestVersion()) {{
-                    case ksf::KUPVERSION: {{
-                        ksf::kup::UniAttribute<ksf::BufferWriterVector, ksf::BufferReader>  _ksfAttr_;
-                        _ksfAttr_.setVersion(_current->getRequestVersion());
-                        _ksfAttr_.decode(_current->getRequestBuffer());
-                        break;
-                    }} 
-                    case ksf::JSONVERSION: {{
-                        ksf::JsonValueObjPtr _jsonPtr = ksf::JsonValueObjPtr::dynamicCast(ksf::KS_Json::getValue(_current->getRequestBuffer()));
-                        break;
-                    }}
-                    default: {{}}
-                }}
-                
-                {f"{self.parse_type(curr_module, operator.return_type)} _ret = " if has_return() else ""}{operator.name}({parse_invoke_vars()}_current);
-                if(_current->isResponse()) {{
-                    switch (_current->getRequestVersion()) {{
-                        case ksf::KUPVERSION: {{
-                            ksf::kup::UniAttribute<ksf::BufferWriterVector, ksf::BufferReader>  _ksfAttr_;
-                            _ksfAttr_.setVersion(_current->getRequestVersion());
-{parse_output_vars(mode='kup', tab=7)}
-                            _ksfAttr_.encode(_sResponseBuffer);
-                            break;
-                        }} 
-                        case ksf::JSONVERSION: {{
-                            ksf::JsonValueObjPtr _p = new ksf::JsonValueObj();
-{parse_output_vars(mode='json', tab=7)}
-                            ksf::KS_Json::writeValue(_p, _sResponseBuffer);
-                            break;
-                        }} 
-                        case ksf::KSFVERSION: {{
-                            ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
-{parse_output_vars(mode='ksf', tab=7)}
-                            _os.swap(_sResponseBuffer);
-                            break;
-                        }}
-                        default: {{}}
-                    }}
-                }}
-                return ksf::KSFSERVERSUCCESS;
-
-            }}\n"""
-            index += 1
+                var = operator.output[name]
+                parsed_list.append(f"""{var.name}, """)
 
-            if self.with_push and self.enable_push(f"{curr_module}.{ksf_interface.name}.{operator.name}"):
-                parsed_push_str += f"""\
-    static void async_response_push_{operator.name}(ksf::KsfCurrentPtr _current_{''.join(parse_all_vars())}, const std::map<std::string, std::string> &_context = ksf::Current::KSF_STATUS())
-    {{
-        {{
-            ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
-{parse_output_vars(mode='ksf', tab=3)}
-            _current_->sendPushResponse(ksf::KSFSERVERSUCCESS, "{operator.name}", _os, _context);
-        }}
-    }}
-\n"""
+        return ''.join(parsed_list)
 
-        parsed_str += f"""public:
-/*异步应答的封装函数*/\n\n"""
-        parsed_str += parsed_async_str
-
-        parsed_str += f"""public:
-/*推送应答的封装函数*/\n\n"""
-
-        parsed_str += parsed_push_str
-
-        parsed_str += f"""\
-public:
-    int onDispatch(ksf::KsfCurrentPtr _current, std::vector<char> &_sResponseBuffer) override
-    {{
-        static std::string __{ksf_interface.name}_all[] = {{"{'", "'.join(ksf_interface.operator.keys())}"}};
-                                            
-        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + 9, _current->getFuncName());
-        
-        if (r.first == r.second) {{
-            return ksf::KSFSERVERNOFUNCERR;
-        }}
-        
-        switch (r.first - __{ksf_interface.name}_all) {{
-"""
+    def parse_OperatorVarlist(self, index, operator: KsfOperator):
+        parsed_list = []
+        for name, is_output in operator.ordered_var:
+            if not is_output:
+                var = operator.input[name]
+            else:
+                var = operator.output[name]
+            parsed_list.append(f"""{self.parse_type(var.value_type)} {var.name};""")
 
-        parsed_str += dispatch_case_str
-        parsed_str += f"""\
-        }} //end switch
-        
-        return ksf::KSFSERVERNOFUNCERR;
-    }} //end onDispatch\n"""
+        return parsed_list
 
-        parsed_str += f"""}}; // end {ksf_interface.name}\n\n"""
-        return parsed_str
+    def parse_OperatorOutputVar(self, index, operator: KsfOperator, mode):
+        parsed_list = []
+        if operator.return_type['name'] != 'void':
+            if mode == 'ksf':
+                parsed_list.append(f"""_os.write(_ret, 0);""")
+            elif mode == 'kup':
+                parsed_list.append(f"""_ksfAttr_.put("", _ret);""")
+                parsed_list.append(f"""_ksfAttr_.put("ksf_ret", _ret);""")
+            elif mode == 'json':
+                parsed_list.append(f"""_p->value["ksf_ret"] = ksf::JsonOutput::writeJson(_ret);""")
+
+        for name in operator.output:
+            var = operator.output[name]
+            if mode == 'ksf':
+                parsed_list.append(f"""_os.write({name}, {var.index});""")
+            elif mode == 'kup':
+                parsed_list.append(f"""_ksfAttr_.put("{name}", {name});""")
+            elif mode == 'json':
+                parsed_list.append(f"""_p->value["{name}"] = ksf::JsonOutput::writeJson({name});""")
+
+        return parsed_list
+
+    def parse_OperatorAllVars(self, index, operator: KsfOperator, with_input=False):
+        parsed_list = []
+        if not with_input and operator.has_return():
+            parsed_list.append(f"const {self.parse_type(operator.return_type)} &_ret")
+
+        for var_name, is_output in operator.ordered_var:
+            if is_output:
+                if with_input:
+                    parsed_list.append(
+                        f"{self.parse_type(operator.output[var_name].value_type)} &{var_name}"
+                    )
+                else:
+                    parsed_list.append(
+                        f"const {self.parse_type(operator.output[var_name].value_type)} &{var_name}"
+                    )
+            elif with_input:
+                if self.is_movable_type(operator.input[var_name].value_type):
+                    if self.with_rvalue_ref:
+                        parsed_list.append(
+                            f"{self.parse_type(operator.input[var_name].value_type)} &&{var_name}"
+                        )
+                    else:
+                        parsed_list.append(
+                            f"const {self.parse_type(operator.input[var_name].value_type)} &{var_name}"
+                        )
+                else:
+                    parsed_list.append(
+                        f"{self.parse_type(operator.input[var_name].value_type)} {var_name}"
+                    )
+
+        return parsed_list
+
+    def parse_InterfaceObjModule(self, ksf_interface: KsfInterface):
+        dispatch_list = []
+
+        virtual_func_list = []
+        async_func_list = []
+        push_func_list = []
+        dispatch_case_list = []
+
+        def parse_Operator(index, operator):
+            async_case = []
+            push_func_case = []
+            # 当这个方法是异步方法时，需要生成一个同步方法纯虚函数和一个异步方法回调
+            if self.enable_async_rsp(f"{self.curr_module}.{ksf_interface.name}.{operator.name}"):
+                # 生成同步方法纯虚函数
+                comment = self.parse_comment_above(operator.comment)
+                return_type = self.parse_type(operator.return_type) if operator.has_return() else 'void'
+                arguments = self.parse_OperatorAllVars(index, operator, True)
+                virtual_func_list.append(fstr(template_server_pure_function,
+                                              comment=comment,
+                                              return_type=return_type,
+                                              function_name=operator.name,
+                                              arguments=arguments,
+                                              argument_current='ksf::KsfCurrentPtr _current_'
+                                              )
+                                         )
+                # 增加kup支持
+                async_case.append(fstr(template_server_async_response_case_kup,
+                                       arguments=self.parse_OperatorOutputVar(index,
+                                                                              operator,
+                                                                              mode='kup'
+                                                                              )
+                                       )
+                                  )
 
-    def parse_interface(self, curr_module, ksf_interface: KsfInterface):
-        interface_str = ''
+                # 增加json支持，当有json解析方法时
+                if self.with_json:
+                    async_case.append(fstr(template_server_async_response_case_json,
+                                           arguments=self.parse_OperatorOutputVar(index,
+                                                                                  operator,
+                                                                                  mode='json'
+                                                                                  )
+                                           )
+                                      )
+
+                async_case.append(fstr(template_server_async_response_case_ksf,
+                                       arguments=self.parse_OperatorOutputVar(index,
+                                                                              operator,
+                                                                              mode='ksf'
+                                                                              )
+                                       )
+                                  )
+
+                # 链路追踪
+                if self.with_trace:
+                    if not self.with_json:
+                        raise SyntaxError("如果需要链路追踪，需要打开生成Json序列化支持(--json)")
+
+                    return_type = '_p_->value[""] = ksf::JsonOutput::writeJson(_ret);' if operator.has_return() else ''
+                    async_func_list.append(fstr(template_server_async_response_trace,
+                                                return_type=return_type,
+                                                function_name=operator.name
+                                                )
+                                           )
+                # 生成异步方法回调
+                async_func_list.append(fstr(template_server_async_function,
+                                            function_name=operator.name,
+                                            arguments=self.parse_OperatorAllVars(index, operator),
+                                            argument_current='ksf::KsfCurrentPtr _current_',
+                                            async_response_case=async_case,
+                                            )
+                                       )
+
+            # 如果方法为推送方法，需要生成一个推送方法的推送应答
+            if self.enable_push(f"{self.curr_module}.{ksf_interface.name}.{operator.name}"):
+                dispatch_case_list.append(f"""    case {index}: return ksf::KSFSERVERNOFUNCERR;""")
+            else:
+                # 填充
+                # case, variable_declare,
+                # request_version_kup, request_version_json, request_version_ksf,
+                # return_type, operator_name, operator_params
+                # response_version_kup, response_version_json, response_version_ksf
+                dispatch_case_list.append(self.add_lines(
+                    fstr(template_dispatch_case_at_server,
+                         case=index,
+                         variable_declare=self.parse_OperatorVarlist(
+                             index,
+                             operator
+                         ),
+                         request_version_kup=self.parse_OperatorParamsList(
+                             operator,
+                             mode='kup'
+                         ),
+                         request_version_json=self.parse_OperatorParamsList(
+                             operator,
+                             mode='json'
+                         ),
+                         request_version_ksf=self.parse_OperatorParamsList(
+                             operator,
+                             mode='ksf'
+                         ),
+                         return_type=f'{self.parse_type(operator.return_type)} _ret = ' if operator.has_return() else '',
+                         function_name=operator.name,
+                         operator_params=self.parse_OperatorInvokeVars(
+                             index,
+                             operator
+                         ),
+                         response_version_kup=self.parse_OperatorOutputVar(
+                             index,
+                             operator,
+                             mode='kup'
+                         ),
+                         response_version_json=self.parse_OperatorOutputVar(
+                             index,
+                             operator,
+                             mode='json'
+                         ),
+                         response_version_ksf=self.parse_OperatorOutputVar(
+                             index,
+                             operator,
+                             mode='ksf'
+                         )
+                         ), 1
+                )
+                )
+
+            if self.with_push and self.enable_push(f"{self.curr_module}.{ksf_interface.name}.{operator.name}"):
+                push_func_case.append(fstr(template_server_push_function_ksf,
+                                           function_name=operator.name,
+                                           arguments=self.parse_OperatorOutputVar(index,
+                                                                                  operator,
+                                                                                  mode='ksf'
+                                                                                  ), )
+                                      )
+
+                arguments = self.parse_OperatorAllVars(index, operator)
+                push_func_list.append(fstr(template_server_push_function,
+                                           function_name=operator.name,
+                                           arguments=arguments,
+                                           argument_request_context=f'const _Context_ &_context_ = _Context_()',
+                                           argument_current='ksf::KsfCurrentPtr _current_',
+                                           push_func_case=push_func_case, )
+                                      )
+
+        def dispatch(function_names):
+            if self.dispatch_mode == 'array':
+                dispatch_list.append(
+                    fstr(template_array_style_onDispatch_at_server,
+                         interface_name=ksf_interface.name,
+                         function_names=function_names,
+                         dispatch_case_str=self.add_lines(dispatch_case_list, 1)
+                         )
+                )
+            elif self.dispatch_mode == 'set':
+                dispatch_list.append(
+                    fstr(template_set_style_onDispatch_at_server,
+                         interface_name=ksf_interface.name,
+                         function_names=function_names,
+                         dispatch_case_str=self.add_lines(dispatch_case_list, 1)
+                         )
+                )
+            elif self.dispatch_mode == 'hash':
+                dispatch_list.append(
+                    fstr(template_hash_style_onDispatch_at_server,
+                         interface_name=ksf_interface.name,
+                         function_names=function_names,
+                         dispatch_case_str=self.add_lines(dispatch_case_list, 1)
+                         )
+                )
+
+        self.parse_DispatchOperatorCallBack(ksf_interface, dispatch, parse_Operator)
+
+        return dispatch_list, virtual_func_list, async_func_list, push_func_list
+
+    def parse_InterfaceObj(self, ksf_interface: KsfInterface):
+        dispatch, virtual_func, parsed_async_list, parsed_push_list = self.parse_InterfaceObjModule(ksf_interface)
+        return fstr(template_server_interface,
+                    interface_name=ksf_interface.name,
+                    functions=virtual_func,
+                    async_functions=parsed_async_list,
+                    push_functions=parsed_push_list,
+                    dispatch=dispatch,
+                    )
+
+    def parse_interface(self, ksf_interface: KsfInterface):
+        interface_declare = []
+
+        if self.with_invoke_client:
+            self.add_include("<servant/Agent.h>")
+            interface_declare.append(self.add_lines(self.parse_InterfacePrxCallBack(ksf_interface)))
+            if self.with_promise:
+                self.add_include("<promise/promise.h>")
+                interface_declare.append(self.parse_InterfacePrxCallbackPromise(ksf_interface))
+
+            if self.with_coroutine:
+                interface_declare.append(self.parse_InterfaceCoroPrxCallback(ksf_interface))
+
+            interface_declare.append(self.parse_InterfaceProxy(ksf_interface))
+
+        if self.with_invoke_server:
+            self.add_include("<servant/Servant.h>")
+            interface_declare.append(self.parse_InterfaceObj(ksf_interface))
+
+        return interface_declare
+
+    def generate(self):
+        self.curr_module = None
+        module_declares = []
+        # 生成头文件（需要判断是否忽略路径)
+        for input_file in self.input_file:
+            for inc, inc_file_name in input_file.includes:
+                if self.with_ignore_relative_path:
+                    self.add_include(f'"{inc.name[:-4]}.h"')
+                else:
+                    self.add_include(self.get_repl_headfile(f'"{inc_file_name[:-4]}.h"'))
 
-        self.add_include("<servant/Agent.h>")
-        self.add_include("<servant/Servant.h>")
+            element_declares = []  # 用于存放每个模块的元素内容
 
-        interface_str += self.add_lines(self.parse_InterfacePrxCallBack(curr_module, ksf_interface))
-        self.add_include("<promise/promise.h>")
-        interface_str += self.add_lines(self.parse_InterfacePrxCallbackPromise(curr_module, ksf_interface))
-        interface_str += self.parse_InterfaceCoroPrxCallback(curr_module, ksf_interface)
-        interface_str += self.parse_InterfaceProxy(curr_module, ksf_interface)
-        interface_str += self.parse_InterfaceObj(curr_module, ksf_interface)
+            for ele in input_file.elements:
+                # 生成命名空间
+                if self.curr_module is None:
+                    self.curr_module = ele.module
+                elif self.curr_module != ele.module:
+                    module_declares.append(fstr(template_namespace,
+                                                module_begin=self.get_ns_begin(),
+                                                module_end=self.get_ns_end(),
+                                                elements=element_declares
+                                                )
+                                           )
+                    self.curr_module = ele.module
+
+                if isinstance(ele, KsfConst):
+                    element_declares.append(self.parse_const(ele))
+                    pass
+                elif isinstance(ele, KsfEnum):
+                    element_declares.append(self.parse_enum(ele))
+                    pass
+                elif isinstance(ele, KsfStruct):
+                    element_declares.append(self.parse_struct(ele))
+                    pass
+                elif isinstance(ele, KsfInterface) and self.with_rpc:
+                    element_declares.append(self.parse_interface(ele))
+
+            if self.curr_module is not None:
+                module_declares.append(fstr(template_namespace,
+                                            module_begin=self.get_ns_begin(self.curr_module),
+                                            module_end=self.get_ns_end(self.curr_module),
+                                            elements=element_declares
+                                            )
+                                       )
+                self.curr_module = None
+
+        header_content = fstr(template_header,
+                              header_description=fstr(template_header_description,
+                                                      file_name=self.output_file.name,
+                                                      date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+                                                      version="1.0.0",
+                                                      ),
+                              import_headers=self.parse_header(with_ksf=True),
+                              namespaces=module_declares
+                              )
 
-        return interface_str
+        with self.output_file.open("w") as f:
+            f.write(header_content)
 
-    def to_file(self):
-        # 生成头文件（需要判断是否忽略路径)
-        for inc, inc_file_name in self.ast_in_file.includes:
-            if self.with_ignore_relative_path:
-                self.add_include(f'"{inc.name[:-4]}.h"')
-            else:
-                self.add_include(self.get_repl_headfile(f'"{inc_file_name[:-4]}.h"'))
+    def generate_all(self):
+        self.curr_module = None
+        const_list = []
+        enum_list = []
+        struct_list = []
+        interface_list = []
+        module_declares = []
 
-        curr_module = None
-        for ele in self.ast_in_file.elements:
-            # 生成命名空间
-            if curr_module is None:
-                curr_module = ele.module
-                self.file_str += self.curr_tab + f"{self.get_ns_begin(ele.module)}\n\n"
-            elif curr_module != ele.module:
-                self.file_str += self.curr_tab + f"}} //end {curr_module}\n\n\nnamespace {ele.module} {{\n\n"
-                self.file_str += self.curr_tab + f"{self.get_ns_end(curr_module)}\n\n\nnamespace {ele.module} {{\n\n"
-                curr_module = ele.module
+        for sym in self.ast.get_all_export_symbol():
+            ele = self.ast.all_element.obj[sym]
+            self.curr_module = ele.module
 
             if isinstance(ele, KsfConst):
-                self.file_str += self.parse_const(curr_module, ele)
-                pass
+                const_list.append((ele.module, self.parse_const(ele)))
             elif isinstance(ele, KsfEnum):
-                self.file_str += self.parse_enum(curr_module, ele)
-                pass
+                enum_list.append((ele.module, self.parse_enum(ele)))
             elif isinstance(ele, KsfStruct):
-                self.file_str += self.parse_struct(curr_module, ele)
-                pass
+                struct_list.append((ele.module, self.parse_struct(ele)))
             elif isinstance(ele, KsfInterface) and self.with_rpc:
-                self.file_str += self.parse_interface(curr_module, ele)
-
-        self.file_str += f"{self.get_ns_end(curr_module)}\n\n"
+                interface_list.append((ele.module, self.parse_interface(ele)))
 
-        self.file_str = f"""\
-/**
- * @brief {self.generated_file.name} generated by ksf2cpp
- * @date {datetime.now().strftime("%Y-%m-%d %H:%M:%S")}
- * @version 1.0.0
- * @copyright kingstar
- */
-#pragma once
-
-{self.parse_header(with_ksf=True)}
-        
-{self.file_str}
-"""
+        # 生成头文件（需要判断是否忽略路径)
+        self.curr_module = None
+        element_declares = []
+        for module, element_declare in const_list + enum_list + struct_list + interface_list:
+            if self.curr_module is not None and self.curr_module != module:
+                module_declares.append(fstr(template_namespace,
+                                            module_begin=self.get_ns_begin(self.curr_module),
+                                            module_end=self.get_ns_end(self.curr_module),
+                                            elements=element_declares
+                                            )
+                                       )
+                element_declares = []
+
+            self.curr_module = module
+
+            element_declares.append(element_declare)
+
+        if self.curr_module is not None:
+            module_declares.append(fstr(template_namespace,
+                                        module_begin=self.get_ns_begin(self.curr_module),
+                                        module_end=self.get_ns_end(self.curr_module),
+                                        elements=element_declares
+                                        )
+                                   )
+            self.curr_module = None
+
+        header_content = fstr(template_header,
+                              header_description=fstr(template_header_description,
+                                                      file_name=self.output_file.name,
+                                                      date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+                                                      version="1.0.0",
+                                                      ),
+                              import_headers=self.parse_header(with_ksf=True),
+                              namespaces=module_declares
+                              )
         # print(self.file_str)
 
-        with self.generated_file.open("w") as f:
-            f.write(self.file_str)
+        with self.output_file.open("w") as f:
+            f.write(header_content)
 
 
-################### sdk 模式 ####################
+#############################################################################################################
+
 class CppSdkGenerator(CppParser):
-    def __init__(self, ast, repl_ns_dict, repl_inc_dir, destination, push_functions, export_symbols, sdk_invoke,
-                 sdk_export, **kwargs):
+    def __init__(self, ast, repl_ns_dict, repl_inc_dir, destination, push_functions, export_symbols, invoke,
+                 export, **kwargs
+                 ):
         super().__init__(ast, repl_ns_dict, repl_inc_dir, destination, push_functions, export_symbols, **kwargs)
-        self.sdk_invoke = Path(destination) / sdk_invoke  # 生成的纯rpc头文件
-        self.sdk_export = Path(destination) / sdk_export  # 生成的纯结构体头文件
-
-        self.to_file()
+        self.sdk_invoke = Path(destination) / invoke  # 生成的纯rpc头文件
+        self.sdk_export = Path(destination) / export  # 生成的纯结构体头文件
 
-    def parse_enum_pure(self, curr_module, ksf_enum: KsfEnum):
-        enum_str = f"{self.parse_comment_above(ksf_enum.comment)}{self.curr_tab}enum {ksf_enum.name} \n{{\n"
-        enum_member_str_list = []
+    def parse_enum_pure(self, ksf_enum: KsfEnum):
+        enum_members = []
         for m in ksf_enum.member:
-            enum_member_str_list.append(self.parse_enum_member(m))
-
-        enum_str += self.add_lines(',\n'.join(enum_member_str_list), 1)
-
-        enum_str += f"}};\n\n"
-        return enum_str
+            enum_members.append(self.parse_enum_member(m))
 
-    def parse_enum_func(self, curr_module, ksf_enum: KsfEnum):
-        enum_member_tostr = []
-        enum_member_strto = []
+        return fstr(template_enum,
+                    comment=self.parse_comment_above(ksf_enum.comment),
+                    enum_name=ksf_enum.name,
+                    enum_members=enum_members,
+                    )
+
+    def parse_enum_func(self, ksf_enum: KsfEnum):
+        function_etos = []
+        function_stoe = []
         for m in ksf_enum.member:
-            enum_member_tostr.append(self.parse_enum_to_str(curr_module, m, True))
-            enum_member_strto.append(self.parse_str_to_enum(curr_module, m, True))
+            function_etos.append(self.parse_enum_to_str(m, True))
+            function_stoe.append(self.parse_str_to_enum(m, True))
 
-        etos_member = '\n'.join(enum_member_tostr)
-        enum_str = f"""\
-inline std::string etos(const {self.get_full_name(curr_module, ksf_enum.name)} &e) {{
-    switch (e) {{
-{self.add_lines(etos_member, 2)}
-        default: return "";
-    }}
-}}
-
-"""
+        return [fstr(template_etos, enum_name=ksf_enum.name, etos_member=function_etos),
+                fstr(template_stoe, enum_name=ksf_enum.name, stoe_member=function_stoe)]
 
-        stoe_member = '\n'.join(enum_member_strto)
-        enum_str += f"""\
-inline int stoe(const std::string &s, {self.get_full_name(curr_module, ksf_enum.name)} &e) {{
-{self.add_lines(stoe_member, 1)}
-    return -1;
-}}
-
-"""
-        return enum_str
-
-    def parse_resetDefault(self, curr_module, ksf_struct: KsfStruct):
-        return f'''\
-///重新赋值为初始构造的结构
-void resetDefault() {{
-    *this = {ksf_struct.name}{{}}; 
-}}'''
+    def parse_resetDefault(self, ksf_struct: KsfStruct):
+        return fstr(template_resetDefault, struct_name=ksf_struct.name, )
 
     def parse_variable_writeTo(self, ksf_field: KsfField):
         value_type = ksf_field.value_type
         if self.with_check_default:
             if isinstance(value_type, KsfBuildInType):
-                if value_type.name != 'bool':
-                    return f"""{self.parse_default_var(f'obj.{ksf_field.name}', value_type, ksf_field.default)} {{_os.write(obj.{ksf_field.name}, {ksf_field.tag});}}"""
+                if isinstance(value_type, KsfBoolType):
+                    check_default = f"""{'!' if not ksf_field.has_default() or ksf_field.default['value'] else ''}obj.{ksf_field.name}"""
                 else:
-                    if ksf_field.default is None or ksf_field.default['value']:
-                        return f"""if (!obj.{ksf_field.name}) {{_os.write(obj.{ksf_field.name}, {ksf_field.tag});}}"""
-                    else:
-                        return f"""if (obj.{ksf_field.name}) {{_os.write(obj.{ksf_field.name}, {ksf_field.tag});}}"""
+                    check_default = self.parse_default_var(f'obj.{ksf_field.name}',
+                                                           value_type,
+                                                           ksf_field.default,
+                                                           is_equal=False
+                                                           )
             elif isinstance(value_type, KsfStructType):
+                return fstr(template_writeTo_variable,
+                            variable_name=f'obj.{ksf_field.name}',
+                            variable_tag=ksf_field.tag, )
+            elif isinstance(value_type, KsfEnumType):
+                module_name = f"{value_type.module}::" if self.curr_module != value_type.module else ""
+
                 # 如果是枚举类型
-                if value_type.name in self.ast.enums:
-                    return f"_os.write((int32_t)obj.{ksf_field.name}, {ksf_field.tag});"
+                if ksf_field.has_default():
+                    # 有枚举默认值的，使用默认值
+                    check_default = f"""obj.{ksf_field.name} != {module_name}{value_type.name}::{ksf_field.default['value']}"""
                 else:
-                    return f"_os.write(obj.{ksf_field.name}, {ksf_field.tag});"
+                    # 没有默认值的，使用第一个枚举值
+                    check_default = f"""obj.{ksf_field.name} != {module_name}{value_type.name}::{ksf_field.value_type.obj_type.member[0].name}"""
             elif isinstance(value_type, KsfVectorType):
-                return f"""if (!obj.{ksf_field.name}.empty()) {{_os.write(obj.{ksf_field.name}, {ksf_field.tag});}}"""
+                check_default = f"""!obj.{ksf_field.name}.empty()"""
             elif isinstance(value_type, KsfMapType):
-                return f"""if (!obj.{ksf_field.name}.empty()) {{_os.write(obj.{ksf_field.name}, {ksf_field.tag});}}"""
+                check_default = f"""!obj.{ksf_field.name}.empty()"""
             else:
                 raise SyntaxError(f"不能被解析的字段类型[{value_type}]")
+
+            return fstr(template_writeTo_variable_with_check,
+                        check_default=check_default,
+                        variable_declare=fstr(template_writeTo_variable,
+                                              variable_name=f'obj.{ksf_field.name}',
+                                              variable_tag=ksf_field.tag, ),
+                        )
         else:
-            return f"_os.write(obj.{ksf_field.name}, {ksf_field.tag});"
+            return fstr(template_writeTo_variable,
+                        variable_name=f'obj.{ksf_field.name}',
+                        variable_tag=ksf_field.tag, )
 
-    def parse_writeTo(self, curr_module, ksf_struct: KsfStruct):
-        var_list = ""
+    def parse_writeTo(self, ksf_struct: KsfStruct):
+        var_list = []
         for var in ksf_struct.variable:
-            var_list += self.parse_variable_writeTo(ksf_struct.variable[var]) + '\n'
-
-        return self.add_lines(f'''\
-    ///序列化为二进制流
-    template<typename WriterT>
-    void writeTo(ksf::KsfOutputStream<WriterT>& _os) const {{
-{self.add_lines(var_list, 2)}\
-    }}\n''')
+            var_list.append(self.parse_variable_writeTo(ksf_struct.variable[var]))
+        return fstr(template_writeTo, variables=var_list)
 
-    def parse_variable_writeToJson(self, curr_module, ksf_field: KsfField):
+    def parse_variable_writeToJson(self, ksf_field: KsfField):
         return f"""p->value["{ksf_field.name}"] = ksf::JsonOutput::writeJson(obj.{ksf_field.name});"""
 
-    def parse_writeToJson(self, curr_module, ksf_struct: KsfStruct):
-        var_list = ""
-        for var in ksf_struct.variable:
-            var_list += self.parse_variable_writeToJson(curr_module, ksf_struct.variable[var]) + '\n'
-
-        return self.add_lines(f'''\
-    ///序列化为Json
-    ksf::JsonValueObjPtr writeToJson() const {{
-        ksf::JsonValueObjPtr p = new ksf::JsonValueObj();
-{self.add_lines(var_list, 2)}\
-        return p;
-    }}
+    def parse_writeToJson(self, ksf_struct: KsfStruct):
+        var_list = []
+        for var in ksf_struct.variable.values():
+            var_list.append(self.parse_variable_writeToJson(var))
 
-    ///序列化为Json字符串
-    std::string writeToJsonString() const {{
-        return ksf::KS_Json::writeValue(writeToJson());
-    }}\n''')
+        return fstr(template_writeToJson, variables=var_list)
 
-    def parse_variable_readFrom(self, curr_module, ksf_field: KsfField):
-        value_type = ksf_field.value_type
-        if isinstance(value_type, KsfBuildInType):
-            return f"""_is.read(obj.{ksf_field.name}, {ksf_field.tag}, false);"""
-        elif isinstance(value_type, KsfStructType):
-            return f"""_is.read(obj.{ksf_field.name}, {ksf_field.tag}, false);"""
-        elif isinstance(value_type, KsfVectorType):
-            return f"""_is.read(obj.{ksf_field.name}, {ksf_field.tag}, false);"""
-        elif isinstance(value_type, KsfMapType):
-            return f"""_is.read(obj.{ksf_field.name}, {ksf_field.tag}, false);"""
-        else:
-            raise SyntaxError(f"不能被解析的字段类型[{value_type}]")
+    def parse_variable_readFrom(self, ksf_field: KsfField):
+        return f"""_is.read(obj.{ksf_field.name}, {ksf_field.tag}, false);"""
 
-    def parse_readFrom(self, curr_module, ksf_struct: KsfStruct):
-        var_list = ""
+    def parse_readFrom(self, ksf_struct: KsfStruct):
+        var_list = []
         for var in ksf_struct.variable:
-            var_list += self.parse_variable_readFrom(curr_module, ksf_struct.variable[var]) + '\n'
+            var_list.append(self.parse_variable_readFrom(ksf_struct.variable[var]))
 
-        return self.add_lines(f'''\
-    ///二进制反序列化为结构体
-    template<typename ReaderT>
-    void readFrom(ksf::KsfInputStream<ReaderT>& _is) {{
-        obj.resetDefault();
-{self.add_lines(var_list, 2)}\
-    }}\n''')
+        return fstr(template_readFrom, variables=var_list)
 
-    def parse_variable_readFromJson(self, curr_module, ksf_field: KsfField):
+    def parse_variable_readFromJson(self, ksf_field: KsfField):
         return f"""ksf::JsonInput::readJson(obj.{ksf_field.name}, pObj->value["{ksf_field.name}"], false);"""
 
-    def parse_readFromJson(self, curr_module, ksf_struct: KsfStruct):
-        var_list = ""
+    def parse_readFromJson(self, ksf_struct: KsfStruct):
+        var_list = []
         for var in ksf_struct.variable:
-            var_list += self.parse_variable_readFromJson(curr_module, ksf_struct.variable[var]) + '\n'
+            var_list.append(self.parse_variable_readFromJson(ksf_struct.variable[var]))
 
-        return self.add_lines(f'''\
-    ///Json反序列化为结构体
-    void readFromJson(const ksf::JsonValuePtr &p, bool isRequire = true) {{
-        obj.resetDefault();
-        if(NULL == p.get() || p->getType() != ksf::eJsonTypeObj) {{
-            char s[128];
-            snprintf(s, sizeof(s), "read 'struct' type mismatch, get type: %d.", (p.get() ? p->getType() : 0));
-            throw ksf::KS_Json_Exception(s);
-        }}
+        return fstr(template_readFromJson, variables=var_list)
 
-        ksf::JsonValueObjPtr pObj=ksf::JsonValueObjPtr::dynamicCast(p);
-{self.add_lines(var_list, 2)}\
-    }}
-
-    ///Json字符串反序列化为结构体
-    void readFromJsonString(const std::string &str) {{
-        readFromJson(ksf::KS_Json::getValue(str));
-    }}\n''')
-
-    def parse_display(self, curr_module, ksf_struct: KsfStruct):
-        var_list = ""
-        for var in ksf_struct.variable:
-            field = ksf_struct.variable[var]
-            if field.value_type['type'] == "class" and self.get_type_id(curr_module,
-                                                                        field.value_type) in self.ast.enums:
-                var_list += f'_ds.display(static_cast<int32_t>(obj.{ksf_struct.variable[var].name}),"{ksf_struct.variable[var].name}");\n'
+    def parse_display(self, ksf_struct: KsfStruct):
+        var_list = []
+        for field in ksf_struct.variable.values():
+            if isinstance(field.value_type, KsfEnumType):
+                var_list.append(f'_ds.display(static_cast<int32_t>(obj.{field.name}), "{field.name}");')
             else:
-                var_list += f'_ds.display(obj.{ksf_struct.variable[var].name}, "{ksf_struct.variable[var].name}");\n'
+                var_list.append(f'_ds.display(obj.{field.name}, "{field.name}");')
 
-        return self.add_lines(f'''\
-    ///打印
-    std::ostream& display(std::ostream& _os, int _level=0) const
-    {{
-        ksf::KsfDisplayer _ds(_os, _level);
-{self.add_lines(var_list, 2)}
-        return _os;
-    }}\n''')
+        return fstr(template_display, variables=var_list)
 
-    def parse_displaySimple(self, curr_module, ksf_struct: KsfStruct):
-        var_list = ""
-        for var in ksf_struct.variable:
-            field = ksf_struct.variable[var]
-            if field.value_type['type'] == "class" and self.get_type_id(curr_module,
-                                                                        field.value_type) in self.ast.enums:
-                var_list += f'_ds.displaySimple(static_cast<int32_t>(obj.{ksf_struct.variable[var].name}), true);\n'
+    def parse_displaySimple(self, ksf_struct: KsfStruct):
+        var_list = []
+        for field in ksf_struct.variable.values():
+            if isinstance(field.value_type, KsfEnumType):
+                var_list.append(f'_ds.displaySimple(static_cast<int32_t>(obj.{field.name}), true);')
             else:
-                var_list += f'_ds.displaySimple(obj.{ksf_struct.variable[var].name}, true);\n'
+                var_list.append(f'_ds.displaySimple(obj.{field.name}, true);')
 
-        return self.add_lines(f'''\
-    ///简单打印
-    std::ostream& displaySimple(std::ostream& _os, int _level=0) const
-    {{
-        ksf::KsfDisplayer _ds(_os, _level);
-{self.add_lines(var_list, 2)}
-        return _os;
-    }}\n''')
+        return fstr(template_displaySimple, variables=var_list)
 
-    def parse_equal(self, curr_module, ksf_struct: KsfStruct):
+    def parse_equal(self, ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             field = ksf_struct.variable[var]
-            if field.value_type['type'] == "native" and field.value_type.name in {'float', 'double'}:
+            if isinstance(field.value_type, KsfFloatType):
                 var_list.append(f'ksf::KS_Common::equal(l.{field.name}, r.{field.name})')
             else:
                 var_list.append(f'l.{field.name} == r.{field.name}')
 
-        in_list = ' && '
-        var_eq = in_list.join(var_list)
-        return self.add_lines(f'''\
-inline bool operator==(const {self.get_full_name(curr_module, ksf_struct.name)} &l, const {self.get_full_name(curr_module, ksf_struct.name)} &r) {{
-    return {var_eq};
-}}\n''')
-
-    def parse_struct_pure(self, curr_module, ksf_struct: KsfStruct):
-        struct_str = f"{self.parse_comment_above(ksf_struct.comment)}"  # 注释(可能没有)
-
-        struct_str += self.add_lines(f"struct {ksf_struct.name} \n{{")
+        return fstr(template_operator_equal,
+                    variables=var_list,
+                    struct_name=self.get_full_name(self.curr_module, ksf_struct.name)
+                    )
 
+    def parse_struct_pure(self, ksf_struct: KsfStruct):
+        variables = []
         # 解析字段
         var_list = []
         for var in ksf_struct.variable:
-            var_list.append(self.parse_variable(curr_module, ksf_struct.variable[var]))
+            var_list.append(self.parse_variable(ksf_struct.variable[var]))
 
         var_widths = self.get_column_widths(var_list)
         for comment, var_type, var_name, var_value in var_list:
             if comment:
-                struct_str += self.add_lines(f"{comment:<{var_widths[0]}}", 1)
-            struct_str += self.add_lines(f"{var_type:<{var_widths[1]}} {var_name:<{var_widths[2]}}{var_value}", 1)
-
-        struct_str += '\npublic:\n'
-        struct_str += self.add_lines(f"using __self__ = {ksf_struct.name}; //结构体自指标识", 1)
-        struct_str += '\npublic:\n'
-        struct_str += self.add_lines(self.parse_resetDefault(curr_module, ksf_struct), 1)  # resetDefault
+                variables.append(f"{comment:<{var_widths[0]}}")
+            variables.append(f"{var_type:<{var_widths[1]}} {var_name:<{var_widths[2]}}{var_value}")
+        return fstr(template_struct_export,
+                    comment=self.parse_comment_above(ksf_struct.comment),
+                    struct_name=ksf_struct.name,
+                    variables=variables,
+                    struct_functions=[self.parse_resetDefault(ksf_struct)]
+                    )
 
-        struct_str += '};\n\n'
-        return struct_str
-
-    def parse_struct_warp(self, curr_module, ksf_struct: KsfStruct):
+    def parse_struct_wrap(self, ksf_struct: KsfStruct):
         full_struct_name = self.get_full_name(ksf_struct.module, ksf_struct.name)
-        struct_str = self.add_lines(f"template<> struct ksf::Wrap<{full_struct_name}> : public ksf::KsfStructBase\n{{")
-        struct_str += f"""\
-public:
-    {full_struct_name} sobj;
-    {full_struct_name} &obj;
+        struct_functions = [
+            self.parse_writeTo(ksf_struct),
+            self.parse_readFrom(ksf_struct),
+        ]
+        struct_operators = [
+            self.parse_equal(ksf_struct),
 
-public:
-    static std::string className() {{
-        return "{ksf_struct.module}.{ksf_struct.name}";
-    }}
-
-    static std::string MD5() {{
-        return "{md5(ksf_struct.id.encode('utf-8')).hexdigest()}";
-    }}
-
-public:
-    ///构造函数&析构函数
-    Wrap(): obj(sobj) {{obj.resetDefault();}}
-    Wrap(Wrap&& wrap): sobj(std::move(wrap.sobj)), obj(sobj) {{}}
-    Wrap({full_struct_name}& object): obj(object) {{}}
-    Wrap(const {full_struct_name}& object): obj(*(const_cast<{full_struct_name}*>(&object))) {{}}
-    virtual ~Wrap() = default;
-
-public:
-"""
-
-        struct_str += self.parse_writeTo(curr_module, ksf_struct)  # writeTo
-
-        struct_str += '\n'
-        struct_str += self.parse_readFrom(curr_module, ksf_struct)  # readFrom
+        ]
 
         if self.with_json:
             self.add_include("<kup/KsfJson.h>")
-            struct_str += '\n'
-            struct_str += self.parse_writeToJson(curr_module, ksf_struct)  # writeToJson
-
-            struct_str += '\n'
-            struct_str += self.parse_readFromJson(curr_module, ksf_struct)  # readFromJson
+            struct_functions.append(self.parse_writeToJson(ksf_struct))  # writeToJson
+            struct_functions.append(self.parse_readFromJson(ksf_struct))  # readFromJson
 
         self.add_include("<ostream>")
-        struct_str += '\n'
-        struct_str += self.parse_display(curr_module, ksf_struct)  # display
-
-        struct_str += '\n'
-        struct_str += self.parse_displaySimple(curr_module, ksf_struct)  # displaySimple
+        struct_functions.append(self.parse_display(ksf_struct))  # display
+        struct_functions.append(self.parse_displaySimple(ksf_struct))  # displaySimple
 
-        struct_str += f"""\
-    ///转换为字符串
-    std::string toString() const {{
-        std::stringstream ss; 
-        display(ss); 
-        return ss.str(); 
-    }}
-"""
-        # };
-        struct_str += f"}};\n"
-
-        # inline bool operator==(const {ksf_struct.name}&l, const {ksf_struct.name}&r)
-        struct_str += f'\n{self.get_ns_begin(curr_module)}\n'
-
-        # operator==
-        struct_str += self.parse_equal(curr_module, ksf_struct)
-        struct_str += '\n'
-        # operator!=
-        struct_str += f"""\
-inline bool operator!=(const {full_struct_name} &l, const {full_struct_name} &r) {{
-    return !(l == r);
-}}
-"""
         if len(ksf_struct.key_fields) != 0:
-            struct_str += f"""\
-inline bool operator<(const {full_struct_name} &l, const {full_struct_name} &r) {{\n"""
+            key_variables = []
             for key_field in ksf_struct.key_fields:
-                struct_str += f"""\
-    if(l.{key_field} != r.{key_field})  return (l.{key_field} < r.{key_field});
-    return false;
-}}
-
-inline bool operator<=(const {full_struct_name} &l, const {full_struct_name} &r) {{
-    return !(r < l);
-}}
-
-inline bool operator>(const {full_struct_name} &l, const {full_struct_name} &r) {{
-    return r < l;
-}}
-
-inline bool operator>=(const {full_struct_name} &l, const {full_struct_name} &r) {{
-    return !(l < r);
-}}
-"""
+                key_variables.append(f'if(l.{key_field} != r.{key_field})  return (l.{key_field} < r.{key_field});')
+            struct_operators.append(fstr(template_operator_compare,
+                                         struct_name=full_struct_name,
+                                         variables=key_variables
+                                         )
+                                    )
 
         if self.with_json:
-            struct_str += '\n'
-            # operator<<
-            struct_str += f"""\
-inline std::ostream &operator<<(std::ostream &os, const {full_struct_name} &r) {{
-    os << ksf::MakeWrap(r).writeToJsonString();
-    return os;
-}}
-
-inline std::ostream &operator<<(std::ostream &os, const ksf::Wrap<{full_struct_name}> &r) {{
-    os << r.writeToJsonString();
-    return os;
-}}
-"""
-
-            struct_str += '\n'
-            # operator>>
-            struct_str += f"""\
-inline std::istream &operator>>(std::istream &is, {full_struct_name} &l) {{
-    std::istreambuf_iterator<char> eos;
-    std::string s(std::istreambuf_iterator<char>(is), eos);
-    ksf::MakeWrap(l).readFromJsonString(s);
-    return is;
-}}
-
-inline std::istream &operator>>(std::istream &is, ksf::Wrap<{full_struct_name}> &l) {{
-    std::istreambuf_iterator<char> eos;
-    std::string s(std::istreambuf_iterator<char>(is), eos);
-    l.readFromJsonString(s);
-    return is;
-}}
-
-using {ksf_struct.name}Wrap = ksf::Wrap<{full_struct_name}>;
-{self.get_ns_end(curr_module, with_endl=False)}
-
-"""
-
-        return struct_str
+            self.add_include("<kup/KsfJson.h>")
+            # export
+            struct_operators.append(fstr(template_operator_stream_with_json,
+                                         wrap_mode=True,
+                                         struct_name=full_struct_name
+                                         )
+                                    )
+
+            # wrap
+            struct_operators.append(fstr(template_operator_stream_with_json,
+                                         wrap_mode=False,
+                                         struct_name=f'{full_struct_name}Wrap'
+                                         )
+                                    )
+
+        return fstr(template_struct_wrap,
+                    module_name=self.curr_module,
+                    struct_name=full_struct_name,
+                    md5sum=md5(ksf_struct.id.encode('utf8')).hexdigest(),
+                    struct_functions=struct_functions,
+                    struct_operators=struct_operators,
+                    namespace_left=self.get_ns_begin(self.curr_module),
+                    namespace_right=self.get_ns_end(self.curr_module),
+                    )
 
-    def parse_InterfacePrxCallBack(self, curr_module, ksf_interface: KsfInterface):
+    def parse_InterfacePrxCallBack(self, ksf_interface: KsfInterface):
         prx_str = f"""\
 class {ksf_interface.name}WrapPrxCallback : public ksf::AgentCallback
 {{
 public:
     virtual ~{ksf_interface.name}WrapPrxCallback() = default;
 
 public:
@@ -1560,28 +1144,29 @@
             operator = ksf_interface.operator[item]
             if not operator.export:
                 continue
 
             def parse_output_vars(with_type=True):
                 def parse_output_var(value_type, name, with_type):
                     if value_type.name != 'void':
-                        if not self.is_movable_type(curr_module, value_type):
-                            return f"{self.parse_type(curr_module, value_type, is_wrap=True)} {name}" if with_type else name
-                        elif self.with_param_rvalue_ref:
-                            return f"{self.parse_type(curr_module, value_type, is_wrap=True)} &&{name}" if with_type else f"std::move({name})"
+                        if not self.is_movable_type(value_type):
+                            return f"{self.parse_type(value_type, is_wrap=True)} {name}" if with_type else name
+                        elif self.with_rvalue_ref:
+                            return f"{self.parse_type(value_type, is_wrap=True)} &&{name}" if with_type else f"std::move({name})"
                         else:
-                            return f"const {self.parse_type(curr_module, value_type, is_wrap=True)} &{name}" if with_type else name
+                            return f"const {self.parse_type(value_type, is_wrap=True)} &{name}" if with_type else name
 
                 vars_list = []
                 if operator.return_type['name'] != 'void':
                     vars_list.append(parse_output_var(operator.return_type, '_ret', with_type))
 
                 for i in operator.output:
                     vars_list.append(
-                        parse_output_var(operator.output[i].value_type, operator.output[i].name, with_type))
+                        parse_output_var(operator.output[i].value_type, operator.output[i].name, with_type)
+                    )
 
                 return ', '.join(vars_list)
 
             prx_str += f"""\
     virtual void callback_{operator.name}Wrap({parse_output_vars(True)}) \
 {{ throw std::runtime_error("callback_{operator.name}Wrap override incorrect."); }}
 
@@ -1591,15 +1176,15 @@
 """
 
             def parse_var_dispatch(var, name, index):
                 if var['name'] == 'void':
                     return ""
 
                 return f"""\
-                {self.parse_type(curr_module, var, is_wrap=True)} {name};
+                {self.parse_type(var, is_wrap=True)} {name};
                 _is.read({name}, {index}, true);\n\n"""
 
             def parse_func_dispatch():
                 """处理函数的分发"""
                 func_case_str = f"""
             case {index}: {{
                 if (msg->response->iRet != ksf::KSFSERVERSUCCESS) {{
@@ -1649,15 +1234,15 @@
     }}\n\n"""
 
         prx_str += f"""\
 public:
     int onDispatch(ksf::ReqMessagePtr msg) override {{
         static std::string __{ksf_interface.name}_all[] = {{"{'", "'.join(ksf_interface.operator.keys())}"}};
 
-        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + 9, std::string(msg->request.sFuncName));
+        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + {len(ksf_interface.operator.keys())}, std::string(msg->request.sFuncName));
 
         if (r.first == r.second) {{
             return ksf::KSFSERVERNOFUNCERR;
         }}
 
         switch (r.first - __{ksf_interface.name}_all) {{
 {func_case_str}
@@ -1668,15 +1253,15 @@
 
         prx_str += f"""}}; //end {ksf_interface.name}PrxCallback
 
 using {ksf_interface.name}WrapPrxCallbackPtr = ksf::KS_AutoPtr<{ksf_interface.name}WrapPrxCallback>;\n\n"""
 
         return prx_str
 
-    def parse_InterfacePrxCallbackPromise(self, curr_module, ksf_interface: KsfInterface):
+    def parse_InterfacePrxCallbackPromise(self, ksf_interface: KsfInterface):
         parsed_str = f"""\
 class {ksf_interface.name}WrapPrxCallbackPromise: public ksf::AgentCallback
 {{
 public:
     virtual ~{ksf_interface.name}WrapPrxCallbackPromise() = default;
 \n"""
 
@@ -1692,20 +1277,20 @@
     struct Promise{operator.name}: virtual public KS_HandleBase 
     {{
     public:
         std::map<std::string, std::string> _mRspContext;\n"""
 
             if operator.return_type['name'] != 'void':
                 parsed_str += f"\
-        {self.parse_type(curr_module, operator.return_type, is_wrap=True)} _ret;\n"
+        {self.parse_type(operator.return_type, is_wrap=True)} _ret;\n"
 
             for item in operator.output:
                 var = operator.output[item]
                 parsed_str += f"\
-        {self.parse_type(curr_module, var.value_type, is_wrap=True)} {var.name};\n"
+        {self.parse_type(var.value_type, is_wrap=True)} {var.name};\n"
 
             parsed_str += f"""\
     }};
 
     using Promise{operator.name}Ptr = ksf::KS_AutoPtr<{ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}>;
 
     {ksf_interface.name}WrapPrxCallbackPromise(const ksf::Promise<{ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}Ptr> &promise): _promise_{operator.name}(promise) {{}}
@@ -1776,15 +1361,15 @@
 
         parsed_str += f"""\
 public:
     int onDispatch(ksf::ReqMessagePtr msg) override
     {{
         static std::string __{ksf_interface.name}_all[] = {{"{'", "'.join(ksf_interface.operator.keys())}"}};
 
-        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + 9, std::string(msg->request.sFuncName));
+        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + {len(ksf_interface.operator.keys())}, std::string(msg->request.sFuncName));
 
         if (r.first == r.second) {{
             return ksf::KSFSERVERNOFUNCERR;
         }}
 
         switch (r.first - __{ksf_interface.name}_all) {{\n"""
         parsed_str += dispatch_case_str
@@ -1795,21 +1380,21 @@
     }} //end onDispatch\n"""
 
         parsed_str += f"\n}}; //end {ksf_interface.name}WrapPrxCallbackPromise\n\n" \
                       f"using {ksf_interface.name}WrapPrxCallbackPromisePtr = ksf::KS_AutoPtr<{ksf_interface.name}WrapPrxCallbackPromise>;\n" \
                       f"\n"
         return parsed_str
 
-    def parse_InterfaceCoroPrxCallback(self, curr_module, ksf_interface: KsfInterface):
+    def parse_InterfaceCoroPrxCallback(self, ksf_interface: KsfInterface):
         def parse_var_dispatch(var, name, index):
             if var['name'] == 'void':
                 return ""
 
             return f"""\
-                    {self.parse_type(curr_module, var)} {name};
+                    {self.parse_type(var)} {name};
                     _is.read({name}, {index}, true);\n\n"""
 
         def parse_func_dispatch():
             """处理函数的分发"""
             func_case_str = ""
             index = 0
             for item in ksf_interface.operator:
@@ -1817,28 +1402,29 @@
                 if not operator.export:
                     index += 1
                     continue
 
                 def parse_output_vars(with_type=True):
                     def parse_output_var(value_type, name, with_type):
                         if value_type.name != 'void':
-                            if not self.is_movable_type(curr_module, value_type):
-                                return f"{self.parse_type(curr_module, value_type)} {name}" if with_type else name
-                            elif self.with_param_rvalue_ref:
-                                return f"{self.parse_type(curr_module, value_type)} &&{name}" if with_type else f"std::move({name})"
+                            if not self.is_movable_type(value_type):
+                                return f"{self.parse_type(value_type)} {name}" if with_type else name
+                            elif self.with_rvalue_ref:
+                                return f"{self.parse_type(value_type)} &&{name}" if with_type else f"std::move({name})"
                             else:
-                                return f"const {self.parse_type(curr_module, value_type)} &{name}" if with_type else name
+                                return f"const {self.parse_type(value_type)} &{name}" if with_type else name
 
                     vars_list = []
                     if operator.return_type.name != 'void':
                         vars_list.append(parse_output_var(operator.return_type, '_ret', with_type))
 
                     for item in operator.output:
                         vars_list.append(
-                            parse_output_var(operator.output[item].value_type, operator.output[item].name, with_type))
+                            parse_output_var(operator.output[item].value_type, operator.output[item].name, with_type)
+                        )
 
                     return ', '.join(vars_list)
 
                 func_case_str += f"""
             case {index}: {{
                 if (msg->response->iRet != ksf::KSFSERVERSUCCESS) {{
                     callback_{operator.name}Wrap_exception(msg->response->iRet);
@@ -1890,15 +1476,15 @@
 """
         parsed_str += f"""\
 public:
     int onDispatch(ksf::ReqMessagePtr msg) override
     {{
         static std::string __{ksf_interface.name}_all[] = {{"{'", "'.join(ksf_interface.operator.keys())}"}};
 
-        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + 9, std::string(msg->request.sFuncName));
+        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + {len(ksf_interface.operator.keys())}, std::string(msg->request.sFuncName));
 
         if (r.first == r.second) {{
             return ksf::KSFSERVERNOFUNCERR;
         }}
 
         switch (r.first - __{ksf_interface.name}_all) {{
 {parse_func_dispatch()}
@@ -1910,76 +1496,78 @@
 protected:
     std::map<std::string, std::string> _mRspContext;
 }}; //end {ksf_interface.name}WrapCoroPrxCallback
 
 using {ksf_interface.name}WrapCoroPrxCallbackPtr = ksf::KS_AutoPtr<{ksf_interface.name}WrapCoroPrxCallback>;\n\n"""
         return parsed_str
 
-    def parse_InterfaceProxy(self, curr_module, ksf_interface: KsfInterface):
+    def parse_InterfaceProxy(self, ksf_interface: KsfInterface):
         def parse_operators():
             parsed_oper_str = ""
             for item in ksf_interface.operator:
                 operator = ksf_interface.operator[item]
                 if not operator.export:
                     continue
 
-                def has_return():
-                    return operator.return_type['name'] != 'void'
-
                 def parse_input_vars():
                     parsed_list = []
                     for name in operator.input:
                         var = operator.input[name]
                         parsed_list.append(f"""\
-        _os.write({name}, {var.index});\n""")
+        _os.write({name}, {var.index});\n"""
+                                           )
                     return parsed_list
 
                 def parse_output_vars():
                     parsed_list = []
                     if operator.return_type['name'] != 'void':
                         parsed_list.append(f"""\
-        {self.parse_type(curr_module, operator.return_type, is_wrap=True)} _ret;
-        _is.read(_ret, 0, true);\n""")
+        {self.parse_type(operator.return_type, is_wrap=True)} _ret;
+        _is.read(_ret, 0, true);\n"""
+                                           )
 
                     for name in operator.output:
                         var = operator.output[name]
                         parsed_list.append(f"""\
-        _is.read({name}, {var.index}, true);\n""")
+        _is.read({name}, {var.index}, true);\n"""
+                                           )
                     return parsed_list
 
                 def parse_all_vars(with_output=False):
                     parsed_list = []
                     for var_name, is_output in operator.ordered_var:
                         if is_output:
                             if with_output:
                                 parsed_list.append(
-                                    f"{self.parse_type(curr_module, operator.output[var_name].value_type, is_wrap=True)} &{var_name}, ")
+                                    f"{self.parse_type(operator.output[var_name].value_type, is_wrap=True)} &{var_name}, "
+                                )
                         else:
                             parsed_list.append(
-                                f"const {self.parse_type(curr_module, operator.input[var_name].value_type, is_wrap=True)} &{var_name}, ")
+                                f"const {self.parse_type(operator.input[var_name].value_type, is_wrap=True)} &{var_name}, "
+                            )
 
                     return parsed_list
 
                 parsed_oper_str += f"""\
 public:
 {self.parse_comment_above(operator.comment, tab='    ')}\
-    {self.parse_type(curr_module, operator.return_type, is_wrap=True) if has_return() else 'void'} {operator.name}({''.join(parse_all_vars(True))}const std::map<std::string, std::string> &mapReqContext = {{}}, std::map<std::string, std::string> *pResponseContext = NULL) {{
+    {self.parse_type(operator.return_type, is_wrap=True) if operator.has_return() else 'void'} {operator.name}({''.join(parse_all_vars(True))}const std::map<std::string, std::string> &mapReqContext = {{}}, std::map<std::string, std::string> *pResponseContext = NULL) {{
         ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
 {''.join(parse_input_vars())}
         std::map<std::string, std::string>   _mStatus;
         std::shared_ptr<ksf::ResponsePacket> rep = ksf_invoke(ksf::KSFNORMAL, "{operator.name}", _os, mapReqContext, _mStatus);
         if (pResponseContext) {{
             pResponseContext->swap(rep->context);
         }}
 
         ksf::KsfInputStream<ksf::BufferReader> _is;
         _is.setBuffer(rep->sBuffer);
 {''.join(parse_output_vars())}
 {f'''        return _ret;
-    }}''' if has_return() else '    }'}
+    }}''' if operator.has_return() else '    }'}
 
     void async_{operator.name}({ksf_interface.name}WrapPrxCallbackPtr callback, {''.join(parse_all_vars())}const std::map<std::string, std::string> &context = {{}}) {{
         ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
 {''.join(parse_input_vars())}
         std::map<std::string, std::string> _mStatus;
         ksf_invoke_async(ksf::KSFNORMAL, "{operator.name}", _os, context, _mStatus, callback);
     }}
@@ -2029,124 +1617,167 @@
 {parse_operators()}
 }}; //end {ksf_interface.name}WrapProxy
 
 using {ksf_interface.name}WrapPrx = ksf::KS_AutoPtr<{ksf_interface.name}WrapProxy>;\n\n"""
 
         return parsed_str
 
-    def parse_interface(self, curr_module, ksf_interface: KsfInterface):
-        interface_str = ''
+    def parse_interface(self, ksf_interface: KsfInterface):
+        interface_declare = []
 
         self.add_include("<servant/Agent.h>")
         self.add_include("<servant/Servant.h>")
 
-        interface_str += self.add_lines(self.parse_InterfacePrxCallBack(curr_module, ksf_interface))
+        interface_declare.append(self.parse_InterfacePrxCallBack(ksf_interface))
         self.add_include("<promise/promise.h>")
-        interface_str += self.add_lines(self.parse_InterfacePrxCallbackPromise(curr_module, ksf_interface))
-        interface_str += self.parse_InterfaceCoroPrxCallback(curr_module, ksf_interface)
-        interface_str += self.parse_InterfaceProxy(curr_module, ksf_interface)
+        interface_declare.append(self.parse_InterfacePrxCallbackPromise(ksf_interface))
+        interface_declare.append(self.parse_InterfaceCoroPrxCallback(ksf_interface))
+        interface_declare.append(self.parse_InterfaceProxy(ksf_interface))
+
+        return fstr(template_namespace,
+                    module_begin=self.get_ns_begin(self.curr_module),
+                    module_end=self.get_ns_end(self.curr_module),
+                    elements=interface_declare
+                    )
 
-        return interface_str
-
-    def to_file(self):
+    def generate(self):
         if len(self.ast.get_all_export_symbol()) == 0:
             raise RuntimeError("no export symbol")
 
-        curr_module = None
+        self.curr_module = None
+        export_module_declares = []
+        invoke_module_declares = []
         const_list = []
         enum_list = []
         struct_list = []
-        hidden_str = ''
+        hidden_str = []
         export_str = ''
 
         for sym in self.ast.get_all_export_symbol():
             ele = self.ast.all_element.obj[sym]
-            module = ele.module
+            self.curr_module = ele.module
 
             if isinstance(ele, KsfConst):
-                const_list.append((ele.module, self.parse_const(module, ele)))
+                const_list.append((ele.module, self.parse_const(ele)))
                 pass
             elif isinstance(ele, KsfEnum):
-                enum_list.append((ele.module, self.parse_enum_pure(module, ele)))
-                hidden_str += self.parse_enum_func(module, ele)
+                enum_list.append((ele.module, self.parse_enum_pure(ele)))
+                invoke_module_declares.append(self.parse_enum_func(ele))
                 pass
             elif isinstance(ele, KsfStruct):
-                struct_list.append((ele.module, self.parse_struct_pure(module, ele)))
-                hidden_str += self.parse_struct_warp(module, ele)
+                struct_list.append((ele.module, self.parse_struct_pure(ele)))
+                invoke_module_declares.append(self.parse_struct_wrap(ele))
                 pass
             elif isinstance(ele, KsfInterface) and self.with_rpc:
-                hidden_str += f"{self.get_ns_begin(ele.module)}"
-                hidden_str += self.parse_interface(module, ele)
-                hidden_str += f"{self.get_ns_end(module)} "
-
-        for module, text in const_list + enum_list + struct_list:
-            if curr_module is None:
-                curr_module = module
-                export_str += f"""\
-{self.get_ns_begin(module)}
-"""
-            elif curr_module != module:
-                export_str += f"""\
-{self.get_ns_end(curr_module)}
-
-{self.get_ns_begin(module)}
-"""
-                curr_module = module
-            export_str += text
+                invoke_module_declares.append(self.parse_interface(ele))
 
-        export_str = f"#pragma once\n\n{self.parse_header(with_ksf=False)}{export_str}{self.get_ns_end(curr_module)}\n\n"
-        hidden_str = "#pragma once\n\n" + self.parse_header(
-            with_ksf=True) + "\n\n" + f'#include "{self.sdk_export.name}"\n\n' + hidden_str
+        self.curr_module = None
+        element_declares = []
+        for module, element_declare in const_list + enum_list + struct_list:
+            if self.curr_module is not None and self.curr_module != module:
+                export_module_declares.append(fstr(template_namespace,
+                                                   module_begin=self.get_ns_begin(self.curr_module),
+                                                   module_end=self.get_ns_end(self.curr_module),
+                                                   elements=element_declares
+                                                   )
+                                              )
+                element_declares = []
+            self.curr_module = module
+
+            element_declares.append(element_declare)
+
+        if self.curr_module is not None:
+            export_module_declares.append(fstr(template_namespace,
+                                               module_begin=self.get_ns_begin(self.curr_module),
+                                               module_end=self.get_ns_end(self.curr_module),
+                                               elements=element_declares
+                                               )
+                                          )
+            self.curr_module = None
+
+        export_file_declare = fstr(template_header,
+                                   header_description=fstr(template_header_description,
+                                                           file_name=self.sdk_export.name,
+                                                           date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+                                                           version="1.0.0",
+                                                           ),
+                                   import_headers=self.parse_header(with_ksf=False),
+                                   namespaces=export_module_declares
+                                   )
+
+        invoke_file_declare = fstr(template_header,
+                                   header_description=fstr(template_header_description,
+                                                           file_name=self.sdk_invoke.name,
+                                                           date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+                                                           version="1.0.0",
+                                                           ),
+                                   import_headers=self.parse_header(with_ksf=True),
+                                   namespaces=invoke_module_declares
+                                   )
 
         with self.sdk_export.open("w") as f:
-            f.write(export_str)
+            f.write(export_file_declare)
 
         with self.sdk_invoke.open("w") as f:
-            f.write(hidden_str)
+            f.write(invoke_file_declare)
 
 
-def cpp_gen(files, repl_ns_dict, repl_inc_dir, include_dirs, destination_dir, push_functions, flags=None):
+def cpp_gen(mode, files,
+            replace_namespace,
+            replace_include_path,
+            include_path,
+            destination_path,
+            push_function,
+            export_symbol,
+            dispatch_mode,
+            flags: dict, **kwargs
+            ):
     """生成cpp文件"""
-    # parser_grammar = {}
     if flags is None:
         flags = defaultdict(bool)
 
     file_path = files
 
     real_inc_dirs = set()
-    for inc in include_dirs:
+    for inc in include_path:
         real_inc_dirs.add(str(Path(inc).resolve()))
-    ast = generate(file_path, real_inc_dirs, flags['with_current_priority'], [])
-    for file in file_path:
-        CppGenerator(ast, file, repl_ns_dict, repl_inc_dir, destination_dir, push_functions, **flags)
 
-
-def cpp_sdk_gen(files, repl_ns_dict, repl_inc_dir, include_dirs, destination_dir, push_functions, export_symbols,
-                sdk_invoke, sdk_export, flags=None):
-    """生成cpp sdk文件"""
-    if flags is None:
-        flags = defaultdict(bool)
-
-    file_path = files
-
-    real_inc_dirs = set()
-    for inc in include_dirs:
-        real_inc_dirs.add(str(Path(inc).resolve()))
-    ast = generate(file_path, real_inc_dirs, flags['with_current_priority'], export_symbols)
-    CppSdkGenerator(ast, repl_ns_dict, repl_inc_dir, destination_dir, push_functions, export_symbols,
-                    sdk_invoke, sdk_export, **flags)
+    if mode == 'file':
+        ast = generate(file_path, real_inc_dirs, flags['with_current_priority'], [])
+        for file in ast.files.values():
+            if file.is_source:
+                output_file = f"{file.path.name[:-4]}.h"
+                CppGenerator(ast, replace_namespace, replace_include_path, destination_path, push_function,
+                             input_file=[file], output_file=output_file, dispatch_mode=dispatch_mode,
+                             **flags
+                             ).generate()
+    elif mode in ('export_import', 'all_in_one'):
+        ast = generate(file_path, real_inc_dirs, flags['with_current_priority'], export_symbol)
+        if mode == 'export_import':
+            CppSdkGenerator(ast, replace_namespace, replace_include_path, destination_path, push_function,
+                            export_symbol,
+                            invoke=kwargs['invoke_file'], export=kwargs['export_file'], dispatch_mode=dispatch_mode,
+                            **flags
+                            ).generate()
+        else:
+            CppGenerator(ast, replace_namespace, replace_include_path, destination_path, push_function,
+                         input_file=ast.files.values(), output_file=kwargs['output_file'], dispatch_mode=dispatch_mode,
+                         **flags
+                         ).generate_all()
+    else:
+        raise RuntimeError(f"未知的模式 {mode}")
 
 
 # 测试用例
 if __name__ == '__main__':
     file_path = [
         'example/enum_simple.ksf',
         'example/const_definition.ksf',
         'example/struct_simple.ksf'
     ]
 
-    include_dirs = ['../../']
+    include_path = ['../../']
 
-    destination_dir = '../../../gen'
+    destination_path = '../../../gen'
 
-    cpp_gen(file_path, {}, {}, include_dirs, destination_dir)
-    cpp_sdk_gen(file_path, {}, {}, include_dirs, destination_dir)
+    cpp_gen('file', file_path, {}, {}, include_path, destination_path)
+    cpp_gen('export_import', file_path, {}, {}, include_path, destination_path)
```

### Comparing `ksfctl-0.2.1/ksfctl/generate/cpp/orm/parser.py` & `ksfctl-0.2.3/ksfctl/generate/ksf/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from ksfctl.parser.ksf_parser import *
-from ksfctl.parser.ksf_yacc import generate
+from ksfctl.parser.ksf import *
+from ksfctl.parser.parser import generate
 
-class OrmParser:
-    def __init__(self, ast, repl_ns_dict, repl_inc_dir, destination, **kwargs):
+
+class KsfParser:
+    def __init__(self, ast, destination, export_symbols, **kwargs):
         self.__dict__.update(kwargs)
         self.ast = ast
 
         Path(destination).mkdir(parents=True, exist_ok=True)
         self.dest_path = Path(destination)
-        self.repl_ns_dict = repl_ns_dict  # 命名空间替换字典
-        self.repl_inc_dir = repl_inc_dir  # 头文件替换字典
+        self.export_symbols = export_symbols  # 导出符号列表
 
     def __getattr__(self, name):
         if name.startswith('with_') and not hasattr(self, 'name'):
             return False
         return super().__getattr__(name)
 
     @staticmethod
@@ -48,41 +48,28 @@
     def enable_async_rsp(self, operator_name):
         """启用异步响应"""
         if not self.push_functions or operator_name not in self.push_functions:
             return True
         return False
 
     def get_repl_headfile(self, header):
-        if header[1:-1] in self.repl_inc_dir:
-            return f'"{self.repl_inc_dir[header[1:-1]]}"'
         return header
 
     def get_module(self, module):
-        if module in self.repl_ns_dict:
-            return self.repl_ns_dict[module]
         return module
 
     def get_full_name(self, module, name):
         return f"{self.get_module(module)}::{name}"
 
     def get_ns_begin(self, module, with_endl=True):
-        """获取命名空间开始，将::替换为{"""
-        ns = self.get_module(module)
-        braces = ""
-        for ns_simple in ns.split('::'):
-            braces += f'namespace {ns_simple} {{{self.endl() if with_endl else " "}'
-        return f"{braces}"
+        return f"module {module} {{\n"
 
     def get_ns_end(self, module, with_endl=True):
         """获取命名空间结束，有多少::就有多少}"""
-        ns = self.get_module(module)
-        braces = ""
-        for ns_simple in ns.split('::'):
-            braces = f'}} {f"// namespace {ns_simple}{self.endl()}" if with_endl else ""}{braces}'
-        return f"{braces}"
+        return f"}};\n"
 
     def parse_header(self, with_ksf):
         output = ""
         for header in self.inc_ordered[0]:
             if self.inc_native[header]:
                 output += "#include " + header + "\n"
 
@@ -113,60 +100,64 @@
         elif isinstance(value_type, KsfVectorType):
             return True
         elif isinstance(value_type, KsfMapType):
             return True
         else:
             return False
 
-    def parse_type(self, module, value_type: KsfType, is_wrap=False):
+    def parse_type(self, module, value_type: KsfType):
         if isinstance(value_type, KsfBuildInType):
             if value_type.name == 'string':
-                self.add_include(f"<string>")
-                return 'std::string'
+                return 'string'
             elif value_type.name == 'int':
                 if value_type.bit == 8:
-                    return f'{"unsigned char" if value_type.unsigned else "char"}'
-                return f'{"u" if value_type.unsigned else ""}int{value_type.bit}_t'
+                    return f'{"unsigned byte" if value_type.unsigned else "byte"}'
+                elif value_type.bit == 16:
+                    return f'{"unsigned short" if value_type.unsigned else "short"}'
+                elif value_type.bit == 32:
+                    return f'{"unsigned int" if value_type.unsigned else "int"}'
+                elif value_type.bit == 64:
+                    return f'{"unsigned long" if value_type.unsigned else "long"}'
+                raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
             elif value_type.name == 'float':
                 return value_type.name
             elif value_type.name == 'double':
                 return value_type.name
             elif value_type.name == 'bool':
                 return value_type.name
             else:
                 raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
         elif isinstance(value_type, KsfStructType):
             if value_type.module is not None and module != value_type.module:
-                return self.get_module(value_type['module']) + "::" + value_type.name + ("Wrap" if is_wrap else "")
+                return self.get_module(value_type['module']) + "::" + value_type.name
             else:
-                return value_type.name + ("Wrap" if is_wrap else "")
+                return value_type.name
         elif isinstance(value_type, KsfVectorType):
-            if value_type.is_ordered and not value_type.is_hashed and not value_type.is_unique_member:
-                true_type = 'std::vector'
-                self.add_include('<vector>')
+            if not self.with_special_container:
+                true_type = 'vector'
+            elif value_type.is_ordered and not value_type.is_hashed and not value_type.is_unique_member:
+                true_type = 'vector'
             elif value_type.is_ordered and not value_type.is_hashed and value_type.is_unique_member:
-                true_type = 'std::set'
-                self.add_include('<set>')
+                true_type = 'vector[set]'
             elif not value_type.is_ordered and value_type.is_hashed and value_type.is_unique_member:
-                true_type = 'std::unordered_set'
-                self.add_include('<unordered_set>')
+                true_type = 'vector[hashset]'
             else:
                 raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
 
-            return f"{true_type}<{self.parse_type(module, value_type.value_type, is_wrap=is_wrap)}>"
+            return f"{true_type}<{self.parse_type(module, value_type.value_type)}>"
         elif isinstance(value_type, KsfMapType):
-            if not value_type.is_ordered and value_type.is_hashed and value_type.is_unique_member:
-                true_type = 'std::unordered_map'
-                self.add_include('<unordered_map>')
+            if not self.with_special_container:
+                true_type = 'map'
+            elif not value_type.is_ordered and value_type.is_hashed and value_type.is_unique_member:
+                true_type = 'map[hashmap]'
             elif value_type.is_ordered and not value_type.is_hashed and value_type.is_unique_member:
-                true_type = 'std::map'
-                self.add_include('<map>')
+                true_type = 'map'
             else:
                 raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
-            return f"{true_type}<{self.parse_type(module, value_type.key_type, is_wrap=is_wrap)}, {self.parse_type(module, value_type.value_type, is_wrap=is_wrap)}>"
+            return f"{true_type}<{self.parse_type(module, value_type.key_type)}, {self.parse_type(module, value_type.value_type)}>"
 
         raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
 
     def parse_comment_above(self, comment, tab=None):
         if comment is None or comment == '':
             return ''
 
@@ -202,21 +193,27 @@
 
     def parse_const(self, curr_module, ksf_const: KsfConst):
         if ksf_const.value_type['name'] == 'string':
             return f"{self.parse_comment_above(ksf_const.comment)}{self.curr_tab}constexpr const char *{ksf_const.name} = {self.parse_value(ksf_const.value)};\n\n"
         return f"{self.parse_comment_above(ksf_const.comment)}{self.curr_tab}constexpr {self.parse_type(curr_module, ksf_const.value_type)} {ksf_const.name} = {self.parse_value(ksf_const.value)};\n\n"
 
     def parse_enum_member(self, ksf_enum_member: KsfEnumMember):
-        return f"{self.curr_tab}{ksf_enum_member.name} = {ksf_enum_member.value}"
+        return f"    {ksf_enum_member.name} = {ksf_enum_member.value}"
 
-    def parse_enum_to_str(self, ksf_enum_member: KsfEnumMember):
-        return f"case {ksf_enum_member.name}: return \"{ksf_enum_member.name}\";"
+    def parse_enum_to_str(self, curr_module, ksf_enum_member: KsfEnumMember, with_module=False):
+        if with_module:
+            return f"case {curr_module}::{ksf_enum_member.name}: return \"{ksf_enum_member.name}\";"
+        else:
+            return f"case {ksf_enum_member.name}: return \"{ksf_enum_member.name}\";"
 
-    def parse_str_to_enum(self, ksf_enum_member: KsfEnumMember):
-        return f"if (s == \"{ksf_enum_member.name}\") {{ e = {ksf_enum_member.name}; return 0; }}"
+    def parse_str_to_enum(self, curr_module, ksf_enum_member: KsfEnumMember, with_module=False):
+        if with_module:
+            return f"if (s == \"{ksf_enum_member.name}\") {{ e = {curr_module}::{ksf_enum_member.name}; return 0; }}"
+        else:
+            return f"if (s == \"{ksf_enum_member.name}\") {{ e = {ksf_enum_member.name}; return 0; }}"
 
     def parse_default_var(self, name, value_type, default):
         if default is None:
             if value_type['name'] == 'int':
                 return f'''if ({name} == 0) '''
             elif value_type['name'] == 'float':
                 return f'if (ksf::KS_Common::equal(0.0f, {name})) '
@@ -230,73 +227,52 @@
                 return ''
 
         # 特殊处理一下bool型
         if default['is_bool']:
             return f'if ({"" if default["value"] else "!"}{name})'
         elif default['is_number']:
             if value_type['name'] == 'float':
-                return f'if (ksf::KS_Common::equal({name}f, {default["value"]})) '
+                return f'if (ksf::KS_Common::equal({name}, {default["value"]}f)) '
             elif value_type['name'] == 'double':
                 return f'if (ksf::KS_Common::equal({name}, {default["value"]})) '
             return f'if ({name} == {default["value"]}) '
         elif default['is_enum']:
             return f'if ({name} == {default["value"]}) '
         else:
             return f'if ({name} == "{default["value"]}") '
 
     def parse_variable(self, curr_module, ksf_var: KsfField):
         def parse_default_var(value_type, default):
             if default is None:
-                if value_type.name == 'int':
-                    return '0'
-                elif value_type.name == 'float':
-                    return '0.0f'
-                elif value_type.name == 'double':
-                    return '0.0'
-                elif value_type.name == 'bool':
-                    return 'true'
-                elif value_type.name == 'string':
-                    return '""'
-                else:
-                    return None
+                return None
 
             # 特殊处理一下bool型
             if default['is_bool']:
                 return f'{"true" if default["value"] else "false"}'
             elif default['is_number'] or default['is_enum']:
                 return f'{default["value"]}'
             else:
                 return f'"{default["value"]}"'
 
         default_var = parse_default_var(ksf_var.value_type, ksf_var.default)
-        comment = self.parse_comment_line(ksf_var.comment)
 
-        return comment, self.parse_type(curr_module,
-                                        ksf_var.value_type), ksf_var.name, f' = {default_var};' if default_var is not None else ';'
+        return ksf_var.tag, 'require' if ksf_var.is_required else 'optional', self.parse_type(curr_module,
+                                                                                              ksf_var.value_type), ksf_var.name, f' = {default_var};' if default_var is not None else ';'
 
     def add_lines(self, lines, tab=0):
         space = ' ' * (4 * tab)
 
-        return f"\n".join(space + line for line in lines.split("\n"))
-
-
-# 测试用例
-if __name__ == '__main__':
-    file_path = [
-        'example/enum_simple.ksf',
-        'example/const_definition.ksf',
-        'example/struct_simple.ksf'
-    ]
-
-    include_dirs = ['../../']
-
-    destination_dir = '../../../gen'
-
-    push_functions = {}
+        return f"\n".join(space + line for line in lines.split("\n")) + self.endl()
 
-    export_symbols = {}
 
-    sdk_invoke = {}
+def create_parser(files, repl_ns_dict, repl_inc_dir, include_dirs, destination_dir, push_functions, export_symbols,
+                  flags=None):
+    if flags is None:
+        flags = defaultdict(bool)
 
-    sdk_export = {}
+    file_path = files
 
-    parser = create_parser(file_path, {}, {}, include_dirs, destination_dir, push_functions, export_symbols, flags={'with_current_priority': True})
+    real_inc_dirs = set()
+    for inc in include_dirs:
+        real_inc_dirs.add(str(Path(inc).resolve()))
+    ast = generate(file_path, real_inc_dirs, flags['with_current_priority'], export_symbols)
+    return KsfParser(ast, repl_ns_dict, repl_inc_dir, destination_dir, push_functions, export_symbols, **flags)
```

### Comparing `ksfctl-0.2.1/ksfctl/generate/cpp/parser.py` & `ksfctl-0.2.3/ksfctl/generate/cpp/parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,33 @@
-from ksfctl.parser.ksf_parser import *
-from ksfctl.parser.ksf_yacc import generate
+from ksfctl.parser.ksf import *
+from ksfctl.parser.parser import generate
+
 
 class CppParser:
-    def __init__(self, ast, repl_ns_dict, repl_inc_dir, destination, push_functions, export_symbols, **kwargs):
+    def __init__(self,
+                 ast,
+                 repl_ns_dict,
+                 repl_inc_dir,
+                 destination,
+                 push_functions,
+                 export_symbols,
+                 dispatch_mode,
+                 **kwargs
+                 ):
         self.__dict__.update(kwargs)
         self.ast = ast
+        self.curr_module = None
 
         Path(destination).mkdir(parents=True, exist_ok=True)
         self.dest_path = Path(destination)
         self.repl_ns_dict = repl_ns_dict  # 命名空间替换字典
         self.repl_inc_dir = repl_inc_dir  # 头文件替换字典
         self.push_functions = push_functions  # 推送函数列表
         self.export_symbols = export_symbols  # 导出符号列表
+        self.dispatch_mode = dispatch_mode  # 分发模式[支持array, set, hash]
 
         self.inc_ordered = [[
             "<ostream>",
             "<string>",
             "<vector>",
             "<set>",
             "<unordered_set>",
@@ -46,15 +58,14 @@
         self.curr_tab = ''
 
     def __getattr__(self, name):
         if name.startswith('with_') and not hasattr(self, 'name'):
             return False
         return super().__getattr__(name)
 
-
     @staticmethod
     def endl():
         return '\n'
 
     @staticmethod
     def get_column_widths(lst):
         # 创建一个空列表来保存每列的最大宽度
@@ -72,46 +83,54 @@
         if header in self.inc_native:
             self.inc_native[header] = True
         elif header in self.inc_depends:
             self.inc_native[header] = True
 
     def enable_push(self, operator_name):
         """启用推送函数"""
-        if not self.push_functions or operator_name in self.push_functions:
+        if operator_name in self.push_functions:
             return True
         return False
 
     def enable_async_rsp(self, operator_name):
         """启用异步响应"""
         if not self.push_functions or operator_name not in self.push_functions:
             return True
         return False
 
+    def has_return(self, operator):
+        return not isinstance(operator.return_type, KsfVoidType)
+
     def get_repl_headfile(self, header):
         if header[1:-1] in self.repl_inc_dir:
             return f'"{self.repl_inc_dir[header[1:-1]]}"'
         return header
 
     def get_module(self, module):
         if module in self.repl_ns_dict:
             return self.repl_ns_dict[module]
         return module
 
     def get_full_name(self, module, name):
         return f"{self.get_module(module)}::{name}"
 
     def get_ns_begin(self, module, with_endl=True):
+        if self.with_cxx17:
+            return f"""namespace {self.get_module(module)} {{"""
         """获取命名空间开始，将::替换为{"""
         ns = self.get_module(module)
         braces = ""
         for ns_simple in ns.split('::'):
             braces += f'namespace {ns_simple} {{{self.endl() if with_endl else " "}'
         return f"{braces}"
 
     def get_ns_end(self, module, with_endl=True):
+        if self.with_cxx17:
+            return f"""}} // namespace {self.get_module(module)}"""
+
         """获取命名空间结束，有多少::就有多少}"""
         ns = self.get_module(module)
         braces = ""
         for ns_simple in ns.split('::'):
             braces = f'}} {f"// namespace {ns_simple}{self.endl()}" if with_endl else ""}{braces}'
         return f"{braces}"
 
@@ -125,56 +144,49 @@
 
         if with_ksf:
             for header in self.inc_ordered[1]:
                 if self.inc_native[header]:
                     output += "#include " + header + "\n"
         return output
 
-    @staticmethod
-    def get_type_id(curr_module, value_type):
-        return f"{curr_module if value_type['module'] is None else value_type['module']}.{value_type['name']}"
-
-    def is_movable_type(self, module, value_type):
+    def is_movable_type(self, value_type):
         """判断是否是可以进行std::move的类型"""
-        if value_type['type'] == 'native':
-            return value_type['name'] == 'string'
-        elif isinstance(value_type, KsfStructType):
-
+        if isinstance(value_type, KsfStringType):
+            return True
+        elif isinstance(value_type, (KsfStructType, KsfEnumType)):
             if hasattr(value_type, 'module'):
                 class_full_name = value_type['module'] + "." + value_type['name']
             else:
-                class_full_name = module + "." + value_type['name']
+                class_full_name = self.curr_module + "." + value_type['name']
 
             return class_full_name not in self.ast.enums
         elif isinstance(value_type, KsfVectorType):
             return True
         elif isinstance(value_type, KsfMapType):
             return True
         else:
             return False
 
-    def parse_type(self, module, value_type: KsfType, is_wrap=False):
+    def parse_type(self, value_type: KsfType, is_wrap=False):
         if isinstance(value_type, KsfBuildInType):
-            if value_type.name == 'string':
-                self.add_include(f"<string>")
-                return 'std::string'
-            elif value_type.name == 'int':
+            if isinstance(value_type, KsfIntType):
                 if value_type.bit == 8:
-                    return f'{"unsigned char" if value_type.unsigned else "char"}'
-                return f'{"u" if value_type.unsigned else ""}int{value_type.bit}_t'
-            elif value_type.name == 'float':
-                return value_type.name
-            elif value_type.name == 'double':
-                return value_type.name
-            elif value_type.name == 'bool':
+                    return f'{"unsigned char" if value_type.is_unsigned else "char"}'
+                return f'{"u" if value_type.is_unsigned else ""}int{value_type.bit}_t'
+            elif isinstance(value_type, KsfFloatType):
                 return value_type.name
+            elif isinstance(value_type, KsfStringType):
+                self.add_include(f"<string>")
+                return 'std::string'
+            elif isinstance(value_type, KsfBoolType):
+                return 'bool'
             else:
                 raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
-        elif isinstance(value_type, KsfStructType):
-            if value_type.module is not None and module != value_type.module:
+        elif isinstance(value_type, (KsfStructType, KsfEnumType)):
+            if value_type.module is not None and self.curr_module != value_type.module:
                 return self.get_module(value_type['module']) + "::" + value_type.name + ("Wrap" if is_wrap else "")
             else:
                 return value_type.name + ("Wrap" if is_wrap else "")
         elif isinstance(value_type, KsfVectorType):
             if value_type.is_ordered and not value_type.is_hashed and not value_type.is_unique_member:
                 true_type = 'std::vector'
                 self.add_include('<vector>')
@@ -183,25 +195,25 @@
                 self.add_include('<set>')
             elif not value_type.is_ordered and value_type.is_hashed and value_type.is_unique_member:
                 true_type = 'std::unordered_set'
                 self.add_include('<unordered_set>')
             else:
                 raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
 
-            return f"{true_type}<{self.parse_type(module, value_type.value_type, is_wrap=is_wrap)}>"
+            return f"{true_type}<{self.parse_type(value_type.value_type, is_wrap=is_wrap)}>"
         elif isinstance(value_type, KsfMapType):
             if not value_type.is_ordered and value_type.is_hashed and value_type.is_unique_member:
                 true_type = 'std::unordered_map'
                 self.add_include('<unordered_map>')
             elif value_type.is_ordered and not value_type.is_hashed and value_type.is_unique_member:
                 true_type = 'std::map'
                 self.add_include('<map>')
             else:
                 raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
-            return f"{true_type}<{self.parse_type(module, value_type.key_type, is_wrap=is_wrap)}, {self.parse_type(module, value_type.value_type, is_wrap=is_wrap)}>"
+            return f"{true_type}<{self.parse_type(value_type.key_type, is_wrap=is_wrap)}, {self.parse_type(value_type.value_type, is_wrap=is_wrap)}>"
 
         raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
 
     def parse_comment_above(self, comment, tab=None):
         if comment is None or comment == '':
             return ''
 
@@ -231,75 +243,78 @@
             return f"//{comment}"
         else:
             raise SyntaxError("不支持的注释方式")
 
     def parse_value(self, value):
         return value['value'] if value['is_number'] else f'"{value["value"]}"'
 
-    def parse_const(self, curr_module, ksf_const: KsfConst):
-        if ksf_const.value_type['name'] == 'string':
-            return f"{self.parse_comment_above(ksf_const.comment)}{self.curr_tab}constexpr const char *{ksf_const.name} = {self.parse_value(ksf_const.value)};\n\n"
-        return f"{self.parse_comment_above(ksf_const.comment)}{self.curr_tab}constexpr {self.parse_type(curr_module, ksf_const.value_type)} {ksf_const.name} = {self.parse_value(ksf_const.value)};\n\n"
+    def parse_const(self, ksf_const: KsfConst):
+        if isinstance(ksf_const.value_type, KsfStringType):
+            return f"{self.parse_comment_above(ksf_const.comment)}{self.curr_tab}constexpr const char *{ksf_const.name} = {self.parse_value(ksf_const.value)};"
+        return f"{self.parse_comment_above(ksf_const.comment)}{self.curr_tab}constexpr {self.parse_type(ksf_const.value_type)} {ksf_const.name} = {self.parse_value(ksf_const.value)};"
 
     def parse_enum_member(self, ksf_enum_member: KsfEnumMember):
-        return f"{self.curr_tab}{ksf_enum_member.name} = {ksf_enum_member.value}"
+        return f"{self.curr_tab}{ksf_enum_member.name} = {ksf_enum_member.value},"
 
-    def parse_enum_to_str(self, curr_module, ksf_enum_member: KsfEnumMember, with_module=False):
+    def parse_enum_to_str(self, ksf_enum_member: KsfEnumMember, with_module=False):
         if with_module:
-            return f"case {curr_module}::{ksf_enum_member.name}: return \"{ksf_enum_member.name}\";"
+            return f"case {self.curr_module}::{ksf_enum_member.name}: return \"{ksf_enum_member.name}\";"
         else:
             return f"case {ksf_enum_member.name}: return \"{ksf_enum_member.name}\";"
 
-    def parse_str_to_enum(self, curr_module, ksf_enum_member: KsfEnumMember, with_module=False):
+    def parse_str_to_enum(self, ksf_enum_member: KsfEnumMember, with_module=False):
         if with_module:
-            return f"if (s == \"{ksf_enum_member.name}\") {{ e = {curr_module}::{ksf_enum_member.name}; return 0; }}"
+            return f"if (s == \"{ksf_enum_member.name}\") {{ e = {self.curr_module}::{ksf_enum_member.name}; return 0; }}"
         else:
             return f"if (s == \"{ksf_enum_member.name}\") {{ e = {ksf_enum_member.name}; return 0; }}"
 
-    def parse_default_var(self, name, value_type, default):
+    def parse_default_var(self, name, value_type, default, is_equal=True):
         if default is None:
-            if value_type['name'] == 'int':
-                return f'''if ({name} == 0) '''
-            elif value_type['name'] == 'float':
-                return f'if (ksf::KS_Common::equal(0.0f, {name})) '
-            elif value_type['name'] == 'double':
-                return f'if (ksf::KS_Common::equal(0.0, {name})) '
-            elif value_type['name'] == 'bool':
-                return f'if ({name})'
-            elif value_type['name'] == 'string':
-                return f'if ({name}.empty())'
-            else:
-                return ''
+            if isinstance(value_type, KsfIntType):
+                return f'''{name} {"=" if is_equal else "!"}= 0'''
+            elif isinstance(value_type, KsfFloatType):
+                if value_type.bit == 32:
+                    return f'{"" if is_equal else "!"}ksf::KS_Common::equal(0.0f, {name})'
+                else:
+                    return f'{"" if is_equal else "!"}ksf::KS_Common::equal(0.0, {name})'
+            elif isinstance(value_type, KsfBoolType):
+                return f'{"" if is_equal else "!"}{name}'
+            elif isinstance(value_type, KsfStringType):
+                return f'{"" if is_equal else "!"}{name}.empty()'
+
+            return ''
 
         # 特殊处理一下bool型
         if default['is_bool']:
-            return f'if ({"" if default["value"] else "!"}{name})'
+            return f'{"" if default["value"] == is_equal else "!"}{name}'
         elif default['is_number']:
-            if value_type['name'] == 'float':
-                return f'if (ksf::KS_Common::equal({name}, {default["value"]}f)) '
-            elif value_type['name'] == 'double':
-                return f'if (ksf::KS_Common::equal({name}, {default["value"]})) '
-            return f'if ({name} == {default["value"]}) '
+            if isinstance(value_type, KsfFloatType):
+                if value_type.bit == 32:
+                    return f'{"" if default["value"] == is_equal else "!"}ksf::KS_Common::equal({name}, {default["value"]}f)'
+                else:
+                    return f'{"" if default["value"] == is_equal else "!"}ksf::KS_Common::equal({name}, {default["value"]})'
+            return f'{name} {"=" if default["value"] == is_equal else "!"}= {default["value"]}'
         elif default['is_enum']:
-            return f'if ({name} == {default["value"]}) '
+            return f'{name} {"=" if default["value"] == is_equal else "!"}= {default["value"]}'
         else:
-            return f'if ({name} == "{default["value"]}") '
+            return f'{name} {"=" if default["value"] == is_equal else "!"}= "{default["value"]}"'
 
-    def parse_variable(self, curr_module, ksf_var: KsfField):
+    def parse_variable(self, ksf_var: KsfField):
         def parse_default_var(value_type, default):
             if default is None:
-                if value_type.name == 'int':
+                if isinstance(value_type, KsfIntType):
                     return '0'
-                elif value_type.name == 'float':
-                    return '0.0f'
-                elif value_type.name == 'double':
-                    return '0.0'
-                elif value_type.name == 'bool':
+                elif isinstance(value_type, KsfFloatType):
+                    if value_type.bit == 32:
+                        return '0.0f'
+                    else:
+                        return '0.0'
+                elif isinstance(value_type, KsfBoolType):
                     return 'true'
-                elif value_type.name == 'string':
+                elif isinstance(value_type, KsfStringType):
                     return '""'
                 else:
                     return None
 
             # 特殊处理一下bool型
             if default['is_bool']:
                 return f'{"true" if default["value"] else "false"}'
@@ -307,24 +322,38 @@
                 return f'{default["value"]}'
             else:
                 return f'"{default["value"]}"'
 
         default_var = parse_default_var(ksf_var.value_type, ksf_var.default)
         comment = self.parse_comment_line(ksf_var.comment)
 
-        return comment, self.parse_type(curr_module,
-                                        ksf_var.value_type), ksf_var.name, f' = {default_var};' if default_var is not None else ';'
+        return comment, self.parse_type(ksf_var.value_type
+                                        ), ksf_var.name, f' = {default_var};' if default_var is not None else ';'
 
     def add_lines(self, lines, tab=0):
-        space = ' ' * (4 * tab)
+        if isinstance(lines, str):
+            lines = lines.split('\n')
+        elif isinstance(lines, (list, tuple, set)):
+            return '\n'.join(self.add_lines(line, tab) for line in lines)
+        else:
+            raise TypeError(f"不支持的类型{type(lines)}")
 
-        return f"\n".join(space + line for line in lines.split("\n")) + self.endl()
+        space = ' ' * (4 * tab)
+        return f"\n".join(space + line for line in lines)
 
 
-def create_parser(files, repl_ns_dict, repl_inc_dir, include_dirs, destination_dir, push_functions, export_symbols, flags=None):
+def create_parser(files,
+                  repl_ns_dict,
+                  repl_inc_dir,
+                  include_dirs,
+                  destination_dir,
+                  push_functions,
+                  export_symbols,
+                  flags=None
+                  ):
     if flags is None:
         flags = defaultdict(bool)
 
     file_path = files
 
     real_inc_dirs = set()
     for inc in include_dirs:
@@ -349,10 +378,18 @@
 
     export_symbols = {}
 
     sdk_invoke = {}
 
     sdk_export = {}
 
-    parser = create_parser(file_path, {}, {}, include_dirs, destination_dir, push_functions, export_symbols, flags={'with_current_priority': True})
+    parser = create_parser(file_path,
+                           {},
+                           {},
+                           include_dirs,
+                           destination_dir,
+                           push_functions,
+                           export_symbols,
+                           flags={'with_current_priority': True}
+                           )
 
     parser.parse_variable(parser.ast.modules[0], parser.ast.modules[0].fields[0])
```

### Comparing `ksfctl-0.2.1/ksfctl/parser/ksf_lex.py` & `ksfctl-0.2.3/ksfctl/parser/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         'UNSIGNED',
 
         # 字段模式
         "REQUIRED",
         "OPTIONAL",
 
         # 基本类型
+        'VOID',
         'INT',
         'LONG',
         'FLOAT',
         'DOUBLE',
         'SHORT',
         'BOOL',
         'CHAR',
@@ -134,14 +135,15 @@
             "out": "OUTPUT",
             "const": "CONST",
             "false": "FALSE",
             "true": "TRUE",
             "using": "USING",
             "import": "IMPORT",
             "export": "EXPORT",
+            "void": "VOID",
         }.get(t.value, "IDENTIFIER")
         return t
 
     # 定义字符串
     def t_STRING_CONSTANT(self, t):
         r""""[^"]*\""""
         t.value = t.value[1:-1]
```

### Comparing `ksfctl-0.2.1/ksfctl/parser/ksf_yacc.py` & `ksfctl-0.2.3/ksfctl/parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import warnings
 
 import ply.yacc as yacc
 
-from ksfctl.parser.ksf_lex import KsfLexer
-from ksfctl.parser.ksf_parser import *
+from ksfctl.parser.token import KsfLexer
+from ksfctl.parser.ksf import *
 from ksfctl.parser.tools import *
 
 
 class KsfParser:
     def __init__(self):
         # 解析语法的准备
         self.lexer = KsfLexer()
@@ -462,21 +462,32 @@
         p[0] = {
             'element': 'type',
             'type': 'array',
             'name': 'array<' + p[1]['name'] + '>',
             'value_type': p[1],
         }
 
+    def p_void_typ(self, p):
+        """
+        void_type : VOID
+        """
+        p[0] = {
+            'element': 'type',
+            'type': 'void',
+            'name': 'void',
+        }
+
     def p_type(self, p):
         """
         type : primitive_type
              | vector_type
              | map_type
              | array_type
              | struct_type
+             | void_type
         """
         p[0] = p[1]
 
     ######## 值定义 ########
     def p_number_value(self, p):
         """
         number_value : EXPR_CONSTANT
@@ -562,27 +573,28 @@
                         'is_required': p[2],
                         'value_type': p[3],
                         'name': p[4],
                         'default': p[6],
                         'comment': p[8]}
 
         # 特殊处理一下bool类型
-        if 'default' in variable and variable['value_type']['name'] == 'bool':
-            variable['default']['is_number'] = False
-            variable['default']['is_bool'] = True
-            if variable['default']['value'] == '1':
-                variable['default']['value'] = True
-            elif variable['default']['value'] == '0':
-                variable['default']['value'] = False
-            elif variable['default']['value'] == 'true':
-                variable['default']['value'] = True
-            elif variable['default']['value'] == 'false':
-                variable['default']['value'] = False
-            else:
-                raise SyntaxError(f'不支持的布尔默认值[{p[6]}]，请检查')
+        if 'default' in variable:
+            if variable['value_type']['name'] == 'bool':
+                variable['default']['is_number'] = False
+                variable['default']['is_bool'] = True
+                if variable['default']['value'] == '1':
+                    variable['default']['value'] = True
+                elif variable['default']['value'] == '0':
+                    variable['default']['value'] = False
+                elif variable['default']['value'] == 'true':
+                    variable['default']['value'] = True
+                elif variable['default']['value'] == 'false':
+                    variable['default']['value'] = False
+                else:
+                    raise SyntaxError(f'不支持的布尔默认值[{p[6]}]，请检查')
 
         p[0] = variable
 
     def p_key_params(self, p):
         """
         key_params : IDENTIFIER
                    | key_params COMMA IDENTIFIER
@@ -598,15 +610,14 @@
         """
         pass
 
     def p_error(self, p):
         if p:
             if p.type in {'COMMENT_MULTILINE', 'COMMENT_LINE'}:
                 self.parser.errok()
-                # print(f"Syntax error at token {p.type} ({p.value}), line {KsfLexer.find_position(p.lexer.lexdata, p.lexer)}")
                 return
             else:
                 raise SyntaxError(
                     f"Syntax error at token {p.type} ({p.value}), line {KsfLexer.find_position(p.lexer.lexdata, p.lexer)}")
         else:
             SyntaxError("Syntax error at EOF")
 
@@ -897,20 +908,20 @@
 
     return None
 
 
 def generate(files, search_dirs: set, with_curr_dir_first: bool, export_symbols):
     parser_grammar = {}
 
-    def parse_depends(file):
+    def parse_depends(file, is_source=False):
         file = find_file(file, search_dirs, with_curr_dir_first)
         if file is None:
             raise FileNotFoundError(f"文件[{file}]没有找到")
 
-        Ksf.add_file(file)
+        Ksf.add_file(file, is_source)
 
         # 创建语法分析器
         parser = KsfParser()
         if file not in parser_grammar:
             with file.open() as f:
                 curr_file_grammar = parser.parse(f.read())
                 parser_grammar[file.name] = curr_file_grammar
@@ -927,18 +938,17 @@
 
                         Ksf.add_include(file, inc_path, include)
 
                         if str(Path(inc_path).name) not in parser_grammar:
                             parse_depends(inc_path)
 
     for file in files:
-        parse_depends(file)
+        parse_depends(file, is_source=True)
 
     # print(parser_grammar.keys())
-
     generate_ksf_ast(parser_grammar, export_symbols)
     return Ksf
 
 
 # 测试用例
 if __name__ == '__main__':
```

### Comparing `ksfctl-0.2.1/ksfctl/parser/tools.py` & `ksfctl-0.2.3/ksfctl/parser/tools.py`

 * *Files identical despite different names*

### Comparing `ksfctl-0.2.1/ksfctl.egg-info/SOURCES.txt` & `ksfctl-0.2.3/ksfctl.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+LICENSE
 README.md
 setup.py
 ksfctl/__init__.py
 ksfctl.egg-info/PKG-INFO
 ksfctl.egg-info/SOURCES.txt
 ksfctl.egg-info/dependency_links.txt
 ksfctl.egg-info/entry_points.txt
 ksfctl.egg-info/requires.txt
 ksfctl.egg-info/top_level.txt
 ksfctl/cmd/__init__.py
 ksfctl/cmd/cmd.py
+ksfctl/cmd/options.py
 ksfctl/generate/__init__.py
 ksfctl/generate/cpp/__init__.py
 ksfctl/generate/cpp/generator.py
 ksfctl/generate/cpp/parser.py
-ksfctl/generate/cpp/orm/__init__.py
-ksfctl/generate/cpp/orm/clickhouse.py
-ksfctl/generate/cpp/orm/generator.py
-ksfctl/generate/cpp/orm/mysql.py
-ksfctl/generate/cpp/orm/parser.py
-ksfctl/generate/cpp/orm/sqlite.py
+ksfctl/generate/cpp/template.py
+ksfctl/generate/ksf/__init__.py
+ksfctl/generate/ksf/generator.py
+ksfctl/generate/ksf/parser.py
 ksfctl/parser/__init__.py
-ksfctl/parser/ksf_lex.py
-ksfctl/parser/ksf_parser.py
-ksfctl/parser/ksf_yacc.py
+ksfctl/parser/ksf.py
+ksfctl/parser/parser.py
+ksfctl/parser/token.py
 ksfctl/parser/tools.py
```

### Comparing `ksfctl-0.2.1/setup.py` & `ksfctl-0.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ksfctl',
-    version='0.2.1',
+    version='0.2.3',
     keywords='ksf, client, generator, tool',
     description='a auto generator tools for ksf protocol files, and some useful tools',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         'ksfctl': ['parser/parser.out'],
     },
@@ -14,10 +14,11 @@
         'Click>=8.0.0',
         'ply>=3.0.0',
         'pyyaml>=5.4.1',
     ],
     entry_points='''
         [console_scripts]
         ksfctl=ksfctl.cmd.cmd:cli
-        ksf2cpp=ksfctl.cmd.cmd:parse_cpp
+        ksf2cpp=ksfctl.cmd.cmd:parse_cxx
+        ksf2cxx=ksfctl.cmd.cmd:parse_cxx
     ''',
 )
```

