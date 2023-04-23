# Comparing `tmp/txapi-1.0.1.tar.gz` & `tmp/txapi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txapi-1.0.1.tar", last modified: Sun Apr 23 05:15:52 2023, max compression
+gzip compressed data, was "txapi-1.0.2.tar", last modified: Sun Apr 23 05:17:52 2023, max compression
```

## Comparing `txapi-1.0.1.tar` & `txapi-1.0.2.tar`

### file list

```diff
@@ -1,1134 +1,1138 @@
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.496486 txapi-1.0.1/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.897711 txapi-1.0.1/.git/
--rw-r--r--   0 linkerui   (501) staff       (20)       40 2023-04-23 05:13:30.000000 txapi-1.0.1/.git/COMMIT_EDITMSG
--rw-r--r--   0 linkerui   (501) staff       (20)      198 2023-04-23 04:55:42.000000 txapi-1.0.1/.git/FETCH_HEAD
--rw-r--r--   0 linkerui   (501) staff       (20)       21 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/HEAD
--rw-r--r--   0 linkerui   (501) staff       (20)       41 2022-11-25 05:52:32.000000 txapi-1.0.1/.git/ORIG_HEAD
--rw-r--r--   0 linkerui   (501) staff       (20)      303 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/config
--rw-r--r--   0 linkerui   (501) staff       (20)       73 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/description
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.904181 txapi-1.0.1/.git/hooks/
--rwxr-xr-x   0 linkerui   (501) staff       (20)      478 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)      896 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)     4655 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)      189 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/post-update.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)      424 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)     1643 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)      416 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)     1374 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/pre-push.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)     4898 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)      544 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)     1492 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)     2783 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 linkerui   (501) staff       (20)     3650 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/hooks/update.sample
--rw-r--r--   0 linkerui   (501) staff       (20)     4228 2023-04-23 05:13:30.000000 txapi-1.0.1/.git/index
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.904602 txapi-1.0.1/.git/info/
--rw-r--r--   0 linkerui   (501) staff       (20)      240 2022-11-22 04:39:00.000000 txapi-1.0.1/.git/info/exclude
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.905008 txapi-1.0.1/.git/logs/
--rw-r--r--   0 linkerui   (501) staff       (20)     1549 2023-04-23 05:13:30.000000 txapi-1.0.1/.git/logs/HEAD
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.841116 txapi-1.0.1/.git/logs/refs/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.905571 txapi-1.0.1/.git/logs/refs/heads/
--rw-r--r--   0 linkerui   (501) staff       (20)     1549 2023-04-23 05:13:30.000000 txapi-1.0.1/.git/logs/refs/heads/main
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.841232 txapi-1.0.1/.git/logs/refs/remotes/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.907068 txapi-1.0.1/.git/logs/refs/remotes/origin/
--rw-r--r--   0 linkerui   (501) staff       (20)      181 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0 linkerui   (501) staff       (20)     1032 2023-04-23 05:13:34.000000 txapi-1.0.1/.git/logs/refs/remotes/origin/main
--rw-r--r--   0 linkerui   (501) staff       (20)      151 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/logs/refs/remotes/origin/py2
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.863137 txapi-1.0.1/.git/objects/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.908259 txapi-1.0.1/.git/objects/05/
--r--r--r--   0 linkerui   (501) staff       (20)       52 2022-11-25 05:42:01.000000 txapi-1.0.1/.git/objects/05/693212a885904ca6a4c4438425d7bc57699092
--r--r--r--   0 linkerui   (501) staff       (20)       73 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/05/7b61b6790d72490e44d5844499747c0e58cda5
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.908648 txapi-1.0.1/.git/objects/07/
--r--r--r--   0 linkerui   (501) staff       (20)      162 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/07/97267a4911e4d2e38af27bba3114850a9cfaed
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.910267 txapi-1.0.1/.git/objects/08/
--r--r--r--   0 linkerui   (501) staff       (20)       51 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/08/2b9381253bc157a355806bc4a2ac9070c72cce
--r--r--r--   0 linkerui   (501) staff       (20)      285 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/08/35cd488581c2ca89e8cce1292218a8c66268e3
--r--r--r--   0 linkerui   (501) staff       (20)      208 2023-04-10 09:59:52.000000 txapi-1.0.1/.git/objects/08/c677658838ab6c0c247c140a3b62bdba60c531
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.911482 txapi-1.0.1/.git/objects/0d/
--r--r--r--   0 linkerui   (501) staff       (20)     1424 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/0d/db97d0b98ea46065d50f4c8b40363d97fbc843
--r--r--r--   0 linkerui   (501) staff       (20)      101 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/0d/e79dff12acb51fbc10df4bed8167d9e8abddff
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.912359 txapi-1.0.1/.git/objects/0e/
--r--r--r--   0 linkerui   (501) staff       (20)       85 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/0e/01571976474ceb8feae36a62d5effb8c04d73f
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.913047 txapi-1.0.1/.git/objects/0f/
--r--r--r--   0 linkerui   (501) staff       (20)      366 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/0f/77e05fc0dfc799199f7f199d50a642fba481be
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.913707 txapi-1.0.1/.git/objects/11/
--r--r--r--   0 linkerui   (501) staff       (20)      719 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/11/1e278133b448d8badadfd73e711d439c6b9abb
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.914338 txapi-1.0.1/.git/objects/12/
--r--r--r--   0 linkerui   (501) staff       (20)      281 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/12/bd257f54fd5a04d5ee924d7a98780694f99d6c
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.915171 txapi-1.0.1/.git/objects/18/
--r--r--r--   0 linkerui   (501) staff       (20)      118 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/18/8aefec4047a9000cb081850bd7c9b201a9aa96
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.916049 txapi-1.0.1/.git/objects/19/
--r--r--r--   0 linkerui   (501) staff       (20)      553 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/19/d1b4f52378f26d4f82a9356b8ede80dcd54eb7
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.916684 txapi-1.0.1/.git/objects/1f/
--r--r--r--   0 linkerui   (501) staff       (20)      285 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/1f/0cff2a4593a484a6e3549a2f4883d3a18d73bc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.917372 txapi-1.0.1/.git/objects/20/
--r--r--r--   0 linkerui   (501) staff       (20)      286 2023-04-23 05:13:30.000000 txapi-1.0.1/.git/objects/20/2fe90f5cee5dacf2f361d7ac488e227d34bc7b
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.919971 txapi-1.0.1/.git/objects/21/
--r--r--r--   0 linkerui   (501) staff       (20)      669 2023-04-10 09:59:52.000000 txapi-1.0.1/.git/objects/21/4c2ea36d2dde3af8296cb4037fb93734b56166
--r--r--r--   0 linkerui   (501) staff       (20)      684 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/21/639dd781776e03375cd81804372559ba2e9bf9
--r--r--r--   0 linkerui   (501) staff       (20)      253 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/21/a4f28d9a5ad8f6e09a92c16b3034cc980717a0
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.922534 txapi-1.0.1/.git/objects/23/
--r--r--r--   0 linkerui   (501) staff       (20)       88 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/23/1286de323c67ae267b9b0957802e8112f8de97
--r--r--r--   0 linkerui   (501) staff       (20)      556 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/23/398032b1b9804ab0dcba15248c71bb418737da
--r--r--r--   0 linkerui   (501) staff       (20)      576 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/23/f661515e73b2b19d9af88e6bab4a169c46406e
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.923351 txapi-1.0.1/.git/objects/25/
--r--r--r--   0 linkerui   (501) staff       (20)      123 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/25/ce766604a031638b2a1986140b7d5b94a01183
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.923927 txapi-1.0.1/.git/objects/26/
--r--r--r--   0 linkerui   (501) staff       (20)      154 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/26/5dbfd4abbbe3deed4bfa548d10e5a0f2de2c7b
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.924682 txapi-1.0.1/.git/objects/2c/
--r--r--r--   0 linkerui   (501) staff       (20)     1638 2023-04-23 04:56:44.000000 txapi-1.0.1/.git/objects/2c/c1a52cf5b91e50837f92540fa79b66bdbb7181
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.925398 txapi-1.0.1/.git/objects/2d/
--r--r--r--   0 linkerui   (501) staff       (20)      180 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/2d/1924ef05bb89db7392ff247c87c00e8831068d
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.927076 txapi-1.0.1/.git/objects/2e/
--r--r--r--   0 linkerui   (501) staff       (20)      343 2022-11-25 05:41:53.000000 txapi-1.0.1/.git/objects/2e/0d531f1af3317d56f2b066f9c214d6384cec11
--r--r--r--   0 linkerui   (501) staff       (20)      124 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/2e/194e7ad8ae57ce0ec200288e5a81eefc99573c
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.927760 txapi-1.0.1/.git/objects/2f/
--r--r--r--   0 linkerui   (501) staff       (20)       94 2023-04-10 09:59:52.000000 txapi-1.0.1/.git/objects/2f/53647fc1a53eadc41031f3844a13742be2125d
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.928630 txapi-1.0.1/.git/objects/30/
--r--r--r--   0 linkerui   (501) staff       (20)      155 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/30/81b0e572b95da26032f088f543cdd98c76abe3
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.929277 txapi-1.0.1/.git/objects/31/
--r--r--r--   0 linkerui   (501) staff       (20)      555 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/31/4296ca74424b305d04be227ad964afb86bf921
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.930292 txapi-1.0.1/.git/objects/32/
--r--r--r--   0 linkerui   (501) staff       (20)     3750 2023-04-23 04:56:44.000000 txapi-1.0.1/.git/objects/32/8a62420ab81f87039d73e6ae31e5b1b54d3bde
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.931041 txapi-1.0.1/.git/objects/33/
--r--r--r--   0 linkerui   (501) staff       (20)       89 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/33/bddaaaa0c46e95be3d138f52f31b60a7136b48
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.932432 txapi-1.0.1/.git/objects/34/
--r--r--r--   0 linkerui   (501) staff       (20)      129 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/34/48bd09b982b355c07252c2f64c88601f40aa2c
--r--r--r--   0 linkerui   (501) staff       (20)       37 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/34/4d17d14b8784e146028da8a18b21dad1c1bda3
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.933268 txapi-1.0.1/.git/objects/37/
--r--r--r--   0 linkerui   (501) staff       (20)      321 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/37/36cb67cb324ab7d27524b9579c3e6a417fc06c
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.934092 txapi-1.0.1/.git/objects/39/
--r--r--r--   0 linkerui   (501) staff       (20)       69 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/39/f3953903273862db7c100c5223913e413dca60
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.935931 txapi-1.0.1/.git/objects/3e/
--r--r--r--   0 linkerui   (501) staff       (20)      155 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/3e/5c111da00b1d6a2c4201572795a4b068ec9c9f
--r--r--r--   0 linkerui   (501) staff       (20)      112 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/3e/e7ef9c853280632b3a27c9599b5a842a0b1967
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.936687 txapi-1.0.1/.git/objects/3f/
--r--r--r--   0 linkerui   (501) staff       (20)     1506 2022-11-25 05:41:53.000000 txapi-1.0.1/.git/objects/3f/03a1b9319f3c3d9941d7ae256b81e045b42363
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.937593 txapi-1.0.1/.git/objects/40/
--r--r--r--   0 linkerui   (501) staff       (20)       38 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/40/a96afc6ff09d58a702b76e3f7dd412fe975e26
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.939323 txapi-1.0.1/.git/objects/41/
--r--r--r--   0 linkerui   (501) staff       (20)      170 2022-11-25 05:42:01.000000 txapi-1.0.1/.git/objects/41/62b43e34e8a87d50e492a2f513b5f98fc38ef7
--r--r--r--   0 linkerui   (501) staff       (20)      153 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/41/7a59650920676ff59e7d08f927fa8ed6504aa5
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.939975 txapi-1.0.1/.git/objects/45/
--r--r--r--   0 linkerui   (501) staff       (20)      619 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/45/219397fd4a9c0cb4ac7ac9018b67b54ba2ef36
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.940642 txapi-1.0.1/.git/objects/46/
--r--r--r--   0 linkerui   (501) staff       (20)      247 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/46/86143cf8e1c6484b70f3322e32c014c6ee8d86
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.942134 txapi-1.0.1/.git/objects/47/
--r--r--r--   0 linkerui   (501) staff       (20)      647 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/47/1c3d59784a99eb3429ccbd100c7038f4859d54
--r--r--r--   0 linkerui   (501) staff       (20)       52 2022-11-25 05:52:30.000000 txapi-1.0.1/.git/objects/47/af7a7c8fe1b9c9da61f5959fed451074291b68
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.943045 txapi-1.0.1/.git/objects/4c/
--r--r--r--   0 linkerui   (501) staff       (20)      362 2023-04-10 09:59:52.000000 txapi-1.0.1/.git/objects/4c/e483925dea807e85f64038ec99e73a5cd46d15
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.944712 txapi-1.0.1/.git/objects/4e/
--r--r--r--   0 linkerui   (501) staff       (20)       89 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/4e/610856bd88c524f7faae8f05004b0736c95ed6
--r--r--r--   0 linkerui   (501) staff       (20)      154 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/4e/e6209932e8c5b6f62f8be128c50655c5a691a4
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.945525 txapi-1.0.1/.git/objects/50/
--r--r--r--   0 linkerui   (501) staff       (20)      301 2023-01-19 02:38:08.000000 txapi-1.0.1/.git/objects/50/7d622c92776e098ae53f1fad82e0623c208335
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.947051 txapi-1.0.1/.git/objects/54/
--r--r--r--   0 linkerui   (501) staff       (20)      150 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/54/1ebdcb8976304f04e1e9e52ab8a5e19f4084c5
--r--r--r--   0 linkerui   (501) staff       (20)      118 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/54/a80afb631926239ffd81091bb558a592735749
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.947641 txapi-1.0.1/.git/objects/57/
--r--r--r--   0 linkerui   (501) staff       (20)      574 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/57/940bdb0c48ade22baee7f4d5775cbbf3334d90
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.949021 txapi-1.0.1/.git/objects/58/
--r--r--r--   0 linkerui   (501) staff       (20)      418 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/58/1a24d98cc8f2a900be6bae0b4679c459453f92
--r--r--r--   0 linkerui   (501) staff       (20)      286 2023-04-23 05:07:43.000000 txapi-1.0.1/.git/objects/58/3f3db9002c6864c1ae3a75e2d74576e7489224
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.949902 txapi-1.0.1/.git/objects/59/
--r--r--r--   0 linkerui   (501) staff       (20)     1455 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/59/6c581887f06e9ab622345a9191e3e09732cc7b
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.950523 txapi-1.0.1/.git/objects/5b/
--r--r--r--   0 linkerui   (501) staff       (20)      286 2023-04-10 09:59:52.000000 txapi-1.0.1/.git/objects/5b/5a1fea3d4818c5e9ce7087044fb384596b43e3
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.951733 txapi-1.0.1/.git/objects/5d/
--r--r--r--   0 linkerui   (501) staff       (20)      281 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/5d/2b6865cbe0450ad11d4fc2cf18706721248b9f
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.952496 txapi-1.0.1/.git/objects/63/
--r--r--r--   0 linkerui   (501) staff       (20)      730 2023-04-23 05:07:43.000000 txapi-1.0.1/.git/objects/63/096a2158e3f8361a3f51091f9fa8008c688049
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.954114 txapi-1.0.1/.git/objects/64/
--r--r--r--   0 linkerui   (501) staff       (20)      248 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/64/48e904dcb43254931d1af079c489e4edfa02ed
--r--r--r--   0 linkerui   (501) staff       (20)      286 2023-01-19 02:38:08.000000 txapi-1.0.1/.git/objects/64/bb73d61ba8e23ded6723a0c0a199d528d88a9a
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.956407 txapi-1.0.1/.git/objects/65/
--r--r--r--   0 linkerui   (501) staff       (20)      126 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/65/7089684405c08caf3d94dc656ef8e932742f42
--r--r--r--   0 linkerui   (501) staff       (20)       89 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/65/be0c194324589fdd100ecf5da077daa823c38d
--r--r--r--   0 linkerui   (501) staff       (20)       86 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/65/c8f6514aaf92c8378cfdd08f351eed76b5404f
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.957594 txapi-1.0.1/.git/objects/67/
--r--r--r--   0 linkerui   (501) staff       (20)       89 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/67/24f268cd8d3dd7e85ee640867ae4c43c40d8b7
--r--r--r--   0 linkerui   (501) staff       (20)      519 2023-04-23 05:07:43.000000 txapi-1.0.1/.git/objects/67/39f71ac4becbfda86f98d6b3ae1a4be3d60ad9
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.958329 txapi-1.0.1/.git/objects/68/
--r--r--r--   0 linkerui   (501) staff       (20)      179 2023-01-19 02:38:08.000000 txapi-1.0.1/.git/objects/68/e2761b38d12e84388046a201fb494de7ecda8c
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.959529 txapi-1.0.1/.git/objects/69/
--r--r--r--   0 linkerui   (501) staff       (20)      301 2023-04-23 04:56:44.000000 txapi-1.0.1/.git/objects/69/a95ad1e84427ae51b0e79743e99e5733a654fe
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.960723 txapi-1.0.1/.git/objects/6b/
--r--r--r--   0 linkerui   (501) staff       (20)       86 2023-04-23 05:07:43.000000 txapi-1.0.1/.git/objects/6b/75c847a627117b395900264ed87e18b55fdd11
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.962111 txapi-1.0.1/.git/objects/6c/
--r--r--r--   0 linkerui   (501) staff       (20)      559 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/6c/4a1313e8ec893fc2ebd5d3b3efce63d11f73db
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.964958 txapi-1.0.1/.git/objects/6d/
--r--r--r--   0 linkerui   (501) staff       (20)       94 2022-11-25 05:42:01.000000 txapi-1.0.1/.git/objects/6d/0dbb49aca3b25be77017accb1a6b9cc75bd5f5
--r--r--r--   0 linkerui   (501) staff       (20)       89 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/6d/b7727950e8b5aed41400abf51ec3a0fe53358e
--r--r--r--   0 linkerui   (501) staff       (20)      286 2022-11-25 05:42:01.000000 txapi-1.0.1/.git/objects/6d/e48d16e8398658c1e1541bfdb450847d976398
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.966142 txapi-1.0.1/.git/objects/71/
--r--r--r--   0 linkerui   (501) staff       (20)      287 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/71/69e48c7afb39b6fa8a868be27cb4626de23fa1
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.967146 txapi-1.0.1/.git/objects/72/
--r--r--r--   0 linkerui   (501) staff       (20)      128 2023-04-23 05:13:30.000000 txapi-1.0.1/.git/objects/72/f76904d91e580dd0b5f70ee565b4c2ffa79734
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.969086 txapi-1.0.1/.git/objects/73/
--r--r--r--   0 linkerui   (501) staff       (20)      107 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/73/4e1cee7f9f3a49efb7e389dbd6c74c56813677
--r--r--r--   0 linkerui   (501) staff       (20)      108 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/73/d41923e7cb9369bd5363d0410814474a9e3009
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.969895 txapi-1.0.1/.git/objects/75/
--r--r--r--   0 linkerui   (501) staff       (20)     1605 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/75/fe7a3d3ccbdaec7b3b95d4c7c44ecee3ed92f3
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.971452 txapi-1.0.1/.git/objects/76/
--r--r--r--   0 linkerui   (501) staff       (20)      653 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/76/0aade4935e771a96525aa507d60f72614c5da6
--r--r--r--   0 linkerui   (501) staff       (20)      167 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/76/353b844acf336aa586ec8d94c3019017948802
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.972423 txapi-1.0.1/.git/objects/77/
--r--r--r--   0 linkerui   (501) staff       (20)      223 2023-04-23 04:56:44.000000 txapi-1.0.1/.git/objects/77/b3e410890f76b6d46395e3378e3ddf86f46edd
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.974347 txapi-1.0.1/.git/objects/78/
--r--r--r--   0 linkerui   (501) staff       (20)      655 2022-11-25 05:52:30.000000 txapi-1.0.1/.git/objects/78/68afd1318032499383a82f4a2b458791e7b990
--r--r--r--   0 linkerui   (501) staff       (20)     3716 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/78/a660592bc694a40b5248e0549c066483452c7a
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.974995 txapi-1.0.1/.git/objects/79/
--r--r--r--   0 linkerui   (501) staff       (20)      285 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/79/21604e32ec96a87935f84fa75b6de1e1ae400c
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.976127 txapi-1.0.1/.git/objects/7a/
--r--r--r--   0 linkerui   (501) staff       (20)      301 2023-04-23 05:07:43.000000 txapi-1.0.1/.git/objects/7a/6d83033af302a944ab27fd7580d33ef12de5f7
--r--r--r--   0 linkerui   (501) staff       (20)      426 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/7a/9553cfe8d189140ffb4739b9def6eddd2b05ae
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.976639 txapi-1.0.1/.git/objects/7e/
--r--r--r--   0 linkerui   (501) staff       (20)      157 2023-01-19 02:38:08.000000 txapi-1.0.1/.git/objects/7e/9e25992722a214ac1c4450faa8af6361190eb6
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.977383 txapi-1.0.1/.git/objects/7f/
--r--r--r--   0 linkerui   (501) staff       (20)      155 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/7f/164528f0ea755e2bbf70cba5ca83d51fab1f56
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.978940 txapi-1.0.1/.git/objects/80/
--r--r--r--   0 linkerui   (501) staff       (20)      465 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/80/0b22e14afd5501a6a46cc7dccf6eb32e0f206f
--r--r--r--   0 linkerui   (501) staff       (20)     1472 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/80/5cc728900be707de58af039739e01221353528
--r--r--r--   0 linkerui   (501) staff       (20)     1605 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/80/b07b0c161d95297f1a537db880d0e98acad82d
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.980551 txapi-1.0.1/.git/objects/81/
--r--r--r--   0 linkerui   (501) staff       (20)      286 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/81/b6056b9090ed2622e20ab2d91bd989a2ed1a03
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.981020 txapi-1.0.1/.git/objects/82/
--r--r--r--   0 linkerui   (501) staff       (20)     1477 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/82/63ddf91052bfe6c6af092051fafc077d86476c
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.981913 txapi-1.0.1/.git/objects/87/
--r--r--r--   0 linkerui   (501) staff       (20)      510 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/87/5310a549269b17f68963634a0c2da344ba245f
--r--r--r--   0 linkerui   (501) staff       (20)       85 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/87/c8b64913054035a4c8f8d0578f24e0d12955ea
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.982413 txapi-1.0.1/.git/objects/88/
--r--r--r--   0 linkerui   (501) staff       (20)      287 2023-01-19 02:38:08.000000 txapi-1.0.1/.git/objects/88/6515f9316155f3954ae1a4a60f4cf3641165d0
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.983414 txapi-1.0.1/.git/objects/89/
--r--r--r--   0 linkerui   (501) staff       (20)      352 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/89/391fb26eb5246ed340f53390899c6f71336231
--r--r--r--   0 linkerui   (501) staff       (20)       39 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/89/7e3130d7653b12be4087a2eb9868f0162974dc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.985175 txapi-1.0.1/.git/objects/8d/
--r--r--r--   0 linkerui   (501) staff       (20)     1490 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/8d/1cdd3e52ed567f61e45e6fcc4feefde445c9e3
--r--r--r--   0 linkerui   (501) staff       (20)      301 2023-04-23 05:13:30.000000 txapi-1.0.1/.git/objects/8d/213a3f1b9d2f3de20df4e41a55b179fdfa249b
--r--r--r--   0 linkerui   (501) staff       (20)      301 2023-01-19 02:38:08.000000 txapi-1.0.1/.git/objects/8d/b3bf09a5f6fe8c4ff29fdb9a5f70475b4a1adc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.985653 txapi-1.0.1/.git/objects/93/
--r--r--r--   0 linkerui   (501) staff       (20)      240 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/93/7db38a1c9decf1ddfbfaef0718b7cf0976dc14
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.986137 txapi-1.0.1/.git/objects/95/
--r--r--r--   0 linkerui   (501) staff       (20)      285 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/95/66a4df3edd828dfddeda104d238e0386738e90
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.987780 txapi-1.0.1/.git/objects/99/
--r--r--r--   0 linkerui   (501) staff       (20)      598 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/99/639a2389a1ee50ace8a7ebfeb6a848085b3ae1
--r--r--r--   0 linkerui   (501) staff       (20)      108 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/99/649150e602754bbdf1cceca82f7ae0042aad43
--r--r--r--   0 linkerui   (501) staff       (20)      128 2022-11-25 05:52:30.000000 txapi-1.0.1/.git/objects/99/e16eaed48da0fa2a08af4eba2ab8b8dcd11ac0
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.989065 txapi-1.0.1/.git/objects/9a/
--r--r--r--   0 linkerui   (501) staff       (20)      301 2022-11-25 05:52:30.000000 txapi-1.0.1/.git/objects/9a/396ba470231fa2cf1a0be23f6c16c2cf807dc0
--r--r--r--   0 linkerui   (501) staff       (20)     3724 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/9a/74267b066cb21fc0a23b33cd3990bc13f9ba1d
--r--r--r--   0 linkerui   (501) staff       (20)     1944 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/9a/ca49ad39bb6aabb57d014726a4a2433206ecc7
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.990278 txapi-1.0.1/.git/objects/9e/
--r--r--r--   0 linkerui   (501) staff       (20)      168 2022-11-25 05:52:30.000000 txapi-1.0.1/.git/objects/9e/336bd58fc96bb88e2b9a86bdcb6971652394b4
--r--r--r--   0 linkerui   (501) staff       (20)      672 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/9e/d55bad89de367003e0a538b16e6c79d32db508
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.991181 txapi-1.0.1/.git/objects/a2/
--r--r--r--   0 linkerui   (501) staff       (20)      643 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/a2/30bd6c3fe5539caed2f8b2b0865c6deea1a026
--r--r--r--   0 linkerui   (501) staff       (20)       31 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/a2/aca1c77e4889bbdba02e722430d6a69a14c2a0
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.991682 txapi-1.0.1/.git/objects/a3/
--r--r--r--   0 linkerui   (501) staff       (20)      961 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/a3/68a8a8fd04e25b619adb09c2bee7ad676d3185
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.992176 txapi-1.0.1/.git/objects/a5/
--r--r--r--   0 linkerui   (501) staff       (20)      696 2023-04-23 04:56:44.000000 txapi-1.0.1/.git/objects/a5/07a598601aea15d6abaafe7bad6ad10e2b22d7
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.992780 txapi-1.0.1/.git/objects/a6/
--r--r--r--   0 linkerui   (501) staff       (20)     1938 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/a6/6d48d9f7ef0c81494621de192b567705157436
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.994301 txapi-1.0.1/.git/objects/a7/
--r--r--r--   0 linkerui   (501) staff       (20)      340 2023-04-23 05:13:30.000000 txapi-1.0.1/.git/objects/a7/7cbef8139fd72d2421e1fbef4b7433022e6683
--r--r--r--   0 linkerui   (501) staff       (20)     1491 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/a7/826960973f479a98bd49313e881c5e93393e38
--r--r--r--   0 linkerui   (501) staff       (20)      154 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/a7/b67376b5ff945537da897b0091bf8de9424ec0
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.994702 txapi-1.0.1/.git/objects/a9/
--r--r--r--   0 linkerui   (501) staff       (20)      339 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/a9/00b9fb2f23ed04d28847f0f78a9abdc6b12595
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.995087 txapi-1.0.1/.git/objects/ad/
--r--r--r--   0 linkerui   (501) staff       (20)      648 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/ad/91fa7d37aa37e20fe58076725790e8aae43bc0
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.995984 txapi-1.0.1/.git/objects/b1/
--r--r--r--   0 linkerui   (501) staff       (20)       85 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/b1/21761178ea0098e11e96a2467f97a80f50d3b6
--r--r--r--   0 linkerui   (501) staff       (20)      251 2023-04-23 05:07:43.000000 txapi-1.0.1/.git/objects/b1/ee6c481e8ce3a307c0983b487a610bbdd7e065
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.996597 txapi-1.0.1/.git/objects/b2/
--r--r--r--   0 linkerui   (501) staff       (20)      285 2023-04-23 04:56:44.000000 txapi-1.0.1/.git/objects/b2/442748fb5ccb3f5801c5dffbb8f8050aff47a6
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.997171 txapi-1.0.1/.git/objects/b3/
--r--r--r--   0 linkerui   (501) staff       (20)      262 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/b3/2da2543d266ca57a7a7072d8a1aa7906a5216f
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.997563 txapi-1.0.1/.git/objects/b4/
--r--r--r--   0 linkerui   (501) staff       (20)     1489 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/b4/09333c2ea63b578a3d08486be3d6e7a44edc7d
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.997948 txapi-1.0.1/.git/objects/b6/
--r--r--r--   0 linkerui   (501) staff       (20)     1011 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/b6/e47617de110dea7ca47e087ff1347cc2646eda
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.998328 txapi-1.0.1/.git/objects/b8/
--r--r--r--   0 linkerui   (501) staff       (20)      181 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/b8/1cd0c71144089c01e5d12b5a82dfcf30feece7
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.998701 txapi-1.0.1/.git/objects/bb/
--r--r--r--   0 linkerui   (501) staff       (20)      343 2022-11-25 05:52:30.000000 txapi-1.0.1/.git/objects/bb/4b30a3ec4305961374dbfa727156c77028a5fb
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.999168 txapi-1.0.1/.git/objects/bd/
--r--r--r--   0 linkerui   (501) staff       (20)      205 2023-04-23 05:13:30.000000 txapi-1.0.1/.git/objects/bd/767b09e07988677a46bff99a44334cb802325c
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.999688 txapi-1.0.1/.git/objects/be/
--r--r--r--   0 linkerui   (501) staff       (20)       88 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/be/9930fc9a74f5ef498dc7de5fb3b48305e261d7
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.000076 txapi-1.0.1/.git/objects/c2/
--r--r--r--   0 linkerui   (501) staff       (20)      339 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/c2/e715407eb2cadf53bd3266569043104528db0c
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.001489 txapi-1.0.1/.git/objects/c4/
--r--r--r--   0 linkerui   (501) staff       (20)      281 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/c4/1329695facbe88753632a6626d521e7136a37e
--r--r--r--   0 linkerui   (501) staff       (20)      603 2022-11-25 05:41:53.000000 txapi-1.0.1/.git/objects/c4/72d537837ad718aac848eb955f676a87e7f2ac
--r--r--r--   0 linkerui   (501) staff       (20)      156 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/c4/be97a7166b002dd20894cacbbc6538e90acf88
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.001875 txapi-1.0.1/.git/objects/c6/
--r--r--r--   0 linkerui   (501) staff       (20)      157 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/c6/7675076ec28c750826f7e5f2170122b8a9d3a3
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.002473 txapi-1.0.1/.git/objects/c9/
--r--r--r--   0 linkerui   (501) staff       (20)      348 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/c9/98aaf6c57e4dd8fd55cdc45f84f7e8ccdad887
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.003252 txapi-1.0.1/.git/objects/cd/
--r--r--r--   0 linkerui   (501) staff       (20)      300 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/cd/316e3e2823326d2d79e861a63228b0c5cf538e
--r--r--r--   0 linkerui   (501) staff       (20)     1944 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/cd/8c8e7cb1c8eb8308a1a70cb48320fdc1db3362
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.004426 txapi-1.0.1/.git/objects/cf/
--r--r--r--   0 linkerui   (501) staff       (20)      106 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/cf/1cd7c9a8eed6d7785ec1f54ebf3737df1c40cf
--r--r--r--   0 linkerui   (501) staff       (20)       52 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/cf/2f8da95e46dbe88e67d6b28cfb2bcf3e092b35
--r--r--r--   0 linkerui   (501) staff       (20)       94 2022-11-25 05:52:30.000000 txapi-1.0.1/.git/objects/cf/30c4ebc092f87f24d127e1724aeead7aeef57f
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.005839 txapi-1.0.1/.git/objects/d1/
--r--r--r--   0 linkerui   (501) staff       (20)     1630 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/d1/30c07e14b682ef444d69930acc214185c9b7db
--r--r--r--   0 linkerui   (501) staff       (20)      240 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/d1/7eb6ac8a7f6a3a69d8254e6fbf552231a0054f
--r--r--r--   0 linkerui   (501) staff       (20)       89 2023-04-23 04:56:44.000000 txapi-1.0.1/.git/objects/d1/d56662595333e313eb7bd388cfab40e7fa2a35
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.006428 txapi-1.0.1/.git/objects/d2/
--r--r--r--   0 linkerui   (501) staff       (20)      126 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/d2/27a48e81fb6f771f6296665b55d379f3569f5c
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.006864 txapi-1.0.1/.git/objects/d4/
--r--r--r--   0 linkerui   (501) staff       (20)      126 2023-04-23 04:56:44.000000 txapi-1.0.1/.git/objects/d4/7949ca42ff77a9f570b08a634182b151695b71
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.007415 txapi-1.0.1/.git/objects/d5/
--r--r--r--   0 linkerui   (501) staff       (20)      286 2022-11-25 05:52:30.000000 txapi-1.0.1/.git/objects/d5/9480059d62735163c88bf127d8f0ca49546a0f
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.007887 txapi-1.0.1/.git/objects/d6/
--r--r--r--   0 linkerui   (501) staff       (20)       51 2023-04-10 09:59:52.000000 txapi-1.0.1/.git/objects/d6/f0964f2c224afc19e38192e2debdafeeba6acd
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.008551 txapi-1.0.1/.git/objects/d8/
--r--r--r--   0 linkerui   (501) staff       (20)      287 2023-04-23 04:56:44.000000 txapi-1.0.1/.git/objects/d8/3e2b6fb80b632a01e951072e47598c70125249
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.009112 txapi-1.0.1/.git/objects/d9/
--r--r--r--   0 linkerui   (501) staff       (20)      643 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/d9/5dcf7e5be1da655caf43d16bfa1735477497a0
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.009493 txapi-1.0.1/.git/objects/da/
--r--r--r--   0 linkerui   (501) staff       (20)      300 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/da/55f873a9f0769f4616f797953c71860a97381c
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.009876 txapi-1.0.1/.git/objects/db/
--r--r--r--   0 linkerui   (501) staff       (20)      320 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/db/0c553587cb305847d9db53169807ca0e641b03
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.010927 txapi-1.0.1/.git/objects/de/
--r--r--r--   0 linkerui   (501) staff       (20)     1614 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/de/07e2c3445f2d8965343f0aa6099392f0ba0c52
--r--r--r--   0 linkerui   (501) staff       (20)       51 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/de/39cf37ad954d80ed5175810061a060c7ccc48d
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.011819 txapi-1.0.1/.git/objects/df/
--r--r--r--   0 linkerui   (501) staff       (20)     1489 2023-01-19 02:38:08.000000 txapi-1.0.1/.git/objects/df/6c3c8d9fa2fd045230e7d7be1b2b81ad15799f
--r--r--r--   0 linkerui   (501) staff       (20)      509 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/df/f1fb8aad73a25844ffb6765ea30040e1e84432
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.013085 txapi-1.0.1/.git/objects/e0/
--r--r--r--   0 linkerui   (501) staff       (20)       94 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/e0/843780558164d7300a78c2a170908b1533768f
--r--r--r--   0 linkerui   (501) staff       (20)      622 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/e0/db285333f977126d50cb01bef5f83bade2d169
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.013758 txapi-1.0.1/.git/objects/e1/
--r--r--r--   0 linkerui   (501) staff       (20)      451 2023-04-23 05:13:30.000000 txapi-1.0.1/.git/objects/e1/f9c3c0091160776f8bf8e555af4c60a93daee8
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.015346 txapi-1.0.1/.git/objects/e6/
--r--r--r--   0 linkerui   (501) staff       (20)      369 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/e6/9897651f87fd20adc69f034578a3a8419aa079
--r--r--r--   0 linkerui   (501) staff       (20)       15 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.015967 txapi-1.0.1/.git/objects/e8/
--r--r--r--   0 linkerui   (501) staff       (20)      461 2023-01-19 02:38:08.000000 txapi-1.0.1/.git/objects/e8/0552c62017ce1d42489c842a6758cc9fa85d42
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.018909 txapi-1.0.1/.git/objects/e9/
--r--r--r--   0 linkerui   (501) staff       (20)     1489 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/e9/09aa2ff53b15d535bcc2de16de52134b952aec
--r--r--r--   0 linkerui   (501) staff       (20)      450 2023-04-23 05:07:43.000000 txapi-1.0.1/.git/objects/e9/1cfc3308bd4c05146f1a135c3399d8cde82e4a
--r--r--r--   0 linkerui   (501) staff       (20)      273 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/e9/c8b75c83886fab11d8c53fbe5be76a8263c255
--r--r--r--   0 linkerui   (501) staff       (20)      180 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/e9/deadcf54da359adb62450efe4ca831b7d76153
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.019605 txapi-1.0.1/.git/objects/ec/
--r--r--r--   0 linkerui   (501) staff       (20)     1019 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/ec/7d22521aa69ab0c5fbea87d1157d781d0aebe6
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.020250 txapi-1.0.1/.git/objects/ed/
--r--r--r--   0 linkerui   (501) staff       (20)       86 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/ed/fcf1e4aa1dc35d7e84d5a81bbd15d73c2e3157
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.021858 txapi-1.0.1/.git/objects/ef/
--r--r--r--   0 linkerui   (501) staff       (20)      126 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/ef/21f242632e536036d59f053ebf3382ff8da058
--r--r--r--   0 linkerui   (501) staff       (20)      128 2023-01-19 02:38:08.000000 txapi-1.0.1/.git/objects/ef/4273e19f2cc3caae8ba7c70a9f56269b02fc01
--r--r--r--   0 linkerui   (501) staff       (20)      610 2022-11-25 05:52:30.000000 txapi-1.0.1/.git/objects/ef/586010c625011d458db7e684a425fcbd1012f1
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.022451 txapi-1.0.1/.git/objects/f3/
--r--r--r--   0 linkerui   (501) staff       (20)      615 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/f3/7b0ee455cd0876fd2a4a12adf4f70cb9855596
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.022928 txapi-1.0.1/.git/objects/f4/
--r--r--r--   0 linkerui   (501) staff       (20)       69 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/f4/9646aeef73b2c0107deed1cc8bf6bc31097917
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.023392 txapi-1.0.1/.git/objects/f6/
--r--r--r--   0 linkerui   (501) staff       (20)      646 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/objects/f6/f35d7b623a39e2342b860f6f080fe5d8275bd5
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.023941 txapi-1.0.1/.git/objects/fe/
--r--r--r--   0 linkerui   (501) staff       (20)      647 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/fe/a22029fd4d0cc03ab16a60109fb3f928dd7747
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.024420 txapi-1.0.1/.git/objects/ff/
--r--r--r--   0 linkerui   (501) staff       (20)     3721 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/objects/ff/3ba9f30b5aa2f45cbcd01a1b08be357c8f22cb
--rw-r--r--   0 linkerui   (501) staff       (20)      112 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/packed-refs
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.863644 txapi-1.0.1/.git/refs/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.024880 txapi-1.0.1/.git/refs/heads/
--rw-r--r--   0 linkerui   (501) staff       (20)       41 2023-04-23 05:13:30.000000 txapi-1.0.1/.git/refs/heads/main
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.863757 txapi-1.0.1/.git/refs/remotes/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.026564 txapi-1.0.1/.git/refs/remotes/origin/
--rw-r--r--   0 linkerui   (501) staff       (20)       30 2022-11-22 04:39:01.000000 txapi-1.0.1/.git/refs/remotes/origin/HEAD
--rw-r--r--   0 linkerui   (501) staff       (20)       41 2023-04-23 05:13:34.000000 txapi-1.0.1/.git/refs/remotes/origin/main
--rw-r--r--   0 linkerui   (501) staff       (20)       41 2022-11-25 05:04:04.000000 txapi-1.0.1/.git/refs/remotes/origin/py2
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.864049 txapi-1.0.1/.github/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.027726 txapi-1.0.1/.github/workflows/
--rw-r--r--   0 linkerui   (501) staff       (20)     1143 2022-11-25 05:47:59.000000 txapi-1.0.1/.github/workflows/python-package-conda.yml
--rw-r--r--   0 linkerui   (501) staff       (20)     1351 2023-04-10 09:59:30.000000 txapi-1.0.1/.github/workflows/python-package.yml
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.031056 txapi-1.0.1/.idea/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.032449 txapi-1.0.1/.idea/inspectionProfiles/
--rw-r--r--   0 linkerui   (501) staff       (20)     1382 2023-01-31 07:15:19.000000 txapi-1.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 linkerui   (501) staff       (20)      174 2023-01-31 07:15:19.000000 txapi-1.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 linkerui   (501) staff       (20)      185 2023-01-31 07:15:19.000000 txapi-1.0.1/.idea/misc.xml
--rw-r--r--   0 linkerui   (501) staff       (20)      262 2023-01-31 07:15:19.000000 txapi-1.0.1/.idea/modules.xml
--rw-r--r--   0 linkerui   (501) staff       (20)      555 2023-01-31 07:15:47.000000 txapi-1.0.1/.idea/txapi.iml
--rw-r--r--   0 linkerui   (501) staff       (20)      180 2023-01-31 07:15:19.000000 txapi-1.0.1/.idea/vcs.xml
--rw-r--r--   0 linkerui   (501) staff       (20)    11859 2023-04-23 05:12:59.000000 txapi-1.0.1/.idea/workspace.xml
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.034746 txapi-1.0.1/.pytest_cache/
--rw-r--r--   0 linkerui   (501) staff       (20)       36 2022-11-25 05:04:56.000000 txapi-1.0.1/.pytest_cache/.gitignore
--rw-r--r--   0 linkerui   (501) staff       (20)      194 2022-11-25 05:04:56.000000 txapi-1.0.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 linkerui   (501) staff       (20)      295 2022-11-25 05:04:56.000000 txapi-1.0.1/.pytest_cache/README.md
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.864886 txapi-1.0.1/.pytest_cache/v/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.037263 txapi-1.0.1/.pytest_cache/v/cache/
--rw-r--r--   0 linkerui   (501) staff       (20)       64 2022-11-25 05:37:01.000000 txapi-1.0.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 linkerui   (501) staff       (20)      244 2022-11-25 05:51:36.000000 txapi-1.0.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 linkerui   (501) staff       (20)        2 2022-11-25 05:51:36.000000 txapi-1.0.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 linkerui   (501) staff       (20)     1065 2022-11-22 04:39:01.000000 txapi-1.0.1/LICENSE
--rw-r--r--   0 linkerui   (501) staff       (20)       23 2022-11-22 04:39:01.000000 txapi-1.0.1/MANIFEST.in
--rw-r--r--   0 linkerui   (501) staff       (20)     1498 2023-04-23 05:15:52.496192 txapi-1.0.1/PKG-INFO
--rw-r--r--   0 linkerui   (501) staff       (20)     1206 2023-04-23 05:05:54.000000 txapi-1.0.1/README.md
--rw-r--r--   0 linkerui   (501) staff       (20)       38 2023-04-23 05:15:52.496575 txapi-1.0.1/setup.cfg
--rw-r--r--   0 linkerui   (501) staff       (20)      811 2023-04-23 05:12:59.000000 txapi-1.0.1/setup.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.043369 txapi-1.0.1/txapi/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.047393 txapi-1.0.1/txapi/QcloudApi/
--rw-r--r--   0 linkerui   (501) staff       (20)       23 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/QcloudApi/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      184 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/QcloudApi/__init__.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.048500 txapi-1.0.1/txapi/QcloudApi/__pycache__/
--rw-r--r--   0 linkerui   (501) staff       (20)      186 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/QcloudApi/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     2391 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/QcloudApi/__pycache__/qcloudapi.cpython-39.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.052935 txapi-1.0.1/txapi/QcloudApi/common/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/QcloudApi/common/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      158 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/QcloudApi/common/__init__.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.055101 txapi-1.0.1/txapi/QcloudApi/common/__pycache__/
--rw-r--r--   0 linkerui   (501) staff       (20)      171 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/QcloudApi/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     2693 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/QcloudApi/common/__pycache__/api_exception.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     5920 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/QcloudApi/common/__pycache__/request.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1444 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/QcloudApi/common/__pycache__/sign.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1381 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/QcloudApi/common/api_exception.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3594 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/QcloudApi/common/api_exception.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     6117 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/QcloudApi/common/request.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7845 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/QcloudApi/common/request.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1197 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/QcloudApi/common/sign.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1937 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/QcloudApi/common/sign.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.057084 txapi-1.0.1/txapi/QcloudApi/modules/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/QcloudApi/modules/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      159 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/QcloudApi/modules/__init__.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.058306 txapi-1.0.1/txapi/QcloudApi/modules/__pycache__/
--rw-r--r--   0 linkerui   (501) staff       (20)      172 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/QcloudApi/modules/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     4455 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/QcloudApi/modules/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     5684 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/QcloudApi/modules/base.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5939 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/QcloudApi/modules/base.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1763 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/QcloudApi/qcloudapi.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3067 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/QcloudApi/qcloudapi.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)      130 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      503 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/__init__.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.060522 txapi-1.0.1/txapi/__pycache__/
--rw-r--r--   0 linkerui   (501) staff       (20)      426 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     3844 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/__pycache__/api2.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     4360 2023-04-23 05:12:11.000000 txapi-1.0.1/txapi/__pycache__/api3.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)      302 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/__pycache__/version.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     4130 2022-11-25 05:39:33.000000 txapi-1.0.1/txapi/api2.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4773 2022-11-25 05:40:23.000000 txapi-1.0.1/txapi/api2.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     4992 2023-04-23 04:27:16.000000 txapi-1.0.1/txapi/api3.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5155 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/api3.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.061303 txapi-1.0.1/txapi/demo/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/demo/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      834 2023-04-23 05:01:34.000000 txapi-1.0.1/txapi/demo/demo.py
--rw-r--r--   0 linkerui   (501) staff       (20)       65 2022-11-25 05:04:29.000000 txapi-1.0.1/txapi/pytest.ini
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.062877 txapi-1.0.1/txapi/tencentcloud/
--rw-r--r--   0 linkerui   (501) staff       (20)      629 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/tencentcloud/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      187 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/__init__.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.063716 txapi-1.0.1/txapi/tencentcloud/__pycache__/
--rw-r--r--   0 linkerui   (501) staff       (20)      189 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/tencentcloud/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.070792 txapi-1.0.1/txapi/tencentcloud/common/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/tencentcloud/common/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      161 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/common/__init__.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.074380 txapi-1.0.1/txapi/tencentcloud/common/__pycache__/
--rw-r--r--   0 linkerui   (501) staff       (20)      174 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/tencentcloud/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     8240 2023-04-23 04:21:47.000000 txapi-1.0.1/txapi/tencentcloud/common/__pycache__/abstract_client.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1081 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/tencentcloud/common/__pycache__/credential.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1755 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/tencentcloud/common/__pycache__/sign.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)    12330 2023-04-23 04:21:46.000000 txapi-1.0.1/txapi/tencentcloud/common/abstract_client.py
--rw-r--r--   0 linkerui   (501) staff       (20)    10568 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/common/abstract_client.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     2066 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/tencentcloud/common/abstract_model.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1325 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/tencentcloud/common/credential.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1228 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/common/credential.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.077816 txapi-1.0.1/txapi/tencentcloud/common/exception/
--rw-r--r--   0 linkerui   (501) staff       (20)       24 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      171 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/common/exception/__init__.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.079314 txapi-1.0.1/txapi/tencentcloud/common/exception/__pycache__/
--rw-r--r--   0 linkerui   (501) staff       (20)      184 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/tencentcloud/common/exception/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1471 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/tencentcloud/common/exception/__pycache__/tencent_cloud_sdk_exception.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)      781 2022-11-25 05:04:29.000000 txapi-1.0.1/txapi/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2017 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/common/exception/tencent_cloud_sdk_exception.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.081731 txapi-1.0.1/txapi/tencentcloud/common/http/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/tencentcloud/common/http/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      166 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/common/http/__init__.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.083198 txapi-1.0.1/txapi/tencentcloud/common/http/__pycache__/
--rw-r--r--   0 linkerui   (501) staff       (20)      179 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/tencentcloud/common/http/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     6235 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/tencentcloud/common/http/__pycache__/request.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     6094 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/tencentcloud/common/http/request.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8460 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/common/http/request.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.087192 txapi-1.0.1/txapi/tencentcloud/common/profile/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      169 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/common/profile/__init__.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.089368 txapi-1.0.1/txapi/tencentcloud/common/profile/__pycache__/
--rw-r--r--   0 linkerui   (501) staff       (20)      182 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/tencentcloud/common/profile/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1037 2023-04-23 04:23:32.000000 txapi-1.0.1/txapi/tencentcloud/common/profile/__pycache__/client_profile.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1052 2023-04-23 04:18:26.000000 txapi-1.0.1/txapi/tencentcloud/common/profile/__pycache__/http_profile.cpython-39.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1308 2023-04-23 04:23:32.000000 txapi-1.0.1/txapi/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1133 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/common/profile/client_profile.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1426 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1257 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/common/profile/http_profile.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)     1595 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/tencentcloud/common/sign.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2283 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tencentcloud/common/sign.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.091474 txapi-1.0.1/txapi/tests/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-25 05:04:29.000000 txapi-1.0.1/txapi/tests/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      147 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/tests/__init__.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.092825 txapi-1.0.1/txapi/tests/__pycache__/
--rw-------   0 linkerui   (501) staff       (20)     5768 2022-11-25 05:51:36.000000 txapi-1.0.1/txapi/tests/__pycache__/apiv2_test.cpython-27-PYTEST.pyc
--rw-------   0 linkerui   (501) staff       (20)     1514 2022-11-25 05:35:32.000000 txapi-1.0.1/txapi/tests/__pycache__/send_request_test.cpython-27-PYTEST.pyc
--rw-r--r--   0 linkerui   (501) staff       (20)      862 2023-04-23 05:11:25.000000 txapi-1.0.1/txapi/tests/apiv2_test.py
--rw-r--r--   0 linkerui   (501) staff       (20)      846 2023-01-31 07:15:48.000000 txapi-1.0.1/txapi/tests/send_request_test.py
--rw-r--r--   0 linkerui   (501) staff       (20)      172 2022-11-22 04:39:01.000000 txapi-1.0.1/txapi/version.py
--rw-r--r--   0 linkerui   (501) staff       (20)      359 2022-11-25 05:04:56.000000 txapi-1.0.1/txapi/version.pyc
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.045397 txapi-1.0.1/txapi.egg-info/
--rw-r--r--   0 linkerui   (501) staff       (20)     1498 2023-04-23 05:15:51.000000 txapi-1.0.1/txapi.egg-info/PKG-INFO
--rw-r--r--   0 linkerui   (501) staff       (20)    53209 2023-04-23 05:15:51.000000 txapi-1.0.1/txapi.egg-info/SOURCES.txt
--rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-04-23 05:15:51.000000 txapi-1.0.1/txapi.egg-info/dependency_links.txt
--rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-04-23 05:15:51.000000 txapi-1.0.1/txapi.egg-info/not-zip-safe
--rw-r--r--   0 linkerui   (501) staff       (20)        6 2023-04-23 05:15:51.000000 txapi-1.0.1/txapi.egg-info/top_level.txt
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.093529 txapi-1.0.1/venv/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.101929 txapi-1.0.1/venv/bin/
--rw-r--r--   0 linkerui   (501) staff       (20)     8834 2022-11-22 06:31:24.000000 txapi-1.0.1/venv/bin/Activate.ps1
--rw-r--r--   0 linkerui   (501) staff       (20)     2200 2022-11-22 06:31:24.000000 txapi-1.0.1/venv/bin/activate
--rw-r--r--   0 linkerui   (501) staff       (20)     1252 2022-11-22 06:31:24.000000 txapi-1.0.1/venv/bin/activate.csh
--rw-r--r--   0 linkerui   (501) staff       (20)     2404 2022-11-22 06:31:24.000000 txapi-1.0.1/venv/bin/activate.fish
--rwxr-xr-x   0 linkerui   (501) staff       (20)      243 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/bin/autopep8
--rwxr-xr-x   0 linkerui   (501) staff       (20)      267 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/bin/easy_install
--rwxr-xr-x   0 linkerui   (501) staff       (20)      267 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/bin/easy_install-3.8
--rwxr-xr-x   0 linkerui   (501) staff       (20)      258 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/bin/pip
--rwxr-xr-x   0 linkerui   (501) staff       (20)      258 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/bin/pip3
--rwxr-xr-x   0 linkerui   (501) staff       (20)      258 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/bin/pip3.8
--rwxr-xr-x   0 linkerui   (501) staff       (20)      248 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/bin/pycodestyle
--rwxr-xr-x   0 linkerui   (501) staff       (20)   151504 2023-03-24 11:18:24.000000 txapi-1.0.1/venv/bin/python
--rwxr-xr-x   0 linkerui   (501) staff       (20)   151504 2023-03-24 11:18:24.000000 txapi-1.0.1/venv/bin/python3
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.871030 txapi-1.0.1/venv/lib/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:51.871161 txapi-1.0.1/venv/lib/python3.8/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.104647 txapi-1.0.1/venv/lib/python3.8/site-packages/
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.109964 txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/
--rw-r--r--   0 linkerui   (501) staff       (20)     2003 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/AUTHORS.rst
--rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/INSTALLER
--rw-r--r--   0 linkerui   (501) staff       (20)     1181 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/LICENSE
--rw-r--r--   0 linkerui   (501) staff       (20)    17205 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/METADATA
--rw-r--r--   0 linkerui   (501) staff       (20)     1064 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/RECORD
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/REQUESTED
--rw-r--r--   0 linkerui   (501) staff       (20)      110 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/WHEEL
--rw-r--r--   0 linkerui   (501) staff       (20)       43 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/entry_points.txt
--rw-r--r--   0 linkerui   (501) staff       (20)        9 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/top_level.txt
--rw-r--r--   0 linkerui   (501) staff       (20)   156040 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8.py
--rw-r--r--   0 linkerui   (501) staff       (20)      126 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/easy_install.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.110991 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/
--rw-r--r--   0 linkerui   (501) staff       (20)      455 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      911 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/__main__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.124824 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/
--rw-r--r--   0 linkerui   (501) staff       (20)      495 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8088 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/build_env.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12249 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cache.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.132006 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/
--rw-r--r--   0 linkerui   (501) staff       (20)      132 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6547 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9302 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0 linkerui   (501) staff       (20)    28782 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0 linkerui   (501) staff       (20)      975 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2616 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2843 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9480 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9121 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0 linkerui   (501) staff       (20)    15132 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5509 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0 linkerui   (501) staff       (20)      156 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/status_codes.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.142382 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/
--rw-r--r--   0 linkerui   (501) staff       (20)     4100 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5676 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1677 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3081 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9344 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7314 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4918 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3452 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1843 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1270 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0 linkerui   (501) staff       (20)    27995 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0 linkerui   (501) staff       (20)    11312 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5756 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6996 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3311 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6419 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0 linkerui   (501) staff       (20)    14115 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/configuration.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.145119 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/distributions/
--rw-r--r--   0 linkerui   (501) staff       (20)      959 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1425 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0 linkerui   (501) staff       (20)      760 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4086 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1294 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12637 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/exceptions.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.146865 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/index/
--rw-r--r--   0 linkerui   (501) staff       (20)       30 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    22838 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0 linkerui   (501) staff       (20)    37364 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6732 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/locations.py
--rw-r--r--   0 linkerui   (501) staff       (20)      437 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/main.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.153488 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/
--rw-r--r--   0 linkerui   (501) staff       (20)       63 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1195 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6900 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2823 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1161 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/index.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7470 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/link.py
--rw-r--r--   0 linkerui   (501) staff       (20)      778 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4751 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2044 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4034 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2772 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/wheel.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.157534 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/
--rw-r--r--   0 linkerui   (501) staff       (20)       50 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    11652 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2329 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5151 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/download.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8138 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0 linkerui   (501) staff       (20)    15208 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/session.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4172 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1882 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/xmlrpc.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.159472 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.161627 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/build/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1254 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2011 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1465 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3356 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5215 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0 linkerui   (501) staff       (20)    10373 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/freeze.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.167385 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/install/
--rw-r--r--   0 linkerui   (501) staff       (20)       51 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1488 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4281 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0 linkerui   (501) staff       (20)    31310 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0 linkerui   (501) staff       (20)    19903 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7400 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/pyproject.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.175564 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/
--rw-r--r--   0 linkerui   (501) staff       (20)     3133 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    16387 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0 linkerui   (501) staff       (20)    19448 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0 linkerui   (501) staff       (20)    33610 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7886 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4690 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/req_tracker.py
--rw-r--r--   0 linkerui   (501) staff       (20)    23706 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/req_uninstall.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.176858 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      682 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/base.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.177790 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    18755 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.182520 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2342 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0 linkerui   (501) staff       (20)    20339 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0 linkerui   (501) staff       (20)    17169 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6134 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4511 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0 linkerui   (501) staff       (20)    10149 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6779 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/self_outdated_check.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.198946 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1349 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8865 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5439 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0 linkerui   (501) staff       (20)      295 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3318 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4359 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1350 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1284 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1152 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6943 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0 linkerui   (501) staff       (20)      571 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3297 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4358 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0 linkerui   (501) staff       (20)      810 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0 linkerui   (501) staff       (20)    13093 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0 linkerui   (501) staff       (20)    28001 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1201 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3035 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3404 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/parallel.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1254 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/pkg_resources.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5058 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9924 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8378 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1401 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/typing.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9488 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1527 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3706 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7303 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/wheel.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.202475 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/
--rw-r--r--   0 linkerui   (501) staff       (20)      617 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3887 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0 linkerui   (501) staff       (20)    13985 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5162 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12399 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0 linkerui   (501) staff       (20)    25966 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9522 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/wheel_builder.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.212805 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/
--rw-r--r--   0 linkerui   (501) staff       (20)     4588 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    25907 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/appdirs.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.221817 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/
--rw-r--r--   0 linkerui   (501) staff       (20)      302 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1295 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4882 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0 linkerui   (501) staff       (20)      805 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.224213 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/
--rw-r--r--   0 linkerui   (501) staff       (20)       86 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4153 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0 linkerui   (501) staff       (20)      856 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0 linkerui   (501) staff       (20)      695 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)    14149 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2533 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4070 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7091 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0 linkerui   (501) staff       (20)      690 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.229226 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-r--r--   0 linkerui   (501) staff       (20)       62 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      255 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0 linkerui   (501) staff       (20)   282394 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0 linkerui   (501) staff       (20)     2315 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/certifi/core.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.254607 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/
--rw-r--r--   0 linkerui   (501) staff       (20)     1559 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    31254 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1757 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9411 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3787 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5110 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.255687 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/
--rw-r--r--   0 linkerui   (501) staff       (20)        1 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2774 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3590 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1134 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1855 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1661 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3950 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0 linkerui   (501) staff       (20)    10510 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3749 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0 linkerui   (501) staff       (20)    13546 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1748 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0 linkerui   (501) staff       (20)    31621 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1747 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0 linkerui   (501) staff       (20)    20715 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1754 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0 linkerui   (501) staff       (20)    13838 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0 linkerui   (501) staff       (20)    25777 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0 linkerui   (501) staff       (20)    19643 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12839 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0 linkerui   (501) staff       (20)    17948 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langcyrillicmodel.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12688 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0 linkerui   (501) staff       (20)    11345 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12592 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0 linkerui   (501) staff       (20)    11290 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0 linkerui   (501) staff       (20)    11102 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5370 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3413 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2012 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0 linkerui   (501) staff       (20)    25481 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5657 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3546 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3774 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12485 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2766 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0 linkerui   (501) staff       (20)      242 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/version.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.259000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/
--rw-r--r--   0 linkerui   (501) staff       (20)      239 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2524 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0 linkerui   (501) staff       (20)    10462 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1915 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5404 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6438 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0 linkerui   (501) staff       (20)    16915 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/contextlib2.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.280103 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/
--rw-r--r--   0 linkerui   (501) staff       (20)      581 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.284912 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/
--rw-r--r--   0 linkerui   (501) staff       (20)      274 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      971 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/misc.py
--rw-r--r--   0 linkerui   (501) staff       (20)    25707 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/shutil.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2617 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/sysconfig.cfg
--rw-r--r--   0 linkerui   (501) staff       (20)    26854 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
--rw-r--r--   0 linkerui   (501) staff       (20)    92628 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/tarfile.py
--rw-r--r--   0 linkerui   (501) staff       (20)    41408 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)    51059 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0 linkerui   (501) staff       (20)    21066 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0 linkerui   (501) staff       (20)    52100 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0 linkerui   (501) staff       (20)    14811 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4387 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0 linkerui   (501) staff       (20)    38962 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0 linkerui   (501) staff       (20)    10766 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0 linkerui   (501) staff       (20)    17180 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0 linkerui   (501) staff       (20)    96768 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0 linkerui   (501) staff       (20)   105984 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0 linkerui   (501) staff       (20)    59845 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0 linkerui   (501) staff       (20)    23391 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0 linkerui   (501) staff       (20)    90112 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0 linkerui   (501) staff       (20)    99840 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0 linkerui   (501) staff       (20)    41144 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0 linkerui   (501) staff       (20)    43628 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distro.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.293267 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/
--rw-r--r--   0 linkerui   (501) staff       (20)     1160 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    16728 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_ihatexml.py
--rw-r--r--   0 linkerui   (501) staff       (20)    32353 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_inputstream.py
--rw-r--r--   0 linkerui   (501) staff       (20)    77040 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_tokenizer.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.295048 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/
--rw-r--r--   0 linkerui   (501) staff       (20)      109 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1013 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/_base.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1775 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/py.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4931 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_utils.py
--rw-r--r--   0 linkerui   (501) staff       (20)    83464 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/constants.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.299450 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      919 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-r--r--   0 linkerui   (501) staff       (20)      286 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/base.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2945 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3643 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/lint.py
--rw-r--r--   0 linkerui   (501) staff       (20)    10588 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
--rw-r--r--   0 linkerui   (501) staff       (20)    26897 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1214 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/whitespace.py
--rw-r--r--   0 linkerui   (501) staff       (20)   117186 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/html5parser.py
--rw-r--r--   0 linkerui   (501) staff       (20)    15759 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/serializer.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.302572 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/
--rw-r--r--   0 linkerui   (501) staff       (20)      679 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1715 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1776 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.304821 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/
--rw-r--r--   0 linkerui   (501) staff       (20)     3592 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    14565 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/base.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8925 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12836 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
--rw-r--r--   0 linkerui   (501) staff       (20)    14766 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.307642 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/
--rw-r--r--   0 linkerui   (501) staff       (20)     5719 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7476 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/base.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1413 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4551 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6357 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2309 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.311494 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/
--rw-r--r--   0 linkerui   (501) staff       (20)       58 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3299 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0 linkerui   (501) staff       (20)      232 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)    11951 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0 linkerui   (501) staff       (20)    42350 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1749 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0 linkerui   (501) staff       (20)       22 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0 linkerui   (501) staff       (20)   202084 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0 linkerui   (501) staff       (20)    79875 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/ipaddress.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.316476 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/
--rw-r--r--   0 linkerui   (501) staff       (20)     1118 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)       20 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/_version.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1081 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6034 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0 linkerui   (501) staff       (20)    37133 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/fallback.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.325243 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/
--rw-r--r--   0 linkerui   (501) staff       (20)      736 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      562 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1128 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2022 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1824 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_typing.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9491 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4903 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0 linkerui   (501) staff       (20)    31944 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0 linkerui   (501) staff       (20)    24067 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1811 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0 linkerui   (501) staff       (20)    15470 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/version.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.331495 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/
--rw-r--r--   0 linkerui   (501) staff       (20)       84 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8438 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/_in_process.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3335 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/build.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5961 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/check.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4098 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/colorlog.py
--rw-r--r--   0 linkerui   (501) staff       (20)      780 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1129 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/dirtools.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6041 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/envbuild.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2463 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/meta.py
--rw-r--r--   0 linkerui   (501) staff       (20)    10783 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/wrappers.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.333985 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/
--rw-r--r--   0 linkerui   (501) staff       (20)   108277 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      562 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/py31compat.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.336248 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/progress/
--rw-r--r--   0 linkerui   (501) staff       (20)     4857 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/progress/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2854 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/progress/bar.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1372 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/progress/counter.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1380 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/progress/spinner.py
--rw-r--r--   0 linkerui   (501) staff       (20)   273394 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.347617 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/
--rw-r--r--   0 linkerui   (501) staff       (20)     4465 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      441 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1096 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0 linkerui   (501) staff       (20)    21548 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6496 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0 linkerui   (501) staff       (20)    10207 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0 linkerui   (501) staff       (20)      465 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2045 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)    18430 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3173 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3578 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0 linkerui   (501) staff       (20)      757 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0 linkerui   (501) staff       (20)    34287 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0 linkerui   (501) staff       (20)      695 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0 linkerui   (501) staff       (20)    29316 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4188 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3005 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0 linkerui   (501) staff       (20)    30176 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/utils.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.350897 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/
--rw-r--r--   0 linkerui   (501) staff       (20)      537 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.351621 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      127 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4547 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1405 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0 linkerui   (501) staff       (20)    15018 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2016 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9972 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/retrying.py
--rw-r--r--   0 linkerui   (501) staff       (20)    34159 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/six.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.354803 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/toml/
--rw-r--r--   0 linkerui   (501) staff       (20)      747 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/toml/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      242 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/toml/common.py
--rw-r--r--   0 linkerui   (501) staff       (20)    38696 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/toml/decoder.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9955 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/toml/encoder.py
--rw-r--r--   0 linkerui   (501) staff       (20)      378 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/toml/ordered.py
--rw-r--r--   0 linkerui   (501) staff       (20)      618 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/toml/tz.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.359280 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/
--rw-r--r--   0 linkerui   (501) staff       (20)     2683 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    10792 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0 linkerui   (501) staff       (20)    14461 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0 linkerui   (501) staff       (20)    35725 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.363092 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      957 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.364494 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    16886 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 linkerui   (501) staff       (20)    11956 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 linkerui   (501) staff       (20)    11034 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4160 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 linkerui   (501) staff       (20)    16582 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 linkerui   (501) staff       (20)    32401 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7036 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7172 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8553 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2440 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/filepost.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.365402 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/
--rw-r--r--   0 linkerui   (501) staff       (20)      108 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.366238 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1418 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0 linkerui   (501) staff       (20)    32536 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/six.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.367202 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/
--rw-r--r--   0 linkerui   (501) staff       (20)      688 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5696 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-r--r--   0 linkerui   (501) staff       (20)    17861 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6018 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0 linkerui   (501) staff       (20)    28221 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/response.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.372166 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/
--rw-r--r--   0 linkerui   (501) staff       (20)     1038 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4637 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0 linkerui   (501) staff       (20)      497 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3815 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2573 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0 linkerui   (501) staff       (20)    15543 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0 linkerui   (501) staff       (20)    14523 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9947 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0 linkerui   (501) staff       (20)    13981 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5406 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0 linkerui   (501) staff       (20)      437 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/vendor.txt
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.374473 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/
--rw-r--r--   0 linkerui   (501) staff       (20)    10579 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8979 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1305 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6563 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4307 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.116810 txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/
--rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/INSTALLER
--rw-r--r--   0 linkerui   (501) staff       (20)     1090 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/LICENSE.txt
--rw-r--r--   0 linkerui   (501) staff       (20)     3708 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/METADATA
--rw-r--r--   0 linkerui   (501) staff       (20)    98502 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/RECORD
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/REQUESTED
--rw-r--r--   0 linkerui   (501) staff       (20)      110 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/WHEEL
--rw-r--r--   0 linkerui   (501) staff       (20)      125 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/entry_points.txt
--rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-22 06:31:23.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/top_level.txt
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.374914 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/
--rw-r--r--   0 linkerui   (501) staff       (20)   108481 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.378640 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    24701 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/appdirs.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.383730 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/
--rw-r--r--   0 linkerui   (501) staff       (20)      744 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      562 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      865 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1416 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8277 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4757 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0 linkerui   (501) staff       (20)    27778 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12933 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1520 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0 linkerui   (501) staff       (20)    11978 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0 linkerui   (501) staff       (20)   232055 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/pyparsing.py
--rw-r--r--   0 linkerui   (501) staff       (20)    30098 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/six.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.384141 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/extern/
--rw-r--r--   0 linkerui   (501) staff       (20)     2101 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/extern/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.387642 txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/
--rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/INSTALLER
--rw-r--r--   0 linkerui   (501) staff       (20)     1254 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/LICENSE
--rw-r--r--   0 linkerui   (501) staff       (20)    31580 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/METADATA
--rw-r--r--   0 linkerui   (501) staff       (20)      919 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/RECORD
--rw-r--r--   0 linkerui   (501) staff       (20)      110 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/WHEEL
--rw-r--r--   0 linkerui   (501) staff       (20)       50 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/entry_points.txt
--rw-r--r--   0 linkerui   (501) staff       (20)       12 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/top_level.txt
--rw-r--r--   0 linkerui   (501) staff       (20)   102313 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.419025 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/
--rw-r--r--   0 linkerui   (501) staff       (20)     7943 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      218 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_deprecation_warning.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.445363 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/
--rw-r--r--   0 linkerui   (501) staff       (20)      250 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    19968 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8572 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0 linkerui   (501) staff       (20)    14894 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0 linkerui   (501) staff       (20)    47437 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0 linkerui   (501) staff       (20)    18079 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/cmd.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.461782 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/
--rw-r--r--   0 linkerui   (501) staff       (20)      799 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5562 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4913 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0 linkerui   (501) staff       (20)    35579 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_msi.py
--rw-r--r--   0 linkerui   (501) staff       (20)    21537 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0 linkerui   (501) staff       (20)    16030 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_wininst.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5767 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8022 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0 linkerui   (501) staff       (20)    31635 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0 linkerui   (501) staff       (20)    17190 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6232 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5637 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2776 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0 linkerui   (501) staff       (20)    13117 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0 linkerui   (501) staff       (20)    27482 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2822 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2603 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1298 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8397 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2017 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0 linkerui   (501) staff       (20)    11712 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0 linkerui   (501) staff       (20)    19005 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7597 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4827 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8876 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0 linkerui   (501) staff       (20)    16380 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0 linkerui   (501) staff       (20)      139 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3491 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7778 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0 linkerui   (501) staff       (20)    50421 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3577 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0 linkerui   (501) staff       (20)    10515 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0 linkerui   (501) staff       (20)    17784 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8148 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12832 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1969 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0 linkerui   (501) staff       (20)    30453 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0 linkerui   (501) staff       (20)    23540 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4408 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0 linkerui   (501) staff       (20)    21349 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12483 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0 linkerui   (501) staff       (20)    14696 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0 linkerui   (501) staff       (20)    20913 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12514 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5133 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2388 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_imp.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.465964 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    15130 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/ordered_set.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.472797 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/
--rw-r--r--   0 linkerui   (501) staff       (20)      744 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      562 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)      865 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1416 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8268 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4742 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0 linkerui   (501) staff       (20)    27778 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0 linkerui   (501) staff       (20)    12933 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1520 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0 linkerui   (501) staff       (20)    11978 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0 linkerui   (501) staff       (20)   232055 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/pyparsing.py
--rw-r--r--   0 linkerui   (501) staff       (20)    30098 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/six.py
--rw-r--r--   0 linkerui   (501) staff       (20)     6638 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/archive_util.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9917 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/build_meta.py
--rw-r--r--   0 linkerui   (501) staff       (20)    65536 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/cli-32.exe
--rw-r--r--   0 linkerui   (501) staff       (20)    74752 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/cli-64.exe
--rw-r--r--   0 linkerui   (501) staff       (20)    65536 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/cli.exe
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.489985 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/
--rw-r--r--   0 linkerui   (501) staff       (20)      568 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2426 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/alias.py
--rw-r--r--   0 linkerui   (501) staff       (20)    18482 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1508 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0 linkerui   (501) staff       (20)      922 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/bdist_wininst.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4415 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0 linkerui   (501) staff       (20)    13187 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9737 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/build_py.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8118 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/develop.py
--rw-r--r--   0 linkerui   (501) staff       (20)      960 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0 linkerui   (501) staff       (20)    86924 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0 linkerui   (501) staff       (20)    25560 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4705 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/install.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2203 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3875 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2519 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0 linkerui   (501) staff       (20)      628 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0 linkerui   (501) staff       (20)     4994 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)      468 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/register.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2176 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/rotate.py
--rw-r--r--   0 linkerui   (501) staff       (20)      658 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8092 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/sdist.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5085 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/setopt.py
--rw-r--r--   0 linkerui   (501) staff       (20)     9623 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/test.py
--rw-r--r--   0 linkerui   (501) staff       (20)      462 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/upload.py
--rw-r--r--   0 linkerui   (501) staff       (20)     7314 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0 linkerui   (501) staff       (20)    21782 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/config.py
--rw-r--r--   0 linkerui   (501) staff       (20)      949 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/dep_util.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5517 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/depends.py
--rw-r--r--   0 linkerui   (501) staff       (20)    39350 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/dist.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1754 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/distutils_patch.py
--rw-r--r--   0 linkerui   (501) staff       (20)      524 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/errors.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1729 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/extension.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.490621 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/extern/
--rw-r--r--   0 linkerui   (501) staff       (20)     2128 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5084 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/glob.py
--rw-r--r--   0 linkerui   (501) staff       (20)    65536 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/gui-32.exe
--rw-r--r--   0 linkerui   (501) staff       (20)    75264 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/gui-64.exe
--rw-r--r--   0 linkerui   (501) staff       (20)    65536 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/gui.exe
--rw-r--r--   0 linkerui   (501) staff       (20)     5343 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/installer.py
--rw-r--r--   0 linkerui   (501) staff       (20)      812 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/launch.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2384 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/lib2to3_ex.py
--rw-r--r--   0 linkerui   (501) staff       (20)     5264 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/monkey.py
--rw-r--r--   0 linkerui   (501) staff       (20)    51225 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/msvc.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3223 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/namespaces.py
--rw-r--r--   0 linkerui   (501) staff       (20)    40777 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/package_index.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1504 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/py27compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)      838 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/py31compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1330 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/py33compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)      245 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/py34compat.py
--rw-r--r--   0 linkerui   (501) staff       (20)    14251 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/sandbox.py
--rw-r--r--   0 linkerui   (501) staff       (20)      218 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0 linkerui   (501) staff       (20)      138 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/script.tmpl
--rw-r--r--   0 linkerui   (501) staff       (20)     8543 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/ssl_support.py
--rw-r--r--   0 linkerui   (501) staff       (20)      996 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0 linkerui   (501) staff       (20)      144 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/version.py
--rw-r--r--   0 linkerui   (501) staff       (20)     8371 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/wheel.py
--rw-r--r--   0 linkerui   (501) staff       (20)      714 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/windows_support.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.425592 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/
--rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/INSTALLER
--rw-r--r--   0 linkerui   (501) staff       (20)     1078 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/LICENSE
--rw-r--r--   0 linkerui   (501) staff       (20)     4819 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/METADATA
--rw-r--r--   0 linkerui   (501) staff       (20)    37957 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/RECORD
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/REQUESTED
--rw-r--r--   0 linkerui   (501) staff       (20)       92 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/WHEEL
--rw-r--r--   0 linkerui   (501) staff       (20)      239 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/dependency_links.txt
--rw-r--r--   0 linkerui   (501) staff       (20)     3143 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/entry_points.txt
--rw-r--r--   0 linkerui   (501) staff       (20)       38 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/top_level.txt
--rw-r--r--   0 linkerui   (501) staff       (20)        1 2022-11-22 06:31:22.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/zip-safe
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.493688 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli/
--rw-r--r--   0 linkerui   (501) staff       (20)      396 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    22633 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli/_parser.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2943 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli/_re.py
--rw-r--r--   0 linkerui   (501) staff       (20)      254 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli/_types.py
--rw-r--r--   0 linkerui   (501) staff       (20)       26 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli/py.typed
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:15:52.495708 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/
--rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/INSTALLER
--rw-r--r--   0 linkerui   (501) staff       (20)     1072 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/LICENSE
--rw-r--r--   0 linkerui   (501) staff       (20)     8875 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/METADATA
--rw-r--r--   0 linkerui   (501) staff       (20)     1349 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/RECORD
--rw-r--r--   0 linkerui   (501) staff       (20)       81 2022-11-25 05:40:39.000000 txapi-1.0.1/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/WHEEL
--rw-r--r--   0 linkerui   (501) staff       (20)      104 2022-11-22 06:31:20.000000 txapi-1.0.1/venv/pyvenv.cfg
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.488251 txapi-1.0.2/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.948953 txapi-1.0.2/.git/
+-rw-r--r--   0 linkerui   (501) staff       (20)       18 2023-04-23 05:17:18.000000 txapi-1.0.2/.git/COMMIT_EDITMSG
+-rw-r--r--   0 linkerui   (501) staff       (20)      198 2023-04-23 04:55:42.000000 txapi-1.0.2/.git/FETCH_HEAD
+-rw-r--r--   0 linkerui   (501) staff       (20)       21 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/HEAD
+-rw-r--r--   0 linkerui   (501) staff       (20)       41 2022-11-25 05:52:32.000000 txapi-1.0.2/.git/ORIG_HEAD
+-rw-r--r--   0 linkerui   (501) staff       (20)      303 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/config
+-rw-r--r--   0 linkerui   (501) staff       (20)       73 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/description
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.953998 txapi-1.0.2/.git/hooks/
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      478 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      896 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)     4655 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      189 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/post-update.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      424 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)     1643 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      416 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)     1374 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)     4898 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      544 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)     1492 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)     2783 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 linkerui   (501) staff       (20)     3650 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/hooks/update.sample
+-rw-r--r--   0 linkerui   (501) staff       (20)     4288 2023-04-23 05:17:40.000000 txapi-1.0.2/.git/index
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.954374 txapi-1.0.2/.git/info/
+-rw-r--r--   0 linkerui   (501) staff       (20)      240 2022-11-22 04:39:00.000000 txapi-1.0.2/.git/info/exclude
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.954654 txapi-1.0.2/.git/logs/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1706 2023-04-23 05:17:18.000000 txapi-1.0.2/.git/logs/HEAD
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.903124 txapi-1.0.2/.git/logs/refs/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.955235 txapi-1.0.2/.git/logs/refs/heads/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1706 2023-04-23 05:17:18.000000 txapi-1.0.2/.git/logs/refs/heads/main
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.903231 txapi-1.0.2/.git/logs/refs/remotes/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.956818 txapi-1.0.2/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 linkerui   (501) staff       (20)      181 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0 linkerui   (501) staff       (20)     1178 2023-04-23 05:17:22.000000 txapi-1.0.2/.git/logs/refs/remotes/origin/main
+-rw-r--r--   0 linkerui   (501) staff       (20)      151 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/logs/refs/remotes/origin/py2
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.925478 txapi-1.0.2/.git/objects/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.958066 txapi-1.0.2/.git/objects/05/
+-r--r--r--   0 linkerui   (501) staff       (20)       52 2022-11-25 05:42:01.000000 txapi-1.0.2/.git/objects/05/693212a885904ca6a4c4438425d7bc57699092
+-r--r--r--   0 linkerui   (501) staff       (20)       73 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/05/7b61b6790d72490e44d5844499747c0e58cda5
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.958459 txapi-1.0.2/.git/objects/07/
+-r--r--r--   0 linkerui   (501) staff       (20)      162 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/07/97267a4911e4d2e38af27bba3114850a9cfaed
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.960129 txapi-1.0.2/.git/objects/08/
+-r--r--r--   0 linkerui   (501) staff       (20)       51 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/08/2b9381253bc157a355806bc4a2ac9070c72cce
+-r--r--r--   0 linkerui   (501) staff       (20)      285 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/08/35cd488581c2ca89e8cce1292218a8c66268e3
+-r--r--r--   0 linkerui   (501) staff       (20)      208 2023-04-10 09:59:52.000000 txapi-1.0.2/.git/objects/08/c677658838ab6c0c247c140a3b62bdba60c531
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.961546 txapi-1.0.2/.git/objects/0d/
+-r--r--r--   0 linkerui   (501) staff       (20)     1424 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/0d/db97d0b98ea46065d50f4c8b40363d97fbc843
+-r--r--r--   0 linkerui   (501) staff       (20)      101 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/0d/e79dff12acb51fbc10df4bed8167d9e8abddff
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.962307 txapi-1.0.2/.git/objects/0e/
+-r--r--r--   0 linkerui   (501) staff       (20)       85 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/0e/01571976474ceb8feae36a62d5effb8c04d73f
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.962923 txapi-1.0.2/.git/objects/0f/
+-r--r--r--   0 linkerui   (501) staff       (20)      366 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/0f/77e05fc0dfc799199f7f199d50a642fba481be
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.963598 txapi-1.0.2/.git/objects/11/
+-r--r--r--   0 linkerui   (501) staff       (20)      719 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/11/1e278133b448d8badadfd73e711d439c6b9abb
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.964243 txapi-1.0.2/.git/objects/12/
+-r--r--r--   0 linkerui   (501) staff       (20)      281 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/12/bd257f54fd5a04d5ee924d7a98780694f99d6c
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.965115 txapi-1.0.2/.git/objects/18/
+-r--r--r--   0 linkerui   (501) staff       (20)      118 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/18/8aefec4047a9000cb081850bd7c9b201a9aa96
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.965987 txapi-1.0.2/.git/objects/19/
+-r--r--r--   0 linkerui   (501) staff       (20)      553 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/19/d1b4f52378f26d4f82a9356b8ede80dcd54eb7
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.966544 txapi-1.0.2/.git/objects/1f/
+-r--r--r--   0 linkerui   (501) staff       (20)      285 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/1f/0cff2a4593a484a6e3549a2f4883d3a18d73bc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.967265 txapi-1.0.2/.git/objects/20/
+-r--r--r--   0 linkerui   (501) staff       (20)      286 2023-04-23 05:13:30.000000 txapi-1.0.2/.git/objects/20/2fe90f5cee5dacf2f361d7ac488e227d34bc7b
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.969394 txapi-1.0.2/.git/objects/21/
+-r--r--r--   0 linkerui   (501) staff       (20)      669 2023-04-10 09:59:52.000000 txapi-1.0.2/.git/objects/21/4c2ea36d2dde3af8296cb4037fb93734b56166
+-r--r--r--   0 linkerui   (501) staff       (20)      684 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/21/639dd781776e03375cd81804372559ba2e9bf9
+-r--r--r--   0 linkerui   (501) staff       (20)      253 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/21/a4f28d9a5ad8f6e09a92c16b3034cc980717a0
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.971910 txapi-1.0.2/.git/objects/23/
+-r--r--r--   0 linkerui   (501) staff       (20)       88 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/23/1286de323c67ae267b9b0957802e8112f8de97
+-r--r--r--   0 linkerui   (501) staff       (20)      556 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/23/398032b1b9804ab0dcba15248c71bb418737da
+-r--r--r--   0 linkerui   (501) staff       (20)      576 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/23/f661515e73b2b19d9af88e6bab4a169c46406e
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.972681 txapi-1.0.2/.git/objects/25/
+-r--r--r--   0 linkerui   (501) staff       (20)      123 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/25/ce766604a031638b2a1986140b7d5b94a01183
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.973283 txapi-1.0.2/.git/objects/26/
+-r--r--r--   0 linkerui   (501) staff       (20)      154 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/26/5dbfd4abbbe3deed4bfa548d10e5a0f2de2c7b
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.974057 txapi-1.0.2/.git/objects/2c/
+-r--r--r--   0 linkerui   (501) staff       (20)     1638 2023-04-23 04:56:44.000000 txapi-1.0.2/.git/objects/2c/c1a52cf5b91e50837f92540fa79b66bdbb7181
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.974769 txapi-1.0.2/.git/objects/2d/
+-r--r--r--   0 linkerui   (501) staff       (20)      180 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/2d/1924ef05bb89db7392ff247c87c00e8831068d
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.976126 txapi-1.0.2/.git/objects/2e/
+-r--r--r--   0 linkerui   (501) staff       (20)      343 2022-11-25 05:41:53.000000 txapi-1.0.2/.git/objects/2e/0d531f1af3317d56f2b066f9c214d6384cec11
+-r--r--r--   0 linkerui   (501) staff       (20)      124 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/2e/194e7ad8ae57ce0ec200288e5a81eefc99573c
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.976629 txapi-1.0.2/.git/objects/2f/
+-r--r--r--   0 linkerui   (501) staff       (20)       94 2023-04-10 09:59:52.000000 txapi-1.0.2/.git/objects/2f/53647fc1a53eadc41031f3844a13742be2125d
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.977310 txapi-1.0.2/.git/objects/30/
+-r--r--r--   0 linkerui   (501) staff       (20)      155 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/30/81b0e572b95da26032f088f543cdd98c76abe3
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.977792 txapi-1.0.2/.git/objects/31/
+-r--r--r--   0 linkerui   (501) staff       (20)      555 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/31/4296ca74424b305d04be227ad964afb86bf921
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.978422 txapi-1.0.2/.git/objects/32/
+-r--r--r--   0 linkerui   (501) staff       (20)     3750 2023-04-23 04:56:44.000000 txapi-1.0.2/.git/objects/32/8a62420ab81f87039d73e6ae31e5b1b54d3bde
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.979010 txapi-1.0.2/.git/objects/33/
+-r--r--r--   0 linkerui   (501) staff       (20)       89 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/33/bddaaaa0c46e95be3d138f52f31b60a7136b48
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.979971 txapi-1.0.2/.git/objects/34/
+-r--r--r--   0 linkerui   (501) staff       (20)      129 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/34/48bd09b982b355c07252c2f64c88601f40aa2c
+-r--r--r--   0 linkerui   (501) staff       (20)       37 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/34/4d17d14b8784e146028da8a18b21dad1c1bda3
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.980536 txapi-1.0.2/.git/objects/37/
+-r--r--r--   0 linkerui   (501) staff       (20)      321 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/37/36cb67cb324ab7d27524b9579c3e6a417fc06c
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.980917 txapi-1.0.2/.git/objects/39/
+-r--r--r--   0 linkerui   (501) staff       (20)       69 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/39/f3953903273862db7c100c5223913e413dca60
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.981992 txapi-1.0.2/.git/objects/3e/
+-r--r--r--   0 linkerui   (501) staff       (20)      155 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/3e/5c111da00b1d6a2c4201572795a4b068ec9c9f
+-r--r--r--   0 linkerui   (501) staff       (20)      112 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/3e/e7ef9c853280632b3a27c9599b5a842a0b1967
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.982371 txapi-1.0.2/.git/objects/3f/
+-r--r--r--   0 linkerui   (501) staff       (20)     1506 2022-11-25 05:41:53.000000 txapi-1.0.2/.git/objects/3f/03a1b9319f3c3d9941d7ae256b81e045b42363
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.982949 txapi-1.0.2/.git/objects/40/
+-r--r--r--   0 linkerui   (501) staff       (20)       38 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/40/a96afc6ff09d58a702b76e3f7dd412fe975e26
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.983967 txapi-1.0.2/.git/objects/41/
+-r--r--r--   0 linkerui   (501) staff       (20)      170 2022-11-25 05:42:01.000000 txapi-1.0.2/.git/objects/41/62b43e34e8a87d50e492a2f513b5f98fc38ef7
+-r--r--r--   0 linkerui   (501) staff       (20)      153 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/41/7a59650920676ff59e7d08f927fa8ed6504aa5
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.984356 txapi-1.0.2/.git/objects/45/
+-r--r--r--   0 linkerui   (501) staff       (20)      619 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/45/219397fd4a9c0cb4ac7ac9018b67b54ba2ef36
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.984739 txapi-1.0.2/.git/objects/46/
+-r--r--r--   0 linkerui   (501) staff       (20)      247 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/46/86143cf8e1c6484b70f3322e32c014c6ee8d86
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.985619 txapi-1.0.2/.git/objects/47/
+-r--r--r--   0 linkerui   (501) staff       (20)      647 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/47/1c3d59784a99eb3429ccbd100c7038f4859d54
+-r--r--r--   0 linkerui   (501) staff       (20)       52 2022-11-25 05:52:30.000000 txapi-1.0.2/.git/objects/47/af7a7c8fe1b9c9da61f5959fed451074291b68
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.986292 txapi-1.0.2/.git/objects/4c/
+-r--r--r--   0 linkerui   (501) staff       (20)      362 2023-04-10 09:59:52.000000 txapi-1.0.2/.git/objects/4c/e483925dea807e85f64038ec99e73a5cd46d15
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.987347 txapi-1.0.2/.git/objects/4e/
+-r--r--r--   0 linkerui   (501) staff       (20)       89 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/4e/610856bd88c524f7faae8f05004b0736c95ed6
+-r--r--r--   0 linkerui   (501) staff       (20)      154 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/4e/e6209932e8c5b6f62f8be128c50655c5a691a4
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.987744 txapi-1.0.2/.git/objects/50/
+-r--r--r--   0 linkerui   (501) staff       (20)      301 2023-01-19 02:38:08.000000 txapi-1.0.2/.git/objects/50/7d622c92776e098ae53f1fad82e0623c208335
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.988801 txapi-1.0.2/.git/objects/54/
+-r--r--r--   0 linkerui   (501) staff       (20)      150 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/54/1ebdcb8976304f04e1e9e52ab8a5e19f4084c5
+-r--r--r--   0 linkerui   (501) staff       (20)      118 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/54/a80afb631926239ffd81091bb558a592735749
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.989237 txapi-1.0.2/.git/objects/57/
+-r--r--r--   0 linkerui   (501) staff       (20)      574 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/57/940bdb0c48ade22baee7f4d5775cbbf3334d90
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.990033 txapi-1.0.2/.git/objects/58/
+-r--r--r--   0 linkerui   (501) staff       (20)      418 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/58/1a24d98cc8f2a900be6bae0b4679c459453f92
+-r--r--r--   0 linkerui   (501) staff       (20)      286 2023-04-23 05:07:43.000000 txapi-1.0.2/.git/objects/58/3f3db9002c6864c1ae3a75e2d74576e7489224
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.990600 txapi-1.0.2/.git/objects/59/
+-r--r--r--   0 linkerui   (501) staff       (20)     1455 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/59/6c581887f06e9ab622345a9191e3e09732cc7b
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.991031 txapi-1.0.2/.git/objects/5b/
+-r--r--r--   0 linkerui   (501) staff       (20)      286 2023-04-10 09:59:52.000000 txapi-1.0.2/.git/objects/5b/5a1fea3d4818c5e9ce7087044fb384596b43e3
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.991685 txapi-1.0.2/.git/objects/5d/
+-r--r--r--   0 linkerui   (501) staff       (20)      281 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/5d/2b6865cbe0450ad11d4fc2cf18706721248b9f
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.992209 txapi-1.0.2/.git/objects/63/
+-r--r--r--   0 linkerui   (501) staff       (20)      730 2023-04-23 05:07:43.000000 txapi-1.0.2/.git/objects/63/096a2158e3f8361a3f51091f9fa8008c688049
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.993258 txapi-1.0.2/.git/objects/64/
+-r--r--r--   0 linkerui   (501) staff       (20)      248 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/64/48e904dcb43254931d1af079c489e4edfa02ed
+-r--r--r--   0 linkerui   (501) staff       (20)      286 2023-01-19 02:38:08.000000 txapi-1.0.2/.git/objects/64/bb73d61ba8e23ded6723a0c0a199d528d88a9a
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.994664 txapi-1.0.2/.git/objects/65/
+-r--r--r--   0 linkerui   (501) staff       (20)      126 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/65/7089684405c08caf3d94dc656ef8e932742f42
+-r--r--r--   0 linkerui   (501) staff       (20)       89 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/65/be0c194324589fdd100ecf5da077daa823c38d
+-r--r--r--   0 linkerui   (501) staff       (20)       86 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/65/c8f6514aaf92c8378cfdd08f351eed76b5404f
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.995462 txapi-1.0.2/.git/objects/67/
+-r--r--r--   0 linkerui   (501) staff       (20)       89 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/67/24f268cd8d3dd7e85ee640867ae4c43c40d8b7
+-r--r--r--   0 linkerui   (501) staff       (20)      519 2023-04-23 05:07:43.000000 txapi-1.0.2/.git/objects/67/39f71ac4becbfda86f98d6b3ae1a4be3d60ad9
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.996042 txapi-1.0.2/.git/objects/68/
+-r--r--r--   0 linkerui   (501) staff       (20)      179 2023-01-19 02:38:08.000000 txapi-1.0.2/.git/objects/68/e2761b38d12e84388046a201fb494de7ecda8c
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.996674 txapi-1.0.2/.git/objects/69/
+-r--r--r--   0 linkerui   (501) staff       (20)      301 2023-04-23 04:56:44.000000 txapi-1.0.2/.git/objects/69/a95ad1e84427ae51b0e79743e99e5733a654fe
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.997281 txapi-1.0.2/.git/objects/6b/
+-r--r--r--   0 linkerui   (501) staff       (20)       86 2023-04-23 05:07:43.000000 txapi-1.0.2/.git/objects/6b/75c847a627117b395900264ed87e18b55fdd11
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.997854 txapi-1.0.2/.git/objects/6c/
+-r--r--r--   0 linkerui   (501) staff       (20)      559 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/6c/4a1313e8ec893fc2ebd5d3b3efce63d11f73db
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.999310 txapi-1.0.2/.git/objects/6d/
+-r--r--r--   0 linkerui   (501) staff       (20)       94 2022-11-25 05:42:01.000000 txapi-1.0.2/.git/objects/6d/0dbb49aca3b25be77017accb1a6b9cc75bd5f5
+-r--r--r--   0 linkerui   (501) staff       (20)       89 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/6d/b7727950e8b5aed41400abf51ec3a0fe53358e
+-r--r--r--   0 linkerui   (501) staff       (20)      286 2022-11-25 05:42:01.000000 txapi-1.0.2/.git/objects/6d/e48d16e8398658c1e1541bfdb450847d976398
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.999899 txapi-1.0.2/.git/objects/71/
+-r--r--r--   0 linkerui   (501) staff       (20)      287 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/71/69e48c7afb39b6fa8a868be27cb4626de23fa1
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.000267 txapi-1.0.2/.git/objects/72/
+-r--r--r--   0 linkerui   (501) staff       (20)      128 2023-04-23 05:13:30.000000 txapi-1.0.2/.git/objects/72/f76904d91e580dd0b5f70ee565b4c2ffa79734
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.001081 txapi-1.0.2/.git/objects/73/
+-r--r--r--   0 linkerui   (501) staff       (20)      107 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/73/4e1cee7f9f3a49efb7e389dbd6c74c56813677
+-r--r--r--   0 linkerui   (501) staff       (20)      108 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/73/d41923e7cb9369bd5363d0410814474a9e3009
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.001460 txapi-1.0.2/.git/objects/75/
+-r--r--r--   0 linkerui   (501) staff       (20)     1605 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/75/fe7a3d3ccbdaec7b3b95d4c7c44ecee3ed92f3
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.002297 txapi-1.0.2/.git/objects/76/
+-r--r--r--   0 linkerui   (501) staff       (20)      653 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/76/0aade4935e771a96525aa507d60f72614c5da6
+-r--r--r--   0 linkerui   (501) staff       (20)      167 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/76/353b844acf336aa586ec8d94c3019017948802
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.002871 txapi-1.0.2/.git/objects/77/
+-r--r--r--   0 linkerui   (501) staff       (20)      223 2023-04-23 04:56:44.000000 txapi-1.0.2/.git/objects/77/b3e410890f76b6d46395e3378e3ddf86f46edd
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.004019 txapi-1.0.2/.git/objects/78/
+-r--r--r--   0 linkerui   (501) staff       (20)      655 2022-11-25 05:52:30.000000 txapi-1.0.2/.git/objects/78/68afd1318032499383a82f4a2b458791e7b990
+-r--r--r--   0 linkerui   (501) staff       (20)     3716 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/78/a660592bc694a40b5248e0549c066483452c7a
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.004417 txapi-1.0.2/.git/objects/79/
+-r--r--r--   0 linkerui   (501) staff       (20)      285 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/79/21604e32ec96a87935f84fa75b6de1e1ae400c
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.005379 txapi-1.0.2/.git/objects/7a/
+-r--r--r--   0 linkerui   (501) staff       (20)      301 2023-04-23 05:07:43.000000 txapi-1.0.2/.git/objects/7a/6d83033af302a944ab27fd7580d33ef12de5f7
+-r--r--r--   0 linkerui   (501) staff       (20)      426 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/7a/9553cfe8d189140ffb4739b9def6eddd2b05ae
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.005858 txapi-1.0.2/.git/objects/7e/
+-r--r--r--   0 linkerui   (501) staff       (20)      157 2023-01-19 02:38:08.000000 txapi-1.0.2/.git/objects/7e/9e25992722a214ac1c4450faa8af6361190eb6
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.006484 txapi-1.0.2/.git/objects/7f/
+-r--r--r--   0 linkerui   (501) staff       (20)      155 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/7f/164528f0ea755e2bbf70cba5ca83d51fab1f56
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.007795 txapi-1.0.2/.git/objects/80/
+-r--r--r--   0 linkerui   (501) staff       (20)      465 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/80/0b22e14afd5501a6a46cc7dccf6eb32e0f206f
+-r--r--r--   0 linkerui   (501) staff       (20)     1472 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/80/5cc728900be707de58af039739e01221353528
+-r--r--r--   0 linkerui   (501) staff       (20)     1605 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/80/b07b0c161d95297f1a537db880d0e98acad82d
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.008176 txapi-1.0.2/.git/objects/81/
+-r--r--r--   0 linkerui   (501) staff       (20)      286 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/81/b6056b9090ed2622e20ab2d91bd989a2ed1a03
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.008600 txapi-1.0.2/.git/objects/82/
+-r--r--r--   0 linkerui   (501) staff       (20)     1477 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/82/63ddf91052bfe6c6af092051fafc077d86476c
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.009509 txapi-1.0.2/.git/objects/87/
+-r--r--r--   0 linkerui   (501) staff       (20)      510 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/87/5310a549269b17f68963634a0c2da344ba245f
+-r--r--r--   0 linkerui   (501) staff       (20)       85 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/87/c8b64913054035a4c8f8d0578f24e0d12955ea
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.009894 txapi-1.0.2/.git/objects/88/
+-r--r--r--   0 linkerui   (501) staff       (20)      287 2023-01-19 02:38:08.000000 txapi-1.0.2/.git/objects/88/6515f9316155f3954ae1a4a60f4cf3641165d0
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.010817 txapi-1.0.2/.git/objects/89/
+-r--r--r--   0 linkerui   (501) staff       (20)      352 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/89/391fb26eb5246ed340f53390899c6f71336231
+-r--r--r--   0 linkerui   (501) staff       (20)       39 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/89/7e3130d7653b12be4087a2eb9868f0162974dc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.012606 txapi-1.0.2/.git/objects/8d/
+-r--r--r--   0 linkerui   (501) staff       (20)     1490 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/8d/1cdd3e52ed567f61e45e6fcc4feefde445c9e3
+-r--r--r--   0 linkerui   (501) staff       (20)      301 2023-04-23 05:13:30.000000 txapi-1.0.2/.git/objects/8d/213a3f1b9d2f3de20df4e41a55b179fdfa249b
+-r--r--r--   0 linkerui   (501) staff       (20)      301 2023-01-19 02:38:08.000000 txapi-1.0.2/.git/objects/8d/b3bf09a5f6fe8c4ff29fdb9a5f70475b4a1adc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.013206 txapi-1.0.2/.git/objects/93/
+-r--r--r--   0 linkerui   (501) staff       (20)      240 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/93/7db38a1c9decf1ddfbfaef0718b7cf0976dc14
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.013871 txapi-1.0.2/.git/objects/95/
+-r--r--r--   0 linkerui   (501) staff       (20)      285 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/95/66a4df3edd828dfddeda104d238e0386738e90
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.015472 txapi-1.0.2/.git/objects/99/
+-r--r--r--   0 linkerui   (501) staff       (20)      598 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/99/639a2389a1ee50ace8a7ebfeb6a848085b3ae1
+-r--r--r--   0 linkerui   (501) staff       (20)      108 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/99/649150e602754bbdf1cceca82f7ae0042aad43
+-r--r--r--   0 linkerui   (501) staff       (20)      128 2022-11-25 05:52:30.000000 txapi-1.0.2/.git/objects/99/e16eaed48da0fa2a08af4eba2ab8b8dcd11ac0
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.017082 txapi-1.0.2/.git/objects/9a/
+-r--r--r--   0 linkerui   (501) staff       (20)      301 2022-11-25 05:52:30.000000 txapi-1.0.2/.git/objects/9a/396ba470231fa2cf1a0be23f6c16c2cf807dc0
+-r--r--r--   0 linkerui   (501) staff       (20)     3724 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/9a/74267b066cb21fc0a23b33cd3990bc13f9ba1d
+-r--r--r--   0 linkerui   (501) staff       (20)     1944 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/9a/ca49ad39bb6aabb57d014726a4a2433206ecc7
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.018170 txapi-1.0.2/.git/objects/9e/
+-r--r--r--   0 linkerui   (501) staff       (20)      168 2022-11-25 05:52:30.000000 txapi-1.0.2/.git/objects/9e/336bd58fc96bb88e2b9a86bdcb6971652394b4
+-r--r--r--   0 linkerui   (501) staff       (20)      672 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/9e/d55bad89de367003e0a538b16e6c79d32db508
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.019197 txapi-1.0.2/.git/objects/a2/
+-r--r--r--   0 linkerui   (501) staff       (20)      643 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/a2/30bd6c3fe5539caed2f8b2b0865c6deea1a026
+-r--r--r--   0 linkerui   (501) staff       (20)       31 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/a2/aca1c77e4889bbdba02e722430d6a69a14c2a0
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.019724 txapi-1.0.2/.git/objects/a3/
+-r--r--r--   0 linkerui   (501) staff       (20)      961 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/a3/68a8a8fd04e25b619adb09c2bee7ad676d3185
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.020316 txapi-1.0.2/.git/objects/a5/
+-r--r--r--   0 linkerui   (501) staff       (20)      696 2023-04-23 04:56:44.000000 txapi-1.0.2/.git/objects/a5/07a598601aea15d6abaafe7bad6ad10e2b22d7
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.021084 txapi-1.0.2/.git/objects/a6/
+-r--r--r--   0 linkerui   (501) staff       (20)     1938 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/a6/6d48d9f7ef0c81494621de192b567705157436
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.022701 txapi-1.0.2/.git/objects/a7/
+-r--r--r--   0 linkerui   (501) staff       (20)      340 2023-04-23 05:13:30.000000 txapi-1.0.2/.git/objects/a7/7cbef8139fd72d2421e1fbef4b7433022e6683
+-r--r--r--   0 linkerui   (501) staff       (20)     1491 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/a7/826960973f479a98bd49313e881c5e93393e38
+-r--r--r--   0 linkerui   (501) staff       (20)      154 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/a7/b67376b5ff945537da897b0091bf8de9424ec0
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.023341 txapi-1.0.2/.git/objects/a9/
+-r--r--r--   0 linkerui   (501) staff       (20)      339 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/a9/00b9fb2f23ed04d28847f0f78a9abdc6b12595
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.023824 txapi-1.0.2/.git/objects/ad/
+-r--r--r--   0 linkerui   (501) staff       (20)      648 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/ad/91fa7d37aa37e20fe58076725790e8aae43bc0
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.024867 txapi-1.0.2/.git/objects/b1/
+-r--r--r--   0 linkerui   (501) staff       (20)       85 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/b1/21761178ea0098e11e96a2467f97a80f50d3b6
+-r--r--r--   0 linkerui   (501) staff       (20)      251 2023-04-23 05:07:43.000000 txapi-1.0.2/.git/objects/b1/ee6c481e8ce3a307c0983b487a610bbdd7e065
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.025865 txapi-1.0.2/.git/objects/b2/
+-r--r--r--   0 linkerui   (501) staff       (20)      287 2023-04-23 05:17:18.000000 txapi-1.0.2/.git/objects/b2/1dc75cb439396e8215e6ae76e4be281da4549f
+-r--r--r--   0 linkerui   (501) staff       (20)      285 2023-04-23 04:56:44.000000 txapi-1.0.2/.git/objects/b2/442748fb5ccb3f5801c5dffbb8f8050aff47a6
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.026614 txapi-1.0.2/.git/objects/b3/
+-r--r--r--   0 linkerui   (501) staff       (20)      262 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/b3/2da2543d266ca57a7a7072d8a1aa7906a5216f
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.027091 txapi-1.0.2/.git/objects/b4/
+-r--r--r--   0 linkerui   (501) staff       (20)     1489 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/b4/09333c2ea63b578a3d08486be3d6e7a44edc7d
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.027527 txapi-1.0.2/.git/objects/b6/
+-r--r--r--   0 linkerui   (501) staff       (20)     1011 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/b6/e47617de110dea7ca47e087ff1347cc2646eda
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.027937 txapi-1.0.2/.git/objects/b8/
+-r--r--r--   0 linkerui   (501) staff       (20)      181 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/b8/1cd0c71144089c01e5d12b5a82dfcf30feece7
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.028360 txapi-1.0.2/.git/objects/bb/
+-r--r--r--   0 linkerui   (501) staff       (20)      343 2022-11-25 05:52:30.000000 txapi-1.0.2/.git/objects/bb/4b30a3ec4305961374dbfa727156c77028a5fb
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.028921 txapi-1.0.2/.git/objects/bd/
+-r--r--r--   0 linkerui   (501) staff       (20)      205 2023-04-23 05:13:30.000000 txapi-1.0.2/.git/objects/bd/767b09e07988677a46bff99a44334cb802325c
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.029393 txapi-1.0.2/.git/objects/be/
+-r--r--r--   0 linkerui   (501) staff       (20)       88 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/be/9930fc9a74f5ef498dc7de5fb3b48305e261d7
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.029806 txapi-1.0.2/.git/objects/c2/
+-r--r--r--   0 linkerui   (501) staff       (20)      339 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/c2/e715407eb2cadf53bd3266569043104528db0c
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.031176 txapi-1.0.2/.git/objects/c4/
+-r--r--r--   0 linkerui   (501) staff       (20)      281 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/c4/1329695facbe88753632a6626d521e7136a37e
+-r--r--r--   0 linkerui   (501) staff       (20)      603 2022-11-25 05:41:53.000000 txapi-1.0.2/.git/objects/c4/72d537837ad718aac848eb955f676a87e7f2ac
+-r--r--r--   0 linkerui   (501) staff       (20)      156 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/c4/be97a7166b002dd20894cacbbc6538e90acf88
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.031558 txapi-1.0.2/.git/objects/c6/
+-r--r--r--   0 linkerui   (501) staff       (20)      157 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/c6/7675076ec28c750826f7e5f2170122b8a9d3a3
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.032082 txapi-1.0.2/.git/objects/c9/
+-r--r--r--   0 linkerui   (501) staff       (20)      348 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/c9/98aaf6c57e4dd8fd55cdc45f84f7e8ccdad887
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.032802 txapi-1.0.2/.git/objects/cd/
+-r--r--r--   0 linkerui   (501) staff       (20)      300 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/cd/316e3e2823326d2d79e861a63228b0c5cf538e
+-r--r--r--   0 linkerui   (501) staff       (20)     1944 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/cd/8c8e7cb1c8eb8308a1a70cb48320fdc1db3362
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.033986 txapi-1.0.2/.git/objects/cf/
+-r--r--r--   0 linkerui   (501) staff       (20)      106 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/cf/1cd7c9a8eed6d7785ec1f54ebf3737df1c40cf
+-r--r--r--   0 linkerui   (501) staff       (20)       52 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/cf/2f8da95e46dbe88e67d6b28cfb2bcf3e092b35
+-r--r--r--   0 linkerui   (501) staff       (20)       94 2022-11-25 05:52:30.000000 txapi-1.0.2/.git/objects/cf/30c4ebc092f87f24d127e1724aeead7aeef57f
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.034547 txapi-1.0.2/.git/objects/d0/
+-r--r--r--   0 linkerui   (501) staff       (20)      169 2023-04-23 05:17:18.000000 txapi-1.0.2/.git/objects/d0/4393b23abcbfb5b566a634f27c764ae6019bc3
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.035689 txapi-1.0.2/.git/objects/d1/
+-r--r--r--   0 linkerui   (501) staff       (20)     1630 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/d1/30c07e14b682ef444d69930acc214185c9b7db
+-r--r--r--   0 linkerui   (501) staff       (20)      240 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/d1/7eb6ac8a7f6a3a69d8254e6fbf552231a0054f
+-r--r--r--   0 linkerui   (501) staff       (20)       89 2023-04-23 04:56:44.000000 txapi-1.0.2/.git/objects/d1/d56662595333e313eb7bd388cfab40e7fa2a35
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.036229 txapi-1.0.2/.git/objects/d2/
+-r--r--r--   0 linkerui   (501) staff       (20)      126 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/d2/27a48e81fb6f771f6296665b55d379f3569f5c
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.036709 txapi-1.0.2/.git/objects/d4/
+-r--r--r--   0 linkerui   (501) staff       (20)      126 2023-04-23 04:56:44.000000 txapi-1.0.2/.git/objects/d4/7949ca42ff77a9f570b08a634182b151695b71
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.037921 txapi-1.0.2/.git/objects/d5/
+-r--r--r--   0 linkerui   (501) staff       (20)      286 2022-11-25 05:52:30.000000 txapi-1.0.2/.git/objects/d5/9480059d62735163c88bf127d8f0ca49546a0f
+-r--r--r--   0 linkerui   (501) staff       (20)      711 2023-04-23 05:17:18.000000 txapi-1.0.2/.git/objects/d5/ee3d14ff70e43fec57164fe9c1f4b40aedeae9
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.038505 txapi-1.0.2/.git/objects/d6/
+-r--r--r--   0 linkerui   (501) staff       (20)       51 2023-04-10 09:59:52.000000 txapi-1.0.2/.git/objects/d6/f0964f2c224afc19e38192e2debdafeeba6acd
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.039127 txapi-1.0.2/.git/objects/d8/
+-r--r--r--   0 linkerui   (501) staff       (20)      287 2023-04-23 04:56:44.000000 txapi-1.0.2/.git/objects/d8/3e2b6fb80b632a01e951072e47598c70125249
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.039687 txapi-1.0.2/.git/objects/d9/
+-r--r--r--   0 linkerui   (501) staff       (20)      643 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/d9/5dcf7e5be1da655caf43d16bfa1735477497a0
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.040092 txapi-1.0.2/.git/objects/da/
+-r--r--r--   0 linkerui   (501) staff       (20)      300 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/da/55f873a9f0769f4616f797953c71860a97381c
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.040469 txapi-1.0.2/.git/objects/db/
+-r--r--r--   0 linkerui   (501) staff       (20)      320 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/db/0c553587cb305847d9db53169807ca0e641b03
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.041415 txapi-1.0.2/.git/objects/de/
+-r--r--r--   0 linkerui   (501) staff       (20)     1614 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/de/07e2c3445f2d8965343f0aa6099392f0ba0c52
+-r--r--r--   0 linkerui   (501) staff       (20)       51 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/de/39cf37ad954d80ed5175810061a060c7ccc48d
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.042257 txapi-1.0.2/.git/objects/df/
+-r--r--r--   0 linkerui   (501) staff       (20)     1489 2023-01-19 02:38:08.000000 txapi-1.0.2/.git/objects/df/6c3c8d9fa2fd045230e7d7be1b2b81ad15799f
+-r--r--r--   0 linkerui   (501) staff       (20)      509 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/df/f1fb8aad73a25844ffb6765ea30040e1e84432
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.043035 txapi-1.0.2/.git/objects/e0/
+-r--r--r--   0 linkerui   (501) staff       (20)       94 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/e0/843780558164d7300a78c2a170908b1533768f
+-r--r--r--   0 linkerui   (501) staff       (20)      622 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/e0/db285333f977126d50cb01bef5f83bade2d169
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.043512 txapi-1.0.2/.git/objects/e1/
+-r--r--r--   0 linkerui   (501) staff       (20)      451 2023-04-23 05:13:30.000000 txapi-1.0.2/.git/objects/e1/f9c3c0091160776f8bf8e555af4c60a93daee8
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.044193 txapi-1.0.2/.git/objects/e6/
+-r--r--r--   0 linkerui   (501) staff       (20)      369 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/e6/9897651f87fd20adc69f034578a3a8419aa079
+-r--r--r--   0 linkerui   (501) staff       (20)       15 2023-04-23 05:17:40.000000 txapi-1.0.2/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.044480 txapi-1.0.2/.git/objects/e8/
+-r--r--r--   0 linkerui   (501) staff       (20)      461 2023-01-19 02:38:08.000000 txapi-1.0.2/.git/objects/e8/0552c62017ce1d42489c842a6758cc9fa85d42
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.046282 txapi-1.0.2/.git/objects/e9/
+-r--r--r--   0 linkerui   (501) staff       (20)     1489 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/e9/09aa2ff53b15d535bcc2de16de52134b952aec
+-r--r--r--   0 linkerui   (501) staff       (20)      450 2023-04-23 05:07:43.000000 txapi-1.0.2/.git/objects/e9/1cfc3308bd4c05146f1a135c3399d8cde82e4a
+-r--r--r--   0 linkerui   (501) staff       (20)      273 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/e9/c8b75c83886fab11d8c53fbe5be76a8263c255
+-r--r--r--   0 linkerui   (501) staff       (20)      180 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/e9/deadcf54da359adb62450efe4ca831b7d76153
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.046661 txapi-1.0.2/.git/objects/ec/
+-r--r--r--   0 linkerui   (501) staff       (20)     1019 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/ec/7d22521aa69ab0c5fbea87d1157d781d0aebe6
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.047123 txapi-1.0.2/.git/objects/ed/
+-r--r--r--   0 linkerui   (501) staff       (20)       86 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/ed/fcf1e4aa1dc35d7e84d5a81bbd15d73c2e3157
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.048303 txapi-1.0.2/.git/objects/ef/
+-r--r--r--   0 linkerui   (501) staff       (20)      126 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/ef/21f242632e536036d59f053ebf3382ff8da058
+-r--r--r--   0 linkerui   (501) staff       (20)      128 2023-01-19 02:38:08.000000 txapi-1.0.2/.git/objects/ef/4273e19f2cc3caae8ba7c70a9f56269b02fc01
+-r--r--r--   0 linkerui   (501) staff       (20)      610 2022-11-25 05:52:30.000000 txapi-1.0.2/.git/objects/ef/586010c625011d458db7e684a425fcbd1012f1
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.048946 txapi-1.0.2/.git/objects/f3/
+-r--r--r--   0 linkerui   (501) staff       (20)      615 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/f3/7b0ee455cd0876fd2a4a12adf4f70cb9855596
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.049333 txapi-1.0.2/.git/objects/f4/
+-r--r--r--   0 linkerui   (501) staff       (20)       69 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/f4/9646aeef73b2c0107deed1cc8bf6bc31097917
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.049726 txapi-1.0.2/.git/objects/f6/
+-r--r--r--   0 linkerui   (501) staff       (20)      646 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/objects/f6/f35d7b623a39e2342b860f6f080fe5d8275bd5
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.050101 txapi-1.0.2/.git/objects/fe/
+-r--r--r--   0 linkerui   (501) staff       (20)      647 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/fe/a22029fd4d0cc03ab16a60109fb3f928dd7747
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.050528 txapi-1.0.2/.git/objects/ff/
+-r--r--r--   0 linkerui   (501) staff       (20)     3721 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/objects/ff/3ba9f30b5aa2f45cbcd01a1b08be357c8f22cb
+-rw-r--r--   0 linkerui   (501) staff       (20)      112 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/packed-refs
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.925953 txapi-1.0.2/.git/refs/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.050946 txapi-1.0.2/.git/refs/heads/
+-rw-r--r--   0 linkerui   (501) staff       (20)       41 2023-04-23 05:17:18.000000 txapi-1.0.2/.git/refs/heads/main
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.926060 txapi-1.0.2/.git/refs/remotes/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.051811 txapi-1.0.2/.git/refs/remotes/origin/
+-rw-r--r--   0 linkerui   (501) staff       (20)       30 2022-11-22 04:39:01.000000 txapi-1.0.2/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0 linkerui   (501) staff       (20)       41 2023-04-23 05:17:22.000000 txapi-1.0.2/.git/refs/remotes/origin/main
+-rw-r--r--   0 linkerui   (501) staff       (20)       41 2022-11-25 05:04:04.000000 txapi-1.0.2/.git/refs/remotes/origin/py2
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.926352 txapi-1.0.2/.github/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.052737 txapi-1.0.2/.github/workflows/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1143 2022-11-25 05:47:59.000000 txapi-1.0.2/.github/workflows/python-package-conda.yml
+-rw-r--r--   0 linkerui   (501) staff       (20)     1351 2023-04-10 09:59:30.000000 txapi-1.0.2/.github/workflows/python-package.yml
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.055642 txapi-1.0.2/.idea/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.056641 txapi-1.0.2/.idea/inspectionProfiles/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1382 2023-01-31 07:15:19.000000 txapi-1.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 linkerui   (501) staff       (20)      174 2023-01-31 07:15:19.000000 txapi-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 linkerui   (501) staff       (20)      185 2023-01-31 07:15:19.000000 txapi-1.0.2/.idea/misc.xml
+-rw-r--r--   0 linkerui   (501) staff       (20)      262 2023-01-31 07:15:19.000000 txapi-1.0.2/.idea/modules.xml
+-rw-r--r--   0 linkerui   (501) staff       (20)      555 2023-01-31 07:15:47.000000 txapi-1.0.2/.idea/txapi.iml
+-rw-r--r--   0 linkerui   (501) staff       (20)      180 2023-01-31 07:15:19.000000 txapi-1.0.2/.idea/vcs.xml
+-rw-r--r--   0 linkerui   (501) staff       (20)    12400 2023-04-23 05:17:49.000000 txapi-1.0.2/.idea/workspace.xml
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.058476 txapi-1.0.2/.pytest_cache/
+-rw-r--r--   0 linkerui   (501) staff       (20)       36 2022-11-25 05:04:56.000000 txapi-1.0.2/.pytest_cache/.gitignore
+-rw-r--r--   0 linkerui   (501) staff       (20)      194 2022-11-25 05:04:56.000000 txapi-1.0.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 linkerui   (501) staff       (20)      295 2022-11-25 05:04:56.000000 txapi-1.0.2/.pytest_cache/README.md
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.927151 txapi-1.0.2/.pytest_cache/v/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.060011 txapi-1.0.2/.pytest_cache/v/cache/
+-rw-r--r--   0 linkerui   (501) staff       (20)       64 2022-11-25 05:37:01.000000 txapi-1.0.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 linkerui   (501) staff       (20)      244 2022-11-25 05:51:36.000000 txapi-1.0.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 linkerui   (501) staff       (20)        2 2022-11-25 05:51:36.000000 txapi-1.0.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 linkerui   (501) staff       (20)     1065 2022-11-22 04:39:01.000000 txapi-1.0.2/LICENSE
+-rw-r--r--   0 linkerui   (501) staff       (20)       23 2022-11-22 04:39:01.000000 txapi-1.0.2/MANIFEST.in
+-rw-r--r--   0 linkerui   (501) staff       (20)     1474 2023-04-23 05:17:52.488009 txapi-1.0.2/PKG-INFO
+-rw-r--r--   0 linkerui   (501) staff       (20)     1182 2023-04-23 05:17:03.000000 txapi-1.0.2/README.md
+-rw-r--r--   0 linkerui   (501) staff       (20)       38 2023-04-23 05:17:52.488350 txapi-1.0.2/setup.cfg
+-rw-r--r--   0 linkerui   (501) staff       (20)      811 2023-04-23 05:17:49.000000 txapi-1.0.2/setup.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.065874 txapi-1.0.2/txapi/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.070701 txapi-1.0.2/txapi/QcloudApi/
+-rw-r--r--   0 linkerui   (501) staff       (20)       23 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/QcloudApi/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      184 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/QcloudApi/__init__.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.072253 txapi-1.0.2/txapi/QcloudApi/__pycache__/
+-rw-r--r--   0 linkerui   (501) staff       (20)      186 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/QcloudApi/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     2391 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/QcloudApi/__pycache__/qcloudapi.cpython-39.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.076856 txapi-1.0.2/txapi/QcloudApi/common/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/QcloudApi/common/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      158 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/QcloudApi/common/__init__.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.079010 txapi-1.0.2/txapi/QcloudApi/common/__pycache__/
+-rw-r--r--   0 linkerui   (501) staff       (20)      171 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/QcloudApi/common/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     2693 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/QcloudApi/common/__pycache__/api_exception.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     5920 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/QcloudApi/common/__pycache__/request.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1444 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/QcloudApi/common/__pycache__/sign.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1381 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/QcloudApi/common/api_exception.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3594 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/QcloudApi/common/api_exception.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     6117 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/QcloudApi/common/request.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7845 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/QcloudApi/common/request.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1197 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/QcloudApi/common/sign.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1937 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/QcloudApi/common/sign.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.080875 txapi-1.0.2/txapi/QcloudApi/modules/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/QcloudApi/modules/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      159 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/QcloudApi/modules/__init__.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.081987 txapi-1.0.2/txapi/QcloudApi/modules/__pycache__/
+-rw-r--r--   0 linkerui   (501) staff       (20)      172 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/QcloudApi/modules/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     4455 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/QcloudApi/modules/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     5684 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/QcloudApi/modules/base.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5939 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/QcloudApi/modules/base.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1763 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/QcloudApi/qcloudapi.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3067 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/QcloudApi/qcloudapi.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)      130 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      503 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/__init__.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.084113 txapi-1.0.2/txapi/__pycache__/
+-rw-r--r--   0 linkerui   (501) staff       (20)      426 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     3844 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/__pycache__/api2.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     4360 2023-04-23 05:12:11.000000 txapi-1.0.2/txapi/__pycache__/api3.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)      302 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/__pycache__/version.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     4130 2022-11-25 05:39:33.000000 txapi-1.0.2/txapi/api2.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4773 2022-11-25 05:40:23.000000 txapi-1.0.2/txapi/api2.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     4992 2023-04-23 04:27:16.000000 txapi-1.0.2/txapi/api3.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5155 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/api3.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.084905 txapi-1.0.2/txapi/demo/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/demo/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      834 2023-04-23 05:01:34.000000 txapi-1.0.2/txapi/demo/demo.py
+-rw-r--r--   0 linkerui   (501) staff       (20)       65 2022-11-25 05:04:29.000000 txapi-1.0.2/txapi/pytest.ini
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.086093 txapi-1.0.2/txapi/tencentcloud/
+-rw-r--r--   0 linkerui   (501) staff       (20)      629 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/tencentcloud/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      187 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/__init__.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.086745 txapi-1.0.2/txapi/tencentcloud/__pycache__/
+-rw-r--r--   0 linkerui   (501) staff       (20)      189 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/tencentcloud/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.091805 txapi-1.0.2/txapi/tencentcloud/common/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/tencentcloud/common/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      161 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/common/__init__.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.094319 txapi-1.0.2/txapi/tencentcloud/common/__pycache__/
+-rw-r--r--   0 linkerui   (501) staff       (20)      174 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/tencentcloud/common/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     8240 2023-04-23 04:21:47.000000 txapi-1.0.2/txapi/tencentcloud/common/__pycache__/abstract_client.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1081 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/tencentcloud/common/__pycache__/credential.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1755 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/tencentcloud/common/__pycache__/sign.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)    12330 2023-04-23 04:21:46.000000 txapi-1.0.2/txapi/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    10568 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/common/abstract_client.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     2066 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1325 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/tencentcloud/common/credential.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1228 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/common/credential.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.096213 txapi-1.0.2/txapi/tencentcloud/common/exception/
+-rw-r--r--   0 linkerui   (501) staff       (20)       24 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      171 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/common/exception/__init__.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.097090 txapi-1.0.2/txapi/tencentcloud/common/exception/__pycache__/
+-rw-r--r--   0 linkerui   (501) staff       (20)      184 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/tencentcloud/common/exception/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1471 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/tencentcloud/common/exception/__pycache__/tencent_cloud_sdk_exception.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)      781 2022-11-25 05:04:29.000000 txapi-1.0.2/txapi/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2017 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/common/exception/tencent_cloud_sdk_exception.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.098620 txapi-1.0.2/txapi/tencentcloud/common/http/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      166 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/common/http/__init__.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.099777 txapi-1.0.2/txapi/tencentcloud/common/http/__pycache__/
+-rw-r--r--   0 linkerui   (501) staff       (20)      179 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/tencentcloud/common/http/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     6235 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/tencentcloud/common/http/__pycache__/request.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     6094 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/tencentcloud/common/http/request.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8460 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/common/http/request.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.102277 txapi-1.0.2/txapi/tencentcloud/common/profile/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      169 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/common/profile/__init__.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.103763 txapi-1.0.2/txapi/tencentcloud/common/profile/__pycache__/
+-rw-r--r--   0 linkerui   (501) staff       (20)      182 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/tencentcloud/common/profile/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1037 2023-04-23 04:23:32.000000 txapi-1.0.2/txapi/tencentcloud/common/profile/__pycache__/client_profile.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1052 2023-04-23 04:18:26.000000 txapi-1.0.2/txapi/tencentcloud/common/profile/__pycache__/http_profile.cpython-39.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1308 2023-04-23 04:23:32.000000 txapi-1.0.2/txapi/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1133 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/common/profile/client_profile.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1426 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1257 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/common/profile/http_profile.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)     1595 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/tencentcloud/common/sign.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2283 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tencentcloud/common/sign.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.105586 txapi-1.0.2/txapi/tests/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-25 05:04:29.000000 txapi-1.0.2/txapi/tests/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      147 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/tests/__init__.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.106840 txapi-1.0.2/txapi/tests/__pycache__/
+-rw-------   0 linkerui   (501) staff       (20)     5768 2022-11-25 05:51:36.000000 txapi-1.0.2/txapi/tests/__pycache__/apiv2_test.cpython-27-PYTEST.pyc
+-rw-------   0 linkerui   (501) staff       (20)     1514 2022-11-25 05:35:32.000000 txapi-1.0.2/txapi/tests/__pycache__/send_request_test.cpython-27-PYTEST.pyc
+-rw-r--r--   0 linkerui   (501) staff       (20)      862 2023-04-23 05:11:25.000000 txapi-1.0.2/txapi/tests/apiv2_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      846 2023-01-31 07:15:48.000000 txapi-1.0.2/txapi/tests/send_request_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      172 2022-11-22 04:39:01.000000 txapi-1.0.2/txapi/version.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      359 2022-11-25 05:04:56.000000 txapi-1.0.2/txapi/version.pyc
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.068077 txapi-1.0.2/txapi.egg-info/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1474 2023-04-23 05:17:51.000000 txapi-1.0.2/txapi.egg-info/PKG-INFO
+-rw-r--r--   0 linkerui   (501) staff       (20)    53374 2023-04-23 05:17:51.000000 txapi-1.0.2/txapi.egg-info/SOURCES.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-04-23 05:17:51.000000 txapi-1.0.2/txapi.egg-info/dependency_links.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-04-23 05:15:51.000000 txapi-1.0.2/txapi.egg-info/not-zip-safe
+-rw-r--r--   0 linkerui   (501) staff       (20)        6 2023-04-23 05:17:51.000000 txapi-1.0.2/txapi.egg-info/top_level.txt
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.107540 txapi-1.0.2/venv/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.117490 txapi-1.0.2/venv/bin/
+-rw-r--r--   0 linkerui   (501) staff       (20)     8834 2022-11-22 06:31:24.000000 txapi-1.0.2/venv/bin/Activate.ps1
+-rw-r--r--   0 linkerui   (501) staff       (20)     2200 2022-11-22 06:31:24.000000 txapi-1.0.2/venv/bin/activate
+-rw-r--r--   0 linkerui   (501) staff       (20)     1252 2022-11-22 06:31:24.000000 txapi-1.0.2/venv/bin/activate.csh
+-rw-r--r--   0 linkerui   (501) staff       (20)     2404 2022-11-22 06:31:24.000000 txapi-1.0.2/venv/bin/activate.fish
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      243 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/bin/autopep8
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      267 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/bin/easy_install
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      267 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/bin/easy_install-3.8
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      258 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/bin/pip
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      258 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/bin/pip3
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      258 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/bin/pip3.8
+-rwxr-xr-x   0 linkerui   (501) staff       (20)      248 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/bin/pycodestyle
+-rwxr-xr-x   0 linkerui   (501) staff       (20)   151504 2023-03-24 11:18:24.000000 txapi-1.0.2/venv/bin/python
+-rwxr-xr-x   0 linkerui   (501) staff       (20)   151504 2023-03-24 11:18:24.000000 txapi-1.0.2/venv/bin/python3
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.931581 txapi-1.0.2/venv/lib/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:51.931687 txapi-1.0.2/venv/lib/python3.8/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.121677 txapi-1.0.2/venv/lib/python3.8/site-packages/
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.128546 txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/
+-rw-r--r--   0 linkerui   (501) staff       (20)     2003 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/AUTHORS.rst
+-rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/INSTALLER
+-rw-r--r--   0 linkerui   (501) staff       (20)     1181 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/LICENSE
+-rw-r--r--   0 linkerui   (501) staff       (20)    17205 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/METADATA
+-rw-r--r--   0 linkerui   (501) staff       (20)     1064 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/RECORD
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/REQUESTED
+-rw-r--r--   0 linkerui   (501) staff       (20)      110 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/WHEEL
+-rw-r--r--   0 linkerui   (501) staff       (20)       43 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/entry_points.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)        9 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/top_level.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)   156040 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      126 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/easy_install.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.129650 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/
+-rw-r--r--   0 linkerui   (501) staff       (20)      455 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      911 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/__main__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.139838 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/
+-rw-r--r--   0 linkerui   (501) staff       (20)      495 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8088 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12249 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cache.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.145143 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/
+-rw-r--r--   0 linkerui   (501) staff       (20)      132 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6547 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9302 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    28782 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      975 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2616 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2843 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9480 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9121 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    15132 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5509 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      156 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/status_codes.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.152676 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/
+-rw-r--r--   0 linkerui   (501) staff       (20)     4100 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5676 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1677 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3081 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9344 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7314 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4918 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3452 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1843 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1270 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    27995 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    11312 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5756 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6996 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3311 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6419 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    14115 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/configuration.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.154676 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/distributions/
+-rw-r--r--   0 linkerui   (501) staff       (20)      959 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1425 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      760 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4086 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1294 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12637 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/exceptions.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.156041 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/index/
+-rw-r--r--   0 linkerui   (501) staff       (20)       30 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    22838 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    37364 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6732 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/locations.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      437 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/main.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.161045 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/
+-rw-r--r--   0 linkerui   (501) staff       (20)       63 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1195 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6900 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2823 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1161 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7470 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      778 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4751 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2044 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4034 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2772 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/wheel.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.166232 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/
+-rw-r--r--   0 linkerui   (501) staff       (20)       50 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    11652 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2329 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5151 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8138 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    15208 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4172 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1882 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/xmlrpc.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.169291 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.172852 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/build/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1254 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2011 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1465 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3356 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5215 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    10373 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/freeze.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.175133 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/install/
+-rw-r--r--   0 linkerui   (501) staff       (20)       51 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1488 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4281 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    31310 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    19903 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7400 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/pyproject.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.180111 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/
+-rw-r--r--   0 linkerui   (501) staff       (20)     3133 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    16387 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    19448 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    33610 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7886 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4690 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/req_tracker.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    23706 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/req_uninstall.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.181326 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      682 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/base.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.182332 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    18755 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.186739 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2342 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    20339 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    17169 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6134 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4511 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    10149 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6779 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/self_outdated_check.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.200338 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1349 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8865 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5439 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      295 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3318 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4359 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1350 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1284 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1152 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6943 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      571 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3297 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4358 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      810 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    13093 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    28001 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1201 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3035 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3404 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/parallel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1254 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/pkg_resources.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5058 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9924 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8378 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1401 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/typing.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9488 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1527 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3706 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7303 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/wheel.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.203271 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/
+-rw-r--r--   0 linkerui   (501) staff       (20)      617 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3887 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    13985 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5162 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12399 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    25966 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9522 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/wheel_builder.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.210074 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/
+-rw-r--r--   0 linkerui   (501) staff       (20)     4588 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    25907 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/appdirs.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.216091 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 linkerui   (501) staff       (20)      302 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1295 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4882 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      805 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.218860 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-r--r--   0 linkerui   (501) staff       (20)       86 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4153 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      856 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      695 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    14149 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2533 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4070 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7091 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      690 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.224255 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 linkerui   (501) staff       (20)       62 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      255 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)   282394 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0 linkerui   (501) staff       (20)     2315 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/certifi/core.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.244525 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1559 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    31254 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1757 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9411 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3787 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5110 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.245298 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/
+-rw-r--r--   0 linkerui   (501) staff       (20)        1 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2774 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3590 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1134 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1855 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1661 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3950 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    10510 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3749 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    13546 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1748 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    31621 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1747 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    20715 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1754 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    13838 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    25777 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    19643 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12839 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    17948 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langcyrillicmodel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12688 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    11345 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12592 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    11290 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    11102 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5370 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3413 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2012 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    25481 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5657 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3546 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3774 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12485 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2766 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      242 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/version.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.248010 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/
+-rw-r--r--   0 linkerui   (501) staff       (20)      239 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2524 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    10462 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1915 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5404 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6438 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    16915 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/contextlib2.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.260085 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/
+-rw-r--r--   0 linkerui   (501) staff       (20)      581 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.266239 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/
+-rw-r--r--   0 linkerui   (501) staff       (20)      274 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      971 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/misc.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    25707 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/shutil.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2617 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/sysconfig.cfg
+-rw-r--r--   0 linkerui   (501) staff       (20)    26854 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    92628 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/tarfile.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    41408 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    51059 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    21066 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    52100 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    14811 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4387 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    38962 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    10766 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    17180 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    96768 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0 linkerui   (501) staff       (20)   105984 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0 linkerui   (501) staff       (20)    59845 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    23391 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    90112 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0 linkerui   (501) staff       (20)    99840 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0 linkerui   (501) staff       (20)    41144 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    43628 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distro.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.276788 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1160 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    16728 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_ihatexml.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    32353 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_inputstream.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    77040 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_tokenizer.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.278658 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/
+-rw-r--r--   0 linkerui   (501) staff       (20)      109 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1013 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/_base.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1775 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/py.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4931 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_utils.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    83464 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/constants.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.283556 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      919 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      286 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/base.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2945 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3643 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/lint.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    10588 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    26897 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1214 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/whitespace.py
+-rw-r--r--   0 linkerui   (501) staff       (20)   117186 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/html5parser.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    15759 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/serializer.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.285455 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/
+-rw-r--r--   0 linkerui   (501) staff       (20)      679 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1715 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1776 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.288958 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/
+-rw-r--r--   0 linkerui   (501) staff       (20)     3592 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    14565 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/base.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8925 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12836 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    14766 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.292558 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/
+-rw-r--r--   0 linkerui   (501) staff       (20)     5719 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7476 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/base.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1413 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4551 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6357 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2309 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.296153 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 linkerui   (501) staff       (20)       58 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3299 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      232 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    11951 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    42350 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1749 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0 linkerui   (501) staff       (20)       22 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0 linkerui   (501) staff       (20)   202084 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    79875 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/ipaddress.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.299576 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1118 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)       20 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/_version.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1081 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6034 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    37133 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/fallback.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.304944 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 linkerui   (501) staff       (20)      736 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      562 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1128 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2022 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1824 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_typing.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9491 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4903 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    31944 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    24067 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1811 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    15470 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/version.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.309153 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/
+-rw-r--r--   0 linkerui   (501) staff       (20)       84 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8438 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/_in_process.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3335 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/build.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5961 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/check.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4098 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/colorlog.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      780 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1129 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/dirtools.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6041 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/envbuild.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2463 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/meta.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    10783 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/wrappers.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.310745 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/
+-rw-r--r--   0 linkerui   (501) staff       (20)   108277 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      562 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/py31compat.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.313296 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/progress/
+-rw-r--r--   0 linkerui   (501) staff       (20)     4857 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/progress/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2854 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/progress/bar.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1372 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/progress/counter.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1380 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/progress/spinner.py
+-rw-r--r--   0 linkerui   (501) staff       (20)   273394 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.327967 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/
+-rw-r--r--   0 linkerui   (501) staff       (20)     4465 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      441 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1096 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    21548 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6496 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    10207 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      465 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2045 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    18430 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3173 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3578 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      757 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    34287 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      695 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    29316 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4188 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3005 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    30176 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/utils.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.331416 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 linkerui   (501) staff       (20)      537 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.332211 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      127 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4547 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1405 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    15018 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2016 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9972 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/retrying.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    34159 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/six.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.336828 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/toml/
+-rw-r--r--   0 linkerui   (501) staff       (20)      747 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/toml/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      242 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/toml/common.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    38696 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/toml/decoder.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9955 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/toml/encoder.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      378 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/toml/ordered.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      618 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/toml/tz.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.342569 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/
+-rw-r--r--   0 linkerui   (501) staff       (20)     2683 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    10792 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    14461 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    35725 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.347163 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      957 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.348909 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    16886 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    11956 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    11034 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4160 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    16582 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    32401 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7036 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7172 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8553 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2440 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/filepost.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.350261 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/
+-rw-r--r--   0 linkerui   (501) staff       (20)      108 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.351440 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1418 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    32536 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/six.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.352529 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/
+-rw-r--r--   0 linkerui   (501) staff       (20)      688 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5696 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    17861 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6018 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    28221 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/response.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.358409 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1038 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4637 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      497 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3815 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2573 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    15543 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    14523 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9947 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    13981 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5406 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      437 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/vendor.txt
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.361479 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/
+-rw-r--r--   0 linkerui   (501) staff       (20)    10579 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8979 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1305 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6563 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4307 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.135237 txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/
+-rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/INSTALLER
+-rw-r--r--   0 linkerui   (501) staff       (20)     1090 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/LICENSE.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)     3708 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/METADATA
+-rw-r--r--   0 linkerui   (501) staff       (20)    98502 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/RECORD
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/REQUESTED
+-rw-r--r--   0 linkerui   (501) staff       (20)      110 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/WHEEL
+-rw-r--r--   0 linkerui   (501) staff       (20)      125 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/entry_points.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-22 06:31:23.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/top_level.txt
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.362097 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/
+-rw-r--r--   0 linkerui   (501) staff       (20)   108481 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.368560 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    24701 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/appdirs.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.375551 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 linkerui   (501) staff       (20)      744 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      562 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      865 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1416 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8277 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4757 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    27778 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12933 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1520 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    11978 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0 linkerui   (501) staff       (20)   232055 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/pyparsing.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    30098 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/six.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.375981 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/extern/
+-rw-r--r--   0 linkerui   (501) staff       (20)     2101 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/extern/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.380159 txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/
+-rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/INSTALLER
+-rw-r--r--   0 linkerui   (501) staff       (20)     1254 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/LICENSE
+-rw-r--r--   0 linkerui   (501) staff       (20)    31580 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/METADATA
+-rw-r--r--   0 linkerui   (501) staff       (20)      919 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/RECORD
+-rw-r--r--   0 linkerui   (501) staff       (20)      110 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/WHEEL
+-rw-r--r--   0 linkerui   (501) staff       (20)       50 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/entry_points.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)       12 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/top_level.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)   102313 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.404016 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/
+-rw-r--r--   0 linkerui   (501) staff       (20)     7943 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      218 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_deprecation_warning.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.432518 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/
+-rw-r--r--   0 linkerui   (501) staff       (20)      250 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    19968 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8572 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    14894 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    47437 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    18079 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/cmd.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.448044 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/
+-rw-r--r--   0 linkerui   (501) staff       (20)      799 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5562 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4913 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    35579 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_msi.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    21537 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    16030 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_wininst.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5767 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8022 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    31635 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    17190 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6232 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5637 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2776 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    13117 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    27482 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2822 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2603 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1298 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8397 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2017 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    11712 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    19005 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7597 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4827 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8876 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    16380 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      139 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3491 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7778 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    50421 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3577 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    10515 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    17784 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8148 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12832 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1969 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    30453 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    23540 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4408 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    21349 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12483 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    14696 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    20913 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12514 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5133 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2388 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_imp.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.452086 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    15130 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/ordered_set.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.459790 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 linkerui   (501) staff       (20)      744 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      562 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      865 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1416 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8268 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4742 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    27778 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    12933 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1520 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    11978 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0 linkerui   (501) staff       (20)   232055 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/pyparsing.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    30098 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/six.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     6638 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/archive_util.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9917 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/build_meta.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    65536 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/cli-32.exe
+-rw-r--r--   0 linkerui   (501) staff       (20)    74752 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/cli-64.exe
+-rw-r--r--   0 linkerui   (501) staff       (20)    65536 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/cli.exe
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.480904 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/
+-rw-r--r--   0 linkerui   (501) staff       (20)      568 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2426 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/alias.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    18482 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1508 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      922 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/bdist_wininst.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4415 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    13187 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9737 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8118 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/develop.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      960 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    86924 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    25560 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4705 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/install.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2203 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3875 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2519 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      628 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0 linkerui   (501) staff       (20)     4994 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      468 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/register.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2176 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      658 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8092 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5085 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     9623 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      462 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/upload.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     7314 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    21782 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/config.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      949 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/dep_util.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5517 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/depends.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    39350 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/dist.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1754 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/distutils_patch.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      524 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/errors.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1729 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/extension.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.481495 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/extern/
+-rw-r--r--   0 linkerui   (501) staff       (20)     2128 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5084 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/glob.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    65536 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/gui-32.exe
+-rw-r--r--   0 linkerui   (501) staff       (20)    75264 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/gui-64.exe
+-rw-r--r--   0 linkerui   (501) staff       (20)    65536 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/gui.exe
+-rw-r--r--   0 linkerui   (501) staff       (20)     5343 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/installer.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      812 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/launch.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2384 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/lib2to3_ex.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     5264 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/monkey.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    51225 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/msvc.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3223 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/namespaces.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    40777 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/package_index.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1504 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/py27compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      838 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/py31compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1330 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/py33compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      245 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/py34compat.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    14251 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/sandbox.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      218 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0 linkerui   (501) staff       (20)      138 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/script.tmpl
+-rw-r--r--   0 linkerui   (501) staff       (20)     8543 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/ssl_support.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      996 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      144 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/version.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     8371 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/wheel.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      714 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/windows_support.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.409205 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/
+-rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/INSTALLER
+-rw-r--r--   0 linkerui   (501) staff       (20)     1078 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/LICENSE
+-rw-r--r--   0 linkerui   (501) staff       (20)     4819 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/METADATA
+-rw-r--r--   0 linkerui   (501) staff       (20)    37957 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/RECORD
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/REQUESTED
+-rw-r--r--   0 linkerui   (501) staff       (20)       92 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/WHEEL
+-rw-r--r--   0 linkerui   (501) staff       (20)      239 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/dependency_links.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)     3143 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/entry_points.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)       38 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/top_level.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)        1 2022-11-22 06:31:22.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/zip-safe
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.484189 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli/
+-rw-r--r--   0 linkerui   (501) staff       (20)      396 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    22633 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli/_parser.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2943 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli/_re.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      254 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli/_types.py
+-rw-r--r--   0 linkerui   (501) staff       (20)       26 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli/py.typed
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-23 05:17:52.487240 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/
+-rw-r--r--   0 linkerui   (501) staff       (20)        4 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/INSTALLER
+-rw-r--r--   0 linkerui   (501) staff       (20)     1072 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/LICENSE
+-rw-r--r--   0 linkerui   (501) staff       (20)     8875 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/METADATA
+-rw-r--r--   0 linkerui   (501) staff       (20)     1349 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/RECORD
+-rw-r--r--   0 linkerui   (501) staff       (20)       81 2022-11-25 05:40:39.000000 txapi-1.0.2/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/WHEEL
+-rw-r--r--   0 linkerui   (501) staff       (20)      104 2022-11-22 06:31:20.000000 txapi-1.0.2/venv/pyvenv.cfg
```

### Comparing `txapi-1.0.1/.git/hooks/commit-msg.sample` & `txapi-1.0.2/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/hooks/fsmonitor-watchman.sample` & `txapi-1.0.2/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/hooks/pre-commit.sample` & `txapi-1.0.2/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/hooks/pre-push.sample` & `txapi-1.0.2/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/hooks/pre-rebase.sample` & `txapi-1.0.2/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/hooks/pre-receive.sample` & `txapi-1.0.2/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/hooks/prepare-commit-msg.sample` & `txapi-1.0.2/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/hooks/push-to-checkout.sample` & `txapi-1.0.2/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/hooks/update.sample` & `txapi-1.0.2/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/index` & `txapi-1.0.2/.git/index`

 * *Files 14% similar despite different names*

#### Comparing `/tmp/diffoscope_0f9fpbv__/tmpau7wnva2_TarContainer/0/22` & `/tmp/diffoscope_0f9fpbv__/tmpiqxea92g_TarContainer/0/22`

```diff
@@ -55,35 +55,46 @@
 Group ID:  20
 Created:   1669091941.616746350
 Modified:  1669091941.616746350
 Inode:     121187545
 Device ID: (0, 4102)
 
 Path:      b'README.md'
-SHA:       63096a2158e3f8361a3f51091f9fa8008c688049
-Size:      1206
+SHA:       d5ee3d14ff70e43fec57164fe9c1f4b40aedeae9
+Size:      1182
 Flags:     0b1001
 User ID:   501
 Group ID:  20
-Created:   1682226354.161219809
-Modified:  1682226354.161219809
+Created:   1682227023.689366962
+Modified:  1682227023.689366962
 Inode:     121187546
 Device ID: (0, 4101)
 
 Path:      b'environment.yml'
 SHA:       dff1fb8aad73a25844ffb6765ea30040e1e84432
 Size:      1041
 Flags:     0b1111
 User ID:   501
 Group ID:  20
 Created:   1669352669.36599650
 Modified:  1669352669.36599650
 Inode:     122043692
 Device ID: (0, 4102)
 
+Path:      b'package.sh'
+SHA:       e69de29bb2d1d6434b8b29ae775ad8c2e48c5391
+Size:      0
+Flags:     0b1010
+User ID:   501
+Group ID:  20
+Created:   1682227058.606962721
+Modified:  1682227058.606962721
+Inode:     160199164
+Device ID: (0, 4101)
+
 Path:      b'setup.py'
 SHA:       e1f9c3c0091160776f8bf8e555af4c60a93daee8
 Size:      811
 Flags:     0b1000
 User ID:   501
 Group ID:  20
 Created:   1682226779.525656041
```

### Comparing `txapi-1.0.1/.git/logs/HEAD` & `txapi-1.0.2/.git/logs/HEAD`

 * *Files 4% similar despite different names*

```diff
@@ -3,7 +3,8 @@
 c67675076ec28c750826f7e5f2170122b8a9d3a3 4162b43e34e8a87d50e492a2f513b5f98fc38ef7 coreylin <coreylin@tencent.com> 1669354921 +0800	commit: add some testcase, and fix some bugs
 4162b43e34e8a87d50e492a2f513b5f98fc38ef7 9e336bd58fc96bb88e2b9a86bdcb6971652394b4 coreylin <coreylin@tencent.com> 1669355550 +0800	commit: add python version for unitest
 9e336bd58fc96bb88e2b9a86bdcb6971652394b4 7e9e25992722a214ac1c4450faa8af6361190eb6 coreylin <coreylin@tencent.com> 1675149348 +0800	merge origin/main: Fast-forward
 7e9e25992722a214ac1c4450faa8af6361190eb6 08c677658838ab6c0c247c140a3b62bdba60c531 coreylin <coreylin@tencent.com> 1681120792 +0800	commit: fix: 完善打包的信息，增加pytest-cov
 08c677658838ab6c0c247c140a3b62bdba60c531 77b3e410890f76b6d46395e3378e3ddf86f46edd coreylin <coreylin@tencent.com> 1682225804 +0800	commit: fix: 增加默认language参数，增加签名的加密算法
 77b3e410890f76b6d46395e3378e3ddf86f46edd b1ee6c481e8ce3a307c0983b487a610bbdd7e065 coreylin <coreylin@tencent.com> 1682226463 +0800	commit: fix:
 b1ee6c481e8ce3a307c0983b487a610bbdd7e065 bd767b09e07988677a46bff99a44334cb802325c coreylin <coreylin@tencent.com> 1682226810 +0800	commit: release: 修改默认签名加密算法
+bd767b09e07988677a46bff99a44334cb802325c d04393b23abcbfb5b566a634f27c764ae6019bc3 coreylin <coreylin@tencent.com> 1682227038 +0800	commit: fix: 修改readme
```

### Comparing `txapi-1.0.1/.git/logs/refs/heads/main` & `txapi-1.0.2/.git/logs/refs/heads/main`

 * *Files 4% similar despite different names*

```diff
@@ -3,7 +3,8 @@
 c67675076ec28c750826f7e5f2170122b8a9d3a3 4162b43e34e8a87d50e492a2f513b5f98fc38ef7 coreylin <coreylin@tencent.com> 1669354921 +0800	commit: add some testcase, and fix some bugs
 4162b43e34e8a87d50e492a2f513b5f98fc38ef7 9e336bd58fc96bb88e2b9a86bdcb6971652394b4 coreylin <coreylin@tencent.com> 1669355550 +0800	commit: add python version for unitest
 9e336bd58fc96bb88e2b9a86bdcb6971652394b4 7e9e25992722a214ac1c4450faa8af6361190eb6 coreylin <coreylin@tencent.com> 1675149348 +0800	merge origin/main: Fast-forward
 7e9e25992722a214ac1c4450faa8af6361190eb6 08c677658838ab6c0c247c140a3b62bdba60c531 coreylin <coreylin@tencent.com> 1681120792 +0800	commit: fix: 完善打包的信息，增加pytest-cov
 08c677658838ab6c0c247c140a3b62bdba60c531 77b3e410890f76b6d46395e3378e3ddf86f46edd coreylin <coreylin@tencent.com> 1682225804 +0800	commit: fix: 增加默认language参数，增加签名的加密算法
 77b3e410890f76b6d46395e3378e3ddf86f46edd b1ee6c481e8ce3a307c0983b487a610bbdd7e065 coreylin <coreylin@tencent.com> 1682226463 +0800	commit: fix:
 b1ee6c481e8ce3a307c0983b487a610bbdd7e065 bd767b09e07988677a46bff99a44334cb802325c coreylin <coreylin@tencent.com> 1682226810 +0800	commit: release: 修改默认签名加密算法
+bd767b09e07988677a46bff99a44334cb802325c d04393b23abcbfb5b566a634f27c764ae6019bc3 coreylin <coreylin@tencent.com> 1682227038 +0800	commit: fix: 修改readme
```

### Comparing `txapi-1.0.1/.git/logs/refs/remotes/origin/main` & `txapi-1.0.2/.git/logs/refs/remotes/origin/main`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 99639a2389a1ee50ace8a7ebfeb6a848085b3ae1 c67675076ec28c750826f7e5f2170122b8a9d3a3 coreylin <coreylin@tencent.com> 1669352644 +0800	fetch: fast-forward
 c67675076ec28c750826f7e5f2170122b8a9d3a3 4162b43e34e8a87d50e492a2f513b5f98fc38ef7 coreylin <coreylin@tencent.com> 1669354925 +0800	update by push
 4162b43e34e8a87d50e492a2f513b5f98fc38ef7 9e336bd58fc96bb88e2b9a86bdcb6971652394b4 coreylin <coreylin@tencent.com> 1669355554 +0800	update by push
 9e336bd58fc96bb88e2b9a86bdcb6971652394b4 7e9e25992722a214ac1c4450faa8af6361190eb6 coreylin <coreylin@tencent.com> 1674095888 +0800	fetch: fast-forward
 7e9e25992722a214ac1c4450faa8af6361190eb6 08c677658838ab6c0c247c140a3b62bdba60c531 coreylin <coreylin@tencent.com> 1681120797 +0800	update by push
 08c677658838ab6c0c247c140a3b62bdba60c531 b1ee6c481e8ce3a307c0983b487a610bbdd7e065 coreylin <coreylin@tencent.com> 1682226468 +0800	update by push
 b1ee6c481e8ce3a307c0983b487a610bbdd7e065 bd767b09e07988677a46bff99a44334cb802325c coreylin <coreylin@tencent.com> 1682226814 +0800	update by push
+bd767b09e07988677a46bff99a44334cb802325c d04393b23abcbfb5b566a634f27c764ae6019bc3 coreylin <coreylin@tencent.com> 1682227042 +0800	update by push
```

### Comparing `txapi-1.0.1/.git/objects/0d/db97d0b98ea46065d50f4c8b40363d97fbc843` & `txapi-1.0.2/.git/objects/0d/db97d0b98ea46065d50f4c8b40363d97fbc843`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/11/1e278133b448d8badadfd73e711d439c6b9abb` & `txapi-1.0.2/.git/objects/11/1e278133b448d8badadfd73e711d439c6b9abb`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/19/d1b4f52378f26d4f82a9356b8ede80dcd54eb7` & `txapi-1.0.2/.git/objects/19/d1b4f52378f26d4f82a9356b8ede80dcd54eb7`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/21/4c2ea36d2dde3af8296cb4037fb93734b56166` & `txapi-1.0.2/.git/objects/21/4c2ea36d2dde3af8296cb4037fb93734b56166`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/21/639dd781776e03375cd81804372559ba2e9bf9` & `txapi-1.0.2/.git/objects/21/639dd781776e03375cd81804372559ba2e9bf9`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/23/398032b1b9804ab0dcba15248c71bb418737da` & `txapi-1.0.2/.git/objects/23/398032b1b9804ab0dcba15248c71bb418737da`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/23/f661515e73b2b19d9af88e6bab4a169c46406e` & `txapi-1.0.2/.git/objects/23/f661515e73b2b19d9af88e6bab4a169c46406e`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/2c/c1a52cf5b91e50837f92540fa79b66bdbb7181` & `txapi-1.0.2/.git/objects/2c/c1a52cf5b91e50837f92540fa79b66bdbb7181`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/31/4296ca74424b305d04be227ad964afb86bf921` & `txapi-1.0.2/.git/objects/31/4296ca74424b305d04be227ad964afb86bf921`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/32/8a62420ab81f87039d73e6ae31e5b1b54d3bde` & `txapi-1.0.2/.git/objects/32/8a62420ab81f87039d73e6ae31e5b1b54d3bde`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/3f/03a1b9319f3c3d9941d7ae256b81e045b42363` & `txapi-1.0.2/.git/objects/3f/03a1b9319f3c3d9941d7ae256b81e045b42363`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/45/219397fd4a9c0cb4ac7ac9018b67b54ba2ef36` & `txapi-1.0.2/.git/objects/45/219397fd4a9c0cb4ac7ac9018b67b54ba2ef36`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/47/1c3d59784a99eb3429ccbd100c7038f4859d54` & `txapi-1.0.2/.git/objects/47/1c3d59784a99eb3429ccbd100c7038f4859d54`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/57/940bdb0c48ade22baee7f4d5775cbbf3334d90` & `txapi-1.0.2/.git/objects/57/940bdb0c48ade22baee7f4d5775cbbf3334d90`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/59/6c581887f06e9ab622345a9191e3e09732cc7b` & `txapi-1.0.2/.git/objects/59/6c581887f06e9ab622345a9191e3e09732cc7b`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/63/096a2158e3f8361a3f51091f9fa8008c688049` & `txapi-1.0.2/.git/objects/63/096a2158e3f8361a3f51091f9fa8008c688049`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/67/39f71ac4becbfda86f98d6b3ae1a4be3d60ad9` & `txapi-1.0.2/.git/objects/67/39f71ac4becbfda86f98d6b3ae1a4be3d60ad9`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/6c/4a1313e8ec893fc2ebd5d3b3efce63d11f73db` & `txapi-1.0.2/.git/objects/6c/4a1313e8ec893fc2ebd5d3b3efce63d11f73db`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/75/fe7a3d3ccbdaec7b3b95d4c7c44ecee3ed92f3` & `txapi-1.0.2/.git/objects/75/fe7a3d3ccbdaec7b3b95d4c7c44ecee3ed92f3`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/76/0aade4935e771a96525aa507d60f72614c5da6` & `txapi-1.0.2/.git/objects/76/0aade4935e771a96525aa507d60f72614c5da6`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/78/68afd1318032499383a82f4a2b458791e7b990` & `txapi-1.0.2/.git/objects/78/68afd1318032499383a82f4a2b458791e7b990`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/78/a660592bc694a40b5248e0549c066483452c7a` & `txapi-1.0.2/.git/objects/78/a660592bc694a40b5248e0549c066483452c7a`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/80/5cc728900be707de58af039739e01221353528` & `txapi-1.0.2/.git/objects/80/5cc728900be707de58af039739e01221353528`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/80/b07b0c161d95297f1a537db880d0e98acad82d` & `txapi-1.0.2/.git/objects/80/b07b0c161d95297f1a537db880d0e98acad82d`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/82/63ddf91052bfe6c6af092051fafc077d86476c` & `txapi-1.0.2/.git/objects/82/63ddf91052bfe6c6af092051fafc077d86476c`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/8d/1cdd3e52ed567f61e45e6fcc4feefde445c9e3` & `txapi-1.0.2/.git/objects/8d/1cdd3e52ed567f61e45e6fcc4feefde445c9e3`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/99/639a2389a1ee50ace8a7ebfeb6a848085b3ae1` & `txapi-1.0.2/.git/objects/99/639a2389a1ee50ace8a7ebfeb6a848085b3ae1`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/9a/74267b066cb21fc0a23b33cd3990bc13f9ba1d` & `txapi-1.0.2/.git/objects/9a/74267b066cb21fc0a23b33cd3990bc13f9ba1d`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/9a/ca49ad39bb6aabb57d014726a4a2433206ecc7` & `txapi-1.0.2/.git/objects/9a/ca49ad39bb6aabb57d014726a4a2433206ecc7`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/9e/d55bad89de367003e0a538b16e6c79d32db508` & `txapi-1.0.2/.git/objects/9e/d55bad89de367003e0a538b16e6c79d32db508`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/a2/30bd6c3fe5539caed2f8b2b0865c6deea1a026` & `txapi-1.0.2/.git/objects/a2/30bd6c3fe5539caed2f8b2b0865c6deea1a026`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/a3/68a8a8fd04e25b619adb09c2bee7ad676d3185` & `txapi-1.0.2/.git/objects/a3/68a8a8fd04e25b619adb09c2bee7ad676d3185`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/a5/07a598601aea15d6abaafe7bad6ad10e2b22d7` & `txapi-1.0.2/.git/objects/a5/07a598601aea15d6abaafe7bad6ad10e2b22d7`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/a6/6d48d9f7ef0c81494621de192b567705157436` & `txapi-1.0.2/.git/objects/a6/6d48d9f7ef0c81494621de192b567705157436`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/a7/826960973f479a98bd49313e881c5e93393e38` & `txapi-1.0.2/.git/objects/a7/826960973f479a98bd49313e881c5e93393e38`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/ad/91fa7d37aa37e20fe58076725790e8aae43bc0` & `txapi-1.0.2/.git/objects/ad/91fa7d37aa37e20fe58076725790e8aae43bc0`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/b4/09333c2ea63b578a3d08486be3d6e7a44edc7d` & `txapi-1.0.2/.git/objects/b4/09333c2ea63b578a3d08486be3d6e7a44edc7d`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/b6/e47617de110dea7ca47e087ff1347cc2646eda` & `txapi-1.0.2/.git/objects/b6/e47617de110dea7ca47e087ff1347cc2646eda`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/c4/72d537837ad718aac848eb955f676a87e7f2ac` & `txapi-1.0.2/.git/objects/c4/72d537837ad718aac848eb955f676a87e7f2ac`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/cd/8c8e7cb1c8eb8308a1a70cb48320fdc1db3362` & `txapi-1.0.2/.git/objects/cd/8c8e7cb1c8eb8308a1a70cb48320fdc1db3362`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/d1/30c07e14b682ef444d69930acc214185c9b7db` & `txapi-1.0.2/.git/objects/d1/30c07e14b682ef444d69930acc214185c9b7db`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/d9/5dcf7e5be1da655caf43d16bfa1735477497a0` & `txapi-1.0.2/.git/objects/d9/5dcf7e5be1da655caf43d16bfa1735477497a0`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/de/07e2c3445f2d8965343f0aa6099392f0ba0c52` & `txapi-1.0.2/.git/objects/de/07e2c3445f2d8965343f0aa6099392f0ba0c52`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/df/6c3c8d9fa2fd045230e7d7be1b2b81ad15799f` & `txapi-1.0.2/.git/objects/df/6c3c8d9fa2fd045230e7d7be1b2b81ad15799f`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/e0/db285333f977126d50cb01bef5f83bade2d169` & `txapi-1.0.2/.git/objects/e0/db285333f977126d50cb01bef5f83bade2d169`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/e9/09aa2ff53b15d535bcc2de16de52134b952aec` & `txapi-1.0.2/.git/objects/e9/09aa2ff53b15d535bcc2de16de52134b952aec`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/ec/7d22521aa69ab0c5fbea87d1157d781d0aebe6` & `txapi-1.0.2/.git/objects/ec/7d22521aa69ab0c5fbea87d1157d781d0aebe6`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/ef/586010c625011d458db7e684a425fcbd1012f1` & `txapi-1.0.2/.git/objects/ef/586010c625011d458db7e684a425fcbd1012f1`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/f3/7b0ee455cd0876fd2a4a12adf4f70cb9855596` & `txapi-1.0.2/.git/objects/f3/7b0ee455cd0876fd2a4a12adf4f70cb9855596`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/f6/f35d7b623a39e2342b860f6f080fe5d8275bd5` & `txapi-1.0.2/.git/objects/f6/f35d7b623a39e2342b860f6f080fe5d8275bd5`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/fe/a22029fd4d0cc03ab16a60109fb3f928dd7747` & `txapi-1.0.2/.git/objects/fe/a22029fd4d0cc03ab16a60109fb3f928dd7747`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.git/objects/ff/3ba9f30b5aa2f45cbcd01a1b08be357c8f22cb` & `txapi-1.0.2/.git/objects/ff/3ba9f30b5aa2f45cbcd01a1b08be357c8f22cb`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.github/workflows/python-package-conda.yml` & `txapi-1.0.2/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.github/workflows/python-package.yml` & `txapi-1.0.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.idea/inspectionProfiles/Project_Default.xml` & `txapi-1.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.idea/txapi.iml` & `txapi-1.0.2/.idea/txapi.iml`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/.idea/workspace.xml` & `txapi-1.0.2/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `txapi-1.0.1/.idea/workspace.xml` & `txapi-1.0.2/.idea/workspace.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="e591b392-b72e-43b9-872d-225595a3ea70" name="Default Changelist" comment="">
+      <change afterPath="$PROJECT_DIR$/package.sh" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/setup.py" beforeDir="false" afterPath="$PROJECT_DIR$/setup.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/txapi/tests/apiv2_test.py" beforeDir="false" afterPath="$PROJECT_DIR$/txapi/tests/apiv2_test.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -100,15 +100,15 @@
       <changelist id="e591b392-b72e-43b9-872d-225595a3ea70" name="Default Changelist" comment=""/>
       <created>1675149315655</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1675149315655</updated>
       <workItem from="1675149316778" duration="1209000"/>
       <workItem from="1681120636818" duration="539000"/>
-      <workItem from="1682223481710" duration="2265000"/>
+      <workItem from="1682223481710" duration="2555000"/>
     </task>
     <task id="LOCAL-00001" summary="fix: 完善打包的信息，增加pytest-cov">
       <created>1681120792969</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1681120792969</updated>
@@ -125,62 +125,76 @@
 2. 修改demo，增加readme说明">
       <created>1682226463541</created>
       <option name="number" value="00003"/>
       <option name="presentableId" value="LOCAL-00003"/>
       <option name="project" value="LOCAL"/>
       <updated>1682226463541</updated>
     </task>
-    <option name="localTasksCounter" value="4"/>
+    <task id="LOCAL-00004" summary="release: 修改默认签名加密算法">
+      <created>1682226810088</created>
+      <option name="number" value="00004"/>
+      <option name="presentableId" value="LOCAL-00004"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1682226810088</updated>
+    </task>
+    <task id="LOCAL-00005" summary="fix: 修改readme">
+      <created>1682227038854</created>
+      <option name="number" value="00005"/>
+      <option name="presentableId" value="LOCAL-00005"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1682227038854</updated>
+    </task>
+    <option name="localTasksCounter" value="6"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="fix: 完善打包的信息，增加pytest-cov"/>
     <MESSAGE value="fix: 增加默认language参数，增加签名的加密算法"/>
     <MESSAGE value="fix: 
 1. 增加默认language参数，增加签名的加密算法
 2. 修改demo，增加readme说明"/>
-    <option name="LAST_COMMIT_MESSAGE" value="fix: 
-1. 增加默认language参数，增加签名的加密算法
-2. 修改demo，增加readme说明"/>
+    <MESSAGE value="release: 修改默认签名加密算法"/>
+    <MESSAGE value="fix: 修改readme"/>
+    <option name="LAST_COMMIT_MESSAGE" value="fix: 修改readme"/>
   </component>
   <component name="WindowStateProjectService">
-    <state x="480" y="156" key="CommitChangelistDialog2" timestamp="1682226463356">
+    <state x="480" y="156" key="CommitChangelistDialog2" timestamp="1682227038677">
       <screen x="45" y="25" width="1747" height="1095"/>
     </state>
-    <state x="480" y="156" key="CommitChangelistDialog2/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682226463356"/>
+    <state x="480" y="156" key="CommitChangelistDialog2/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682227038677"/>
     <state x="480" y="156" key="CommitChangelistDialog2/45.25.1747.1095@45.25.1747.1095" timestamp="1681120792781"/>
     <state x="200" y="122" width="1544" height="895" key="DiffContextDialog" timestamp="1682223817494">
       <screen x="45" y="25" width="1747" height="1095"/>
     </state>
     <state x="200" y="122" width="1544" height="895" key="DiffContextDialog/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682223817494"/>
     <state x="148" y="125" width="1544" height="895" key="DiffContextDialog/45.25.1747.1095@45.25.1747.1095" timestamp="1681120653198"/>
-    <state width="1705" height="301" key="GridCell.Tab.0.bottom" timestamp="1682226731003">
+    <state width="1705" height="301" key="GridCell.Tab.0.bottom" timestamp="1682226900952">
       <screen x="45" y="25" width="1747" height="1095"/>
     </state>
-    <state width="1705" height="301" key="GridCell.Tab.0.bottom/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682226731003"/>
-    <state width="1705" height="301" key="GridCell.Tab.0.center" timestamp="1682226731002">
+    <state width="1705" height="301" key="GridCell.Tab.0.bottom/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682226900952"/>
+    <state width="1705" height="301" key="GridCell.Tab.0.center" timestamp="1682226900952">
       <screen x="45" y="25" width="1747" height="1095"/>
     </state>
-    <state width="1705" height="301" key="GridCell.Tab.0.center/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682226731002"/>
-    <state width="1705" height="301" key="GridCell.Tab.0.left" timestamp="1682226731002">
+    <state width="1705" height="301" key="GridCell.Tab.0.center/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682226900952"/>
+    <state width="1705" height="301" key="GridCell.Tab.0.left" timestamp="1682226900952">
       <screen x="45" y="25" width="1747" height="1095"/>
     </state>
-    <state width="1705" height="301" key="GridCell.Tab.0.left/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682226731002"/>
-    <state width="1705" height="301" key="GridCell.Tab.0.right" timestamp="1682226731003">
+    <state width="1705" height="301" key="GridCell.Tab.0.left/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682226900952"/>
+    <state width="1705" height="301" key="GridCell.Tab.0.right" timestamp="1682226900952">
       <screen x="45" y="25" width="1747" height="1095"/>
     </state>
-    <state width="1705" height="301" key="GridCell.Tab.0.right/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682226731003"/>
-    <state x="529" y="309" key="Vcs.Push.Dialog.v2" timestamp="1682226591315">
+    <state width="1705" height="301" key="GridCell.Tab.0.right/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682226900952"/>
+    <state x="529" y="309" key="Vcs.Push.Dialog.v2" timestamp="1682227040621">
       <screen x="45" y="25" width="1747" height="1095"/>
     </state>
     <state x="496" y="309" key="Vcs.Push.Dialog.v2/0.25.1792.1095/-42.-1055.1920.1055@0.25.1792.1095" timestamp="1675149356226"/>
-    <state x="529" y="309" key="Vcs.Push.Dialog.v2/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682226591315"/>
+    <state x="529" y="309" key="Vcs.Push.Dialog.v2/45.25.1747.1095/-42.-1055.1920.1055@45.25.1747.1095" timestamp="1682227040621"/>
     <state x="529" y="309" key="Vcs.Push.Dialog.v2/45.25.1747.1095@45.25.1747.1095" timestamp="1681120795798"/>
     <state x="697" y="490" key="com.intellij.openapi.vcs.update.UpdateOrStatusOptionsDialogupdate-v2" timestamp="1675149347138">
       <screen x="0" y="25" width="1792" height="1095"/>
     </state>
     <state x="697" y="490" key="com.intellij.openapi.vcs.update.UpdateOrStatusOptionsDialogupdate-v2/0.25.1792.1095/-42.-1055.1920.1055@0.25.1792.1095" timestamp="1675149347138"/>
     <state x="620" y="327" width="597" height="490" key="find.popup" timestamp="1682224108544">
       <screen x="45" y="25" width="1747" height="1095"/>
```

### Comparing `txapi-1.0.1/LICENSE` & `txapi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/PKG-INFO` & `txapi-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txapi
-Version: 1.0.1
+Version: 1.0.2
 Summary: api project for v2&v3
 Home-page: https://github.com/coreylam/txapi
 Author: coreylam
 Author-email: coreylam@163.com
 License: GPL
 Platform: UNKNOWN
 Requires-Python: >=2.7
@@ -21,16 +21,14 @@
 pip install txapi
 ```
 
 Project: https://pypi.org/project/txapi/1.0.0/
 
 ## DEMO
 
-配置文件 config.py
-
 ```python
 # -*- coding:utf-8 -*-
 from txapi import API
 
 client = API.v3(
     api_domain="云API请求的域名",
     region="地域名称",
```

### Comparing `txapi-1.0.1/README.md` & `txapi-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 pip install txapi
 ```
 
 Project: https://pypi.org/project/txapi/1.0.0/
 
 ## DEMO
 
-配置文件 config.py
-
 ```python
 # -*- coding:utf-8 -*-
 from txapi import API
 
 client = API.v3(
     api_domain="云API请求的域名",
     region="地域名称",
```

### Comparing `txapi-1.0.1/setup.py` & `txapi-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         with open(filename, "r") as fid:
             desc = fid.read()
     return desc
 
 
 setup(
     name='txapi',
-    version="1.0.1",
+    version="1.0.2",
     description='api project for v2&v3',
     long_description=read_desc(),
     long_description_content_type="text/markdown",
     author='coreylam',
     author_email='coreylam@163.com',
     url='https://github.com/coreylam/txapi',
     license='GPL',
```

### Comparing `txapi-1.0.1/txapi/QcloudApi/__pycache__/qcloudapi.cpython-39.pyc` & `txapi-1.0.2/txapi/QcloudApi/__pycache__/qcloudapi.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/common/__pycache__/api_exception.cpython-39.pyc` & `txapi-1.0.2/txapi/QcloudApi/common/__pycache__/api_exception.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/common/__pycache__/request.cpython-39.pyc` & `txapi-1.0.2/txapi/QcloudApi/common/__pycache__/request.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/common/__pycache__/sign.cpython-39.pyc` & `txapi-1.0.2/txapi/QcloudApi/common/__pycache__/sign.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/common/api_exception.py` & `txapi-1.0.2/txapi/QcloudApi/common/api_exception.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/common/api_exception.pyc` & `txapi-1.0.2/txapi/QcloudApi/common/api_exception.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/common/request.py` & `txapi-1.0.2/txapi/QcloudApi/common/request.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/common/request.pyc` & `txapi-1.0.2/txapi/QcloudApi/common/request.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/common/sign.py` & `txapi-1.0.2/txapi/QcloudApi/common/sign.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/common/sign.pyc` & `txapi-1.0.2/txapi/QcloudApi/common/sign.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/modules/__pycache__/base.cpython-39.pyc` & `txapi-1.0.2/txapi/QcloudApi/modules/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/modules/base.py` & `txapi-1.0.2/txapi/QcloudApi/modules/base.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/modules/base.pyc` & `txapi-1.0.2/txapi/QcloudApi/modules/base.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/qcloudapi.py` & `txapi-1.0.2/txapi/QcloudApi/qcloudapi.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/QcloudApi/qcloudapi.pyc` & `txapi-1.0.2/txapi/QcloudApi/qcloudapi.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/__pycache__/api2.cpython-39.pyc` & `txapi-1.0.2/txapi/__pycache__/api2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/__pycache__/api3.cpython-39.pyc` & `txapi-1.0.2/txapi/__pycache__/api3.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/api2.py` & `txapi-1.0.2/txapi/api2.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/api2.pyc` & `txapi-1.0.2/txapi/api2.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/api3.py` & `txapi-1.0.2/txapi/api3.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/api3.pyc` & `txapi-1.0.2/txapi/api3.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/demo/demo.py` & `txapi-1.0.2/txapi/demo/demo.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/__init__.py` & `txapi-1.0.2/txapi/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/__pycache__/abstract_client.cpython-39.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/__pycache__/abstract_client.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/__pycache__/credential.cpython-39.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/__pycache__/credential.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/__pycache__/sign.cpython-39.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/__pycache__/sign.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/abstract_client.py` & `txapi-1.0.2/txapi/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/abstract_client.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/abstract_client.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/abstract_model.py` & `txapi-1.0.2/txapi/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/credential.py` & `txapi-1.0.2/txapi/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/credential.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/credential.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/exception/__pycache__/tencent_cloud_sdk_exception.cpython-39.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/exception/__pycache__/tencent_cloud_sdk_exception.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `txapi-1.0.2/txapi/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/exception/tencent_cloud_sdk_exception.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/exception/tencent_cloud_sdk_exception.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/http/__pycache__/request.cpython-39.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/http/__pycache__/request.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/http/request.py` & `txapi-1.0.2/txapi/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/http/request.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/http/request.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/profile/__pycache__/client_profile.cpython-39.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/profile/__pycache__/client_profile.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/profile/__pycache__/http_profile.cpython-39.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/profile/__pycache__/http_profile.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/profile/client_profile.py` & `txapi-1.0.2/txapi/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/profile/client_profile.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/profile/client_profile.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/profile/http_profile.py` & `txapi-1.0.2/txapi/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/profile/http_profile.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/profile/http_profile.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/sign.py` & `txapi-1.0.2/txapi/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tencentcloud/common/sign.pyc` & `txapi-1.0.2/txapi/tencentcloud/common/sign.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tests/__pycache__/apiv2_test.cpython-27-PYTEST.pyc` & `txapi-1.0.2/txapi/tests/__pycache__/apiv2_test.cpython-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tests/__pycache__/send_request_test.cpython-27-PYTEST.pyc` & `txapi-1.0.2/txapi/tests/__pycache__/send_request_test.cpython-27-PYTEST.pyc`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tests/apiv2_test.py` & `txapi-1.0.2/txapi/tests/apiv2_test.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi/tests/send_request_test.py` & `txapi-1.0.2/txapi/tests/send_request_test.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/txapi.egg-info/PKG-INFO` & `txapi-1.0.2/txapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txapi
-Version: 1.0.1
+Version: 1.0.2
 Summary: api project for v2&v3
 Home-page: https://github.com/coreylam/txapi
 Author: coreylam
 Author-email: coreylam@163.com
 License: GPL
 Platform: UNKNOWN
 Requires-Python: >=2.7
@@ -21,16 +21,14 @@
 pip install txapi
 ```
 
 Project: https://pypi.org/project/txapi/1.0.0/
 
 ## DEMO
 
-配置文件 config.py
-
 ```python
 # -*- coding:utf-8 -*-
 from txapi import API
 
 client = API.v3(
     api_domain="云API请求的域名",
     region="地域名称",
```

### Comparing `txapi-1.0.1/txapi.egg-info/SOURCES.txt` & `txapi-1.0.2/txapi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 .git/objects/a7/7cbef8139fd72d2421e1fbef4b7433022e6683
 .git/objects/a7/826960973f479a98bd49313e881c5e93393e38
 .git/objects/a7/b67376b5ff945537da897b0091bf8de9424ec0
 .git/objects/a9/00b9fb2f23ed04d28847f0f78a9abdc6b12595
 .git/objects/ad/91fa7d37aa37e20fe58076725790e8aae43bc0
 .git/objects/b1/21761178ea0098e11e96a2467f97a80f50d3b6
 .git/objects/b1/ee6c481e8ce3a307c0983b487a610bbdd7e065
+.git/objects/b2/1dc75cb439396e8215e6ae76e4be281da4549f
 .git/objects/b2/442748fb5ccb3f5801c5dffbb8f8050aff47a6
 .git/objects/b3/2da2543d266ca57a7a7072d8a1aa7906a5216f
 .git/objects/b4/09333c2ea63b578a3d08486be3d6e7a44edc7d
 .git/objects/b6/e47617de110dea7ca47e087ff1347cc2646eda
 .git/objects/b8/1cd0c71144089c01e5d12b5a82dfcf30feece7
 .git/objects/bb/4b30a3ec4305961374dbfa727156c77028a5fb
 .git/objects/bd/767b09e07988677a46bff99a44334cb802325c
@@ -168,20 +169,22 @@
 .git/objects/c6/7675076ec28c750826f7e5f2170122b8a9d3a3
 .git/objects/c9/98aaf6c57e4dd8fd55cdc45f84f7e8ccdad887
 .git/objects/cd/316e3e2823326d2d79e861a63228b0c5cf538e
 .git/objects/cd/8c8e7cb1c8eb8308a1a70cb48320fdc1db3362
 .git/objects/cf/1cd7c9a8eed6d7785ec1f54ebf3737df1c40cf
 .git/objects/cf/2f8da95e46dbe88e67d6b28cfb2bcf3e092b35
 .git/objects/cf/30c4ebc092f87f24d127e1724aeead7aeef57f
+.git/objects/d0/4393b23abcbfb5b566a634f27c764ae6019bc3
 .git/objects/d1/30c07e14b682ef444d69930acc214185c9b7db
 .git/objects/d1/7eb6ac8a7f6a3a69d8254e6fbf552231a0054f
 .git/objects/d1/d56662595333e313eb7bd388cfab40e7fa2a35
 .git/objects/d2/27a48e81fb6f771f6296665b55d379f3569f5c
 .git/objects/d4/7949ca42ff77a9f570b08a634182b151695b71
 .git/objects/d5/9480059d62735163c88bf127d8f0ca49546a0f
+.git/objects/d5/ee3d14ff70e43fec57164fe9c1f4b40aedeae9
 .git/objects/d6/f0964f2c224afc19e38192e2debdafeeba6acd
 .git/objects/d8/3e2b6fb80b632a01e951072e47598c70125249
 .git/objects/d9/5dcf7e5be1da655caf43d16bfa1735477497a0
 .git/objects/da/55f873a9f0769f4616f797953c71860a97381c
 .git/objects/db/0c553587cb305847d9db53169807ca0e641b03
 .git/objects/de/07e2c3445f2d8965343f0aa6099392f0ba0c52
 .git/objects/de/39cf37ad954d80ed5175810061a060c7ccc48d
```

### Comparing `txapi-1.0.1/venv/bin/Activate.ps1` & `txapi-1.0.2/venv/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/bin/activate` & `txapi-1.0.2/venv/bin/activate`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/bin/activate.csh` & `txapi-1.0.2/venv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/bin/activate.fish` & `txapi-1.0.2/venv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/bin/python` & `txapi-1.0.2/venv/bin/python`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/bin/python3` & `txapi-1.0.2/venv/bin/python3`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/AUTHORS.rst` & `txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/LICENSE` & `txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/METADATA` & `txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/RECORD` & `txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8-2.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/autopep8.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/autopep8.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/__main__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/build_env.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cache.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/autocompletion.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/base_command.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/cmdoptions.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/command_context.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/main.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/main_parser.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/parser.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/progress_bars.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/req_command.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/cli/spinners.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/cache.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/check.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/completion.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/configuration.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/debug.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/download.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/freeze.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/hash.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/help.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/install.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/list.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/search.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/show.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/uninstall.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/commands/wheel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/configuration.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/distributions/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/distributions/base.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/distributions/installed.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/distributions/sdist.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/distributions/wheel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/exceptions.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/index/collector.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/index/package_finder.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/locations.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/locations.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/candidate.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/direct_url.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/format_control.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/index.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/link.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/scheme.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/search_scope.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/selection_prefs.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/target_python.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/models/wheel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/auth.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/cache.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/download.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/lazy_wheel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/session.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/utils.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/network/xmlrpc.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/check.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/freeze.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/install/editable_legacy.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/install/legacy.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/install/wheel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/operations/prepare.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/pyproject.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/constructors.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/req_file.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/req_install.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/req_set.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/req_tracker.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/req_tracker.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/req/req_uninstall.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/base.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/resolver.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/base.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/self_outdated_check.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/appdirs.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/compatibility_tags.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/deprecation.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/direct_url_helpers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/distutils_args.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/encoding.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/entrypoints.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/filesystem.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/filetypes.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/glibc.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/hashes.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/inject_securetransport.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/logging.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/misc.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/models.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/packaging.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/parallel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/pkg_resources.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/setuptools_build.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/subprocess.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/temp_dir.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/typing.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/typing.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/unpacking.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/urls.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/virtualenv.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/utils/wheel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/bazaar.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/git.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/mercurial.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/subversion.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/vcs/versioncontrol.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_internal/wheel_builder.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/appdirs.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/adapter.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/cache.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/controller.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/serialize.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/certifi/core.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5freq.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5prober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/chardistribution.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cp949prober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/enums.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escsm.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/eucjpprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrfreq.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwfreq.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312freq.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312prober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/hebrewprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jisfreq.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jpcntx.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langcyrillicmodel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langthaimodel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/latin1prober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcssm.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sjisprober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/universaldetector.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/chardet/utf8prober.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansi.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansitowin32.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/initialise.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/win32.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/colorama/winterm.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/contextlib2.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/contextlib2.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/misc.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/misc.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/shutil.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/shutil.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/sysconfig.cfg` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/sysconfig.cfg`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/sysconfig.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/sysconfig.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/tarfile.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/_backport/tarfile.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/database.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/index.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/locators.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/manifest.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/markers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/metadata.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/resources.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/scripts.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t32.exe` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t64.exe` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/util.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/version.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w32.exe` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w64.exe` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distlib/wheel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/distro.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/distro.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_ihatexml.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_ihatexml.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_inputstream.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_inputstream.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_tokenizer.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/_base.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/_base.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/py.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_trie/py.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_utils.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/_utils.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/constants.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/constants.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/lint.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/lint.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/optionaltags.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/optionaltags.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/sanitizer.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/sanitizer.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/whitespace.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/filters/whitespace.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/html5parser.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/html5parser.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/serializer.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/serializer.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/sax.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treeadapters/sax.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/base.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/base.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/dom.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/dom.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/etree.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/etree.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/base.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/base.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/dom.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/dom.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/etree.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/etree.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/codec.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/core.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/idnadata.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/intranges.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/idna/uts46data.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/ipaddress.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/ipaddress.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/exceptions.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/ext.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/fallback.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/__about__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_structures.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_typing.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/markers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/requirements.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/specifiers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/tags.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/utils.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/packaging/version.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/_in_process.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/_in_process.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/build.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/build.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/check.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/check.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/colorlog.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/colorlog.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/dirtools.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/dirtools.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/envbuild.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/envbuild.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/meta.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/meta.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pep517/wrappers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pep517/wrappers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/progress/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/progress/bar.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/progress/bar.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/progress/counter.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/progress/counter.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/progress/spinner.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/_internal_utils.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/adapters.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/api.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/auth.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/cookies.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/exceptions.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/help.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/hooks.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/models.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/packages.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/sessions.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/status_codes.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/structures.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/requests/utils.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/providers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/reporters.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/resolvers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/structs.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/retrying.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/retrying.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/six.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/toml/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/toml/decoder.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/toml/encoder.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/toml/tz.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/toml/tz.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/_collections.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connection.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connectionpool.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/exceptions.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/fields.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/filepost.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/six.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/poolmanager.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/request.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/response.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/connection.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/request.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/response.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/retry.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/timeout.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/url.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/wait.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/labels.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/mklabels.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/tests.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/LICENSE.txt` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/METADATA` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/RECORD` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pip-20.2.3.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/appdirs.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/markers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/tags.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/utils.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/version.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/pyparsing.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/_vendor/six.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pkg_resources/extern/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/LICENSE` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/METADATA` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/RECORD` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle-2.10.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/pycodestyle.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/pycodestyle.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/_msvccompiler.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/archive_util.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/bcppcompiler.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/ccompiler.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/cmd.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_msi.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_msi.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_wininst.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_wininst.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_clib.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_ext.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_py.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_scripts.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/check.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/clean.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/config.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_data.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_egg_info.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_headers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_lib.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_scripts.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/register.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/sdist.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/command/upload.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/config.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/core.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/cygwinccompiler.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/dep_util.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/dir_util.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/dist.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/errors.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/extension.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/fancy_getopt.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/file_util.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/filelist.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/log.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/msvc9compiler.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/msvccompiler.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/spawn.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/sysconfig.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/text_file.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/unixccompiler.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/util.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/version.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_distutils/versionpredicate.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_imp.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/ordered_set.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__about__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_structures.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/markers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/requirements.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/specifiers.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/tags.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/utils.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/version.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/pyparsing.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/_vendor/six.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/archive_util.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/build_meta.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/cli-32.exe` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/cli-64.exe` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/cli.exe` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/alias.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/bdist_egg.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/bdist_rpm.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/bdist_wininst.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/bdist_wininst.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/build_clib.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/build_ext.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/build_py.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/develop.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/dist_info.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/easy_install.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/egg_info.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/install.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/install_egg_info.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/install_lib.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/install_scripts.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/py36compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/rotate.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/saveopts.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/sdist.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/setopt.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/test.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/command/upload_docs.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/config.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/config.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/dep_util.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/depends.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/dist.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/distutils_patch.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/distutils_patch.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/errors.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/extension.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/extern/__init__.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/glob.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/gui-32.exe` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/gui-64.exe` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/gui.exe` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/installer.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/launch.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/lib2to3_ex.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/lib2to3_ex.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/monkey.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/msvc.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/namespaces.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/package_index.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/py27compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/py27compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/py31compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/py31compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/py33compat.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/py33compat.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/sandbox.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/ssl_support.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/ssl_support.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/unicode_utils.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/wheel.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools/windows_support.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/LICENSE` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/METADATA` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/RECORD` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/entry_points.txt` & `txapi-1.0.2/venv/lib/python3.8/site-packages/setuptools-49.2.1.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/tomli/_parser.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/tomli/_re.py` & `txapi-1.0.2/venv/lib/python3.8/site-packages/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/LICENSE` & `txapi-1.0.2/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/METADATA` & `txapi-1.0.2/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `txapi-1.0.1/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/RECORD` & `txapi-1.0.2/venv/lib/python3.8/site-packages/tomli-2.0.1.dist-info/RECORD`

 * *Files identical despite different names*

