# Comparing `tmp/microkanren-0.3.0.tar.gz` & `tmp/microkanren-0.4.0.tar.gz`

## Comparing `microkanren-0.3.0.tar` & `microkanren-0.4.0.tar`

### file list

```diff
@@ -1,132 +1,140 @@
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 microkanren-0.3.0/.dir-locals.el
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 microkanren-0.3.0/.flake8
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 microkanren-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 microkanren-0.3.0/eqstats
--rw-r--r--   0        0        0    24114 2020-02-02 00:00:00.000000 microkanren-0.3.0/lambdastats
--rw-r--r--   0        0        0   108899 2020-02-02 00:00:00.000000 microkanren-0.3.0/pyrsistent-0.19.3-cp311-cp311-linux_x86_64.whl
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/12b2473498b257a5
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/12d5c5076e7d661a
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/1a3971a8088378fa
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/1ac35766268534af
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/1ba464f4c461a443
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/1db7621172052592
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/219203f970303938
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/2221493465c4b87c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/243fc0a435fe8f24
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/25656f03f40dcde
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/25a8329fc375eaac
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/25ac391031dd7c74
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/28366a523c2300fd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/2ea134d4cabb0ac8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/33b0347acbfe4163
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/366e123530c9524
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/373241c8743e947e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/374bbc681e8f1ee5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3b292f2356fbe91c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3d08eaa4c0663b06
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3da6c59c12991cbb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3f4396daed32427
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3f9291a0c909e64
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/3fc0f873b0fec10f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/46a84ef7a4c12eaa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/47d34b5487e1022f
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/48d7c5a897f27f49
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/49807e9e41e0b2a1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/4ab853408bf4916a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/4ba429114b57df44
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/4dc4c5f638d543a4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/4f110938ecd8bb76
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/502609f0ad43ade4
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/50657b35c5c172b4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/526a985106bd7b39
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5361b343dc6e7004
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5605e5849372f227
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5a75c3340a4cd45e
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5c1634ffc9b61f89
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5c3ef838607d0ee6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5cd7fb71b6f2c48f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5d7f57c24d828a26
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/5fa638bed8d56fff
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/6055ed0423c9a8b8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/624bb3c1d125bc54
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/67187c816079efa4
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/67b5173fb3386e82
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/6922fb0aa8d4c0c9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/6dd791724c3e1488
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/71543a4e69af6bc4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/748abe5b3f808eae
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/7624bbf3fea25119
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/765d8af091e9b4d8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/7a4a1940926d293f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/7cf868287e752f7d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/7d36ce32b4f6711e
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/7dfad8bf24d12528
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/851365d30f59e319
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/853a33a5ce08b754
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/854565afaee83f71
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/87e3ca4168ccaadf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/89b01049b2d1276b
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/89b43b5f4dedf5b3
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/8a5b4c99aa1ab2d9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/8c43736823982fd7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/8d5565da6200359c
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/9576ec1ba4f157e1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/9701ba061431517a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/990796e76d4d0614
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/99790a41b39e7c16
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/9ca2234c1578fc42
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/9e3acf28b1ccb741
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/9f438292f325350a
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/a156cdb409b56217
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/a1d60687ae98bfdf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/a23d92b739778f3b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/a6f301fad936dd8f
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/a8865d2ebb297bd8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/acb49a39c8a7a7cf
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/ad3088309877b0ca
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/adf8bdbca0957709
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/ae46c6398f715f02
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/b1f7beb124810ce9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/b5bfa3cb56426832
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/b5e3aa96b9c3b299
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/b5f4a66125330968
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/b867605c7e0fa821
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/bc1ae9ffd6f8fe46
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/c11ec8839ed17196
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/c2c13b7ef1746d68
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/c329f98e76946bbc
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/c99eaab4de8198ec
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/cd51bf2f97b44d00
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/d2a2f01d5f84bc18
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/d2b0d38843ee4213
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/d87db07b1718fea9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/d975526c6a6286f7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/da5966ee78c9b514
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/ddc3f3c3e6f84c92
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/de1cd4657a693176
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/df8d6288e2a15497
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/e06a399e832adab1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/e2158c003835f1fc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/e4afce302a4a3f5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/e8f138dfce2dce04
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/e99b79fb0295b34c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/eae6a6608bcaf8f1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/f44fcef21f89bda
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/f5c966baff1008b8
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 microkanren-0.3.0/.ruff_cache/content/fec3c4b9409ef258
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 microkanren-0.3.0/src/microkanren/__init__.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 microkanren-0.3.0/src/microkanren/cons.py
--rw-r--r--   0        0        0    27492 2020-02-02 00:00:00.000000 microkanren-0.3.0/src/microkanren/core.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 microkanren-0.3.0/src/microkanren/goals.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 microkanren-0.3.0/src/microkanren/utils.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 microkanren-0.3.0/tests/test_ast.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 microkanren-0.3.0/tests/test_core.py
--rw-r--r--   0        0        0     7826 2020-02-02 00:00:00.000000 microkanren-0.3.0/tests/test_fd.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 microkanren-0.3.0/tests/test_lambda.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 microkanren-0.3.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 microkanren-0.3.0/LICENSE
--rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 microkanren-0.3.0/README.md
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 microkanren-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 microkanren-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ccls
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 microkanren-0.4.0/.clang-format
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 microkanren-0.4.0/.dir-locals.el
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 microkanren-0.4.0/.flake8
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 microkanren-0.4.0/.gdb_history
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 microkanren-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 microkanren-0.4.0/eqstats
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 microkanren-0.4.0/krivino.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 microkanren-0.4.0/krivinofd.py
+-rw-r--r--   0        0        0    24114 2020-02-02 00:00:00.000000 microkanren-0.4.0/lambdastats
+-rw-r--r--   0        0        0   108899 2020-02-02 00:00:00.000000 microkanren-0.4.0/pyrsistent-0.19.3-cp311-cp311-linux_x86_64.whl
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 microkanren-0.4.0/setup.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/12b2473498b257a5
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/12d5c5076e7d661a
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/1a3971a8088378fa
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/1ac35766268534af
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/1ba464f4c461a443
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/1db7621172052592
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/219203f970303938
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/2221493465c4b87c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/243fc0a435fe8f24
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/25656f03f40dcde
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/25a8329fc375eaac
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/25ac391031dd7c74
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/28366a523c2300fd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/2ea134d4cabb0ac8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/33b0347acbfe4163
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/366e123530c9524
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/373241c8743e947e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/374bbc681e8f1ee5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/3b292f2356fbe91c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/3d08eaa4c0663b06
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/3da6c59c12991cbb
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/3f4396daed32427
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/3f9291a0c909e64
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/3fc0f873b0fec10f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/46a84ef7a4c12eaa
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/47d34b5487e1022f
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/48d7c5a897f27f49
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/49807e9e41e0b2a1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/4ab853408bf4916a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/4ba429114b57df44
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/4dc4c5f638d543a4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/4f110938ecd8bb76
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/502609f0ad43ade4
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/50657b35c5c172b4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/526a985106bd7b39
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/5361b343dc6e7004
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/5605e5849372f227
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/5a75c3340a4cd45e
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/5c1634ffc9b61f89
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/5c3ef838607d0ee6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/5cd7fb71b6f2c48f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/5d7f57c24d828a26
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/5fa638bed8d56fff
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/6055ed0423c9a8b8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/624bb3c1d125bc54
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/67187c816079efa4
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/67b5173fb3386e82
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/6922fb0aa8d4c0c9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/6dd791724c3e1488
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/71543a4e69af6bc4
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/748abe5b3f808eae
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/7624bbf3fea25119
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/765d8af091e9b4d8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/7a4a1940926d293f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/7cf868287e752f7d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/7d36ce32b4f6711e
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/7dfad8bf24d12528
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/851365d30f59e319
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/853a33a5ce08b754
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/854565afaee83f71
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/87e3ca4168ccaadf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/89b01049b2d1276b
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/89b43b5f4dedf5b3
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/8a5b4c99aa1ab2d9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/8c43736823982fd7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/8d5565da6200359c
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/9576ec1ba4f157e1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/9701ba061431517a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/990796e76d4d0614
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/99790a41b39e7c16
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/9ca2234c1578fc42
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/9e3acf28b1ccb741
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/9f438292f325350a
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/a156cdb409b56217
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/a1d60687ae98bfdf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/a23d92b739778f3b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/a6f301fad936dd8f
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/a8865d2ebb297bd8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/acb49a39c8a7a7cf
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/ad3088309877b0ca
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/adf8bdbca0957709
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/ae46c6398f715f02
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/b1f7beb124810ce9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/b5bfa3cb56426832
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/b5e3aa96b9c3b299
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/b5f4a66125330968
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/b867605c7e0fa821
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/bc1ae9ffd6f8fe46
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/c11ec8839ed17196
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/c2c13b7ef1746d68
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/c329f98e76946bbc
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/c99eaab4de8198ec
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/cd51bf2f97b44d00
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/d2a2f01d5f84bc18
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/d2b0d38843ee4213
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/d87db07b1718fea9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/d975526c6a6286f7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/da5966ee78c9b514
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/ddc3f3c3e6f84c92
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/de1cd4657a693176
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/df8d6288e2a15497
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/e06a399e832adab1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/e2158c003835f1fc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/e4afce302a4a3f5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/e8f138dfce2dce04
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/e99b79fb0295b34c
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/eae6a6608bcaf8f1
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/f44fcef21f89bda
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/f5c966baff1008b8
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 microkanren-0.4.0/.ruff_cache/content/fec3c4b9409ef258
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 microkanren-0.4.0/src/microkanren/__init__.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 microkanren-0.4.0/src/microkanren/cons.py
+-rw-r--r--   0        0        0    17006 2020-02-02 00:00:00.000000 microkanren-0.4.0/src/microkanren/core.py
+-rw-r--r--   0        0        0    10851 2020-02-02 00:00:00.000000 microkanren-0.4.0/src/microkanren/fd.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 microkanren-0.4.0/src/microkanren/goals.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 microkanren-0.4.0/src/microkanren/utils.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 microkanren-0.4.0/tests/test_ast.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 microkanren-0.4.0/tests/test_core.py
+-rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 microkanren-0.4.0/tests/test_fd.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 microkanren-0.4.0/tests/test_lambda.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microkanren-0.4.0/tests/test_substitution.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 microkanren-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 microkanren-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5979 2020-02-02 00:00:00.000000 microkanren-0.4.0/README.md
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 microkanren-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8266 2020-02-02 00:00:00.000000 microkanren-0.4.0/PKG-INFO
```

### Comparing `microkanren-0.3.0/eqstats` & `microkanren-0.4.0/eqstats`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/lambdastats` & `microkanren-0.4.0/lambdastats`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/pyrsistent-0.19.3-cp311-cp311-linux_x86_64.whl` & `microkanren-0.4.0/pyrsistent-0.19.3-cp311-cp311-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/48d7c5a897f27f49` & `microkanren-0.4.0/.ruff_cache/content/48d7c5a897f27f49`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/4dc4c5f638d543a4` & `microkanren-0.4.0/.ruff_cache/content/4dc4c5f638d543a4`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/5605e5849372f227` & `microkanren-0.4.0/.ruff_cache/content/5605e5849372f227`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/5c1634ffc9b61f89` & `microkanren-0.4.0/.ruff_cache/content/5c1634ffc9b61f89`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/67b5173fb3386e82` & `microkanren-0.4.0/.ruff_cache/content/67b5173fb3386e82`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/7dfad8bf24d12528` & `microkanren-0.4.0/.ruff_cache/content/7dfad8bf24d12528`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/854565afaee83f71` & `microkanren-0.4.0/.ruff_cache/content/854565afaee83f71`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/8a5b4c99aa1ab2d9` & `microkanren-0.4.0/.ruff_cache/content/8a5b4c99aa1ab2d9`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/9576ec1ba4f157e1` & `microkanren-0.4.0/.ruff_cache/content/9576ec1ba4f157e1`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/99790a41b39e7c16` & `microkanren-0.4.0/.ruff_cache/content/99790a41b39e7c16`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/a1d60687ae98bfdf` & `microkanren-0.4.0/.ruff_cache/content/a1d60687ae98bfdf`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/a8865d2ebb297bd8` & `microkanren-0.4.0/.ruff_cache/content/a8865d2ebb297bd8`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/ad3088309877b0ca` & `microkanren-0.4.0/.ruff_cache/content/ad3088309877b0ca`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/adf8bdbca0957709` & `microkanren-0.4.0/.ruff_cache/content/adf8bdbca0957709`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/c11ec8839ed17196` & `microkanren-0.4.0/.ruff_cache/content/c11ec8839ed17196`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/d87db07b1718fea9` & `microkanren-0.4.0/.ruff_cache/content/d87db07b1718fea9`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/df8d6288e2a15497` & `microkanren-0.4.0/.ruff_cache/content/df8d6288e2a15497`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.ruff_cache/content/f5c966baff1008b8` & `microkanren-0.4.0/.ruff_cache/content/f5c966baff1008b8`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/tests/test_core.py` & `microkanren-0.4.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/tests/test_fd.py` & `microkanren-0.4.0/tests/test_fd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from itertools import permutations
 from math import sqrt
 
 import pytest
 
 from microkanren import (
     Hooks,
-    alldifffd,
     compose_constraints,
     conj,
     default_enforce_constraints,
     default_process_prefix,
-    domfd,
-    enforce_constraints_fd,
     enforce_constraints_neq,
     eq,
     freshn,
+    neq,
+    process_prefix_neq,
+    run,
+    run_all,
+)
+from microkanren.fd import (
+    alldifffd,
+    domfd,
+    enforce_constraints_fd,
     infd,
     ltefd,
+    ltfd,
     make_domain,
     mkrange,
-    neq,
     neqfd,
     plusfd,
     process_prefix_fd,
-    process_prefix_neq,
-    run,
-    run_all,
 )
 
 
 @pytest.fixture(autouse=True, scope="module")
 def setup_process_prefix():
     def process_prefix(prefix, constraints):
         return compose_constraints(
@@ -87,30 +90,46 @@
     )
     def test_ltefd(self, a, b, expected_x):
         result = run_all(lambda x, y: domfd(x, a) & domfd(y, b) & ltefd(x, y))
         assert {x[0] for x in result} == expected_x
         for x, y in result:
             assert x <= y
 
+    @pytest.mark.parametrize(
+        ("a", "b", "expected_x"),
+        [
+            (make_domain(1, 2, 3, 4), make_domain(2, 3), make_domain(1, 2)),
+            (make_domain(1, 2, 3), make_domain(4, 5), make_domain(1, 2, 3)),
+            (make_domain(4, 5), make_domain(1, 2), make_domain()),
+            (make_domain(3, 4), make_domain(2, 3, 4, 5), make_domain(3, 4)),
+            (make_domain(1, 2, 3, 4), make_domain(1, 2, 3, 4), make_domain(1, 2, 3)),
+        ],
+    )
+    def test_ltfd(self, a, b, expected_x):
+        result = run_all(lambda x, y: domfd(x, a) & domfd(y, b) & ltfd(x, y))
+        assert {x[0] for x in result} == expected_x
+        for x, y in result:
+            assert x < y
+
     def test_neq_with_domfd(self):
         """
         If neq(x, n), then n cannot be in the domain of x.
         """
-        result = run_all(lambda x: domfd(x, make_domain(1, 2, 3)) & neq((x, 2)))
+        result = run_all(lambda x: domfd(x, make_domain(1, 2, 3)) & neq(x, 2))
         assert set(result) == {1, 3}
 
     def test_neq_with_ltefd(self):
         """
         If neq(x, n), then n cannot be in the domain of x.
         """
         result = run_all(
             lambda x, y: domfd(x, make_domain(1, 2, 3))
             & domfd(y, make_domain(1, 2))
             & ltefd(x, y)
-            & neq((x, 1))
+            & neq(x, 1)
         )
         assert result == [(2, 2)]
 
     def test_plusfd(self):
         result = run_all(
             lambda x, y, z: domfd(x, mkrange(1, 3))
             & domfd(y, mkrange(1, 3))
```

### Comparing `microkanren-0.3.0/tests/test_lambda.py` & `microkanren-0.4.0/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/.gitignore` & `microkanren-0.4.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -128,7 +128,8 @@
 # Pyre type checker
 .pyre/
 
 prof
 
 profiling.py
 sudoku.py
+.ccls-cache
```

### Comparing `microkanren-0.3.0/LICENSE` & `microkanren-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/README.md` & `microkanren-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `microkanren-0.3.0/pyproject.toml` & `microkanren-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "microkanren"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
     { name="Joshua Munn", email="public@elysee-munn.family" },
 ]
 description = "A Python implementation of microkanren extended with constraints"
 readme = "README.md"
 requires-python = "~=3.11"
 classifiers = [
@@ -12,28 +12,30 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 2 - Pre-Alpha",
 ]
 dependencies = [
     "pyrsistent ~= 0.19",
-    "fastcons ~= 0.2.0",
+    "fastcons ~= 0.3.0",
+    "immutables ~= 0.19",
 ]
 license = {file = "LICENSE"}
 
 [project.urls]
 "Homepage" = "https://github.com/jams2/microkanren"
 "Bug Tracker" = "https://github.com/jams2/microkanren/issues"
 
 [project.optional-dependencies]
 dev = [
     "black ~= 23.1.0",
     "ruff ~= 0.0.256",
 ]
 testing = ["pytest ~= 7.2.2", "pytest-profiling ~= 1.7.0"]
+build = ["hatch ~= 1.7.0"]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
```

### Comparing `microkanren-0.3.0/PKG-INFO` & `microkanren-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microkanren
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python implementation of microkanren extended with constraints
 Project-URL: Homepage, https://github.com/jams2/microkanren
 Project-URL: Bug Tracker, https://github.com/jams2/microkanren/issues
 Author-email: Joshua Munn <public@elysee-munn.family>
 License: MIT License
         
         Copyright (c) 2023 Joshua Munn
@@ -29,16 +29,19 @@
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: ~=3.11
-Requires-Dist: fastcons~=0.2.0
+Requires-Dist: fastcons~=0.3.0
+Requires-Dist: immutables~=0.19
 Requires-Dist: pyrsistent~=0.19
+Provides-Extra: build
+Requires-Dist: hatch~=1.7.0; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: black~=23.1.0; extra == 'dev'
 Requires-Dist: ruff~=0.0.256; extra == 'dev'
 Provides-Extra: testing
 Requires-Dist: pytest-profiling~=1.7.0; extra == 'testing'
 Requires-Dist: pytest~=7.2.2; extra == 'testing'
 Description-Content-Type: text/markdown
```

