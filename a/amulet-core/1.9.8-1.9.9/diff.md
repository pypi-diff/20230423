# Comparing `tmp/amulet-core-1.9.8.tar.gz` & `tmp/amulet-core-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amulet-core-1.9.8.tar", last modified: Wed Oct  5 13:20:17 2022, max compression
+gzip compressed data, was "/Users/runner/work/Amulet-Core/Amulet-Core/dist/tmp74akva0m/amulet-core-1.9.9.tar", last modified: Wed Oct 26 08:49:24 2022, max compression
```

## Comparing `amulet-core-1.9.8.tar` & `amulet-core-1.9.9.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.300459 amulet-core-1.9.8/
--rw-r--r--   0 runner     (501) staff       (20)       60 2022-10-05 13:19:40.000000 amulet-core-1.9.8/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3792 2022-10-05 13:20:17.300637 amulet-core-1.9.8/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3330 2022-10-05 13:19:40.000000 amulet-core-1.9.8/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.302355 amulet-core-1.9.8/amulet/
--rw-r--r--   0 runner     (501) staff       (20)      385 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.183869 amulet-core-1.9.8/amulet/__pyinstaller/
--rw-r--r--   0 runner     (501) staff       (20)       41 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/__pyinstaller/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      426 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/__pyinstaller/hook-amulet.py
--rw-r--r--   0 runner     (501) staff       (20)      497 2022-10-05 13:20:17.302464 amulet-core-1.9.8/amulet/_version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.190230 amulet-core-1.9.8/amulet/api/
--rw-r--r--   0 runner     (501) staff       (20)       46 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3784 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/abstract_base_entity.py
--rw-r--r--   0 runner     (501) staff       (20)    23048 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/block.py
--rw-r--r--   0 runner     (501) staff       (20)     2004 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/block_entity.py
--rw-r--r--   0 runner     (501) staff       (20)     3080 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/cache.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.193855 amulet-core-1.9.8/amulet/api/chunk/
--rw-r--r--   0 runner     (501) staff       (20)      217 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/chunk/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7414 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/chunk/biomes.py
--rw-r--r--   0 runner     (501) staff       (20)     6182 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/chunk/block_entity_dict.py
--rw-r--r--   0 runner     (501) staff       (20)     1652 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/chunk/blocks.py
--rw-r--r--   0 runner     (501) staff       (20)    13385 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/chunk/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)     2047 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/chunk/entity_list.py
--rw-r--r--   0 runner     (501) staff       (20)     4908 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/chunk/status.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.196667 amulet-core-1.9.8/amulet/api/data_types/
--rw-r--r--   0 runner     (501) staff       (20)      116 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/data_types/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       78 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/data_types/generic_types.py
--rw-r--r--   0 runner     (501) staff       (20)      598 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/data_types/operation_types.py
--rw-r--r--   0 runner     (501) staff       (20)     2261 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/data_types/world_types.py
--rw-r--r--   0 runner     (501) staff       (20)     2580 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/data_types/wrapper_types.py
--rw-r--r--   0 runner     (501) staff       (20)     1839 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/entity.py
--rw-r--r--   0 runner     (501) staff       (20)     2825 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/errors.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.198472 amulet-core-1.9.8/amulet/api/history/
--rw-r--r--   0 runner     (501) staff       (20)     2329 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.200617 amulet-core-1.9.8/amulet/api/history/base/
--rw-r--r--   0 runner     (501) staff       (20)      128 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/base/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      674 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/base/base_history.py
--rw-r--r--   0 runner     (501) staff       (20)     2055 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/base/history_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     2816 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/base/revision_manager.py
--rw-r--r--   0 runner     (501) staff       (20)      432 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/changeable.py
--rw-r--r--   0 runner     (501) staff       (20)      226 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/data_types.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.202916 amulet-core-1.9.8/amulet/api/history/history_manager/
--rw-r--r--   0 runner     (501) staff       (20)      123 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/history_manager/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3480 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/history_manager/container.py
--rw-r--r--   0 runner     (501) staff       (20)    11327 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/history_manager/database.py
--rw-r--r--   0 runner     (501) staff       (20)     3023 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/history_manager/meta.py
--rw-r--r--   0 runner     (501) staff       (20)     4064 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/history_manager/object.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.204374 amulet-core-1.9.8/amulet/api/history/revision_manager/
--rw-r--r--   0 runner     (501) staff       (20)       72 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/revision_manager/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1023 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/revision_manager/disk.py
--rw-r--r--   0 runner     (501) staff       (20)      376 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/history/revision_manager/ram.py
--rw-r--r--   0 runner     (501) staff       (20)     1819 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/item.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.205960 amulet-core-1.9.8/amulet/api/level/
--rw-r--r--   0 runner     (501) staff       (20)      144 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/level/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.208973 amulet-core-1.9.8/amulet/api/level/base_level/
--rw-r--r--   0 runner     (501) staff       (20)       34 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/level/base_level/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    43105 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/level/base_level/base_level.py
--rw-r--r--   0 runner     (501) staff       (20)     8921 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/level/base_level/chunk_manager.py
--rw-r--r--   0 runner     (501) staff       (20)    19325 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/level/base_level/clone.py
--rw-r--r--   0 runner     (501) staff       (20)     3226 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/level/base_level/player_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.210881 amulet-core-1.9.8/amulet/api/level/immutable_structure/
--rw-r--r--   0 runner     (501) staff       (20)       52 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/level/immutable_structure/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3302 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/level/immutable_structure/immutable_structure.py
--rw-r--r--   0 runner     (501) staff       (20)     3065 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/level/immutable_structure/void_format_wrapper.py
--rw-r--r--   0 runner     (501) staff       (20)      619 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/level/structure.py
--rw-r--r--   0 runner     (501) staff       (20)      613 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/level/world.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.213979 amulet-core-1.9.8/amulet/api/partial_3d_array/
--rw-r--r--   0 runner     (501) staff       (20)      124 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/partial_3d_array/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     9215 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/partial_3d_array/base_partial_3d_array.py
--rw-r--r--   0 runner     (501) staff       (20)    21753 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/partial_3d_array/bounded_partial_3d_array.py
--rw-r--r--   0 runner     (501) staff       (20)      547 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/partial_3d_array/data_types.py
--rw-r--r--   0 runner     (501) staff       (20)     9270 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/partial_3d_array/unbounded_partial_3d_array.py
--rw-r--r--   0 runner     (501) staff       (20)     3969 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/partial_3d_array/util.py
--rw-r--r--   0 runner     (501) staff       (20)     1743 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/paths.py
--rw-r--r--   0 runner     (501) staff       (20)     1941 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/player.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.216112 amulet-core-1.9.8/amulet/api/registry/
--rw-r--r--   0 runner     (501) staff       (20)       80 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/registry/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      835 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/registry/base_registry.py
--rw-r--r--   0 runner     (501) staff       (20)     5157 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/registry/biome_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     4957 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/registry/block_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.218631 amulet-core-1.9.8/amulet/api/selection/
--rw-r--r--   0 runner     (501) staff       (20)       64 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/selection/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8433 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/selection/abstract_selection.py
--rw-r--r--   0 runner     (501) staff       (20)    30066 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/selection/box.py
--rw-r--r--   0 runner     (501) staff       (20)    18513 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/selection/group.py
--rw-r--r--   0 runner     (501) staff       (20)     1219 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/structure.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.220955 amulet-core-1.9.8/amulet/api/wrapper/
--rw-r--r--   0 runner     (501) staff       (20)      388 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/wrapper/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.223206 amulet-core-1.9.8/amulet/api/wrapper/chunk/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/wrapper/chunk/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    14692 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/wrapper/chunk/interface.py
--rw-r--r--   0 runner     (501) staff       (20)    22232 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/wrapper/chunk/translator.py
--rw-r--r--   0 runner     (501) staff       (20)    26001 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/wrapper/format_wrapper.py
--rw-r--r--   0 runner     (501) staff       (20)     3674 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/wrapper/structure_format_wrapper.py
--rw-r--r--   0 runner     (501) staff       (20)     1646 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/api/wrapper/world_format_wrapper.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.224000 amulet-core-1.9.8/amulet/img/
--rw-r--r--   0 runner     (501) staff       (20)    32841 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/img/missing_world_icon.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.225919 amulet-core-1.9.8/amulet/level/
--rw-r--r--   0 runner     (501) staff       (20)       42 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.226836 amulet-core-1.9.8/amulet/level/formats/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1124 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/anvil_forge_world.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.229781 amulet-core-1.9.8/amulet/level/formats/anvil_world/
--rw-r--r--   0 runner     (501) staff       (20)       54 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/anvil_world/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12660 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/anvil_world/_sector_manager.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.231729 amulet-core-1.9.8/amulet/level/formats/anvil_world/data_pack/
--rw-r--r--   0 runner     (501) staff       (20)       79 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/anvil_world/data_pack/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6161 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/anvil_world/data_pack/data_pack.py
--rw-r--r--   0 runner     (501) staff       (20)     2250 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/anvil_world/data_pack/data_pack_manager.py
--rw-r--r--   0 runner     (501) staff       (20)     6069 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/anvil_world/dimension.py
--rw-r--r--   0 runner     (501) staff       (20)    26951 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/anvil_world/format.py
--rw-r--r--   0 runner     (501) staff       (20)    14095 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/anvil_world/region.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.235129 amulet-core-1.9.8/amulet/level/formats/construction/
--rw-r--r--   0 runner     (501) staff       (20)       90 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/construction/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    18745 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/construction/format_wrapper.py
--rw-r--r--   0 runner     (501) staff       (20)     4951 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/construction/interface.py
--rw-r--r--   0 runner     (501) staff       (20)     1672 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/construction/section.py
--rw-r--r--   0 runner     (501) staff       (20)     4930 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/construction/util.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.237423 amulet-core-1.9.8/amulet/level/formats/leveldb_world/
--rw-r--r--   0 runner     (501) staff       (20)       58 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1202 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)    16304 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/dimension.py
--rw-r--r--   0 runner     (501) staff       (20)    18982 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/format.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.239251 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.262731 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/
--rw-r--r--   0 runner     (501) staff       (20)     1180 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    32388 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/base_leveldb_interface.py
--rw-r--r--   0 runner     (501) staff       (20)      738 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/generate_interface.py
--rw-r--r--   0 runner     (501) staff       (20)      880 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_0.py
--rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_1.py
--rw-r--r--   0 runner     (501) staff       (20)      186 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_10.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_11.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_12.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_13.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_14.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_15.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_16.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_17.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_18.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_19.py
--rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_2.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_20.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_21.py
--rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_22.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_23.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_24.py
--rw-r--r--   0 runner     (501) staff       (20)      673 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_25.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_26.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_27.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_28.py
--rw-r--r--   0 runner     (501) staff       (20)      752 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_29.py
--rw-r--r--   0 runner     (501) staff       (20)     1559 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_3.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_30.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_31.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_32.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_33.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_34.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_35.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_36.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_37.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_38.py
--rw-r--r--   0 runner     (501) staff       (20)      205 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_39.py
--rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_4.py
--rw-r--r--   0 runner     (501) staff       (20)      304 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_40.py
--rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_5.py
--rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_6.py
--rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_7.py
--rw-r--r--   0 runner     (501) staff       (20)     7326 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_8.py
--rw-r--r--   0 runner     (501) staff       (20)      456 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_9.py
--rw-r--r--   0 runner     (501) staff       (20)     3444 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_chunk_versions.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.264893 amulet-core-1.9.8/amulet/level/formats/mcstructure/
--rw-r--r--   0 runner     (501) staff       (20)       88 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/mcstructure/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1378 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/mcstructure/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)    15060 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/mcstructure/format_wrapper.py
--rw-r--r--   0 runner     (501) staff       (20)     6392 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/mcstructure/interface.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.267546 amulet-core-1.9.8/amulet/level/formats/schematic/
--rw-r--r--   0 runner     (501) staff       (20)       84 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/schematic/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1566 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/schematic/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)      111 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/schematic/data_types.py
--rw-r--r--   0 runner     (501) staff       (20)    12556 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/schematic/format_wrapper.py
--rw-r--r--   0 runner     (501) staff       (20)     5265 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/schematic/interface.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.269563 amulet-core-1.9.8/amulet/level/formats/sponge_schem/
--rw-r--r--   0 runner     (501) staff       (20)      102 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/sponge_schem/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1715 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/sponge_schem/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)    16612 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/sponge_schem/format_wrapper.py
--rw-r--r--   0 runner     (501) staff       (20)     4508 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/sponge_schem/interface.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.270451 amulet-core-1.9.8/amulet/level/formats/sponge_schem/varint/
--rw-r--r--   0 runner     (501) staff       (20)       81 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/sponge_schem/varint/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2361 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/formats/sponge_schem/varint/varint.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.270921 amulet-core-1.9.8/amulet/level/interfaces/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.271337 amulet-core-1.9.8/amulet/level/interfaces/chunk/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.283286 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2032 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_0.py
--rw-r--r--   0 runner     (501) staff       (20)    11153 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1444.py
--rw-r--r--   0 runner     (501) staff       (20)     3145 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1466.py
--rw-r--r--   0 runner     (501) staff       (20)      966 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1467.py
--rw-r--r--   0 runner     (501) staff       (20)      400 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1484.py
--rw-r--r--   0 runner     (501) staff       (20)      406 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1503.py
--rw-r--r--   0 runner     (501) staff       (20)      971 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1519.py
--rw-r--r--   0 runner     (501) staff       (20)      434 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1901.py
--rw-r--r--   0 runner     (501) staff       (20)      412 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1908.py
--rw-r--r--   0 runner     (501) staff       (20)      461 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1912.py
--rw-r--r--   0 runner     (501) staff       (20)      407 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1934.py
--rw-r--r--   0 runner     (501) staff       (20)     2114 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_2203.py
--rw-r--r--   0 runner     (501) staff       (20)      478 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_2529.py
--rw-r--r--   0 runner     (501) staff       (20)     2319 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_2681.py
--rw-r--r--   0 runner     (501) staff       (20)      417 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_2709.py
--rw-r--r--   0 runner     (501) staff       (20)     9618 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_2844.py
--rw-r--r--   0 runner     (501) staff       (20)    22007 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_na.py
--rw-r--r--   0 runner     (501) staff       (20)    11970 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/base_anvil_interface.py
--rw-r--r--   0 runner     (501) staff       (20)     2218 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/load.py
--rw-r--r--   0 runner     (501) staff       (20)     2869 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/loader.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.283901 amulet-core-1.9.8/amulet/level/translators/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/translators/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.284244 amulet-core-1.9.8/amulet/level/translators/chunk/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/translators/chunk/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.286319 amulet-core-1.9.8/amulet/level/translators/chunk/bedrock/
--rw-r--r--   0 runner     (501) staff       (20)    10226 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/translators/chunk/bedrock/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1654 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/translators/chunk/bedrock/bedrock_nbt_blockstate_translator.py
--rw-r--r--   0 runner     (501) staff       (20)     1314 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/translators/chunk/bedrock/bedrock_numerical_translator.py
--rw-r--r--   0 runner     (501) staff       (20)     1266 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/translators/chunk/bedrock/bedrock_psudo_numerical_translator.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.288458 amulet-core-1.9.8/amulet/level/translators/chunk/java/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/translators/chunk/java/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      907 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/translators/chunk/java/java_1_18_translator.py
--rw-r--r--   0 runner     (501) staff       (20)     3351 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/translators/chunk/java/java_blockstate_translator.py
--rw-r--r--   0 runner     (501) staff       (20)     1999 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/level/translators/chunk/java/java_numerical_translator.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.288918 amulet-core-1.9.8/amulet/libs/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/libs/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.289341 amulet-core-1.9.8/amulet/libs/leveldb/
--rw-r--r--   0 runner     (501) staff       (20)      242 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/libs/leveldb/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.292761 amulet-core-1.9.8/amulet/operations/
--rw-r--r--   0 runner     (501) staff       (20)      141 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/operations/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      587 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/operations/clone.py
--rw-r--r--   0 runner     (501) staff       (20)      947 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/operations/delete_chunk.py
--rw-r--r--   0 runner     (501) staff       (20)      901 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/operations/fill.py
--rw-r--r--   0 runner     (501) staff       (20)     1457 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/operations/paste.py
--rw-r--r--   0 runner     (501) staff       (20)     2029 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/operations/replace.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.296426 amulet-core-1.9.8/amulet/utils/
--rw-r--r--   0 runner     (501) staff       (20)      326 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/utils/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1192 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/utils/format_utils.py
--rw-r--r--   0 runner     (501) staff       (20)      364 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/utils/generator.py
--rw-r--r--   0 runner     (501) staff       (20)     7665 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/utils/matrix.py
--rw-r--r--   0 runner     (501) staff       (20)     1232 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/utils/numpy_helpers.py
--rw-r--r--   0 runner     (501) staff       (20)    12559 2022-10-05 13:19:40.000000 amulet-core-1.9.8/amulet/utils/world_utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-05 13:20:17.299910 amulet-core-1.9.8/amulet_core.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3792 2022-10-05 13:20:17.000000 amulet-core-1.9.8/amulet_core.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     9656 2022-10-05 13:20:17.000000 amulet-core-1.9.8/amulet_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-10-05 13:20:17.000000 amulet-core-1.9.8/amulet_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       63 2022-10-05 13:20:17.000000 amulet-core-1.9.8/amulet_core.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      202 2022-10-05 13:20:17.000000 amulet-core-1.9.8/amulet_core.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        7 2022-10-05 13:20:17.000000 amulet-core-1.9.8/amulet_core.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      174 2022-10-05 13:19:40.000000 amulet-core-1.9.8/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)     1078 2022-10-05 13:20:17.301784 amulet-core-1.9.8/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      547 2022-10-05 13:19:40.000000 amulet-core-1.9.8/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/
+-rw-r--r--   0 runner     (501) staff       (20)       60 2022-10-26 08:48:47.000000 amulet-core-1.9.9/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3792 2022-10-26 08:49:24.000000 amulet-core-1.9.9/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3330 2022-10-26 08:48:47.000000 amulet-core-1.9.9/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/
+-rw-r--r--   0 runner     (501) staff       (20)      385 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/__pyinstaller/
+-rw-r--r--   0 runner     (501) staff       (20)       41 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/__pyinstaller/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      498 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/__pyinstaller/hook-amulet.py
+-rw-r--r--   0 runner     (501) staff       (20)      497 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/_version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/
+-rw-r--r--   0 runner     (501) staff       (20)       46 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3739 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/abstract_base_entity.py
+-rw-r--r--   0 runner     (501) staff       (20)    23048 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/block.py
+-rw-r--r--   0 runner     (501) staff       (20)     2004 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/block_entity.py
+-rw-r--r--   0 runner     (501) staff       (20)     3080 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/cache.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/chunk/
+-rw-r--r--   0 runner     (501) staff       (20)      217 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/chunk/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7414 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/chunk/biomes.py
+-rw-r--r--   0 runner     (501) staff       (20)     6182 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/chunk/block_entity_dict.py
+-rw-r--r--   0 runner     (501) staff       (20)     1652 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/chunk/blocks.py
+-rw-r--r--   0 runner     (501) staff       (20)    13385 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/chunk/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)     2047 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/chunk/entity_list.py
+-rw-r--r--   0 runner     (501) staff       (20)     4908 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/chunk/status.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/data_types/
+-rw-r--r--   0 runner     (501) staff       (20)      116 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/data_types/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       78 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/data_types/generic_types.py
+-rw-r--r--   0 runner     (501) staff       (20)      598 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/data_types/operation_types.py
+-rw-r--r--   0 runner     (501) staff       (20)     2261 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/data_types/world_types.py
+-rw-r--r--   0 runner     (501) staff       (20)     2580 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/data_types/wrapper_types.py
+-rw-r--r--   0 runner     (501) staff       (20)     1839 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/entity.py
+-rw-r--r--   0 runner     (501) staff       (20)     2825 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/errors.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/history/
+-rw-r--r--   0 runner     (501) staff       (20)     2329 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/history/base/
+-rw-r--r--   0 runner     (501) staff       (20)      128 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/base/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      674 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/base/base_history.py
+-rw-r--r--   0 runner     (501) staff       (20)     2055 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/base/history_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     2816 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/base/revision_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)      432 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/changeable.py
+-rw-r--r--   0 runner     (501) staff       (20)      226 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/data_types.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/history/history_manager/
+-rw-r--r--   0 runner     (501) staff       (20)      123 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/history_manager/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3480 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/history_manager/container.py
+-rw-r--r--   0 runner     (501) staff       (20)    11327 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/history_manager/database.py
+-rw-r--r--   0 runner     (501) staff       (20)     3023 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/history_manager/meta.py
+-rw-r--r--   0 runner     (501) staff       (20)     4064 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/history_manager/object.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/history/revision_manager/
+-rw-r--r--   0 runner     (501) staff       (20)       72 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/revision_manager/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1023 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/revision_manager/disk.py
+-rw-r--r--   0 runner     (501) staff       (20)      376 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/history/revision_manager/ram.py
+-rw-r--r--   0 runner     (501) staff       (20)     1819 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/item.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/level/
+-rw-r--r--   0 runner     (501) staff       (20)      144 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/level/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/level/base_level/
+-rw-r--r--   0 runner     (501) staff       (20)       34 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/level/base_level/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    43105 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/level/base_level/base_level.py
+-rw-r--r--   0 runner     (501) staff       (20)     8921 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/level/base_level/chunk_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)    19325 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/level/base_level/clone.py
+-rw-r--r--   0 runner     (501) staff       (20)     3226 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/level/base_level/player_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/level/immutable_structure/
+-rw-r--r--   0 runner     (501) staff       (20)       52 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/level/immutable_structure/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3302 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/level/immutable_structure/immutable_structure.py
+-rw-r--r--   0 runner     (501) staff       (20)     3065 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/level/immutable_structure/void_format_wrapper.py
+-rw-r--r--   0 runner     (501) staff       (20)      619 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/level/structure.py
+-rw-r--r--   0 runner     (501) staff       (20)      613 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/level/world.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/partial_3d_array/
+-rw-r--r--   0 runner     (501) staff       (20)      124 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/partial_3d_array/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     9215 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/partial_3d_array/base_partial_3d_array.py
+-rw-r--r--   0 runner     (501) staff       (20)    21753 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/partial_3d_array/bounded_partial_3d_array.py
+-rw-r--r--   0 runner     (501) staff       (20)      547 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/partial_3d_array/data_types.py
+-rw-r--r--   0 runner     (501) staff       (20)     9270 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/partial_3d_array/unbounded_partial_3d_array.py
+-rw-r--r--   0 runner     (501) staff       (20)     3969 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/partial_3d_array/util.py
+-rw-r--r--   0 runner     (501) staff       (20)     1743 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/paths.py
+-rw-r--r--   0 runner     (501) staff       (20)     1941 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/player.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/registry/
+-rw-r--r--   0 runner     (501) staff       (20)       80 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/registry/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      835 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/registry/base_registry.py
+-rw-r--r--   0 runner     (501) staff       (20)     5157 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/registry/biome_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     4957 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/registry/block_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/selection/
+-rw-r--r--   0 runner     (501) staff       (20)       64 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/selection/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8433 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/selection/abstract_selection.py
+-rw-r--r--   0 runner     (501) staff       (20)    30066 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/selection/box.py
+-rw-r--r--   0 runner     (501) staff       (20)    18513 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/selection/group.py
+-rw-r--r--   0 runner     (501) staff       (20)     1219 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/structure.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/wrapper/
+-rw-r--r--   0 runner     (501) staff       (20)      388 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/wrapper/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/api/wrapper/chunk/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/wrapper/chunk/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14692 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/wrapper/chunk/interface.py
+-rw-r--r--   0 runner     (501) staff       (20)    22232 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/wrapper/chunk/translator.py
+-rw-r--r--   0 runner     (501) staff       (20)    26001 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/wrapper/format_wrapper.py
+-rw-r--r--   0 runner     (501) staff       (20)     3674 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/wrapper/structure_format_wrapper.py
+-rw-r--r--   0 runner     (501) staff       (20)     1646 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/api/wrapper/world_format_wrapper.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/img/
+-rw-r--r--   0 runner     (501) staff       (20)    32841 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/img/missing_world_icon.png
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/
+-rw-r--r--   0 runner     (501) staff       (20)       42 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/formats/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1124 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/anvil_forge_world.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/formats/anvil_world/
+-rw-r--r--   0 runner     (501) staff       (20)       54 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/anvil_world/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12660 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/anvil_world/_sector_manager.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/formats/anvil_world/data_pack/
+-rw-r--r--   0 runner     (501) staff       (20)       79 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/anvil_world/data_pack/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6161 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/anvil_world/data_pack/data_pack.py
+-rw-r--r--   0 runner     (501) staff       (20)     2250 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/anvil_world/data_pack/data_pack_manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     6069 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/anvil_world/dimension.py
+-rw-r--r--   0 runner     (501) staff       (20)    26951 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/anvil_world/format.py
+-rw-r--r--   0 runner     (501) staff       (20)    14095 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/anvil_world/region.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/formats/construction/
+-rw-r--r--   0 runner     (501) staff       (20)       90 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/construction/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    18745 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/construction/format_wrapper.py
+-rw-r--r--   0 runner     (501) staff       (20)     4951 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/construction/interface.py
+-rw-r--r--   0 runner     (501) staff       (20)     1672 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/construction/section.py
+-rw-r--r--   0 runner     (501) staff       (20)     4930 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/construction/util.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/
+-rw-r--r--   0 runner     (501) staff       (20)       58 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1202 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)    16304 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/dimension.py
+-rw-r--r--   0 runner     (501) staff       (20)    18983 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/format.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/
+-rw-r--r--   0 runner     (501) staff       (20)     1180 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    32471 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/base_leveldb_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)      738 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/generate_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)      880 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_0.py
+-rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_1.py
+-rw-r--r--   0 runner     (501) staff       (20)      186 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_10.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_11.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_12.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_13.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_14.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_15.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_16.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_17.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_18.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_19.py
+-rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_2.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_20.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_21.py
+-rw-r--r--   0 runner     (501) staff       (20)      189 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_22.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_23.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_24.py
+-rw-r--r--   0 runner     (501) staff       (20)      673 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_25.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_26.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_27.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_28.py
+-rw-r--r--   0 runner     (501) staff       (20)      752 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_29.py
+-rw-r--r--   0 runner     (501) staff       (20)     1559 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_3.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_30.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_31.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_32.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_33.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_34.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_35.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_36.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_37.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_38.py
+-rw-r--r--   0 runner     (501) staff       (20)      205 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_39.py
+-rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_4.py
+-rw-r--r--   0 runner     (501) staff       (20)      304 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_40.py
+-rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_5.py
+-rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_6.py
+-rw-r--r--   0 runner     (501) staff       (20)      183 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_7.py
+-rw-r--r--   0 runner     (501) staff       (20)     7326 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_8.py
+-rw-r--r--   0 runner     (501) staff       (20)      456 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_9.py
+-rw-r--r--   0 runner     (501) staff       (20)     3444 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_chunk_versions.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/formats/mcstructure/
+-rw-r--r--   0 runner     (501) staff       (20)       88 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/mcstructure/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1378 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/mcstructure/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)    15060 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/mcstructure/format_wrapper.py
+-rw-r--r--   0 runner     (501) staff       (20)     6467 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/mcstructure/interface.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/formats/schematic/
+-rw-r--r--   0 runner     (501) staff       (20)       84 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/schematic/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1566 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/schematic/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)      111 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/schematic/data_types.py
+-rw-r--r--   0 runner     (501) staff       (20)    12556 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/schematic/format_wrapper.py
+-rw-r--r--   0 runner     (501) staff       (20)     5265 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/schematic/interface.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/formats/sponge_schem/
+-rw-r--r--   0 runner     (501) staff       (20)      102 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/sponge_schem/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1715 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/sponge_schem/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)    16612 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/sponge_schem/format_wrapper.py
+-rw-r--r--   0 runner     (501) staff       (20)     4508 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/sponge_schem/interface.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/formats/sponge_schem/varint/
+-rw-r--r--   0 runner     (501) staff       (20)       81 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/sponge_schem/varint/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2361 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/formats/sponge_schem/varint/varint.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/interfaces/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2032 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_0.py
+-rw-r--r--   0 runner     (501) staff       (20)    11153 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1444.py
+-rw-r--r--   0 runner     (501) staff       (20)     3145 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1466.py
+-rw-r--r--   0 runner     (501) staff       (20)      966 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1467.py
+-rw-r--r--   0 runner     (501) staff       (20)      400 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1484.py
+-rw-r--r--   0 runner     (501) staff       (20)      406 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1503.py
+-rw-r--r--   0 runner     (501) staff       (20)      971 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1519.py
+-rw-r--r--   0 runner     (501) staff       (20)      434 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1901.py
+-rw-r--r--   0 runner     (501) staff       (20)      412 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1908.py
+-rw-r--r--   0 runner     (501) staff       (20)      461 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1912.py
+-rw-r--r--   0 runner     (501) staff       (20)      407 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1934.py
+-rw-r--r--   0 runner     (501) staff       (20)     2114 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_2203.py
+-rw-r--r--   0 runner     (501) staff       (20)      478 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_2529.py
+-rw-r--r--   0 runner     (501) staff       (20)     2319 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_2681.py
+-rw-r--r--   0 runner     (501) staff       (20)      417 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_2709.py
+-rw-r--r--   0 runner     (501) staff       (20)     9618 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_2844.py
+-rw-r--r--   0 runner     (501) staff       (20)    22007 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_na.py
+-rw-r--r--   0 runner     (501) staff       (20)    11970 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/base_anvil_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)     2218 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/load.py
+-rw-r--r--   0 runner     (501) staff       (20)     2869 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/loader.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/translators/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/translators/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/translators/chunk/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/translators/chunk/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/translators/chunk/bedrock/
+-rw-r--r--   0 runner     (501) staff       (20)    10226 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/translators/chunk/bedrock/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1654 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/translators/chunk/bedrock/bedrock_nbt_blockstate_translator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1314 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/translators/chunk/bedrock/bedrock_numerical_translator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1266 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/translators/chunk/bedrock/bedrock_psudo_numerical_translator.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/level/translators/chunk/java/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/translators/chunk/java/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      907 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/translators/chunk/java/java_1_18_translator.py
+-rw-r--r--   0 runner     (501) staff       (20)     3351 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/translators/chunk/java/java_blockstate_translator.py
+-rw-r--r--   0 runner     (501) staff       (20)     1999 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/level/translators/chunk/java/java_numerical_translator.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/libs/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/libs/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/libs/leveldb/
+-rw-r--r--   0 runner     (501) staff       (20)      242 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/libs/leveldb/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/operations/
+-rw-r--r--   0 runner     (501) staff       (20)      141 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/operations/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      587 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/operations/clone.py
+-rw-r--r--   0 runner     (501) staff       (20)      947 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/operations/delete_chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)      901 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/operations/fill.py
+-rw-r--r--   0 runner     (501) staff       (20)     1457 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/operations/paste.py
+-rw-r--r--   0 runner     (501) staff       (20)     2029 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/operations/replace.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet/utils/
+-rw-r--r--   0 runner     (501) staff       (20)      326 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/utils/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1192 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/utils/format_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)      364 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/utils/generator.py
+-rw-r--r--   0 runner     (501) staff       (20)     7665 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/utils/matrix.py
+-rw-r--r--   0 runner     (501) staff       (20)     1232 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/utils/numpy_helpers.py
+-rw-r--r--   0 runner     (501) staff       (20)    12559 2022-10-26 08:48:47.000000 amulet-core-1.9.9/amulet/utils/world_utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet_core.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3792 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     9656 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       63 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      202 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet_core.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        7 2022-10-26 08:49:24.000000 amulet-core-1.9.9/amulet_core.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      174 2022-10-26 08:48:47.000000 amulet-core-1.9.9/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)     1078 2022-10-26 08:49:24.000000 amulet-core-1.9.9/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      547 2022-10-26 08:48:47.000000 amulet-core-1.9.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `amulet-core-1.9.8/PKG-INFO` & `amulet-core-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amulet-core
-Version: 1.9.8
+Version: 1.9.9
 Summary: A Python library for reading/writing Minecraft's various save formats.
 Home-page: https://www.amuletmc.com
 Author: James Clare, Ben Gothard et al.
 Author-email: amuleteditor@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `amulet-core-1.9.8/README.md` & `amulet-core-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/abstract_base_entity.py` & `amulet-core-1.9.9/amulet/api/abstract_base_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,18 +58,16 @@
         :return: The namespace:base_name of the block entity or just base_name if no namespace
         """
         return self._namespaced_name
 
     @namespaced_name.setter
     def namespaced_name(self, value: str):
         self._namespaced_name = value
-        if ":" in value:
-            self._namespace, self._base_name = value.split(":", 1)
-        else:
-            self._namespace, self._base_name = "", value
+        *namespace, self._base_name = value.split(":", 1)
+        self._namespace = namespace[0] if namespace else ""
 
     @property
     def namespace(self) -> str:
         """
         The namespace of the block entity represented by the BlockEntity object (eg: `minecraft`)
 
         :return: The namespace of the block entity
```

### Comparing `amulet-core-1.9.8/amulet/api/block.py` & `amulet-core-1.9.9/amulet/api/block.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/block_entity.py` & `amulet-core-1.9.9/amulet/api/block_entity.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/cache.py` & `amulet-core-1.9.9/amulet/api/cache.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/chunk/biomes.py` & `amulet-core-1.9.9/amulet/api/chunk/biomes.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/chunk/block_entity_dict.py` & `amulet-core-1.9.9/amulet/api/chunk/block_entity_dict.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/chunk/blocks.py` & `amulet-core-1.9.9/amulet/api/chunk/blocks.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/chunk/chunk.py` & `amulet-core-1.9.9/amulet/api/chunk/chunk.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/chunk/entity_list.py` & `amulet-core-1.9.9/amulet/api/chunk/entity_list.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/chunk/status.py` & `amulet-core-1.9.9/amulet/api/chunk/status.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/data_types/operation_types.py` & `amulet-core-1.9.9/amulet/api/data_types/operation_types.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/data_types/world_types.py` & `amulet-core-1.9.9/amulet/api/data_types/world_types.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/data_types/wrapper_types.py` & `amulet-core-1.9.9/amulet/api/data_types/wrapper_types.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/entity.py` & `amulet-core-1.9.9/amulet/api/entity.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/errors.py` & `amulet-core-1.9.9/amulet/api/errors.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/history/__init__.py` & `amulet-core-1.9.9/amulet/api/history/__init__.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/history/base/base_history.py` & `amulet-core-1.9.9/amulet/api/history/base/base_history.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/history/base/history_manager.py` & `amulet-core-1.9.9/amulet/api/history/base/history_manager.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/history/base/revision_manager.py` & `amulet-core-1.9.9/amulet/api/history/base/revision_manager.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/history/history_manager/container.py` & `amulet-core-1.9.9/amulet/api/history/history_manager/container.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/history/history_manager/database.py` & `amulet-core-1.9.9/amulet/api/history/history_manager/database.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/history/history_manager/meta.py` & `amulet-core-1.9.9/amulet/api/history/history_manager/meta.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/history/history_manager/object.py` & `amulet-core-1.9.9/amulet/api/history/history_manager/object.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/history/revision_manager/disk.py` & `amulet-core-1.9.9/amulet/api/history/revision_manager/disk.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/item.py` & `amulet-core-1.9.9/amulet/api/item.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/level/base_level/base_level.py` & `amulet-core-1.9.9/amulet/api/level/base_level/base_level.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/level/base_level/chunk_manager.py` & `amulet-core-1.9.9/amulet/api/level/base_level/chunk_manager.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/level/base_level/clone.py` & `amulet-core-1.9.9/amulet/api/level/base_level/clone.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/level/base_level/player_manager.py` & `amulet-core-1.9.9/amulet/api/level/base_level/player_manager.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/level/immutable_structure/immutable_structure.py` & `amulet-core-1.9.9/amulet/api/level/immutable_structure/immutable_structure.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/level/immutable_structure/void_format_wrapper.py` & `amulet-core-1.9.9/amulet/api/level/immutable_structure/void_format_wrapper.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/level/structure.py` & `amulet-core-1.9.9/amulet/api/level/structure.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/level/world.py` & `amulet-core-1.9.9/amulet/api/level/world.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/partial_3d_array/base_partial_3d_array.py` & `amulet-core-1.9.9/amulet/api/partial_3d_array/base_partial_3d_array.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/partial_3d_array/bounded_partial_3d_array.py` & `amulet-core-1.9.9/amulet/api/partial_3d_array/bounded_partial_3d_array.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/partial_3d_array/data_types.py` & `amulet-core-1.9.9/amulet/api/partial_3d_array/data_types.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/partial_3d_array/unbounded_partial_3d_array.py` & `amulet-core-1.9.9/amulet/api/partial_3d_array/unbounded_partial_3d_array.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/partial_3d_array/util.py` & `amulet-core-1.9.9/amulet/api/partial_3d_array/util.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/paths.py` & `amulet-core-1.9.9/amulet/api/paths.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/player.py` & `amulet-core-1.9.9/amulet/api/player.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/registry/base_registry.py` & `amulet-core-1.9.9/amulet/api/registry/base_registry.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/registry/biome_manager.py` & `amulet-core-1.9.9/amulet/api/registry/biome_manager.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/registry/block_manager.py` & `amulet-core-1.9.9/amulet/api/registry/block_manager.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/selection/abstract_selection.py` & `amulet-core-1.9.9/amulet/api/selection/abstract_selection.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/selection/box.py` & `amulet-core-1.9.9/amulet/api/selection/box.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/selection/group.py` & `amulet-core-1.9.9/amulet/api/selection/group.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/structure.py` & `amulet-core-1.9.9/amulet/api/structure.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/wrapper/chunk/interface.py` & `amulet-core-1.9.9/amulet/api/wrapper/chunk/interface.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/wrapper/chunk/translator.py` & `amulet-core-1.9.9/amulet/api/wrapper/chunk/translator.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/wrapper/format_wrapper.py` & `amulet-core-1.9.9/amulet/api/wrapper/format_wrapper.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/wrapper/structure_format_wrapper.py` & `amulet-core-1.9.9/amulet/api/wrapper/structure_format_wrapper.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/api/wrapper/world_format_wrapper.py` & `amulet-core-1.9.9/amulet/api/wrapper/world_format_wrapper.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/img/missing_world_icon.png` & `amulet-core-1.9.9/amulet/img/missing_world_icon.png`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/anvil_forge_world.py` & `amulet-core-1.9.9/amulet/level/formats/anvil_forge_world.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/anvil_world/_sector_manager.py` & `amulet-core-1.9.9/amulet/level/formats/anvil_world/_sector_manager.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/anvil_world/data_pack/data_pack.py` & `amulet-core-1.9.9/amulet/level/formats/anvil_world/data_pack/data_pack.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/anvil_world/data_pack/data_pack_manager.py` & `amulet-core-1.9.9/amulet/level/formats/anvil_world/data_pack/data_pack_manager.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/anvil_world/dimension.py` & `amulet-core-1.9.9/amulet/level/formats/anvil_world/dimension.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/anvil_world/format.py` & `amulet-core-1.9.9/amulet/level/formats/anvil_world/format.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/anvil_world/region.py` & `amulet-core-1.9.9/amulet/level/formats/anvil_world/region.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/construction/format_wrapper.py` & `amulet-core-1.9.9/amulet/level/formats/construction/format_wrapper.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/construction/interface.py` & `amulet-core-1.9.9/amulet/level/formats/construction/interface.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/construction/section.py` & `amulet-core-1.9.9/amulet/level/formats/construction/section.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/construction/util.py` & `amulet-core-1.9.9/amulet/level/formats/construction/util.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/chunk.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/chunk.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/dimension.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/dimension.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/format.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     def path(self) -> Optional[str]:
         return self._path
 
     @staticmethod
     def _read_from(path: str) -> Tuple[int, str, AbstractBaseTag]:
         with open(path, "rb") as f:
             level_dat_version = struct.unpack("<i", f.read(4))[0]
-            if 4 <= level_dat_version <= 9:
+            if 4 <= level_dat_version <= 10:
                 data_length = struct.unpack("<i", f.read(4))[0]
                 root_tag = load_nbt(
                     f.read(data_length),
                     compressed=False,
                     little_endian=True,
                     string_decoder=utf8_escape_decoder,
                 )
```

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/__init__.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/__init__.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/base_leveldb_interface.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/base_leveldb_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,15 +425,16 @@
                         sub_chunk_blocks[:, :, :, storage_index],
                         palette_data,
                         data,
                     ) = self._load_palette_blocks(data)
                     palette_data_out: List[Tuple[Optional[int], Block]] = []
                     for block in palette_data:
                         block = block.compound
-                        namespace, base_name = block["name"].py_str.split(":", 1)
+                        *namespace_, base_name = block["name"].py_str.split(":", 1)
+                        namespace = namespace_[0] if namespace_ else "minecraft"
                         if "version" in block:
                             version: Optional[int] = block.get_int("version").py_int
                         else:
                             version = None
 
                         if "states" in block or "val" not in block:  # 1.13 format
                             properties = block.get_compound(
```

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/generate_interface.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/generate_interface.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_0.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_0.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_25.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_25.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_29.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_29.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_3.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_3.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_8.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_8.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/leveldb_world/interface/chunk/leveldb_chunk_versions.py` & `amulet-core-1.9.9/amulet/level/formats/leveldb_world/interface/chunk/leveldb_chunk_versions.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/mcstructure/chunk.py` & `amulet-core-1.9.9/amulet/level/formats/mcstructure/chunk.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/mcstructure/format_wrapper.py` & `amulet-core-1.9.9/amulet/level/formats/mcstructure/format_wrapper.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/mcstructure/interface.py` & `amulet-core-1.9.9/amulet/level/formats/mcstructure/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,16 @@
                 ),
             ),
         )
 
         for index, blocks in enumerate(data.palette):
             block_layers: List[Tuple[Optional[int], Block]] = []
             for block in blocks:
-                namespace, base_name = block["name"].py_str.split(":", 1)
+                *namespace_, base_name = block["name"].py_str.split(":", 1)
+                namespace = namespace_[0] if namespace_ else "minecraft"
                 if "version" in block:
                     version: Optional[int] = block["version"].py_int
                 else:
                     version = None
 
                 if "states" in block:  # 1.13 format
                     properties = block["states"].py_dict
```

### Comparing `amulet-core-1.9.8/amulet/level/formats/schematic/chunk.py` & `amulet-core-1.9.9/amulet/level/formats/schematic/chunk.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/schematic/format_wrapper.py` & `amulet-core-1.9.9/amulet/level/formats/schematic/format_wrapper.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/schematic/interface.py` & `amulet-core-1.9.9/amulet/level/formats/schematic/interface.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/sponge_schem/chunk.py` & `amulet-core-1.9.9/amulet/level/formats/sponge_schem/chunk.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/sponge_schem/format_wrapper.py` & `amulet-core-1.9.9/amulet/level/formats/sponge_schem/format_wrapper.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/sponge_schem/interface.py` & `amulet-core-1.9.9/amulet/level/formats/sponge_schem/interface.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/formats/sponge_schem/varint/varint.py` & `amulet-core-1.9.9/amulet/level/formats/sponge_schem/varint/varint.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_0.py` & `amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_0.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1444.py` & `amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1444.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1466.py` & `amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1466.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1467.py` & `amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1467.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_1519.py` & `amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_1519.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_2203.py` & `amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_2203.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_2681.py` & `amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_2681.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_2844.py` & `amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_2844.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/anvil_na.py` & `amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/anvil_na.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/interfaces/chunk/anvil/base_anvil_interface.py` & `amulet-core-1.9.9/amulet/level/interfaces/chunk/anvil/base_anvil_interface.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/load.py` & `amulet-core-1.9.9/amulet/level/load.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/loader.py` & `amulet-core-1.9.9/amulet/level/loader.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/translators/chunk/bedrock/__init__.py` & `amulet-core-1.9.9/amulet/level/translators/chunk/bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/translators/chunk/bedrock/bedrock_nbt_blockstate_translator.py` & `amulet-core-1.9.9/amulet/level/translators/chunk/bedrock/bedrock_nbt_blockstate_translator.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/translators/chunk/bedrock/bedrock_numerical_translator.py` & `amulet-core-1.9.9/amulet/level/translators/chunk/bedrock/bedrock_numerical_translator.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/translators/chunk/bedrock/bedrock_psudo_numerical_translator.py` & `amulet-core-1.9.9/amulet/level/translators/chunk/bedrock/bedrock_psudo_numerical_translator.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/translators/chunk/java/java_1_18_translator.py` & `amulet-core-1.9.9/amulet/level/translators/chunk/java/java_1_18_translator.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/translators/chunk/java/java_blockstate_translator.py` & `amulet-core-1.9.9/amulet/level/translators/chunk/java/java_blockstate_translator.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/level/translators/chunk/java/java_numerical_translator.py` & `amulet-core-1.9.9/amulet/level/translators/chunk/java/java_numerical_translator.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/operations/clone.py` & `amulet-core-1.9.9/amulet/operations/clone.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/operations/delete_chunk.py` & `amulet-core-1.9.9/amulet/operations/delete_chunk.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/operations/fill.py` & `amulet-core-1.9.9/amulet/operations/fill.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/operations/paste.py` & `amulet-core-1.9.9/amulet/operations/paste.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/operations/replace.py` & `amulet-core-1.9.9/amulet/operations/replace.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/utils/format_utils.py` & `amulet-core-1.9.9/amulet/utils/format_utils.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/utils/matrix.py` & `amulet-core-1.9.9/amulet/utils/matrix.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/utils/numpy_helpers.py` & `amulet-core-1.9.9/amulet/utils/numpy_helpers.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet/utils/world_utils.py` & `amulet-core-1.9.9/amulet/utils/world_utils.py`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/amulet_core.egg-info/PKG-INFO` & `amulet-core-1.9.9/amulet_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amulet-core
-Version: 1.9.8
+Version: 1.9.9
 Summary: A Python library for reading/writing Minecraft's various save formats.
 Home-page: https://www.amuletmc.com
 Author: James Clare, Ben Gothard et al.
 Author-email: amuleteditor@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `amulet-core-1.9.8/amulet_core.egg-info/SOURCES.txt` & `amulet-core-1.9.9/amulet_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/setup.cfg` & `amulet-core-1.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `amulet-core-1.9.8/setup.py` & `amulet-core-1.9.9/setup.py`

 * *Files identical despite different names*

