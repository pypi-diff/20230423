# Comparing `tmp/sphere_base-0.1.5.tar.gz` & `tmp/sphere_base-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphere_base-0.1.5.tar", last modified: Sat Apr 22 14:33:24 2023, max compression
+gzip compressed data, was "sphere_base-0.1.6.tar", last modified: Sat Apr 22 14:49:00 2023, max compression
```

## Comparing `sphere_base-0.1.5.tar` & `sphere_base-0.1.6.tar`

### file list

```diff
@@ -1,168 +1,215 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.131435 sphere_base-0.1.5/
--rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.5/HISTORY.rst
--rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      252 2023-03-15 14:22:33.000000 sphere_base-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1987 2023-04-22 14:33:24.130435 sphere_base-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-04-21 08:51:12.000000 sphere_base-0.1.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:23.918423 sphere_base-0.1.5/docs/
--rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.5/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:23.894422 sphere_base-0.1.5/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:23.895422 sphere_base-0.1.5/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:23.922423 sphere_base-0.1.5/docs/build/html/_static/
--rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.5/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.5/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.5/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.5/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:23.924423 sphere_base-0.1.5/docs/source/
--rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.5/docs/source/conf.py
--rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.5/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.015428 sphere_base-0.1.5/docs/source/rst/
--rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.model.mesh.rst
--rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.model.model.rst
--rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.model.models.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.model.obj_file_loader.rst
--rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.model.rst
--rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.rst
--rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_base_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
--rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
--rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_default_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_node_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.shader.uv_square_shader.rst
--rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_overlay.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
--rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
--rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
--rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
--rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
--rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
--rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
--rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
--rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
--rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
--rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
--rw-rw-rw-   0        0        0      154 2023-04-22 14:15:57.000000 sphere_base-0.1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 14:33:24.131435 sphere_base-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1574 2023-04-22 14:33:20.000000 sphere_base-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.025429 sphere_base-0.1.5/sphere_base/
--rw-rw-rw-   0        0        0      106 2023-04-21 12:08:43.000000 sphere_base-0.1.5/sphere_base/__init__.py
--rw-rw-rw-   0        0        0     8512 2023-04-20 14:05:18.000000 sphere_base-0.1.5/sphere_base/calc.py
--rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.5/sphere_base/clipboard.py
--rw-rw-rw-   0        0        0     5131 2023-04-22 13:52:18.000000 sphere_base-0.1.5/sphere_base/config.py
--rw-rw-rw-   0        0        0     4839 2023-04-20 17:12:04.000000 sphere_base-0.1.5/sphere_base/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.054431 sphere_base-0.1.5/sphere_base/edge/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.5/sphere_base/edge/__init__.py
--rw-rw-rw-   0        0        0     7711 2023-04-20 09:15:29.000000 sphere_base-0.1.5/sphere_base/edge/edge_drag.py
--rw-rw-rw-   0        0        0     4592 2023-04-20 07:51:22.000000 sphere_base-0.1.5/sphere_base/edge/graphic_edge.py
--rw-rw-rw-   0        0        0      809 2023-04-19 12:36:22.000000 sphere_base-0.1.5/sphere_base/edge/graphic_line.py
--rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.5/sphere_base/edge/inter_sphere_edge.py
--rw-rw-rw-   0        0        0    14126 2023-04-22 13:09:36.000000 sphere_base-0.1.5/sphere_base/edge/surface_edge.py
--rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.5/sphere_base/history.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.061431 sphere_base-0.1.5/sphere_base/model/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.5/sphere_base/model/__init__.py
--rw-rw-rw-   0        0        0     4197 2023-04-20 17:16:58.000000 sphere_base-0.1.5/sphere_base/model/mesh.py
--rw-rw-rw-   0        0        0     6415 2023-04-22 13:52:18.000000 sphere_base-0.1.5/sphere_base/model/model.py
--rw-rw-rw-   0        0        0     3379 2023-04-22 13:55:17.000000 sphere_base-0.1.5/sphere_base/model/models.py
--rw-rw-rw-   0        0        0    23247 2023-04-22 13:52:18.000000 sphere_base-0.1.5/sphere_base/model/obj_file_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.063431 sphere_base-0.1.5/sphere_base/model/resources/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.5/sphere_base/model/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.064431 sphere_base-0.1.5/sphere_base/model/resources/meshes/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.5/sphere_base/model/resources/meshes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.066431 sphere_base-0.1.5/sphere_base/model/resources/shaders/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.5/sphere_base/model/resources/shaders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.073432 sphere_base-0.1.5/sphere_base/node/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.5/sphere_base/node/__init__.py
--rw-rw-rw-   0        0        0     8053 2023-04-22 13:09:36.000000 sphere_base-0.1.5/sphere_base/node/graphic_disc.py
--rw-rw-rw-   0        0        0     2676 2023-04-03 06:31:17.000000 sphere_base-0.1.5/sphere_base/node/graphic_node.py
--rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.5/sphere_base/node/graphic_socket.py
--rw-rw-rw-   0        0        0    13296 2023-04-22 13:09:36.000000 sphere_base-0.1.5/sphere_base/node/node.py
--rw-rw-rw-   0        0        0     8804 2023-04-22 13:09:36.000000 sphere_base-0.1.5/sphere_base/node/socket.py
--rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.5/sphere_base/serializable.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.094433 sphere_base-0.1.5/sphere_base/shader/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.5/sphere_base/shader/__init__.py
--rw-rw-rw-   0        0        0     9269 2023-04-22 11:12:03.000000 sphere_base-0.1.5/sphere_base/shader/base_shader.py
--rw-rw-rw-   0        0        0     1979 2023-04-20 17:16:57.000000 sphere_base-0.1.5/sphere_base/shader/circle_shader.py
--rw-rw-rw-   0        0        0     1969 2023-04-20 17:16:57.000000 sphere_base-0.1.5/sphere_base/shader/cross_shader.py
--rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.5/sphere_base/shader/default_shader.py
--rw-rw-rw-   0        0        0     2235 2023-04-20 09:28:14.000000 sphere_base-0.1.5/sphere_base/shader/drag_edge_shader.py
--rw-rw-rw-   0        0        0     1164 2023-04-20 17:31:03.000000 sphere_base-0.1.5/sphere_base/shader/edge_shader.py
--rw-rw-rw-   0        0        0      909 2023-04-20 17:16:58.000000 sphere_base-0.1.5/sphere_base/shader/flat_shader.py
--rw-rw-rw-   0        0        0     1467 2023-04-20 17:16:57.000000 sphere_base-0.1.5/sphere_base/shader/holo_sphere_shader.py
--rw-rw-rw-   0        0        0     1166 2023-04-20 17:16:57.000000 sphere_base-0.1.5/sphere_base/shader/node_shader.py
--rw-rw-rw-   0        0        0     2150 2023-04-20 17:12:04.000000 sphere_base-0.1.5/sphere_base/shader/skybox_shader.py
--rw-rw-rw-   0        0        0     1261 2023-04-20 17:16:58.000000 sphere_base-0.1.5/sphere_base/shader/socket_shader.py
--rw-rw-rw-   0        0        0     3117 2023-04-20 17:31:03.000000 sphere_base-0.1.5/sphere_base/shader/sphere_edge_shader.py
--rw-rw-rw-   0        0        0     1668 2023-04-20 17:16:58.000000 sphere_base-0.1.5/sphere_base/shader/sphere_shader.py
--rw-rw-rw-   0        0        0     1254 2023-04-20 17:16:58.000000 sphere_base-0.1.5/sphere_base/shader/sphere_small_shader.py
--rw-rw-rw-   0        0        0     1845 2023-04-20 17:16:58.000000 sphere_base-0.1.5/sphere_base/shader/square_shader.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.098433 sphere_base-0.1.5/sphere_base/sphere/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.5/sphere_base/sphere/__init__.py
--rw-rw-rw-   0        0        0    28884 2023-04-22 08:44:12.000000 sphere_base-0.1.5/sphere_base/sphere/sphere.py
--rw-rw-rw-   0        0        0     6068 2023-04-21 07:05:58.000000 sphere_base-0.1.5/sphere_base/sphere/sphere_lines.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.103433 sphere_base-0.1.5/sphere_base/sphere_overlay/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.5/sphere_base/sphere_overlay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.105434 sphere_base-0.1.5/sphere_base/sphere_overlay/icons/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.5/sphere_base/sphere_overlay/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.108434 sphere_base-0.1.5/sphere_base/sphere_overlay/qss/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.5/sphere_base/sphere_overlay/qss/__init__.py
--rw-rw-rw-   0        0        0    30464 2021-01-18 11:54:48.000000 sphere_base-0.1.5/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py
--rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.5/sphere_base/sphere_overlay/sov_conf.py
--rw-rw-rw-   0        0        0     2161 2023-04-20 13:43:23.000000 sphere_base-0.1.5/sphere_base/sphere_overlay/sov_sphere.py
--rw-rw-rw-   0        0        0     1605 2023-04-22 13:09:36.000000 sphere_base-0.1.5/sphere_base/sphere_overlay/sov_sphere_node_base.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.113434 sphere_base-0.1.5/sphere_base/sphere_overlay/sphere_nodes/
--rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.5/sphere_base/sphere_overlay/sphere_nodes/__init__.py
--rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.5/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
--rw-rw-rw-   0        0        0     1084 2023-04-13 12:16:43.000000 sphere_base-0.1.5/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
--rw-rw-rw-   0        0        0     1002 2023-04-13 12:14:08.000000 sphere_base-0.1.5/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.126435 sphere_base-0.1.5/sphere_base/sphere_universe_base/
--rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.5/sphere_base/sphere_universe_base/__init__.py
--rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_cam.py
--rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_cam_movement.py
--rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_graphic_item.py
--rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_mouse_ray.py
--rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_rubber_band.py
--rw-rw-rw-   0        0        0     5378 2023-04-22 11:55:42.000000 sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_skybox.py
--rw-rw-rw-   0        0        0    14150 2023-04-22 12:54:26.000000 sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_universe.py
--rw-rw-rw-   0        0        0    17954 2023-04-20 15:39:40.000000 sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_widget.py
--rw-rw-rw-   0        0        0     1493 2023-04-21 11:08:11.000000 sphere_base-0.1.5/sphere_base/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.045430 sphere_base-0.1.5/sphere_base.egg-info/
--rw-rw-rw-   0        0        0     1987 2023-04-22 14:33:23.000000 sphere_base-0.1.5/sphere_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6381 2023-04-22 14:33:23.000000 sphere_base-0.1.5/sphere_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 14:33:23.000000 sphere_base-0.1.5/sphere_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.5/sphere_base.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      145 2023-04-22 14:33:23.000000 sphere_base-0.1.5/sphere_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-22 14:33:23.000000 sphere_base-0.1.5/sphere_base.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-22 14:33:24.128435 sphere_base-0.1.5/tests/
--rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.5/tests/test_000_import.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:49:00.104970 sphere_base-0.1.6/
+-rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.6/HISTORY.rst
+-rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      358 2023-04-22 14:48:51.000000 sphere_base-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1987 2023-04-22 14:49:00.104970 sphere_base-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-04-21 08:51:12.000000 sphere_base-0.1.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.747949 sphere_base-0.1.6/docs/
+-rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.6/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.698947 sphere_base-0.1.6/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.699947 sphere_base-0.1.6/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.751950 sphere_base-0.1.6/docs/build/html/_static/
+-rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.6/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.6/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.6/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.6/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.754950 sphere_base-0.1.6/docs/source/
+-rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.6/docs/source/conf.py
+-rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.6/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.835955 sphere_base-0.1.6/docs/source/rst/
+-rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.model.mesh.rst
+-rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.model.model.rst
+-rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.model.models.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.model.obj_file_loader.rst
+-rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.model.rst
+-rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.rst
+-rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_base_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
+-rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
+-rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_default_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_node_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.shader.uv_square_shader.rst
+-rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_overlay.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
+-rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
+-rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
+-rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
+-rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
+-rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
+-rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
+-rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
+-rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
+-rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
+-rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
+-rw-rw-rw-   0        0        0      154 2023-04-22 14:15:57.000000 sphere_base-0.1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 14:49:00.105970 sphere_base-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1574 2023-04-22 14:42:55.000000 sphere_base-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.845955 sphere_base-0.1.6/sphere_base/
+-rw-rw-rw-   0        0        0      106 2023-04-21 12:08:43.000000 sphere_base-0.1.6/sphere_base/__init__.py
+-rw-rw-rw-   0        0        0     8512 2023-04-20 14:05:18.000000 sphere_base-0.1.6/sphere_base/calc.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.6/sphere_base/clipboard.py
+-rw-rw-rw-   0        0        0     5131 2023-04-22 13:52:18.000000 sphere_base-0.1.6/sphere_base/config.py
+-rw-rw-rw-   0        0        0     4839 2023-04-20 17:12:04.000000 sphere_base-0.1.6/sphere_base/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.872957 sphere_base-0.1.6/sphere_base/edge/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.6/sphere_base/edge/__init__.py
+-rw-rw-rw-   0        0        0     7711 2023-04-20 09:15:29.000000 sphere_base-0.1.6/sphere_base/edge/edge_drag.py
+-rw-rw-rw-   0        0        0     4592 2023-04-20 07:51:22.000000 sphere_base-0.1.6/sphere_base/edge/graphic_edge.py
+-rw-rw-rw-   0        0        0      809 2023-04-19 12:36:22.000000 sphere_base-0.1.6/sphere_base/edge/graphic_line.py
+-rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.6/sphere_base/edge/inter_sphere_edge.py
+-rw-rw-rw-   0        0        0    14126 2023-04-22 13:09:36.000000 sphere_base-0.1.6/sphere_base/edge/surface_edge.py
+-rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.6/sphere_base/history.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.878957 sphere_base-0.1.6/sphere_base/model/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.6/sphere_base/model/__init__.py
+-rw-rw-rw-   0        0        0     4197 2023-04-20 17:16:58.000000 sphere_base-0.1.6/sphere_base/model/mesh.py
+-rw-rw-rw-   0        0        0     6415 2023-04-22 13:52:18.000000 sphere_base-0.1.6/sphere_base/model/model.py
+-rw-rw-rw-   0        0        0     3379 2023-04-22 13:55:17.000000 sphere_base-0.1.6/sphere_base/model/models.py
+-rw-rw-rw-   0        0        0    23247 2023-04-22 13:52:18.000000 sphere_base-0.1.6/sphere_base/model/obj_file_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.880957 sphere_base-0.1.6/sphere_base/model/resources/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.6/sphere_base/model/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.931960 sphere_base-0.1.6/sphere_base/model/resources/meshes/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/crosshair.mtl
+-rw-rw-rw-   0        0        0     1720 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/crosshair.obj
+-rw-rw-rw-   0        0        0      339 2023-04-19 15:51:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/cubesphere.mtl
+-rw-rw-rw-   0        0        0  3258439 2023-04-20 06:45:02.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/cubesphere.obj
+-rw-rw-rw-   0        0        0      144 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/line_1x1.mtl
+-rw-rw-rw-   0        0        0      377 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/line_1x1.obj
+-rw-rw-rw-   0        0        0      319 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/node_disc1.mtl
+-rw-rw-rw-   0        0        0     4438 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/node_disc1.obj
+-rw-rw-rw-   0        0        0      241 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/skybox.mtl
+-rw-rw-rw-   0        0        0     1184 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/skybox.obj
+-rw-rw-rw-   0        0        0      327 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/sphere1.mtl
+-rw-rw-rw-   0        0        0   334766 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/sphere1.obj
+-rw-rw-rw-   0        0        0      148 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/sphere_small.mtl
+-rw-rw-rw-   0        0        0    61720 2023-03-06 12:34:58.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/sphere_small.obj
+-rw-rw-rw-   0        0        0      134 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/square1x1.mtl
+-rw-rw-rw-   0        0        0      362 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/square1x1.obj
+-rw-rw-rw-   0        0        0       49 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/vertex1.mtl
+-rw-rw-rw-   0        0        0      127 2023-03-13 10:54:30.000000 sphere_base-0.1.6/sphere_base/model/resources/meshes/vertex1.obj
+drwxrwxrwx   0        0        0        0 2023-04-22 14:49:00.023965 sphere_base-0.1.6/sphere_base/model/resources/shaders/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/__init__.py
+-rw-rw-rw-   0        0        0       99 2021-02-20 15:08:02.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_2d.glsl
+-rw-rw-rw-   0        0        0      103 2021-03-09 15:04:34.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_circle.glsl
+-rw-rw-rw-   0        0        0     3157 2021-02-20 08:36:12.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_default.glsl
+-rw-rw-rw-   0        0        0     2128 2021-08-09 11:38:22.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_holo.glsl
+-rw-rw-rw-   0        0        0      531 2021-08-10 08:30:00.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_holo_sphere.glsl
+-rw-rw-rw-   0        0        0      533 2021-08-18 14:31:52.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_node.glsl
+-rw-rw-rw-   0        0        0      147 2023-03-11 11:21:38.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_skybox.glsl
+-rw-rw-rw-   0        0        0      541 2021-08-17 08:34:24.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_socket.glsl
+-rw-rw-rw-   0        0        0     3162 2021-08-18 15:12:02.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_sphere.glsl
+-rw-rw-rw-   0        0        0       99 2023-04-14 14:44:46.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_sphere_edge.glsl
+-rw-rw-rw-   0        0        0      412 2021-08-20 07:35:34.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_sphere_small.glsl
+-rw-rw-rw-   0        0        0      243 2021-03-01 09:41:30.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/frag_square.glsl
+-rw-rw-rw-   0        0        0      693 2023-04-14 14:40:36.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/geom_circle.glsl
+-rw-rw-rw-   0        0        0     2451 2023-04-05 15:16:56.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/geom_cross.glsl
+-rw-rw-rw-   0        0        0     2961 2023-04-14 12:24:33.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/geom_edge.glsl
+-rw-rw-rw-   0        0        0      693 2023-04-14 14:39:33.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/geom_edge2.glsl
+-rw-rw-rw-   0        0        0      972 2021-03-08 11:27:56.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/geom_square.glsl
+-rw-rw-rw-   0        0        0      254 2021-03-01 09:26:34.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_2d.glsl
+-rw-rw-rw-   0        0        0      194 2021-03-09 14:50:48.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_circle.glsl
+-rw-rw-rw-   0        0        0     2776 2021-02-20 08:36:12.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_default.glsl
+-rw-rw-rw-   0        0        0     1384 2021-08-09 11:54:12.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_holo.glsl
+-rw-rw-rw-   0        0        0      524 2021-08-10 08:30:00.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_holo_sphere.glsl
+-rw-rw-rw-   0        0        0      528 2021-02-24 20:35:30.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_node.glsl
+-rw-rw-rw-   0        0        0      246 2023-03-11 11:21:44.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_skybox.glsl
+-rw-rw-rw-   0        0        0      524 2021-02-27 18:53:28.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_socket.glsl
+-rw-rw-rw-   0        0        0     2692 2021-08-09 14:04:40.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_sphere.glsl
+-rw-rw-rw-   0        0        0      524 2021-04-01 08:39:08.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_sphere_edge.glsl
+-rw-rw-rw-   0        0        0      522 2021-08-20 07:11:26.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_sphere_small.glsl
+-rw-rw-rw-   0        0        0      338 2021-03-01 10:55:38.000000 sphere_base-0.1.6/sphere_base/model/resources/shaders/vert_square.glsl
+drwxrwxrwx   0        0        0        0 2023-04-22 14:49:00.048967 sphere_base-0.1.6/sphere_base/node/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.6/sphere_base/node/__init__.py
+-rw-rw-rw-   0        0        0     8053 2023-04-22 13:09:36.000000 sphere_base-0.1.6/sphere_base/node/graphic_disc.py
+-rw-rw-rw-   0        0        0     2676 2023-04-03 06:31:17.000000 sphere_base-0.1.6/sphere_base/node/graphic_node.py
+-rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.6/sphere_base/node/graphic_socket.py
+-rw-rw-rw-   0        0        0    13296 2023-04-22 13:09:36.000000 sphere_base-0.1.6/sphere_base/node/node.py
+-rw-rw-rw-   0        0        0     8804 2023-04-22 13:09:36.000000 sphere_base-0.1.6/sphere_base/node/socket.py
+-rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.6/sphere_base/serializable.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:49:00.071968 sphere_base-0.1.6/sphere_base/shader/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.6/sphere_base/shader/__init__.py
+-rw-rw-rw-   0        0        0     9269 2023-04-22 11:12:03.000000 sphere_base-0.1.6/sphere_base/shader/base_shader.py
+-rw-rw-rw-   0        0        0     1979 2023-04-20 17:16:57.000000 sphere_base-0.1.6/sphere_base/shader/circle_shader.py
+-rw-rw-rw-   0        0        0     1969 2023-04-20 17:16:57.000000 sphere_base-0.1.6/sphere_base/shader/cross_shader.py
+-rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.6/sphere_base/shader/default_shader.py
+-rw-rw-rw-   0        0        0     2235 2023-04-20 09:28:14.000000 sphere_base-0.1.6/sphere_base/shader/drag_edge_shader.py
+-rw-rw-rw-   0        0        0     1164 2023-04-20 17:31:03.000000 sphere_base-0.1.6/sphere_base/shader/edge_shader.py
+-rw-rw-rw-   0        0        0      909 2023-04-20 17:16:58.000000 sphere_base-0.1.6/sphere_base/shader/flat_shader.py
+-rw-rw-rw-   0        0        0     1467 2023-04-20 17:16:57.000000 sphere_base-0.1.6/sphere_base/shader/holo_sphere_shader.py
+-rw-rw-rw-   0        0        0     1166 2023-04-20 17:16:57.000000 sphere_base-0.1.6/sphere_base/shader/node_shader.py
+-rw-rw-rw-   0        0        0     2150 2023-04-20 17:12:04.000000 sphere_base-0.1.6/sphere_base/shader/skybox_shader.py
+-rw-rw-rw-   0        0        0     1261 2023-04-20 17:16:58.000000 sphere_base-0.1.6/sphere_base/shader/socket_shader.py
+-rw-rw-rw-   0        0        0     3117 2023-04-20 17:31:03.000000 sphere_base-0.1.6/sphere_base/shader/sphere_edge_shader.py
+-rw-rw-rw-   0        0        0     1668 2023-04-20 17:16:58.000000 sphere_base-0.1.6/sphere_base/shader/sphere_shader.py
+-rw-rw-rw-   0        0        0     1254 2023-04-20 17:16:58.000000 sphere_base-0.1.6/sphere_base/shader/sphere_small_shader.py
+-rw-rw-rw-   0        0        0     1845 2023-04-20 17:16:58.000000 sphere_base-0.1.6/sphere_base/shader/square_shader.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:49:00.075968 sphere_base-0.1.6/sphere_base/sphere/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.6/sphere_base/sphere/__init__.py
+-rw-rw-rw-   0        0        0    28884 2023-04-22 08:44:12.000000 sphere_base-0.1.6/sphere_base/sphere/sphere.py
+-rw-rw-rw-   0        0        0     6068 2023-04-21 07:05:58.000000 sphere_base-0.1.6/sphere_base/sphere/sphere_lines.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:49:00.080968 sphere_base-0.1.6/sphere_base/sphere_overlay/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.6/sphere_base/sphere_overlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:49:00.081968 sphere_base-0.1.6/sphere_base/sphere_overlay/icons/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.6/sphere_base/sphere_overlay/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:49:00.084969 sphere_base-0.1.6/sphere_base/sphere_overlay/qss/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.6/sphere_base/sphere_overlay/qss/__init__.py
+-rw-rw-rw-   0        0        0    30464 2021-01-18 11:54:48.000000 sphere_base-0.1.6/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py
+-rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.6/sphere_base/sphere_overlay/sov_conf.py
+-rw-rw-rw-   0        0        0     2161 2023-04-20 13:43:23.000000 sphere_base-0.1.6/sphere_base/sphere_overlay/sov_sphere.py
+-rw-rw-rw-   0        0        0     1605 2023-04-22 13:09:36.000000 sphere_base-0.1.6/sphere_base/sphere_overlay/sov_sphere_node_base.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:49:00.090969 sphere_base-0.1.6/sphere_base/sphere_overlay/sphere_nodes/
+-rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.6/sphere_base/sphere_overlay/sphere_nodes/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.6/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
+-rw-rw-rw-   0        0        0     1084 2023-04-13 12:16:43.000000 sphere_base-0.1.6/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
+-rw-rw-rw-   0        0        0     1002 2023-04-13 12:14:08.000000 sphere_base-0.1.6/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:49:00.101970 sphere_base-0.1.6/sphere_base/sphere_universe_base/
+-rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.6/sphere_base/sphere_universe_base/__init__.py
+-rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_cam.py
+-rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_cam_movement.py
+-rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_graphic_item.py
+-rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_mouse_ray.py
+-rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_rubber_band.py
+-rw-rw-rw-   0        0        0     5378 2023-04-22 11:55:42.000000 sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_skybox.py
+-rw-rw-rw-   0        0        0    14150 2023-04-22 12:54:26.000000 sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_universe.py
+-rw-rw-rw-   0        0        0    17954 2023-04-20 15:39:40.000000 sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_widget.py
+-rw-rw-rw-   0        0        0     1493 2023-04-21 11:08:11.000000 sphere_base-0.1.6/sphere_base/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:48:59.864956 sphere_base-0.1.6/sphere_base.egg-info/
+-rw-rw-rw-   0        0        0     1987 2023-04-22 14:48:59.000000 sphere_base-0.1.6/sphere_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8808 2023-04-22 14:48:59.000000 sphere_base-0.1.6/sphere_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 14:48:59.000000 sphere_base-0.1.6/sphere_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.6/sphere_base.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      145 2023-04-22 14:48:59.000000 sphere_base-0.1.6/sphere_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-22 14:48:59.000000 sphere_base-0.1.6/sphere_base.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 14:49:00.102970 sphere_base-0.1.6/tests/
+-rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.6/tests/test_000_import.py
```

### Comparing `sphere_base-0.1.5/HISTORY.rst` & `sphere_base-0.1.6/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/LICENSE` & `sphere_base-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/PKG-INFO` & `sphere_base-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphere_base
-Version: 0.1.5
+Version: 0.1.6
 Summary: library for applications were information should appear on the surface of a sphere. It allows for creating spheres with nodes and edges that can be dragged on its surface. 
 Home-page: https://github.com/rboltze/spherebase
 Author: Richard Boltze
 Author-email: rboltze@protonmail.com
 License: MIT license
 Keywords: sphere_base
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sphere_base-0.1.5/README.rst` & `sphere_base-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/docs/Makefile` & `sphere_base-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/docs/make.bat` & `sphere_base-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/docs/source/conf.py` & `sphere_base-0.1.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/docs/source/rst/sphere_base.shader.rst` & `sphere_base-0.1.6/docs/source/rst/sphere_base.shader.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_overlay.rst` & `sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_overlay.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/docs/source/rst/sphere_base.sphere_universe_base.rst` & `sphere_base-0.1.6/docs/source/rst/sphere_base.sphere_universe_base.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/setup.py` & `sphere_base-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     keywords='sphere_base',
     name='sphere_base',
     packages=find_packages(include=['sphere_base*'], exclude=['examples*', 'test*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rboltze/spherebase',
-    version='0.1.5',
+    version='0.1.6',
     zip_safe=False,
 )
```

### Comparing `sphere_base-0.1.5/sphere_base/calc.py` & `sphere_base-0.1.6/sphere_base/calc.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/clipboard.py` & `sphere_base-0.1.6/sphere_base/clipboard.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/config.py` & `sphere_base-0.1.6/sphere_base/config.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/constants.py` & `sphere_base-0.1.6/sphere_base/constants.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/edge/edge_drag.py` & `sphere_base-0.1.6/sphere_base/edge/edge_drag.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/edge/graphic_edge.py` & `sphere_base-0.1.6/sphere_base/edge/graphic_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/edge/graphic_line.py` & `sphere_base-0.1.6/sphere_base/edge/graphic_line.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/edge/inter_sphere_edge.py` & `sphere_base-0.1.6/sphere_base/edge/inter_sphere_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/edge/surface_edge.py` & `sphere_base-0.1.6/sphere_base/edge/surface_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/history.py` & `sphere_base-0.1.6/sphere_base/history.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/model/mesh.py` & `sphere_base-0.1.6/sphere_base/model/mesh.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/model/model.py` & `sphere_base-0.1.6/sphere_base/model/model.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/model/models.py` & `sphere_base-0.1.6/sphere_base/model/models.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/model/obj_file_loader.py` & `sphere_base-0.1.6/sphere_base/model/obj_file_loader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/node/graphic_disc.py` & `sphere_base-0.1.6/sphere_base/node/graphic_disc.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/node/graphic_node.py` & `sphere_base-0.1.6/sphere_base/node/graphic_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/node/graphic_socket.py` & `sphere_base-0.1.6/sphere_base/node/graphic_socket.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/node/node.py` & `sphere_base-0.1.6/sphere_base/node/node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/node/socket.py` & `sphere_base-0.1.6/sphere_base/node/socket.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/serializable.py` & `sphere_base-0.1.6/sphere_base/serializable.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/base_shader.py` & `sphere_base-0.1.6/sphere_base/shader/base_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/circle_shader.py` & `sphere_base-0.1.6/sphere_base/shader/circle_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/cross_shader.py` & `sphere_base-0.1.6/sphere_base/shader/cross_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/default_shader.py` & `sphere_base-0.1.6/sphere_base/shader/default_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/drag_edge_shader.py` & `sphere_base-0.1.6/sphere_base/shader/drag_edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/edge_shader.py` & `sphere_base-0.1.6/sphere_base/shader/edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/flat_shader.py` & `sphere_base-0.1.6/sphere_base/shader/flat_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/holo_sphere_shader.py` & `sphere_base-0.1.6/sphere_base/shader/holo_sphere_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/node_shader.py` & `sphere_base-0.1.6/sphere_base/shader/node_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/skybox_shader.py` & `sphere_base-0.1.6/sphere_base/shader/skybox_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/socket_shader.py` & `sphere_base-0.1.6/sphere_base/shader/socket_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/sphere_edge_shader.py` & `sphere_base-0.1.6/sphere_base/shader/sphere_edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/sphere_shader.py` & `sphere_base-0.1.6/sphere_base/shader/sphere_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/sphere_small_shader.py` & `sphere_base-0.1.6/sphere_base/shader/sphere_small_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/shader/square_shader.py` & `sphere_base-0.1.6/sphere_base/shader/square_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere/sphere.py` & `sphere_base-0.1.6/sphere_base/sphere/sphere.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere/sphere_lines.py` & `sphere_base-0.1.6/sphere_base/sphere/sphere_lines.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py` & `sphere_base-0.1.6/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_overlay/sov_conf.py` & `sphere_base-0.1.6/sphere_base/sphere_overlay/sov_conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_overlay/sov_sphere.py` & `sphere_base-0.1.6/sphere_base/sphere_overlay/sov_sphere.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_overlay/sov_sphere_node_base.py` & `sphere_base-0.1.6/sphere_base/sphere_overlay/sov_sphere_node_base.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py` & `sphere_base-0.1.6/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py` & `sphere_base-0.1.6/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_cam.py` & `sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_cam.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_cam_movement.py` & `sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_cam_movement.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_mouse_ray.py` & `sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_mouse_ray.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_rubber_band.py` & `sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_rubber_band.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_skybox.py` & `sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_skybox.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_universe.py` & `sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_universe.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/sphere_universe_base/suv_widget.py` & `sphere_base-0.1.6/sphere_base/sphere_universe_base/suv_widget.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base/utils.py` & `sphere_base-0.1.6/sphere_base/utils.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.5/sphere_base.egg-info/PKG-INFO` & `sphere_base-0.1.6/sphere_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphere-base
-Version: 0.1.5
+Version: 0.1.6
 Summary: library for applications were information should appear on the surface of a sphere. It allows for creating spheres with nodes and edges that can be dragged on its surface. 
 Home-page: https://github.com/rboltze/spherebase
 Author: Richard Boltze
 Author-email: rboltze@protonmail.com
 License: MIT license
 Keywords: sphere_base
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sphere_base-0.1.5/sphere_base.egg-info/SOURCES.txt` & `sphere_base-0.1.6/sphere_base.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -90,15 +90,62 @@
 sphere_base/model/__init__.py
 sphere_base/model/mesh.py
 sphere_base/model/model.py
 sphere_base/model/models.py
 sphere_base/model/obj_file_loader.py
 sphere_base/model/resources/__init__.py
 sphere_base/model/resources/meshes/__init__.py
+sphere_base/model/resources/meshes/crosshair.mtl
+sphere_base/model/resources/meshes/crosshair.obj
+sphere_base/model/resources/meshes/cubesphere.mtl
+sphere_base/model/resources/meshes/cubesphere.obj
+sphere_base/model/resources/meshes/line_1x1.mtl
+sphere_base/model/resources/meshes/line_1x1.obj
+sphere_base/model/resources/meshes/node_disc1.mtl
+sphere_base/model/resources/meshes/node_disc1.obj
+sphere_base/model/resources/meshes/skybox.mtl
+sphere_base/model/resources/meshes/skybox.obj
+sphere_base/model/resources/meshes/sphere1.mtl
+sphere_base/model/resources/meshes/sphere1.obj
+sphere_base/model/resources/meshes/sphere_small.mtl
+sphere_base/model/resources/meshes/sphere_small.obj
+sphere_base/model/resources/meshes/square1x1.mtl
+sphere_base/model/resources/meshes/square1x1.obj
+sphere_base/model/resources/meshes/vertex1.mtl
+sphere_base/model/resources/meshes/vertex1.obj
 sphere_base/model/resources/shaders/__init__.py
+sphere_base/model/resources/shaders/frag_2d.glsl
+sphere_base/model/resources/shaders/frag_circle.glsl
+sphere_base/model/resources/shaders/frag_default.glsl
+sphere_base/model/resources/shaders/frag_holo.glsl
+sphere_base/model/resources/shaders/frag_holo_sphere.glsl
+sphere_base/model/resources/shaders/frag_node.glsl
+sphere_base/model/resources/shaders/frag_skybox.glsl
+sphere_base/model/resources/shaders/frag_socket.glsl
+sphere_base/model/resources/shaders/frag_sphere.glsl
+sphere_base/model/resources/shaders/frag_sphere_edge.glsl
+sphere_base/model/resources/shaders/frag_sphere_small.glsl
+sphere_base/model/resources/shaders/frag_square.glsl
+sphere_base/model/resources/shaders/geom_circle.glsl
+sphere_base/model/resources/shaders/geom_cross.glsl
+sphere_base/model/resources/shaders/geom_edge.glsl
+sphere_base/model/resources/shaders/geom_edge2.glsl
+sphere_base/model/resources/shaders/geom_square.glsl
+sphere_base/model/resources/shaders/vert_2d.glsl
+sphere_base/model/resources/shaders/vert_circle.glsl
+sphere_base/model/resources/shaders/vert_default.glsl
+sphere_base/model/resources/shaders/vert_holo.glsl
+sphere_base/model/resources/shaders/vert_holo_sphere.glsl
+sphere_base/model/resources/shaders/vert_node.glsl
+sphere_base/model/resources/shaders/vert_skybox.glsl
+sphere_base/model/resources/shaders/vert_socket.glsl
+sphere_base/model/resources/shaders/vert_sphere.glsl
+sphere_base/model/resources/shaders/vert_sphere_edge.glsl
+sphere_base/model/resources/shaders/vert_sphere_small.glsl
+sphere_base/model/resources/shaders/vert_square.glsl
 sphere_base/node/__init__.py
 sphere_base/node/graphic_disc.py
 sphere_base/node/graphic_node.py
 sphere_base/node/graphic_socket.py
 sphere_base/node/node.py
 sphere_base/node/socket.py
 sphere_base/shader/__init__.py
```

### Comparing `sphere_base-0.1.5/tests/test_000_import.py` & `sphere_base-0.1.6/tests/test_000_import.py`

 * *Files identical despite different names*

