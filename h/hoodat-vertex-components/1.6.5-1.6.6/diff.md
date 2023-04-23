# Comparing `tmp/hoodat_vertex_components-1.6.5.tar.gz` & `tmp/hoodat_vertex_components-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoodat_vertex_components-1.6.5.tar", max compression
+gzip compressed data, was "hoodat_vertex_components-1.6.6.tar", max compression
```

## Comparing `hoodat_vertex_components-1.6.5.tar` & `hoodat_vertex_components-1.6.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1069 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/LICENSE.txt
--rw-r--r--   0        0        0     2368 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/README.md
--rw-r--r--   0        0        0       22 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/__init__.py
--rw-r--r--   0        0        0     1919 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/__init__.py
--rw-r--r--   0        0        0       61 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/add_py/Dockerfile
--rw-r--r--   0        0        0      295 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/add_py/add.py
--rw-r--r--   0        0        0      490 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/add_py/component.yaml
--rw-r--r--   0        0        0     1895 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile
--rw-r--r--   0        0        0     1305 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile_orig
--rw-r--r--   0        0        0     3423 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/component.py
--rw-r--r--   0        0        0     5107 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/component.yaml
--rw-r--r--   0        0        0   154659 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/friends-Scene-008.mp4
--rw-r--r--   0        0        0    25708 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/poetry.lock
--rw-r--r--   0        0        0      568 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/pyproject.toml
--rw-r--r--   0        0        0      160 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/requirements.txt
--rw-r--r--   0        0        0    14976 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/tools/demo_track.py
--rw-r--r--   0        0        0     1895 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/Dockerfile
--rw-r--r--   0        0        0     5862 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/component.py
--rw-r--r--   0        0        0     7736 2023-04-23 11:12:50.900604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/component.yaml
--rw-r--r--   0        0        0   154659 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/friends-Scene-008.mp4
--rw-r--r--   0        0        0    25708 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/poetry.lock
--rw-r--r--   0        0        0      568 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/pyproject.toml
--rw-r--r--   0        0        0      160 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/requirements.txt
--rw-r--r--   0        0        0    14976 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/tools/demo_track.py
--rw-r--r--   0        0        0       70 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/haar_from_frames/Dockerfile
--rw-r--r--   0        0        0     4294 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/haar_from_frames/component.py
--rw-r--r--   0        0        0     5711 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/haar_from_frames/component.yaml
--rw-r--r--   0        0        0      159 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/make_cascade_file/Dockerfile
--rw-r--r--   0        0        0      327 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/make_cascade_file/cascades.csv
--rw-r--r--   0        0        0      798 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/make_cascade_file/component.yaml
--rw-r--r--   0        0        0     1732 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/make_cascade_file/make_cascade_file.py
--rw-r--r--   0        0        0    14340 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/make_cascade_file/poetry.lock
--rw-r--r--   0        0        0      328 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/make_cascade_file/pyproject.toml
--rw-r--r--   0        0        0      707 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/make_cascade_file/tests/test_filter_cascades.py
--rw-r--r--   0        0        0      272 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/pyscenedetect/Dockerfile
--rw-r--r--   0        0        0     5631 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/pyscenedetect/component.py
--rw-r--r--   0        0        0     8128 2023-04-23 11:12:50.904604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/pyscenedetect/component.yaml
--rw-r--r--   0        0        0  2709671 2023-04-23 11:12:50.916604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/pyscenedetect/friends.mp4
--rw-r--r--   0        0        0     4827 2023-04-23 11:12:50.916604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/pyscenedetect/poetry.lock
--rw-r--r--   0        0        0      389 2023-04-23 11:12:50.916604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/pyscenedetect/pyproject.toml
--rw-r--r--   0        0        0      159 2023-04-23 11:12:50.916604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_data/Dockerfile
--rw-r--r--   0        0        0      963 2023-04-23 11:12:50.916604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_data/component.yaml
--rw-r--r--   0        0        0    49727 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_data/poetry.lock
--rw-r--r--   0        0        0      383 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_data/pyproject.toml
--rw-r--r--   0        0        0     1393 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_data/src/query_db.py
--rw-r--r--   0        0        0      159 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_string/Dockerfile
--rw-r--r--   0        0        0      955 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_string/component.yaml
--rw-r--r--   0        0        0    49727 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_string/poetry.lock
--rw-r--r--   0        0        0      383 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_string/pyproject.toml
--rw-r--r--   0        0        0     1756 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_string/src/query_db.py
--rw-r--r--   0        0        0      318 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/Dockerfile
--rw-r--r--   0        0        0      955 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/component.py
--rw-r--r--   0        0        0     1967 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/component.yaml
--rw-r--r--   0        0        0    73030 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/poetry.lock
--rw-r--r--   0        0        0      422 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/pyproject.toml
--rw-r--r--   0        0        0    78906 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-001.mp4
--rw-r--r--   0        0        0    76382 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-002.mp4
--rw-r--r--   0        0        0    92195 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-003.mp4
--rw-r--r--   0        0        0      159 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_in_database/Dockerfile
--rw-r--r--   0        0        0     4965 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_in_database/component.py
--rw-r--r--   0        0        0     6840 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_in_database/component.yaml
--rw-r--r--   0        0        0    20204 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_in_database/poetry.lock
--rw-r--r--   0        0        0      525 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_in_database/pyproject.toml
--rw-r--r--   0        0        0      194 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_to_frames/Dockerfile
--rw-r--r--   0        0        0     5490 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_to_frames/component.py
--rw-r--r--   0        0        0     7578 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_to_frames/component.yaml
--rw-r--r--   0        0        0     1285 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_to_frames/poetry.lock
--rw-r--r--   0        0        0      308 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_to_frames/pyproject.toml
--rw-r--r--   0        0        0      886 2023-04-23 11:12:50.920604 hoodat_vertex_components-1.6.5/pyproject.toml
--rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 hoodat_vertex_components-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-23 17:13:43.197737 hoodat_vertex_components-1.6.6/LICENSE.txt
+-rw-r--r--   0        0        0     2368 2023-04-23 17:13:43.197737 hoodat_vertex_components-1.6.6/README.md
+-rw-r--r--   0        0        0       22 2023-04-23 17:13:43.197737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/__init__.py
+-rw-r--r--   0        0        0     1919 2023-04-23 17:13:43.197737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-23 17:13:43.197737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/add_py/Dockerfile
+-rw-r--r--   0        0        0      295 2023-04-23 17:13:43.197737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/add_py/add.py
+-rw-r--r--   0        0        0      490 2023-04-23 17:13:43.197737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/add_py/component.yaml
+-rw-r--r--   0        0        0     1895 2023-04-23 17:13:43.197737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile
+-rw-r--r--   0        0        0     1305 2023-04-23 17:13:43.197737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile_orig
+-rw-r--r--   0        0        0     3423 2023-04-23 17:13:43.197737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/component.py
+-rw-r--r--   0        0        0     5107 2023-04-23 17:13:43.197737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/component.yaml
+-rw-r--r--   0        0        0   154659 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/friends-Scene-008.mp4
+-rw-r--r--   0        0        0    25708 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/poetry.lock
+-rw-r--r--   0        0        0      568 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/requirements.txt
+-rw-r--r--   0        0        0    14976 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/tools/demo_track.py
+-rw-r--r--   0        0        0     1895 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/Dockerfile
+-rw-r--r--   0        0        0     5862 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/component.py
+-rw-r--r--   0        0        0     8227 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/component.yaml
+-rw-r--r--   0        0        0   154659 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/friends-Scene-008.mp4
+-rw-r--r--   0        0        0    25708 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/poetry.lock
+-rw-r--r--   0        0        0      568 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/requirements.txt
+-rw-r--r--   0        0        0    14976 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/tools/demo_track.py
+-rw-r--r--   0        0        0       70 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/haar_from_frames/Dockerfile
+-rw-r--r--   0        0        0     4294 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/haar_from_frames/component.py
+-rw-r--r--   0        0        0     5711 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/haar_from_frames/component.yaml
+-rw-r--r--   0        0        0      159 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/make_cascade_file/Dockerfile
+-rw-r--r--   0        0        0      327 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/make_cascade_file/cascades.csv
+-rw-r--r--   0        0        0      798 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/make_cascade_file/component.yaml
+-rw-r--r--   0        0        0     1732 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/make_cascade_file/make_cascade_file.py
+-rw-r--r--   0        0        0    14340 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/make_cascade_file/poetry.lock
+-rw-r--r--   0        0        0      328 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/make_cascade_file/pyproject.toml
+-rw-r--r--   0        0        0      707 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/make_cascade_file/tests/test_filter_cascades.py
+-rw-r--r--   0        0        0      272 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/pyscenedetect/Dockerfile
+-rw-r--r--   0        0        0     5631 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/pyscenedetect/component.py
+-rw-r--r--   0        0        0     8128 2023-04-23 17:13:43.201737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/pyscenedetect/component.yaml
+-rw-r--r--   0        0        0  2709671 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/pyscenedetect/friends.mp4
+-rw-r--r--   0        0        0     4827 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/pyscenedetect/poetry.lock
+-rw-r--r--   0        0        0      389 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/pyscenedetect/pyproject.toml
+-rw-r--r--   0        0        0      159 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_data/Dockerfile
+-rw-r--r--   0        0        0      963 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_data/component.yaml
+-rw-r--r--   0        0        0    49727 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_data/poetry.lock
+-rw-r--r--   0        0        0      383 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_data/pyproject.toml
+-rw-r--r--   0        0        0     1393 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_data/src/query_db.py
+-rw-r--r--   0        0        0      159 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_string/Dockerfile
+-rw-r--r--   0        0        0      955 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_string/component.yaml
+-rw-r--r--   0        0        0    49727 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_string/poetry.lock
+-rw-r--r--   0        0        0      383 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_string/pyproject.toml
+-rw-r--r--   0        0        0     1756 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_string/src/query_db.py
+-rw-r--r--   0        0        0      318 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/Dockerfile
+-rw-r--r--   0        0        0      955 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/component.py
+-rw-r--r--   0        0        0     1967 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/component.yaml
+-rw-r--r--   0        0        0    73030 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/poetry.lock
+-rw-r--r--   0        0        0      422 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/pyproject.toml
+-rw-r--r--   0        0        0    78906 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-001.mp4
+-rw-r--r--   0        0        0    76382 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-002.mp4
+-rw-r--r--   0        0        0    92195 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-003.mp4
+-rw-r--r--   0        0        0      159 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_in_database/Dockerfile
+-rw-r--r--   0        0        0     4965 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_in_database/component.py
+-rw-r--r--   0        0        0     6840 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_in_database/component.yaml
+-rw-r--r--   0        0        0    20204 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_in_database/poetry.lock
+-rw-r--r--   0        0        0      525 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_in_database/pyproject.toml
+-rw-r--r--   0        0        0      194 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_to_frames/Dockerfile
+-rw-r--r--   0        0        0     5490 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_to_frames/component.py
+-rw-r--r--   0        0        0     7578 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_to_frames/component.yaml
+-rw-r--r--   0        0        0     1285 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_to_frames/poetry.lock
+-rw-r--r--   0        0        0      308 2023-04-23 17:13:43.217737 hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_to_frames/pyproject.toml
+-rw-r--r--   0        0        0      886 2023-04-23 17:13:43.221737 hoodat_vertex_components-1.6.6/pyproject.toml
+-rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 hoodat_vertex_components-1.6.6/PKG-INFO
```

### Comparing `hoodat_vertex_components-1.6.5/LICENSE.txt` & `hoodat_vertex_components-1.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/README.md` & `hoodat_vertex_components-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/__init__.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/__init__.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile_orig` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/Dockerfile_orig`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/component.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/component.yaml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/friends-Scene-008.mp4` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/friends-Scene-008.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/poetry.lock` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/pyproject.toml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_video/tools/demo_track.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_video/tools/demo_track.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/Dockerfile` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/Dockerfile`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/component.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/component.yaml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/component.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -89,24 +89,30 @@
 
           # List the videos in the input directory
           file_names = os.listdir(input_video_dir.path)
           file_paths = [
               os.path.join(input_video_dir.path, file_name) for file_name in file_names
           ]
           file_names_and_paths = list(zip(file_names, file_paths))
+          file_names_and_paths.sort()
           logger.info(f"Number of files to process: {len(file_names)}")
 
-          logger.info(f"output_video_dir.path: {output_video_dir.path}, output_video_dir.uri: {output_video_dir.uri}")
-          logger.info(f"output_text_file_dataset_dir.path: {output_text_file_dataset_dir.path}, output_text_file_dataset_dir.uri: {output_text_file_dataset_dir.uri}")
+          logger.info(
+              f"output_video_dir.path: {output_video_dir.path}, output_video_dir.uri: {output_video_dir.uri}"
+          )
+          logger.info(
+              f"output_text_file_dataset_dir.path: {output_text_file_dataset_dir.path}, output_text_file_dataset_dir.uri: {output_text_file_dataset_dir.uri}"
+          )
 
           ################################
           # Run bytetrack
           ################################
 
           video_processing_times = []
+          file_index = 0
           for file_name_and_path in file_names_and_paths:
               # Log start time
               start_time_this_video = time.time()
               logger.info(f"Processing {file_name_and_path[1]}")
               # Create arguments for bytetrack
               arg_list = [
                   "video",
@@ -135,26 +141,34 @@
                   output_video_dir.path, file_name_and_path[0]
               )
               logger.info(f"output_video_path_local: {output_video_path_local}")
               output_text_file_dataset_path_local = (
                   os.path.join(output_text_file_dataset_dir.path, file_name_and_path[0])
                   + ".csv"
               )
-              logger.info(f"output_text_file_dataset_path_local: {output_text_file_dataset_path_local}")
+              logger.info(
+                  f"output_text_file_dataset_path_local: {output_text_file_dataset_path_local}"
+              )
               shutil.copyfile(source_video, output_video_path_local)
               shutil.copyfile(source_results, output_text_file_dataset_path_local)
+              # Add video number to results file
+              df = pd.read_csv(output_text_file_dataset_path_local)
+              df["video_number"] = file_index
+              df.to_csv(output_text_file_dataset_path_local, index=None)
               # Log end time
               end_time_this_video = time.time()
               video_processing_time = timedelta(
                   seconds=(end_time_this_video - start_time_this_video)
               )
               video_processing_time = video_processing_time - timedelta(
                   microseconds=video_processing_time.microseconds
               )
               video_processing_times.append(str(video_processing_time))
+              logger.info(f"Processing time: {str(video_processing_time)}")
+              file_index += 1
 
           # Log all the video processing times
           logger.info(f"Video processing times: {video_processing_times}")
 
           # Log total time
           end_time = time.time()
           total_time = timedelta(seconds=(end_time - start_time))
```

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/friends-Scene-008.mp4` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/friends-Scene-008.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/poetry.lock` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/pyproject.toml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/bytetrack_from_videos/tools/demo_track.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/bytetrack_from_videos/tools/demo_track.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/haar_from_frames/component.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/haar_from_frames/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/haar_from_frames/component.yaml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/haar_from_frames/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/make_cascade_file/component.yaml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/make_cascade_file/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/make_cascade_file/make_cascade_file.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/make_cascade_file/make_cascade_file.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/make_cascade_file/poetry.lock` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/make_cascade_file/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/make_cascade_file/tests/test_filter_cascades.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/make_cascade_file/tests/test_filter_cascades.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/pyscenedetect/component.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/pyscenedetect/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/pyscenedetect/component.yaml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/pyscenedetect/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/pyscenedetect/friends.mp4` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/pyscenedetect/friends.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/pyscenedetect/poetry.lock` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/pyscenedetect/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_data/component.yaml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_data/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_data/poetry.lock` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_data/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_data/src/query_db.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_data/src/query_db.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_string/component.yaml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_string/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_string/poetry.lock` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_string/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/query_database_output_string/src/query_db.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/query_database_output_string/src/query_db.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/component.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/component.yaml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/poetry.lock` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-001.mp4` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-001.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-002.mp4` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-002.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-003.mp4` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/stitch_videos/sample/friends-Scene-003.mp4`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_in_database/component.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_in_database/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_in_database/component.yaml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_in_database/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_in_database/poetry.lock` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_in_database/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_in_database/pyproject.toml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_in_database/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_to_frames/component.py` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_to_frames/component.py`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_to_frames/component.yaml` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_to_frames/component.yaml`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/hoodat_vertex_components/components/video_to_frames/poetry.lock` & `hoodat_vertex_components-1.6.6/hoodat_vertex_components/components/video_to_frames/poetry.lock`

 * *Files identical despite different names*

### Comparing `hoodat_vertex_components-1.6.5/pyproject.toml` & `hoodat_vertex_components-1.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "hoodat-vertex-components"
-version = "1.6.5"
+version = "1.6.6"
 description = "Re-usable kfp components for hoodat"
 authors = ["Eugene Brown <efbbrown@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = [
     "LICENSE.txt",
 ]
 
 [tool.commitizen]
-version = "1.6.5"
+version = "1.6.6"
 version_files = [
     "pyproject.toml:version",
     "hoodat_vertex_components/__init__.py:__version__",
 ]
 tag_format = "v$major.$minor.$patch$prerelease"
 
 [tool.poetry.dependencies]
```

### Comparing `hoodat_vertex_components-1.6.5/PKG-INFO` & `hoodat_vertex_components-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoodat-vertex-components
-Version: 1.6.5
+Version: 1.6.6
 Summary: Re-usable kfp components for hoodat
 License: MIT
 Author: Eugene Brown
 Author-email: efbbrown@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

