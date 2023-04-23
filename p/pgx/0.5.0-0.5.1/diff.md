# Comparing `tmp/pgx-0.5.0.tar.gz` & `tmp/pgx-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.5.0.tar", last modified: Fri Apr 21 12:12:49 2023, max compression
+gzip compressed data, was "pgx-0.5.1.tar", last modified: Sun Apr 23 03:41:09 2023, max compression
```

## Comparing `pgx-0.5.0.tar` & `pgx-0.5.1.tar`

### file list

```diff
@@ -1,139 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.531345 pgx-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 12:12:38.000000 pgx-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-21 12:12:49.531345 pgx-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-21 12:12:38.000000 pgx-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.515344 pgx-0.5.0/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 11106175 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.519344 pgx-0.5.0/pgx/_dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.519344 pgx-0.5.0/pgx/_dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.519344 pgx-0.5.0/pgx/_dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.523344 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_dwg/tictactoe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.523344 pgx-0.5.0/pgx/_flax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_flax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_flax/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_flax/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.523344 pgx-0.5.0/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_mahjong/_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27595 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18324 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    44190 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.527345 pgx-0.5.0/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/experimental/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/experimental/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18437 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.527345 pgx-0.5.0/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    25922 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-21 12:12:38.000000 pgx-0.5.0/pgx/tic_tac_toe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.515344 pgx-0.5.0/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-21 12:12:49.000000 pgx-0.5.0/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-21 12:12:49.000000 pgx-0.5.0/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:12:49.000000 pgx-0.5.0/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-21 12:12:49.000000 pgx-0.5.0/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 12:12:49.000000 pgx-0.5.0/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-21 12:12:38.000000 pgx-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:12:49.531345 pgx-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-21 12:12:38.000000 pgx-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:49.531345 pgx-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    61403 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    39629 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-21 12:12:38.000000 pgx-0.5.0/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.852263 pgx-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 03:41:00.000000 pgx-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-23 03:41:09.852263 pgx-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-04-23 03:41:00.000000 pgx-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_mahjong/_hand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx/_src/dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx/_src/dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.844263 pgx-0.5.1/pgx/_src/dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.848263 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/dwg/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27792 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/_src/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44159 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28910 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/connect_four.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.848263 pgx-0.5.1/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/pettingzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/experimental/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.848263 pgx-0.5.1/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25891 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20618 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21201 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-23 03:41:00.000000 pgx-0.5.1/pgx/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.840263 pgx-0.5.1/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-23 03:41:09.000000 pgx-0.5.1/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-23 03:41:09.000000 pgx-0.5.1/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 03:41:09.000000 pgx-0.5.1/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-23 03:41:09.000000 pgx-0.5.1/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 03:41:09.000000 pgx-0.5.1/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-23 03:41:00.000000 pgx-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 03:41:09.852263 pgx-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-23 03:41:00.000000 pgx-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:09.852263 pgx-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61403 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39629 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-23 03:41:00.000000 pgx-0.5.1/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.5.0/LICENSE` & `pgx-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/PKG-INFO` & `pgx-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.5.0
+Version: 0.5.1
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.5.0 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.5.1 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
```

### Comparing `pgx-0.5.0/README.md` & `pgx-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/animalshogi.py` & `pgx-0.5.1/pgx/_src/dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/backgammon.py` & `pgx-0.5.1/pgx/_src/dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/bridge_bidding.py` & `pgx-0.5.1/pgx/_src/dwg/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/chess.py` & `pgx-0.5.1/pgx/_src/dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/connect_four.py` & `pgx-0.5.1/pgx/_src/dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/go.py` & `pgx-0.5.1/pgx/_src/dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/hex.py` & `pgx-0.5.1/pgx/_src/dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/LICENSE` & `pgx-0.5.1/pgx/_src/dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/bBishop.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/bKing.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/bKnight.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/bPawn.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/bQueen.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/bRook.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/wBishop.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/wKing.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/wKnight.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/wPawn.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/wQueen.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/chess/wRook.svg` & `pgx-0.5.1/pgx/_src/dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/b.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.5.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/kuhn_poker.py` & `pgx-0.5.1/pgx/_src/dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/leduc_holdem.py` & `pgx-0.5.1/pgx/_src/dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/othello.py` & `pgx-0.5.1/pgx/_src/dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/play2048.py` & `pgx-0.5.1/pgx/_src/dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/shogi.py` & `pgx-0.5.1/pgx/_src/dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/sparrow_mahjong.py` & `pgx-0.5.1/pgx/_src/dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_dwg/tictactoe.py` & `pgx-0.5.1/pgx/_src/dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_flax/struct.py` & `pgx-0.5.1/pgx/_src/struct.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+# NOTE: This file is copied from Flax (https://github.com/google/flax).
+# Copyright belongs to the original authors.
+# We keep tracking the updates of original Flax implementation.
+# We try to minimize the modification to this file. Exceptions includes:
+#   - automatic formatting
+#   - type checking suppression
+#   - support for various JAX versions
+#   - dynamic import of Flax to support dataclass serialization
+
 # Copyright 2023 The Flax Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,214 +21,236 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utilities for defining custom classes that can be used with jax transformations.
 """
 
 import dataclasses
-from typing import TypeVar, Callable, Tuple, Union, Any
-
-from . import serialization
+from typing import TypeVar
 
 import jax
-from typing_extensions import dataclass_transform  # pytype: disable=not-supported-yet
-
+from typing_extensions import (  # pytype: disable=not-supported-yet
+    dataclass_transform,
+)
+
+has_flax = True
+try:
+    from flax import serialization  # type: ignore
+except ImportError:
+    has_flax = False
 
 _T = TypeVar("_T")
 
 
 def field(pytree_node=True, **kwargs):
-  return dataclasses.field(metadata={'pytree_node': pytree_node}, **kwargs)
+    return dataclasses.field(metadata={"pytree_node": pytree_node}, **kwargs)
 
 
-@dataclass_transform(field_descriptors=(field,)) # type: ignore[literal-required]
+@dataclass_transform(field_descriptors=(field,))  # type: ignore[literal-required]
 def dataclass(clz: _T) -> _T:
-  """Create a class which can be passed to functional transformations.
+    """Create a class which can be passed to functional transformations.
 
-  NOTE: Inherit from ``PyTreeNode`` instead to avoid type checking issues when
-  using PyType.
+    NOTE: Inherit from ``PyTreeNode`` instead to avoid type checking issues when
+    using PyType.
 
-  Jax transformations such as `jax.jit` and `jax.grad` require objects that are
-  immutable and can be mapped over using the `jax.tree_util` methods.
-  The `dataclass` decorator makes it easy to define custom classes that can be
-  passed safely to Jax. For example::
-
-    from flax import struct
-
-    @struct.dataclass
-    class Model:
-      params: Any
-      # use pytree_node=False to indicate an attribute should not be touched
-      # by Jax transformations.
-      apply_fn: FunctionType = struct.field(pytree_node=False)
-
-      def __apply__(self, *args):
-        return self.apply_fn(*args)
-
-    model = Model(params, apply_fn)
-
-    model.params = params_b  # Model is immutable. This will raise an error.
-    model_b = model.replace(params=params_b)  # Use the replace method instead.
-
-    # This class can now be used safely in Jax to compute gradients w.r.t. the
-    # parameters.
-    model = Model(params, apply_fn)
-    model_grad = jax.grad(some_loss_fn)(model)
-
-  Note that dataclasses have an auto-generated ``__init__`` where
-  the arguments of the constructor and the attributes of the created
-  instance match 1:1. This correspondence is what makes these objects
-  valid containers that work with JAX transformations and
-  more generally the `jax.tree_util` library.
-
-  Sometimes a "smart constructor" is desired, for example because
-  some of the attributes can be (optionally) derived from others.
-  The way to do this with Flax dataclasses is to make a static or
-  class method that provides the smart constructor.
-  This way the simple constructor used by `jax.tree_util` is
-  preserved. Consider the following example::
-
-    @struct.dataclass
-    class DirectionAndScaleKernel:
-      direction: Array
-      scale: Array
-
-      @classmethod
-      def create(cls, kernel):
-        scale = jax.numpy.linalg.norm(kernel, axis=0, keepdims=True)
-        directin = direction / scale
-        return cls(direction, scale)
-
-  Args:
-    clz: the class that will be transformed by the decorator.
-  Returns:
-    The new class.
-  """
-  # check if already a flax dataclass
-  if '_flax_dataclass' in clz.__dict__:
-    return clz
-
-  data_clz = dataclasses.dataclass(frozen=True)(clz) # type: ignore
-  meta_fields = []
-  data_fields = []
-  for field_info in dataclasses.fields(data_clz):
-    is_pytree_node = field_info.metadata.get('pytree_node', True)
-    if is_pytree_node:
-      data_fields.append(field_info.name)
+    Jax transformations such as `jax.jit` and `jax.grad` require objects that are
+    immutable and can be mapped over using the `jax.tree_util` methods.
+    The `dataclass` decorator makes it easy to define custom classes that can be
+    passed safely to Jax. For example::
+
+      from flax import struct
+
+      @struct.dataclass
+      class Model:
+        params: Any
+        # use pytree_node=False to indicate an attribute should not be touched
+        # by Jax transformations.
+        apply_fn: FunctionType = struct.field(pytree_node=False)
+
+        def __apply__(self, *args):
+          return self.apply_fn(*args)
+
+      model = Model(params, apply_fn)
+
+      model.params = params_b  # Model is immutable. This will raise an error.
+      model_b = model.replace(params=params_b)  # Use the replace method instead.
+
+      # This class can now be used safely in Jax to compute gradients w.r.t. the
+      # parameters.
+      model = Model(params, apply_fn)
+      model_grad = jax.grad(some_loss_fn)(model)
+
+    Note that dataclasses have an auto-generated ``__init__`` where
+    the arguments of the constructor and the attributes of the created
+    instance match 1:1. This correspondence is what makes these objects
+    valid containers that work with JAX transformations and
+    more generally the `jax.tree_util` library.
+
+    Sometimes a "smart constructor" is desired, for example because
+    some of the attributes can be (optionally) derived from others.
+    The way to do this with Flax dataclasses is to make a static or
+    class method that provides the smart constructor.
+    This way the simple constructor used by `jax.tree_util` is
+    preserved. Consider the following example::
+
+      @struct.dataclass
+      class DirectionAndScaleKernel:
+        direction: Array
+        scale: Array
+
+        @classmethod
+        def create(cls, kernel):
+          scale = jax.numpy.linalg.norm(kernel, axis=0, keepdims=True)
+          directin = direction / scale
+          return cls(direction, scale)
+
+    Args:
+      clz: the class that will be transformed by the decorator.
+    Returns:
+      The new class.
+    """
+    # check if already a flax dataclass
+    if "_flax_dataclass" in clz.__dict__:
+        return clz
+
+    data_clz = dataclasses.dataclass(frozen=True)(clz)  # type: ignore
+    meta_fields = []
+    data_fields = []
+    for field_info in dataclasses.fields(data_clz):
+        is_pytree_node = field_info.metadata.get("pytree_node", True)
+        if is_pytree_node:
+            data_fields.append(field_info.name)
+        else:
+            meta_fields.append(field_info.name)
+
+    def replace(self, **updates):
+        """ "Returns a new object replacing the specified fields with new values."""
+        return dataclasses.replace(self, **updates)
+
+    data_clz.replace = replace
+
+    def iterate_clz(x):
+        meta = tuple(getattr(x, name) for name in meta_fields)
+        data = tuple(getattr(x, name) for name in data_fields)
+        return data, meta
+
+    def iterate_clz_with_keys(x):
+        meta = tuple(getattr(x, name) for name in meta_fields)
+        data = tuple(
+            (jax.tree_util.GetAttrKey(name), getattr(x, name))
+            for name in data_fields
+        )
+        return data, meta
+
+    def clz_from_iterable(meta, data):
+        meta_args = tuple(zip(meta_fields, meta))
+        data_args = tuple(zip(data_fields, data))
+        kwargs = dict(meta_args + data_args)
+        return data_clz(**kwargs)
+
+    if hasattr(jax.tree_util, "register_pytree_with_keys"):
+        jax.tree_util.register_pytree_with_keys(
+            data_clz, iterate_clz_with_keys, clz_from_iterable
+        )
     else:
-      meta_fields.append(field_info.name)
-
-  def replace(self, **updates):
-    """"Returns a new object replacing the specified fields with new values."""
-    return dataclasses.replace(self, **updates)
-
-  data_clz.replace = replace
-
-  def iterate_clz(x):
-    meta = tuple(getattr(x, name) for name in meta_fields)
-    data = tuple(getattr(x, name) for name in data_fields)
-    return data, meta
-
-  def iterate_clz_with_keys(x):
-    meta = tuple(getattr(x, name) for name in meta_fields)
-    data = tuple(
-        (jax.tree_util.GetAttrKey(name), getattr(x, name))
-        for name in data_fields
-    )
-    return data, meta
-
-  def clz_from_iterable(meta, data):
-    meta_args = tuple(zip(meta_fields, meta))
-    data_args = tuple(zip(data_fields, data))
-    kwargs = dict(meta_args + data_args)
-    return data_clz(**kwargs)
-
-  if hasattr(jax.tree_util, 'register_pytree_with_keys'):
-    jax.tree_util.register_pytree_with_keys(
-        data_clz, iterate_clz_with_keys, clz_from_iterable
-    )
-  else:
-    jax.tree_util.register_pytree_node(data_clz, iterate_clz, clz_from_iterable)
-    def keypaths(_):
-      return [
-          jax.tree_util.AttributeKeyPathEntry(name) for name in data_fields
-      ]
-    jax.tree_util.register_keypaths(data_clz, keypaths)
-
-  def to_state_dict(x):
-    state_dict = {name: serialization.to_state_dict(getattr(x, name))
-                  for name in data_fields}
-    return state_dict
-
-  def from_state_dict(x, state):
-    """Restore the state of a data class."""
-    state = state.copy()  # copy the state so we can pop the restored fields.
-    updates = {}
-    for name in data_fields:
-      if name not in state:
-        raise ValueError(f'Missing field {name} in state dict while restoring'
-                         f' an instance of {clz.__name__},'
-                         f' at path {serialization.current_path()}')
-      value = getattr(x, name)
-      value_state = state.pop(name)
-      updates[name] = serialization.from_state_dict(value, value_state, name=name)
-    if state:
-      names = ','.join(state.keys())
-      raise ValueError(f'Unknown field(s) "{names}" in state dict while'
-                       f' restoring an instance of {clz.__name__}'
-                       f' at path {serialization.current_path()}')
-    return x.replace(**updates)
-
-  serialization.register_serialization_state(
-      data_clz, to_state_dict, from_state_dict)
-
-  # add a _flax_dataclass flag to distinguish from regular dataclasses
-  data_clz._flax_dataclass = True # type: ignore[attr-defined]
+        jax.tree_util.register_pytree_node(
+            data_clz, iterate_clz, clz_from_iterable
+        )
+
+        def keypaths(_):
+            return [
+                jax.tree_util.AttributeKeyPathEntry(name)
+                for name in data_fields
+            ]
+
+        jax.tree_util.register_keypaths(data_clz, keypaths)
+
+    def to_state_dict(x):
+        state_dict = {
+            name: serialization.to_state_dict(getattr(x, name))
+            for name in data_fields
+        }
+        return state_dict
+
+    def from_state_dict(x, state):
+        """Restore the state of a data class."""
+        state = (
+            state.copy()
+        )  # copy the state so we can pop the restored fields.
+        updates = {}
+        for name in data_fields:
+            if name not in state:
+                raise ValueError(
+                    f"Missing field {name} in state dict while restoring"
+                    f" an instance of {clz.__name__},"
+                    f" at path {serialization.current_path()}"
+                )
+            value = getattr(x, name)
+            value_state = state.pop(name)
+            updates[name] = serialization.from_state_dict(
+                value, value_state, name=name
+            )
+        if state:
+            names = ",".join(state.keys())
+            raise ValueError(
+                f'Unknown field(s) "{names}" in state dict while'
+                f" restoring an instance of {clz.__name__}"
+                f" at path {serialization.current_path()}"
+            )
+        return x.replace(**updates)
+
+    if has_flax:
+        serialization.register_serialization_state(
+            data_clz, to_state_dict, from_state_dict
+        )
+
+    # add a _flax_dataclass flag to distinguish from regular dataclasses
+    data_clz._flax_dataclass = True  # type: ignore[attr-defined]
 
-  return data_clz # type: ignore
+    return data_clz  # type: ignore
 
 
-TNode = TypeVar('TNode', bound='PyTreeNode')
+TNode = TypeVar("TNode", bound="PyTreeNode")
 
 
-@dataclass_transform(field_descriptors=(field,)) # type: ignore[literal-required]
+@dataclass_transform(field_descriptors=(field,))  # type: ignore[literal-required]
 class PyTreeNode:
-  """Base class for dataclasses that should act like a JAX pytree node.
+    """Base class for dataclasses that should act like a JAX pytree node.
 
-  See ``flax.struct.dataclass`` for the ``jax.tree_util`` behavior.
-  This base class additionally avoids type checking errors when using PyType.
+    See ``flax.struct.dataclass`` for the ``jax.tree_util`` behavior.
+    This base class additionally avoids type checking errors when using PyType.
 
-  Example::
+    Example::
 
-    from flax import struct
+      from flax import struct
 
-    class Model(struct.PyTreeNode):
-      params: Any
-      # use pytree_node=False to indicate an attribute should not be touched
-      # by Jax transformations.
-      apply_fn: FunctionType = struct.field(pytree_node=False)
+      class Model(struct.PyTreeNode):
+        params: Any
+        # use pytree_node=False to indicate an attribute should not be touched
+        # by Jax transformations.
+        apply_fn: FunctionType = struct.field(pytree_node=False)
 
-      def __apply__(self, *args):
-        return self.apply_fn(*args)
+        def __apply__(self, *args):
+          return self.apply_fn(*args)
 
-    model = Model(params, apply_fn)
+      model = Model(params, apply_fn)
 
-    model.params = params_b  # Model is immutable. This will raise an error.
-    model_b = model.replace(params=params_b)  # Use the replace method instead.
+      model.params = params_b  # Model is immutable. This will raise an error.
+      model_b = model.replace(params=params_b)  # Use the replace method instead.
 
-    # This class can now be used safely in Jax to compute gradients w.r.t. the
-    # parameters.
-    model = Model(params, apply_fn)
-    model_grad = jax.grad(some_loss_fn)(model)
+      # This class can now be used safely in Jax to compute gradients w.r.t. the
+      # parameters.
+      model = Model(params, apply_fn)
+      model_grad = jax.grad(some_loss_fn)(model)
 
-  """
+    """
 
-  def __init_subclass__(cls):
-    dataclass(cls)  # pytype: disable=wrong-arg-types
+    def __init_subclass__(cls):
+        dataclass(cls)  # pytype: disable=wrong-arg-types
 
-  def __init__(self, *args, **kwargs):
-    # stub for pytype
-    raise NotImplementedError
+    def __init__(self, *args, **kwargs):
+        # stub for pytype
+        raise NotImplementedError
 
-  def replace(self: TNode, **overrides) -> TNode:
-    # stub for pytype
-    raise NotImplementedError
+    def replace(self: TNode, **overrides) -> TNode:
+        # stub for pytype
+        raise NotImplementedError
```

### Comparing `pgx-0.5.0/pgx/_mahjong/_hand.py` & `pgx-0.5.1/pgx/_mahjong/_hand.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/_shogi_utils.py` & `pgx-0.5.1/pgx/_src/shogi_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,43 +8,99 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+
 import jax
 import jax.numpy as jnp
-
-from pgx._cache import load_shogi_init_legal_action_mask  # type: ignore
-from pgx._cache import load_shogi_is_on_the_way  # type: ignore
-from pgx._cache import load_shogi_legal_from_idx  # type: ignore
-from pgx._cache import load_shogi_raw_effect_boards  # type: ignore
+import numpy as np
 
 # fmt: off
 INIT_PIECE_BOARD = jnp.int8([[15, -1, 14, -1, -1, -1, 0, -1, 1],  # noqa: E241
                              [16, 18, 14, -1, -1, -1, 0,  5, 2],  # noqa: E241
                              [17, -1, 14, -1, -1, -1, 0, -1, 3],  # noqa: E241
                              [20, -1, 14, -1, -1, -1, 0, -1, 6],  # noqa: E241
                              [21, -1, 14, -1, -1, -1, 0, -1, 7],  # noqa: E241
                              [20, -1, 14, -1, -1, -1, 0, -1, 6],  # noqa: E241
                              [17, -1, 14, -1, -1, -1, 0, -1, 3],  # noqa: E241
                              [16, 19, 14, -1, -1, -1, 0,  4, 2],  # noqa: E241
                              [15, -1, 14, -1, -1, -1, 0, -1, 1]]).flatten()  # noqa: E241
 # fmt: on
 
 # Can <piece,14> reach from <from,81> to <to,81> ignoring pieces on board?
-CAN_MOVE = load_shogi_raw_effect_boards()  # bool (14, 81, 81)
+file_path = "assets/can_move.npy"
+with open(os.path.join(os.path.dirname(__file__), file_path), "rb") as f:
+    CAN_MOVE = jnp.load(f)
+assert CAN_MOVE.sum() == 8228
+
+
 # When <lance/bishop/rook/horse/dragon,5> moves from <from,81> to <to,81>,
 # is <point,81> on the way between two points?
-BETWEEN = load_shogi_is_on_the_way()  # bool (5, 81, 81, 81)
-# Give <dir,10> and <to,81>, return the legal from idx
-# E.g. LEGAL_FROM_IDX[Up, to=19] = [20, 21, ..., -1]
+file_path = "assets/between.npy"
+with open(os.path.join(os.path.dirname(__file__), file_path), "rb") as f:
+    BETWEEN = jnp.load(f)
+assert BETWEEN.sum() == 10564
+
+# Give <dir,10> and <to,81>, return the legal <from> idx
+# E.g. LEGAL_FROM_IDX[Up, to=19] = [20, 21, ..., -1] (filled by -1)
 # Used for computing dlshogi action
-LEGAL_FROM_IDX = load_shogi_legal_from_idx()  # (10, 81, 8)
+#
+#  dir, to, from
+#  (10, 81, 81)
+#
+#  0 Up
+#  1 Up left
+#  2 Up right
+#  3 Left
+#  4 Right
+#  5 Down
+#  6 Down left
+#  7 Down right
+#  8 Up2 left
+#  9 Up2 right
+
+LEGAL_FROM_IDX = -np.ones((10, 81, 8), dtype=jnp.int32)  # type: ignore
+
+for dir_ in range(10):
+    for to in range(81):
+        x, y = to // 9, to % 9
+        if dir_ == 0:  # Up
+            dx, dy = 0, +1
+        elif dir_ == 1:  # Up left
+            dx, dy = -1, +1
+        elif dir_ == 2:  # Up right
+            dx, dy = +1, +1
+        elif dir_ == 3:  # Left
+            dx, dy = -1, 0
+        elif dir_ == 4:  # Right
+            dx, dy = +1, 0
+        elif dir_ == 5:  # Down
+            dx, dy = 0, -1
+        elif dir_ == 6:  # Down left
+            dx, dy = -1, -1
+        elif dir_ == 7:  # Down right
+            dx, dy = +1, -1
+        elif dir_ == 8:  # Up2 left
+            dx, dy = -1, +2
+        elif dir_ == 9:  # Up2 right
+            dx, dy = +1, +2
+        for i in range(8):
+            x += dx
+            y += dy
+            if x < 0 or 8 < x or y < 0 or 8 < y:
+                break
+            LEGAL_FROM_IDX[dir_, to, i] = x * 9 + y
+            if dir_ == 8 or dir_ == 9:
+                break
+
+LEGAL_FROM_IDX = jnp.array(LEGAL_FROM_IDX)  # type: ignore
 
 
 @jax.jit
 @jax.vmap
 def can_move_any_ix(from_):
     return jnp.nonzero(
         (CAN_MOVE[:, from_, :] | CAN_MOVE[:, :, from_]).any(axis=0),
@@ -76,15 +132,22 @@
         (0, None, None),
     )
 )(jnp.arange(5), jnp.arange(81), jnp.arange(81))
 
 
 CAN_MOVE_ANY = can_move_any_ix(jnp.arange(81))  # (81, 36)
 
-INIT_LEGAL_ACTION_MASK = load_shogi_init_legal_action_mask()
+INIT_LEGAL_ACTION_MASK = jnp.zeros(81 * 27, dtype=jnp.bool_)
+# fmt: off
+ixs = [5, 7, 14, 23, 25, 32, 34, 41, 43, 50, 52, 59, 61, 68, 77, 79, 115, 124, 133, 142, 187, 196, 205, 214, 268, 277, 286, 295, 304, 331]
+# fmt: on
+for ix in ixs:
+    INIT_LEGAL_ACTION_MASK = INIT_LEGAL_ACTION_MASK.at[ix].set(True)
+assert INIT_LEGAL_ACTION_MASK.shape == (81 * 27,)
+assert INIT_LEGAL_ACTION_MASK.sum() == 30
 
 
 def _around(c):
     x, y = c // 9, c % 9
     dx = jnp.int8([-1, -1, 0, +1, +1, +1, 0, -1])
     dy = jnp.int8([0, -1, -1, -1, 0, +1, +1, +1])
```

### Comparing `pgx-0.5.0/pgx/_test.py` & `pgx-0.5.1/pgx/_src/api_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 import os
 from dataclasses import fields
 
 import jax
 import jax.numpy as jnp
 
-from pgx.core import Env, State, available_games
 from pgx.experimental.utils import act_randomly
+from pgx.v1 import Env, State, available_games
 
 act_randomly = jax.jit(act_randomly)
 
 
 def api_test(env: Env, num: int = 100):
     api_test_single(env, num)
     api_test_batch(env, num)
```

### Comparing `pgx-0.5.0/pgx/_visualizer.py` & `pgx-0.5.1/pgx/_src/visualizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import math
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Literal, Optional, Sequence, Union
 
 import svgwrite  # type: ignore
 
-from .core import State
+from pgx.v1 import State
 
 ColorTheme = Literal["light", "dark"]
 
 
 @dataclass
 class Config:
     color_theme: ColorTheme = "light"
@@ -182,15 +182,15 @@
             )
         group.scale(SCALE)
         dwg.add(group)
         return dwg
 
     def _set_config_by_state(self, _state: State):  # noqa: C901
         if _state.env_id == "animal_shogi":
-            from ._dwg.animalshogi import _make_animalshogi_dwg
+            from pgx._src.dwg.animalshogi import _make_animalshogi_dwg
 
             self.config["GRID_SIZE"] = 60
             self.config["BOARD_WIDTH"] = 4
             self.config["BOARD_HEIGHT"] = 4
             self._make_dwg_group = _make_animalshogi_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -212,15 +212,15 @@
                     "black",
                     "black",
                     "white",
                     "black",
                     "",
                 )
         elif _state.env_id == "backgammon":
-            from ._dwg.backgammon import _make_backgammon_dwg
+            from pgx._src.dwg.backgammon import _make_backgammon_dwg
 
             self.config["GRID_SIZE"] = 25
             self.config["BOARD_WIDTH"] = 17
             self.config["BOARD_HEIGHT"] = 14
             self._make_dwg_group = _make_backgammon_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -242,15 +242,15 @@
                     "lightgray",
                     "white",
                     "white",
                     "black",
                     "gray",
                 )
         elif _state.env_id == "bridge_bidding":
-            from ._dwg.bridge_bidding import _make_bridge_dwg
+            from pgx._src.dwg.bridge_bidding import _make_bridge_dwg
 
             self.config["GRID_SIZE"] = 50
             self.config["BOARD_WIDTH"] = 14
             self.config["BOARD_HEIGHT"] = 10
             self._make_dwg_group = _make_bridge_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -272,15 +272,15 @@
                     "lightgray",
                     "white",
                     "white",
                     "black",
                     "black",
                 )
         elif _state.env_id == "chess":
-            from ._dwg.chess import _make_chess_dwg
+            from pgx._src.dwg.chess import _make_chess_dwg
 
             self.config["GRID_SIZE"] = 50
             self.config["BOARD_WIDTH"] = 8
             self.config["BOARD_HEIGHT"] = 8
             self._make_dwg_group = _make_chess_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -302,15 +302,15 @@
                     "gray",
                     "white",
                     "white",
                     "black",
                     "",
                 )
         elif _state.env_id == "connect_four":
-            from ._dwg.connect_four import _make_connect_four_dwg
+            from pgx._src.dwg.connect_four import _make_connect_four_dwg
 
             self.config["GRID_SIZE"] = 35
             self.config["BOARD_WIDTH"] = 7
             self.config["BOARD_HEIGHT"] = 7
             self._make_dwg_group = _make_connect_four_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -332,15 +332,15 @@
                     "black",
                     "black",
                     "white",
                     "black",
                     "gray",
                 )
         elif _state.env_id in ("go-9x9", "go-19x19"):
-            from ._dwg.go import _make_go_dwg
+            from pgx._src.dwg.go import _make_go_dwg
 
             self.config["GRID_SIZE"] = 25
             try:
                 self.config["BOARD_WIDTH"] = int(_state.size[0])  # type:ignore
                 self.config["BOARD_HEIGHT"] = int(
                     _state.size[0]  # type:ignore
                 )
@@ -370,15 +370,15 @@
                     "white",
                     "black",
                     "",
                 )
         elif _state.env_id == "hex":
             import jax.numpy as jnp
 
-            from ._dwg.hex import _make_hex_dwg, four_dig
+            from pgx._src.dwg.hex import _make_hex_dwg, four_dig
 
             self.config["GRID_SIZE"] = 30
             try:
                 self.config["BOARD_WIDTH"] = four_dig(
                     _state.size[0] * 1.5  # type:ignore
                 )
                 self.config["BOARD_HEIGHT"] = four_dig(
@@ -412,15 +412,15 @@
                     "black",
                     "black",
                     "white",
                     "black",
                     "lightgray",
                 )
         elif _state.env_id == "kuhn_poker":
-            from ._dwg.kuhn_poker import _make_kuhnpoker_dwg
+            from pgx._src.dwg.kuhn_poker import _make_kuhnpoker_dwg
 
             self.config["GRID_SIZE"] = 30
             self.config["BOARD_WIDTH"] = 8
             self.config["BOARD_HEIGHT"] = 8
             self._make_dwg_group = _make_kuhnpoker_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -442,15 +442,15 @@
                     "black",
                     "black",
                     "white",
                     "black",
                     "",
                 )
         elif _state.env_id == "leduc_holdem":
-            from ._dwg.leduc_holdem import _make_leducHoldem_dwg
+            from pgx._src.dwg.leduc_holdem import _make_leducHoldem_dwg
 
             self.config["GRID_SIZE"] = 30
             self.config["BOARD_WIDTH"] = 8
             self.config["BOARD_HEIGHT"] = 8
             self._make_dwg_group = _make_leducHoldem_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -472,15 +472,15 @@
                     "",
                     "",
                     "white",
                     "black",
                     "",
                 )
         elif _state.env_id == "othello":
-            from ._dwg.othello import _make_othello_dwg
+            from pgx._src.dwg.othello import _make_othello_dwg
 
             self.config["GRID_SIZE"] = 30
             self.config["BOARD_WIDTH"] = 8
             self.config["BOARD_HEIGHT"] = 8
             self._make_dwg_group = _make_othello_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -502,15 +502,15 @@
                     "black",
                     "black",
                     "white",
                     "black",
                     "",
                 )
         elif _state.env_id == "2048":
-            from ._dwg.play2048 import _make_2048_dwg
+            from pgx._src.dwg.play2048 import _make_2048_dwg
 
             self.config["GRID_SIZE"] = 50
             self.config["BOARD_WIDTH"] = 4
             self.config["BOARD_HEIGHT"] = 4
             self._make_dwg_group = _make_2048_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -532,15 +532,15 @@
                     "",
                     "",
                     "white",
                     "black",
                     "black",
                 )
         elif _state.env_id == "shogi":
-            from ._dwg.shogi import _make_shogi_dwg
+            from pgx._src.dwg.shogi import _make_shogi_dwg
 
             self.config["GRID_SIZE"] = 50
             self.config["BOARD_WIDTH"] = 10
             self.config["BOARD_HEIGHT"] = 9
             self._make_dwg_group = _make_shogi_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -556,15 +556,15 @@
                     "black",
                     "black",
                     "white",
                     "black",
                     "",
                 )
         elif _state.env_id == "sparrow_mahjong":
-            from ._dwg.sparrow_mahjong import _make_sparrowmahjong_dwg
+            from pgx._src.dwg.sparrow_mahjong import _make_sparrowmahjong_dwg
 
             self.config["GRID_SIZE"] = 50
             self.config["BOARD_WIDTH"] = 15
             self.config["BOARD_HEIGHT"] = 10
             self._make_dwg_group = _make_sparrowmahjong_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -586,15 +586,15 @@
                     "gray",
                     "white",
                     "white",
                     "silver",
                     "black",
                 )
         elif _state.env_id == "tic_tac_toe":
-            from ._dwg.tictactoe import _make_tictactoe_dwg
+            from pgx._src.dwg.tictactoe import _make_tictactoe_dwg
 
             self.config["GRID_SIZE"] = 60
             self.config["BOARD_WIDTH"] = 3
             self.config["BOARD_HEIGHT"] = 3
             self._make_dwg_group = _make_tictactoe_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
@@ -614,122 +614,122 @@
                 )
         else:
             assert False
 
     # TODO: simplify me
     def _get_nth_state(self, _states: State, _i):
         if _states.env_id == "animal_shogi":
-            from ._dwg.animalshogi import AnimalShogiState
+            from pgx._src.dwg.animalshogi import AnimalShogiState
 
             return AnimalShogiState(
                 turn=_states.turn[_i],  # type:ignore
                 board=_states.board[_i],  # type:ignore
                 hand=_states.hand[_i],  # type:ignore
             )
         elif _states.env_id == "backgammon":
-            from ._dwg.backgammon import BackgammonState
+            from pgx._src.dwg.backgammon import BackgammonState
 
             return BackgammonState(
                 turn=_states.turn[_i],  # type:ignore
                 board=_states.board[_i],  # type:ignore
             )
         elif _states.env_id == "connect_four":
-            from ._dwg.connect_four import ConnectFourState
+            from pgx._src.dwg.connect_four import ConnectFourState
 
             return ConnectFourState(  # type:ignore
                 turn=_states.turn[_i],  # type:ignore
                 board=_states.board[_i],  # type:ignore
             )
         elif _states.env_id == "chess":
-            from ._dwg.chess import ChessState
+            from pgx._src.dwg.chess import ChessState
 
             return ChessState(
                 turn=_states.turn[_i],  # type:ignore
                 board=_states.board[_i],  # type:ignore
             )
         elif _states.env_id == "bridge_bidding":
-            from ._dwg.bridge_bidding import BridgeBiddingState
+            from pgx._src.dwg.bridge_bidding import BridgeBiddingState
 
             return BridgeBiddingState(  # type:ignore
                 turn=_states.turn[_i],  # type:ignore
                 dealer=_states.dealer[_i],  # type:ignore
                 current_player=_states.current_player[_i],  # type:ignore
                 hand=_states.hand[_i],  # type:ignore
                 bidding_history=_states.bidding_history[_i],  # type:ignore
                 vul_NS=_states.vul_NS[_i],  # type:ignore
                 vul_EW=_states.vul_EW[_i],  # type:ignore
             )
         elif _states.env_id in ("go-9x9", "go-19x19"):
-            from ._dwg.go import GoState
+            from pgx._src.dwg.go import GoState
 
             return GoState(  # type:ignore
                 size=_states.size[_i],  # type:ignore
                 chain_id_board=_states.chain_id_board[_i],  # type:ignore
                 turn=_states.turn[_i],  # type:ignore
             )
         elif _states.env_id == "hex":
-            from ._dwg.hex import HexState
+            from pgx._src.dwg.hex import HexState
 
             return HexState(
                 size=_states.size[_i],  # type:ignore
                 turn=_states.turn[_i],  # type:ignore
                 board=_states.board[_i],  # type:ignore
             )
         elif _states.env_id == "kuhn_poker":
-            from ._dwg.kuhn_poker import KuhnPokerState
+            from pgx._src.dwg.kuhn_poker import KuhnPokerState
 
             return KuhnPokerState(
                 cards=_states.cards[_i], pot=_states.pot[_i]  # type:ignore
             )
         elif _states.env_id == "leduc_holdem":
-            from ._dwg.leduc_holdem import LeducHoldemState
+            from pgx._src.dwg.leduc_holdem import LeducHoldemState
 
             return LeducHoldemState(
                 cards=_states.cards[_i],  # type:ignore
                 chips=_states.chips[_i],  # type:ignore
                 round=_states.round[_i],  # type:ignore
             )
         elif _states.env_id == "othello":
-            from ._dwg.othello import OthelloState
+            from pgx._src.dwg.othello import OthelloState
 
             return OthelloState(
                 turn=_states.turn[_i],  # type:ignore
                 board=_states.board[_i],  # type:ignore
             )
         elif _states.env_id == "2048":
-            from ._dwg.play2048 import Play2048State
+            from pgx._src.dwg.play2048 import Play2048State
 
             return Play2048State(
                 board=_states.board[_i],  # type:ignore
             )
         elif _states.env_id == "shogi":
-            from ._dwg.shogi import ShogiState
+            from pgx._src.dwg.shogi import ShogiState
 
             return ShogiState(  # type:ignore
                 turn=_states.turn[_i],  # type:ignore
                 piece_board=_states.piece_board[_i],  # type:ignore
                 hand=_states.hand[_i],  # type:ignore
             )
         elif _states.env_id == "sparrow_mahjong":
-            from ._dwg.sparrow_mahjong import SparrowMahjongState
+            from pgx._src.dwg.sparrow_mahjong import SparrowMahjongState
 
             return SparrowMahjongState(
                 current_player=_states.current_player[_i],  # type:ignore
                 turn=_states.turn[_i],  # type:ignore
                 rivers=_states.rivers[_i],  # type:ignore
                 hands=_states.hands[_i],  # type:ignore
                 n_red_in_hands=_states.n_red_in_hands[_i],  # type:ignore
                 is_red_in_river=_states.is_red_in_river[_i],  # type:ignore
                 wall=_states.wall[_i],  # type:ignore
                 draw_ix=_states.draw_ix[_i],  # type:ignore
                 shuffled_players=_states.shuffled_players[_i],  # type:ignore
                 dora=_states.dora[_i],  # type:ignore
             )
         elif _states.env_id == "tic_tac_toe":
-            from ._dwg.tictactoe import TictactoeState
+            from pgx._src.dwg.tictactoe import TictactoeState
 
             return TictactoeState(
                 current_player=_states.current_player[_i],  # type:ignore
                 legal_action_mask=_states.legal_action_mask[_i],  # type:ignore
                 terminated=_states.terminated[_i],  # type:ignore
                 turn=_states.turn[_i],  # type:ignore
                 board=_states.board[_i],  # type:ignore
```

### Comparing `pgx-0.5.0/pgx/animal_shogi.py` & `pgx-0.5.1/pgx/animal_shogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 
 EMPTY = jnp.int8(-1)
 PAWN = jnp.int8(0)
@@ -34,30 +34,30 @@
 #  7: OPP_BISHOP
 #  8: OPP_KING
 #  9: OPP_GOLD
 INIT_BOARD = jnp.int8([6, -1, -1, 2, 8, 5, 0, 3, 7, -1, -1, 1])  # (12,)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(132, dtype=jnp.bool_)  # (132,)
     observation: jnp.ndarray = jnp.zeros((4, 3, 22), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Animal Shogi specific ---
     turn: jnp.ndarray = jnp.int8(0)
     board: jnp.ndarray = INIT_BOARD  # (12,)
     hand: jnp.ndarray = jnp.zeros((2, 3), dtype=jnp.int8)
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "animal_shogi"
 
 
 @dataclass
 class Action:
     is_drop: jnp.ndarray = FALSE
     from_: jnp.ndarray = jnp.int8(-1)
@@ -75,46 +75,44 @@
         return jax.lax.cond(
             is_drop,
             lambda: Action(is_drop=TRUE, to=sq, drop_piece=x - 8),  # type: ignore
             lambda: Action(is_drop=FALSE, from_=sq, to=_to(sq, x)),  # type: ignore
         )
 
 
-class AnimalShogi(core.Env):
+class AnimalShogi(v1.Env):
     def __init__(self, max_termination_steps: int = 200):
         super().__init__()
         self.max_termination_steps = max_termination_steps
 
     def _init(self, key: jax.random.KeyArray) -> State:
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
         state = State(current_player=current_player)  # type: ignore
         state = state.replace(legal_action_mask=_legal_action_mask(state))  # type: ignore
         return state
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         state = _step(state, action)
         state = jax.lax.cond(
             (0 <= self.max_termination_steps)
             & (self.max_termination_steps <= state._step_count),
             # end with tie
             lambda: state.replace(terminated=TRUE),  # type: ignore
             lambda: state,
         )
         return state  # type: ignore
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "animal_shogi"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/backgammon.py` & `pgx-0.5.1/pgx/backgammon.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 # limitations under the License.
 
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros(34, dtype=jnp.int8)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     # micro action = 6 * src + die
     legal_action_mask: jnp.ndarray = jnp.zeros(6 * 26 + 6, dtype=jnp.bool_)
@@ -46,39 +46,37 @@
     playable_dice: jnp.ndarray = jnp.zeros(4, dtype=jnp.int16)
     # プレイしたサイコロの目の数
     played_dice_num: jnp.ndarray = jnp.int16(0)
     # 黒0, 白1
     turn: jnp.ndarray = jnp.int8(1)
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "backgammon"
 
 
-class Backgammon(core.Env):
+class Backgammon(v1.Env):
     def __init__(
         self,
     ):
         super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "backgammon"
 
     @property
     def version(self) -> str:
         return "beta"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/bridge_bidding.py` & `pgx-0.5.1/pgx/bridge_bidding.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 import copy
 from typing import Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 # カードと数字の対応
 # 0~12 spade, 13~25 heart, 26~38 diamond, 39~51 club
 # それぞれのsuitにおいて以下の順で数字が並ぶ
 TO_CARD = ["A", "2", "3", "4", "5", "6", "7", "8", "9", "T", "J", "Q", "K"]
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     _step_count: jnp.ndarray = jnp.int32(0)
     # turn 現在のターン数
     turn: jnp.ndarray = jnp.int16(0)
     # current_player 現在のプレイヤーid
     current_player: jnp.ndarray = jnp.int8(-1)
     # 各プレイヤーの観測
     observation: jnp.ndarray = jnp.zeros(478, dtype=jnp.bool_)
@@ -85,41 +85,39 @@
     # first_denominaton_EW EWチームにおいて、各denominationをどのプレイヤー
     # が最初にbidしたかを表す
     first_denomination_EW: jnp.ndarray = jnp.full(5, -1, dtype=jnp.int8)
     # passの回数
     pass_num: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "bridge_bidding"
 
 
-class BridgeBidding(core.Env):
+class BridgeBidding(v1.Env):
     def __init__(self):
         super().__init__()
         # fmt: off
         self.hash_keys, self.hash_values = jnp.array([[19556549, 61212362, 52381660, 50424958], [53254536, 21854346, 37287883, 14009558], [44178585, 6709002, 23279217, 16304124], [36635659, 48114215, 13583653, 26208086], [44309474, 39388022, 28376136, 59735189], [61391908, 52173479, 29276467, 31670621], [34786519, 13802254, 57433417, 43152306], [48319039, 55845612, 44614774, 58169152], [47062227, 32289487, 12941848, 21338650], [36579116, 15643926, 64729756, 18678099], [62136384, 37064817, 59701038, 39188202], [13417016, 56577539, 25995845, 27248037], [61125047, 43238281, 23465183, 20030494], [7139188, 31324229, 58855042, 14296487], [2653767, 47502150, 35507905, 43823846], [31453323, 11605145, 6716808, 41061859], [21294711, 49709, 26110952, 50058629], [48130172, 3340423, 60445890, 7686579], [16041939, 27817393, 37167847, 9605779], [61154057, 17937858, 12254613, 12568801], [13796245, 46546127, 49123920, 51772041], [7195005, 45581051, 41076865, 17429796], [20635965, 14642724, 7001617, 45370595], [35616421, 19938131, 45131030, 16524847], [14559399, 15413729, 39188470, 535365], [48743216, 39672069, 60203571, 60210880], [63862780, 2462075, 23267370, 36595020], [11229980, 11616119, 20292263, 3695004], [24135854, 37532826, 54421444, 14130249], [42798085, 33026223, 2460251, 18566823], [49558558, 65537599, 14768519, 31103243], [44321156, 20075251, 42663767, 11615602], [20186726, 42678073, 11763300, 56739471], [57534601, 16703645, 6039937, 17088125], [50795278, 17350238, 11955835, 21538127], [45919621, 5520088, 27736513, 52674927], [13928720, 57324148, 28222453, 15480785], [910719, 47238830, 26345802, 56166394], [58841430, 1098476, 61890558, 26907706], [10379825, 8624220, 39701822, 29045990], [54444873, 50000486, 48563308, 55867521], [47291672, 22084522, 45484828, 32878832], [55350706, 23903891, 46142039, 11499952], [4708326, 27588734, 31010458, 11730972], [27078872, 59038086, 62842566, 51147874], [28922172, 32377861, 9109075, 10154350], [26104086, 62786977, 224865, 14335943], [20448626, 33187645, 34338784, 26382893], [29194006, 19635744, 24917755, 8532577], [64047742, 34885257, 5027048, 58399668], [27603972, 26820121, 44837703, 63748595], [60038456, 19611050, 7928914, 38555047], [13583610, 19626473, 22239272, 19888268], [28521006, 1743692, 31319264, 15168920], [64585849, 63931241, 57019799, 14189800], [2632453, 7269809, 60404342, 57986125], [1996183, 49918209, 49490468, 47760867], [6233580, 15318425, 51356120, 55074857], [15769884, 61654638, 8374039, 43685186], [44162419, 47272176, 62693156, 35359329], [36345796, 15667465, 53341561, 2978505], [1664472, 12761950, 34145519, 55197543], [37567005, 3228834, 6198166, 15646487], [63233399, 42640049, 12969011, 41620641], [22090925, 3386355, 56655568, 31631004], [16442787, 9420273, 48595545, 29770176], [49404288, 37823218, 58551818, 6772527], [36575583, 53847347, 32379432, 1630009], [9004247, 12999580, 48379959, 14252211], [25850203, 26136823, 64934025, 29362603], [10214276, 43557352, 33387586, 55512773], [45810841, 49561478, 41130845, 27034816], [34460081, 16560450, 57722793, 41007718], [53414778, 6845803, 15340368, 16647575], [30535873, 5193469, 43608154, 11391114], [20622004, 34424126, 31475211, 29619615], [10428836, 49656416, 7912677, 33427787], [57600861, 18251799, 46147432, 58946294], [6760779, 14675737, 42952146, 5480498], [46037552, 39969058, 30103468, 55330772], [64466305, 29376674, 49914839, 55269895], [36494113, 27010567, 65752150, 12395385], [49385632, 19550767, 39809394, 58806235], [20987521, 37444597, 49290126, 42326125], [37150229, 37487849, 28254397, 32949826], [9724895, 53813417, 19431235, 27438556], [42132748, 47073733, 19396568, 10026137], [3961481, 27204521, 62087205, 37602005], [22178323, 17505521, 42006207, 44143605], [12753258, 63063515, 61993175, 8920985], [10998000, 64833190, 6446892, 63676805], [66983817, 63684932, 18378359, 39946382], [63476803, 60000436, 19442420, 66417845], [38004446, 64752157, 42570179, 52844512], [1270809, 23735482, 17543294, 18795903], [4862706, 16352249, 57100612, 6219870], [63203206, 25630930, 35608240, 51357885], [59819625, 64662579, 50925335, 55670434], [29216830, 26446697, 52243336, 58475666], [43138915, 30592834, 43931516, 50628002]], dtype=jnp.int32), jnp.array([[71233, 771721, 71505, 706185], [289177, 484147, 358809, 484147], [359355, 549137, 359096, 549137], [350631, 558133, 350630, 554037], [370087, 538677, 370087, 538677], [4432, 899725, 4432, 904077], [678487, 229987, 678487, 229987], [423799, 480614, 423799, 480870], [549958, 284804, 549958, 280708], [423848, 480565, 423848, 480549], [489129, 283940, 554921, 283940], [86641, 822120, 86641, 822120], [206370, 702394, 206370, 567209], [500533, 407959, 500533, 407959], [759723, 79137, 759723, 79137], [563305, 345460, 559209, 345460], [231733, 611478, 231733, 611478], [502682, 406082, 498585, 406082], [554567, 288662, 554567, 288662], [476823, 427846, 476823, 427846], [488823, 415846, 488823, 415846], [431687, 477078, 431687, 477078], [419159, 424070, 415062, 424070], [493399, 345734, 493143, 345718], [678295, 230451, 678295, 230451], [496520, 342596, 496520, 346709], [567109, 276116, 567109, 276116], [624005, 284758, 624005, 284758], [420249, 484420, 420248, 484420], [217715, 621418, 217715, 621418], [344884, 493977, 344884, 493977], [550841, 292132, 550841, 292132], [284262, 558967, 284006, 558967], [152146, 756616, 152146, 756616], [144466, 698763, 144466, 694667], [284261, 624504, 284261, 624504], [288406, 620102, 288405, 620358], [301366, 607383, 301366, 607382], [468771, 435882, 468771, 435882], [555688, 283444, 555688, 283444], [485497, 414820, 485497, 414820], [633754, 275010, 633754, 275010], [419141, 489608, 419157, 489608], [694121, 214387, 694121, 214387], [480869, 427639, 481125, 427639], [489317, 419447, 489301, 419447], [152900, 747672, 152900, 747672], [348516, 494457, 348516, 494457], [534562, 370088, 534562, 370088], [371272, 537475, 371274, 537475], [144194, 760473, 144194, 760473], [567962, 275011, 567962, 275011], [493161, 350052, 493161, 350052], [490138, 348979, 490138, 348979], [328450, 506552, 328450, 506552], [148882, 759593, 148626, 755497], [642171, 266593, 642171, 266593], [685894, 218774, 685894, 218774], [674182, 234548, 674214, 234548], [756347, 152146, 690811, 86353], [612758, 291894, 612758, 291894], [296550, 612214, 296550, 612214], [363130, 475730, 363130, 475730], [691559, 16496, 691559, 16496], [340755, 502202, 336659, 502218], [632473, 210499, 628377, 210483], [564410, 266513, 564410, 266513], [427366, 481399, 427366, 481399], [493159, 349797, 493159, 415605], [331793, 576972, 331793, 576972], [416681, 492084, 416681, 492084], [813496, 95265, 813496, 91153], [695194, 213571, 695194, 213571], [436105, 407124, 436105, 407124], [836970, 6243, 902506, 6243], [160882, 747882, 160882, 747882], [493977, 414788, 489624, 414788], [29184, 551096, 29184, 616888], [903629, 4880, 899517, 4880], [351419, 553250, 351419, 553250], [75554, 767671, 75554, 767671], [279909, 563304, 279909, 563304], [215174, 628054, 215174, 628054], [361365, 481864, 361365, 481864], [424022, 484743, 358486, 484725], [271650, 633018, 271650, 633018], [681896, 226867, 616088, 226867], [222580, 686184, 222564, 686184], [144451, 698778, 209987, 698778], [532883, 310086, 532883, 310086], [628872, 279893, 628872, 279893], [533797, 374951, 533797, 374951], [91713, 817036, 91713, 817036], [427605, 477046, 431718, 477046], [145490, 689529, 145490, 689529], [551098, 291875, 551098, 291875], [349781, 558984, 349781, 558983], [205378, 703115, 205378, 703115], [362053, 546456, 362053, 546456], [612248, 226371, 678040, 226371]], dtype=jnp.int32)
         # fmt: on
 
     def _init(self, key: jax.random.KeyArray) -> State:
         key1, key2, key3 = jax.random.split(key, num=3)
         return _init_by_key(jax.random.choice(key2, self.hash_keys), key3)
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action, self.hash_keys, self.hash_values)
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "bridge_bidding"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/chess.py` & `pgx-0.5.1/pgx/chess.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._chess_utils import (  # type: ignore
+import pgx.v1 as v1
+from pgx._src.chess_utils import (  # type: ignore
     BETWEEN,
     CAN_MOVE,
     CAN_MOVE_ANY,
     HASH_TABLE,
     INIT_LEGAL_ACTION_MASK,
     INIT_POSSIBLE_PIECE_POSITIONS,
     PLANE_MAP,
     TO_MAP,
 )
-from pgx._flax.struct import dataclass
+from pgx._src.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 EMPTY = jnp.int8(0)
 PAWN = jnp.int8(1)
 KNIGHT = jnp.int8(2)
@@ -101,15 +101,15 @@
 #          40          12          61
 #       39             11             62
 #    38                10                64
 # 37                    9                   64
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = INIT_LEGAL_ACTION_MASK  # 64 * 73 = 4672
     observation: jnp.ndarray = jnp.zeros((8, 8, 19), dtype=jnp.float32)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -130,15 +130,15 @@
         .at[0]
         .set(jnp.uint32([1429435994, 901419182]))
     )
     # index to possible piece positions for speeding up. Flips every turn.
     possible_piece_positions: jnp.ndarray = INIT_POSSIBLE_PIECE_POSITIONS
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "chess"
 
     @staticmethod
     def _from_fen(fen: str):
         return _from_fen(fen)
 
     def _to_fen(self) -> str:
@@ -179,47 +179,45 @@
 
     def _to_label(self):
         plane = PLANE_MAP[self.from_, self.to]
         # plane = jax.lax.select(self.underpromotion >= 0, ..., plane)
         return jnp.int32(self.from_) * 73 + jnp.int32(plane)
 
 
-class Chess(core.Env):
+class Chess(v1.Env):
     def __init__(self):
         super().__init__()
         # AlphaZero paper does not mention the number of max termination steps
         # but we believe 1000 is large enough for Chess.
         self.max_termination_steps = 1000
 
     def _init(self, key: jax.random.KeyArray) -> State:
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
         state = State(current_player=current_player)  # type: ignore
         return state
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         state = _step(state, action)
         state = jax.lax.cond(
             (0 <= self.max_termination_steps)
             & (self.max_termination_steps <= state._step_count),
             # end with tie
             lambda: state.replace(terminated=TRUE),  # type: ignore
             lambda: state,
         )
         return state  # type: ignore
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "chess"
 
     @property
     def version(self) -> str:
         return "beta"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/connect_four.py` & `pgx-0.5.1/pgx/connect_four.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((6, 7, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(7, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -41,39 +41,37 @@
     #  [21, 22, 23, 24, 25, 26, 27],
     #  [28, 29, 30, 31, 32, 33, 34],
     #  [35, 36, 37, 38, 39, 40, 41]]
     board: jnp.ndarray = -jnp.ones(42, jnp.int8)  # -1 (empty), 0, 1
     blank_row: jnp.ndarray = jnp.full(7, 5)
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "connect_four"
 
 
-class ConnectFour(core.Env):
+class ConnectFour(v1.Env):
     def __init__(
         self,
     ):
         super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "connect_four"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/core.py` & `pgx-0.5.1/pgx/v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import abc
 from typing import Literal, Optional, Tuple, get_args
 
 import jax
 import jax.numpy as jnp
 
-from pgx._flax.struct import dataclass
+from pgx._src.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 
 # Pgx environments are versioned like OpenAI Gym or Brax.
 # OpenAI Gym forces user to specify version (e.g., `MountainCar-v0`); while Brax does not (e.g., `ant`)
@@ -121,15 +121,15 @@
         Args:
             color_theme (Optional[Literal["light", "dark"]]): xxx see also global config.
             scale (Optional[float]): change image size. Default(None) is 1.0
 
         Returns:
             str: SVG string
         """
-        from pgx._visualizer import Visualizer
+        from pgx._src.visualizer import Visualizer
 
         v = Visualizer(color_theme=color_theme, scale=scale)
         return v.get_dwg(states=self).tostring()
 
     def save_svg(
         self,
         filename,
@@ -143,15 +143,15 @@
         Args:
             color_theme (Optional[Literal["light", "dark"]]): xxx see also global config.
             scale (Optional[float]): change image size. Default(None) is 1.0
 
         Returns:
             None
         """
-        from pgx._visualizer import save_svg
+        from pgx._src.visualizer import save_svg
 
         save_svg(self, filename, color_theme=color_theme, scale=scale)
 
 
 class Env(abc.ABC):
     """Environment class API.
```

### Comparing `pgx-0.5.0/pgx/experimental/bridge_bidding.py` & `pgx-0.5.1/pgx/experimental/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/experimental/gym.py` & `pgx-0.5.1/pgx/experimental/gym.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
 import jax
 import jax.numpy as jnp
 
-from pgx.core import EnvId, State, make
+from pgx.v1 import EnvId, State, make
 
 
 class RandomOpponentEnv:
     def __init__(
         self,
         env_id: EnvId,
         num_envs: int,
```

### Comparing `pgx-0.5.0/pgx/experimental/pettingzoo.py` & `pgx-0.5.1/pgx/experimental/pettingzoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import jax.numpy as jnp
 import numpy as np
 from gymnasium import spaces  # type: ignore
 from IPython.display import display_svg  # type:ignore
 from pettingzoo import AECEnv  # type: ignore
 from pettingzoo.utils import wrappers  # type: ignore
 
-from pgx.core import Env, EnvId, State, make
+from pgx.v1 import Env, EnvId, State, make
 
 
 def pettingzoo_env(
     env_id: EnvId, render_mode=Optional[Literal["svg"]]
 ) -> AECEnv:
     env = PettingZooEnv(env_id, render_mode=render_mode)
     env = wrappers.TerminateIllegalWrapper(env, illegal_reward=-1)
```

### Comparing `pgx-0.5.0/pgx/experimental/visualize.py` & `pgx-0.5.1/pgx/experimental/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Union
 
-from pgx.core import State
+from pgx.v1 import State
 
 
 def show_state_seq(
     states: Union[State, List[State]],
 ) -> None:
     """Visualize list of states on notebook."""
     import sys
```

### Comparing `pgx-0.5.0/pgx/experimental/wrappers.py` & `pgx-0.5.1/pgx/experimental/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 Third, personally, I feel `env = wrapper(env)` style is not easy to follow what actually happens
 """
 
 import jax
 import jax.numpy as jnp
 
-from pgx.core import State
+from pgx.v1 import State
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 
 def auto_reset(step_fn, init_fn):
     """Auto reset wrapper.
```

### Comparing `pgx-0.5.0/pgx/go.py` & `pgx-0.5.1/pgx/go.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 # limitations under the License.
 
 from functools import partial
 
 import jax
 from jax import numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.zeros(19 * 19 + 1, dtype=jnp.bool_)
     observation: jnp.ndarray = jnp.zeros((19, 19, 17), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -47,23 +47,23 @@
     )  # [0]=black, [1]=white
     passed: jnp.ndarray = FALSE  # TRUE if last action is pass
     ko: jnp.ndarray = jnp.int32(-1)  # by SSK
     komi: jnp.ndarray = jnp.float32(7.5)
     black_player: jnp.ndarray = jnp.int8(0)
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         try:
             size = int(self.size.item())
         except TypeError:
             size = int(self.size[0].item())
         return f"go-{size}x{size}"  # type: ignore
 
 
-class Go(core.Env):
+class Go(v1.Env):
     def __init__(
         self,
         *,
         size: int = 19,
         komi: float = 7.5,
         history_length: int = 8,
     ):
@@ -73,39 +73,37 @@
         self.komi = komi
         self.history_length = history_length
         self.max_termination_steps = self.size * self.size * 2
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return partial(_init, size=self.size, komi=self.komi)(key=key)
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         state = partial(_step, size=self.size)(state, action)
         # terminates if size * size * 2 (722 if size=19) steps are elapsed
         state = jax.lax.cond(
             (0 <= self.max_termination_steps)
             & (self.max_termination_steps <= state._step_count),
             lambda: state.replace(  # type: ignore
                 terminated=TRUE,
                 reward=partial(_get_reward, size=self.size)(state),
             ),
             lambda: state,
         )
         return state  # type: ignore
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return partial(
             _observe, size=self.size, history_length=self.history_length
         )(state=state, player_id=player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return f"go-{int(self.size)}x{int(self.size)}"  # type: ignore
 
     @property
     def version(self) -> str:
         return "beta"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/hex.py` & `pgx-0.5.1/pgx/hex.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 # limitations under the License.
 
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((11, 11, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(11 * 11, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -46,43 +46,41 @@
     #  .
     #  [110, 111, 112, ...,  119, 120]]
     board: jnp.ndarray = -jnp.zeros(
         11 * 11, jnp.int32
     )  # <0(oppo), 0(empty), 0<(self)
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "hex"
 
 
-class Hex(core.Env):
+class Hex(v1.Env):
     def __init__(
         self,
         *,
         size: int = 11,
     ):
         super().__init__()
         assert isinstance(size, int)
         self.size = size
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return partial(_init, size=self.size)(rng=key)
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return partial(_step, size=self.size)(state, action)
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return partial(_observe, size=self.size)(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "hex"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/kuhn_poker.py` & `pgx-0.5.1/pgx/kuhn_poker.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 CALL = jnp.int8(0)
 BET = jnp.int8(1)
 FOLD = jnp.int8(2)
 CHECK = jnp.int8(3)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((8, 8, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(4, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -40,39 +40,37 @@
     cards: jnp.ndarray = jnp.int8([-1, -1])
     # [(player 0),(player 1)]
     last_action: jnp.ndarray = jnp.int8(-1)
     # 0(Call)  1(Bet)  2(Fold)  3(Check)
     pot: jnp.ndarray = jnp.int8([0, 0])
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "kuhn_poker"
 
 
-class KuhnPoker(core.Env):
+class KuhnPoker(v1.Env):
     def __init__(
         self,
     ):
         super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "kuhn_poker"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/leduc_holdem.py` & `pgx-0.5.1/pgx/leduc_holdem.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 INVALID_ACTION = jnp.int8(-1)
 CALL = jnp.int8(0)
 RAISE = jnp.int8(1)
 FOLD = jnp.int8(2)
 
 MAX_RAISE = jnp.int8(2)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((8, 8, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(3, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -49,39 +49,37 @@
     last_action: jnp.ndarray = INVALID_ACTION
 
     chips: jnp.ndarray = jnp.ones(2, dtype=jnp.int8)
     round: jnp.ndarray = jnp.int8(0)
     raise_count: jnp.ndarray = jnp.int8(0)
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "leduc_holdem"
 
 
-class LeducHoldem(core.Env):
+class LeducHoldem(v1.Env):
     def __init__(
         self,
     ):
         super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "leduc_holdem"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/minatar/asterix.py` & `pgx-0.5.1/pgx/minatar/asterix.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     * https://github.com/kenjyoung/MinAtar/blob/master/License.txt
 """
 from typing import Literal, Optional
 
 import jax
 from jax import numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 ramp_interval: jnp.ndarray = jnp.array(100, dtype=jnp.int32)
 init_spawn_speed: jnp.ndarray = jnp.array(10, dtype=jnp.int32)
 init_move_interval: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
 shot_cool_down: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
 INF: jnp.ndarray = jnp.array(99, dtype=jnp.int32)
 
@@ -26,15 +26,15 @@
 NINE = jnp.array(9, dtype=jnp.int32)
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 4), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -50,15 +50,15 @@
     move_timer: jnp.ndarray = init_move_interval
     ramp_timer: jnp.ndarray = ramp_interval
     ramp_index: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
     terminal: jnp.ndarray = FALSE  # duplicated but necessary for checking the consistency to the original MinAtar
     last_action: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "minatar/asterix"
 
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
@@ -70,43 +70,41 @@
         scale: Optional[float] = None,
     ) -> None:
         from pgx.minatar.utils import visualize_minatar
 
         visualize_minatar(self, filename)
 
 
-class MinAtarAsterix(core.Env):
+class MinAtarAsterix(v1.Env):
     def __init__(
         self,
         *,
         minatar_version: Literal["v0", "v1"] = "v1",
         sticky_action_prob: float = 0.1,
     ):
         super().__init__()
         self.minatar_version: Literal["v0", "v1"] = minatar_version
         self.sticky_action_prob: float = sticky_action_prob
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return State(_rng_key=key)  # type: ignore
 
-    def _step(self, state: core.State, action) -> State:
+    def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
         state = _step(
             state, action, sticky_action_prob=self.sticky_action_prob
         )
         return state.replace(terminated=state.terminal)  # type: ignore
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "minatar/asterix"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/minatar/breakout.py` & `pgx-0.5.1/pgx/minatar/breakout.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,29 @@
     * https://github.com/kenjyoung/MinAtar/blob/master/License.txt
 """
 from typing import Literal, Optional
 
 import jax
 from jax import numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 ZERO = jnp.array(0, dtype=jnp.int32)
 ONE = jnp.array(1, dtype=jnp.int32)
 TWO = jnp.array(2, dtype=jnp.int32)
 THREE = jnp.array(3, dtype=jnp.int32)
 FOUR = jnp.array(4, dtype=jnp.int32)
 NINE = jnp.array(9, dtype=jnp.int32)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 4), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -51,15 +51,15 @@
     strike: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
     last_x: jnp.ndarray = ZERO
     last_y: jnp.ndarray = THREE
     terminal: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
     last_action: jnp.ndarray = ZERO
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "minatar/breakout"
 
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
@@ -71,43 +71,41 @@
         scale: Optional[float] = None,
     ) -> None:
         from pgx.minatar.utils import visualize_minatar
 
         visualize_minatar(self, filename)
 
 
-class MinAtarBreakout(core.Env):
+class MinAtarBreakout(v1.Env):
     def __init__(
         self,
         *,
         minatar_version: Literal["v0", "v1"] = "v1",
         sticky_action_prob: float = 0.1,
     ):
         super().__init__()
         self.minatar_version: Literal["v0", "v1"] = minatar_version
         self.sticky_action_prob: float = sticky_action_prob
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)  # type: ignore
 
-    def _step(self, state: core.State, action) -> State:
+    def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
         state = _step(
             state, action, sticky_action_prob=self.sticky_action_prob
         )
         return state.replace(terminated=state.terminal)  # type: ignore
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "minatar/asterix"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/minatar/freeway.py` & `pgx-0.5.1/pgx/minatar/freeway.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     * https://github.com/kenjyoung/MinAtar/blob/master/License.txt
 """
 from typing import Literal, Optional
 
 import jax
 from jax import numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 player_speed = jnp.array(3, dtype=jnp.int32)
 time_limit = jnp.array(2500, dtype=jnp.int32)
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 ZERO = jnp.array(0, dtype=jnp.int32)
 ONE = jnp.array(1, dtype=jnp.int32)
 NINE = jnp.array(9, dtype=jnp.int32)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 7), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -41,15 +41,15 @@
     pos: jnp.ndarray = jnp.array(9, dtype=jnp.int32)
     move_timer: jnp.ndarray = jnp.array(player_speed, dtype=jnp.int32)
     terminate_timer: jnp.ndarray = jnp.array(time_limit, dtype=jnp.int32)
     terminal: jnp.ndarray = jnp.array(False, dtype=jnp.bool_)
     last_action: jnp.ndarray = jnp.array(0, dtype=jnp.int32)
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "minatar/freeway"
 
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
@@ -61,43 +61,41 @@
         scale: Optional[float] = None,
     ) -> None:
         from pgx.minatar.utils import visualize_minatar
 
         visualize_minatar(self, filename)
 
 
-class MinAtarFreeway(core.Env):
+class MinAtarFreeway(v1.Env):
     def __init__(
         self,
         *,
         minatar_version: Literal["v0", "v1"] = "v1",
         sticky_action_prob: float = 0.1,
     ):
         super().__init__()
         self.minatar_version: Literal["v0", "v1"] = minatar_version
         self.sticky_action_prob: float = sticky_action_prob
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)  # type: ignore
 
-    def _step(self, state: core.State, action) -> State:
+    def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
         state = _step(
             state, action, sticky_action_prob=self.sticky_action_prob
         )
         return state.replace(terminated=state.terminal)  # type: ignore
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "minatar/freeway"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/minatar/seaquest.py` & `pgx-0.5.1/pgx/minatar/seaquest.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 """
 from typing import Literal, Optional
 
 import jax
 import jax.lax as lax
 from jax import numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 RAMP_INTERVAL: jnp.ndarray = jnp.int32(100)
 MAX_OXYGEN: jnp.ndarray = jnp.int32(200)
 INIT_SPAWN_SPEED: jnp.ndarray = jnp.int32(20)
 DIVER_SPAWN_SPEED: jnp.ndarray = jnp.int32(30)
 INIT_MOVE_INTERVAL: jnp.ndarray = jnp.int32(5)
 SHOT_COOL_DOWN: jnp.ndarray = jnp.int32(5)
@@ -29,15 +29,15 @@
 ZERO: jnp.ndarray = jnp.int32(0)
 NINE: jnp.ndarray = jnp.int32(9)
 TRUE: jnp.ndarray = jnp.bool_(True)
 FALSE: jnp.ndarray = jnp.bool_(False)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 10), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -62,15 +62,15 @@
     ramp_index: jnp.ndarray = ZERO
     shot_timer: jnp.ndarray = ZERO
     surface: jnp.ndarray = TRUE
     terminal: jnp.ndarray = FALSE
     last_action: jnp.ndarray = ZERO
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "minatar/seaquest"
 
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
@@ -82,43 +82,41 @@
         scale: Optional[float] = None,
     ) -> None:
         from pgx.minatar.utils import visualize_minatar
 
         visualize_minatar(self, filename)
 
 
-class MinAtarSeaquest(core.Env):
+class MinAtarSeaquest(v1.Env):
     def __init__(
         self,
         *,
         minatar_version: Literal["v0", "v1"] = "v1",
         sticky_action_prob: float = 0.1,
     ):
         super().__init__()
         self.minatar_version: Literal["v0", "v1"] = minatar_version
         self.sticky_action_prob: float = sticky_action_prob
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init_det()
 
-    def _step(self, state: core.State, action) -> State:
+    def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
         state = _step(
             state, action, sticky_action_prob=self.sticky_action_prob
         )
         return state.replace(terminated=state.terminal)  # type: ignore
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "minatar/seaquest"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/minatar/space_invaders.py` & `pgx-0.5.1/pgx/minatar/space_invaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 """
 from typing import Literal, Optional
 
 import jax
 import jax.lax as lax
 from jax import numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 SHOT_COOL_DOWN = jnp.int32(5)
 ENEMY_MOVE_INTERVAL = jnp.int32(12)
 ENEMY_SHOT_INTERVAL = jnp.int32(10)
 
 ZERO = jnp.int32(0)
 NINE = jnp.int32(9)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 6), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -51,15 +51,15 @@
     alien_shot_timer: jnp.ndarray = ENEMY_SHOT_INTERVAL
     ramp_index: jnp.ndarray = jnp.int32(0)
     shot_timer: jnp.ndarray = jnp.int32(0)
     terminal: jnp.ndarray = FALSE
     last_action: jnp.ndarray = jnp.int32(0)
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "minatar/space_invaders"
 
     def _repr_html_(self) -> str:
         from pgx.minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
@@ -71,43 +71,41 @@
         scale: Optional[float] = None,
     ) -> None:
         from pgx.minatar.utils import visualize_minatar
 
         visualize_minatar(self, filename)
 
 
-class MinAtarSpaceInvaders(core.Env):
+class MinAtarSpaceInvaders(v1.Env):
     def __init__(
         self,
         *,
         minatar_version: Literal["v0", "v1"] = "v1",
         sticky_action_prob: float = 0.1,
     ):
         super().__init__()
         self.minatar_version: Literal["v0", "v1"] = minatar_version
         self.sticky_action_prob: float = sticky_action_prob
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init_det()
 
-    def _step(self, state: core.State, action) -> State:
+    def _step(self, state: v1.State, action) -> State:
         assert isinstance(state, State)
         state = _step(
             state, action, sticky_action_prob=self.sticky_action_prob
         )
         return state.replace(terminated=state.terminal)  # type: ignore
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "minatar/space_invaders"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/minatar/utils.py` & `pgx-0.5.1/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/pgx/othello.py` & `pgx-0.5.1/pgx/othello.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((8, 8, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(64 + 1, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -43,39 +43,37 @@
     #  [40, 41, 42, 43, 44, 45, 46, 47],
     #  [48, 49, 50, 51, 52, 53, 54, 55],
     #  [56, 57, 58, 59, 60, 61, 62, 63]]
     board: jnp.ndarray = jnp.zeros(64, jnp.int8)  # -1(opp), 0(empty), 1(self)
     passed: jnp.ndarray = FALSE
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "othello"
 
 
-class Othello(core.Env):
+class Othello(v1.Env):
     def __init__(
         self,
     ):
         super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "othello"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/play2048.py` & `pgx-0.5.1/pgx/play2048.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import jax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 ZERO = jnp.int8(0)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros(16, dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(4, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -51,39 +51,37 @@
     # means
     # [[ 0,  0,  2,  2],
     #  [ 2,  0,  2,  4],
     #  [ 8,  8, 64,128],
     #  [ 8, 64,128,512]]
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "2048"
 
 
-class Play2048(core.Env):
+class Play2048(v1.Env):
     def __init__(
         self,
     ):
         super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "2048"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/shogi.py` & `pgx-0.5.1/pgx/shogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 
 
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
-from pgx._shogi_utils import (
+import pgx.v1 as v1
+from pgx._src.shogi_utils import (
     AROUND_IX,
     BETWEEN_IX,
     CAN_MOVE,
     CAN_MOVE_ANY,
     INIT_LEGAL_ACTION_MASK,
     INIT_PIECE_BOARD,
     LEGAL_FROM_IDX,
     NEIGHBOUR_IX,
     _from_sfen,
     _to_sfen,
 )
+from pgx._src.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 
 EMPTY = jnp.int8(-1)  # 空白
 PAWN = jnp.int8(0)  # 歩
 LANCE = jnp.int8(1)  # 香
@@ -66,15 +66,15 @@
 OPP_HORSE = jnp.int8(26)  # 相手馬
 OPP_DRAGON = jnp.int8(27)  # 相手龍
 
 ALL_SQ = jnp.arange(81)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = INIT_LEGAL_ACTION_MASK  # (27 * 81,)
     observation: jnp.ndarray = jnp.zeros((119, 9, 9), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -85,15 +85,15 @@
     hand: jnp.ndarray = jnp.zeros((2, 7), dtype=jnp.int8)  # 後手のときにはflipする
     # cache
     # Redundant information used only in _is_checked for speeding-up
     cache_m2b: jnp.ndarray = -jnp.ones(8, dtype=jnp.int8)
     cache_king: jnp.ndarray = jnp.int32(44)
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "shogi"
 
     @staticmethod
     def _from_board(turn, piece_board: jnp.ndarray, hand: jnp.ndarray):
         """Mainly for debugging purpose.
         terminated, reward, and current_player are not changed"""
         state = State(turn=turn, piece_board=piece_board, hand=hand)  # type: ignore
@@ -110,46 +110,44 @@
         )
 
     def _to_sfen(self):
         state = self if self.turn % 2 == 0 else _flip(self)
         return _to_sfen(state)
 
 
-class Shogi(core.Env):
+class Shogi(v1.Env):
     def __init__(self, max_termination_steps: int = 1000):
         super().__init__()
         self.max_termination_steps = max_termination_steps
 
     def _init(self, key: jax.random.KeyArray) -> State:
         state = _init_board()
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
         return state.replace(current_player=current_player)  # type: ignore
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         # Note: Assume that illegal action is already filtered by Env.step
         state = _step(state, action)
         state = jax.lax.cond(
             (0 <= self.max_termination_steps)
             & (self.max_termination_steps <= state._step_count),
             # end with tie
             lambda: state.replace(terminated=TRUE),  # type: ignore
             lambda: state,
         )
         return state  # type: ignore
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "shogi"
 
     @property
     def version(self) -> str:
         return "beta"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/sparrow_mahjong.py` & `pgx-0.5.1/pgx/sparrow_mahjong.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
   * 誰も一つも行動を取らずにエピソードが終わるのを避けるため、親の第一ツモでの和了の場合は配牌し直し（天和を避けている）
 """
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 TRUE = jnp.bool_(True)
 FALSE = jnp.bool_(False)
 NUM_TILES = 44
 NUM_TILE_TYPES = 11
 N_PLAYER = 3
 MAX_RIVER_LENGTH = 10
@@ -50,15 +50,15 @@
 WIN_HANDS = jnp.int32([18, 78, 90, 378, 390, 450, 778, 790, 850, 1150, 1550, 1878, 1890, 1950, 2250, 2650, 3878, 3890, 3950, 4250, 4650, 5750, 7750, 9378, 9390, 9450, 9750, 10150, 11250, 13250, 19378, 19390, 19450, 19750, 20150, 21250, 23250, 28750, 38750, 46878, 46890, 46950, 47250, 47650, 48750, 50750, 56250, 66250, 96878, 96890, 96950, 97250, 97650, 98750, 100750, 106250, 116250, 143750, 193750, 234378, 234390, 234450, 234750, 235150, 236250, 238250, 243750, 253750, 281250, 331250, 484378, 484390, 484450, 484750, 485150, 486250, 488250, 493750, 503750, 531250, 581250, 718750, 968750, 1171878, 1171890, 1171950, 1172250, 1172650, 1173750, 1175750, 1181250, 1191250, 1218750, 1268750, 1406250, 1656250, 2421878, 2421890, 2421950, 2422250, 2422650, 2423750, 2425750, 2431250, 2441250, 2468750, 2518750, 2656250, 2906250, 3593750, 4843750, 5859378, 5859390, 5859450, 5859750, 5860150, 5861250, 5863250, 5868750, 5878750, 5906250, 5956250, 6093750, 6343750, 7031250, 8281250, 12109378, 12109390, 12109450, 12109750, 12110150, 12111250, 12113250, 12118750, 12128750, 12156250, 12206250, 12343750, 12593750, 13281250, 14531250, 17968750, 24218750, 29296878, 29296890, 29296950, 29297250, 29297650, 29298750, 29300750, 29306250, 29316250, 29343750, 29393750, 29531250, 29781250, 30468750, 31718750, 35156250, 41406250])  # type: ignore
 BASE_SCORES = jnp.int32([4, 4, 4, 4, 4, 4, 3, 3, 3, 3, 2, 4, 4, 4, 4, 3, 3, 3, 3, 3, 2, 3, 2, 4, 4, 4, 4, 3, 4, 3, 3, 3, 3, 3, 2, 3, 2, 3, 2, 4, 4, 4, 4, 3, 4, 3, 4, 3, 3, 3, 3, 3, 2, 3, 2, 3, 2, 3, 2, 4, 4, 4, 4, 3, 4, 3, 4, 3, 4, 3, 3, 3, 3, 3, 2, 3, 2, 3, 2, 3, 2, 3, 2, 4, 4, 4, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 3, 3, 3, 3, 2, 3, 2, 3, 2, 3, 2, 3, 2, 3, 2, 4, 4, 4, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 3, 3, 3, 3, 2, 3, 2, 3, 2, 3, 2, 3, 2, 3, 2, 3, 2, 4, 4, 4, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3, 4, 3])  # type: ignore
 YAKU_SCORES = jnp.int32([15, 15, 15, 0, 10, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 1, 1, 0, 10, 0, 10, 0, 1, 1, 0, 0, 0, 1, 0, 1, 1, 1, 1, 0, 0, 0, 1, 0, 1, 1, 1, 1, 0, 0, 0, 1, 0, 1, 1, 1, 1, 1, 1, 0, 10, 0, 10, 0, 1, 1, 10, 1, 1, 1, 0, 0, 0, 1, 0, 1, 1, 1, 1, 1, 1, 1, 1, 0, 10, 0, 10, 0, 1, 1, 10, 1, 1, 1, 10, 1, 0, 10, 0, 10, 0, 1, 1, 10, 1, 1, 1, 10, 1, 10, 10, 0, 10, 0, 10, 0, 1, 1, 10, 1, 1, 1, 10, 1, 10, 10, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 15, 15, 15, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0])  # type: ignore
 MAX_SCORE = 26  # 親の中含むスーパーレッド自摸和了 (1 + 2 + 20 + 2) // 2 * 2
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((15, 11), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.zeros(3, dtype=jnp.float32)
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.zeros(9, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -85,19 +85,19 @@
     shuffled_players: jnp.ndarray = jnp.zeros(
         N_PLAYER, dtype=jnp.int8
     )  # 0: dealer, ...
     dora: jnp.ndarray = jnp.int32(0)  # tile type (0~10) is set
     scores: jnp.ndarray = jnp.zeros(3, dtype=jnp.int32)  # 0 = dealer
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "sparrow_mahjong"
 
 
-class SparrowMahjong(core.Env):
+class SparrowMahjong(v1.Env):
     def __init__(
         self,
     ):
         super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         key, subkey = jax.random.split(key)
@@ -110,15 +110,15 @@
 
         # avoid tenhou
         key, state = lax.while_loop(
             lambda x: x[-1].terminated, f, (key, state)
         )
         return state
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         # discard tile
         hands = state.hands.at[state.turn % N_PLAYER, action].add(-1)
         is_red_discarded = (
             hands[state.turn % N_PLAYER, action]
             < state.n_red_in_hands[state.turn % N_PLAYER, action]
         )
@@ -148,22 +148,20 @@
             lambda: lax.cond(
                 jnp.bool_(NUM_TILES - 1 <= state.draw_ix),  # type: ignore
                 lambda: _step_by_tie(state),
                 lambda: _step_non_tied(state, scores),  # type: ignore
             ),
         )
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "sparrow_mahjong"
 
     @property
     def version(self) -> str:
         return "alpha"
 
     @property
```

### Comparing `pgx-0.5.0/pgx/tic_tac_toe.py` & `pgx-0.5.1/pgx/tic_tac_toe.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import jax
 import jax.numpy as jnp
 
-import pgx.core as core
-from pgx._flax.struct import dataclass
+import pgx.v1 as v1
+from pgx._src.struct import dataclass
 
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
-class State(core.State):
+class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((3, 3, 2), dtype=jnp.bool_)
     reward: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
     truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(9, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
@@ -36,39 +36,37 @@
     turn: jnp.ndarray = jnp.int8(0)
     # 0 1 2
     # 3 4 5
     # 6 7 8
     board: jnp.ndarray = -jnp.ones(9, jnp.int8)  # -1 (empty), 0, 1
 
     @property
-    def env_id(self) -> core.EnvId:
+    def env_id(self) -> v1.EnvId:
         return "tic_tac_toe"
 
 
-class TicTacToe(core.Env):
+class TicTacToe(v1.Env):
     def __init__(
         self,
     ):
         super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
-    def _step(self, state: core.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
 
-    def _observe(
-        self, state: core.State, player_id: jnp.ndarray
-    ) -> jnp.ndarray:
+    def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
     @property
-    def id(self) -> core.EnvId:
+    def id(self) -> v1.EnvId:
         return "tic_tac_toe"
 
     @property
     def version(self) -> str:
         return "beta"
 
     @property
```

### Comparing `pgx-0.5.0/pgx.egg-info/PKG-INFO` & `pgx-0.5.1/pgx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.5.0
+Version: 0.5.1
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.5.0 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.5.1 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
```

### Comparing `pgx-0.5.0/setup.py` & `pgx-0.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="pgx",
-    version="0.5.0",
+    version="0.5.1",
     description="GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/sotetsuk/pgx",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
     packages=find_packages(),
     package_data={"": ["LICENSE", "*.svg"]},
     include_package_data=True,
     install_requires=[
         "jax>=0.3.25",  # JAX version on Colab (TPU)
         "svgwrite",
-        "msgpack",
         "typing_extensions"
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
```

### Comparing `pgx-0.5.0/tests/minatar_utils.py` & `pgx-0.5.1/tests/minatar_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_animal_shogi.py` & `pgx-0.5.1/tests/test_animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_asterix.py` & `pgx-0.5.1/tests/test_asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_backgammon.py` & `pgx-0.5.1/tests/test_backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_breakout.py` & `pgx-0.5.1/tests/test_breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_bridge_bidding.py` & `pgx-0.5.1/tests/test_bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_chess.py` & `pgx-0.5.1/tests/test_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_connect_four.py` & `pgx-0.5.1/tests/test_connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_freeway.py` & `pgx-0.5.1/tests/test_freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_go.py` & `pgx-0.5.1/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_hex.py` & `pgx-0.5.1/tests/test_hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_kuhn_poker.py` & `pgx-0.5.1/tests/test_kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_leduc_holdem.py` & `pgx-0.5.1/tests/test_leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_mahjong.py` & `pgx-0.5.1/tests/test_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_othello.py` & `pgx-0.5.1/tests/test_othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_play2048.py` & `pgx-0.5.1/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_seaquest.py` & `pgx-0.5.1/tests/test_seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_shogi.py` & `pgx-0.5.1/tests/test_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_space_invaders.py` & `pgx-0.5.1/tests/test_space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_sparrow_mahjong.py` & `pgx-0.5.1/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.5.0/tests/test_tic_tac_toe.py` & `pgx-0.5.1/tests/test_tic_tac_toe.py`

 * *Files identical despite different names*

