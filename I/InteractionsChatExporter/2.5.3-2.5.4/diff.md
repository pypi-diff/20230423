# Comparing `tmp/InteractionsChatExporter-2.5.3.tar.gz` & `tmp/InteractionsChatExporter-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InteractionsChatExporter-2.5.3.tar", last modified: Sat Apr 22 22:14:18 2023, max compression
+gzip compressed data, was "InteractionsChatExporter-2.5.4.tar", last modified: Sat Apr 22 23:42:55 2023, max compression
```

## Comparing `InteractionsChatExporter-2.5.3.tar` & `InteractionsChatExporter-2.5.4.tar`

### file list

```diff
@@ -1,82 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.176448 InteractionsChatExporter-2.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.164447 InteractionsChatExporter-2.5.3/InteractionsChatExporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-04-22 22:14:18.000000 InteractionsChatExporter-2.5.3/InteractionsChatExporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-22 22:14:18.000000 InteractionsChatExporter-2.5.3/InteractionsChatExporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 22:14:18.000000 InteractionsChatExporter-2.5.3/InteractionsChatExporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-22 22:14:18.000000 InteractionsChatExporter-2.5.3/InteractionsChatExporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 22:14:18.000000 InteractionsChatExporter-2.5.3/InteractionsChatExporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-04-22 22:14:18.176448 InteractionsChatExporter-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.164447 InteractionsChatExporter-2.5.3/chat_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/chat_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.164447 InteractionsChatExporter-2.5.3/chat_exporter/construct/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/construct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.164447 InteractionsChatExporter-2.5.3/chat_exporter/construct/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/construct/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/construct/assets/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/construct/assets/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/construct/assets/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/construct/assets/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/construct/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/construct/transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.164447 InteractionsChatExporter-2.5.3/chat_exporter/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/ext/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/ext/discord_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/ext/discord_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/ext/emoji_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/ext/html_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.164447 InteractionsChatExporter-2.5.3/chat_exporter/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.168448 InteractionsChatExporter-2.5.3/chat_exporter/html/attachment/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/attachment/audio.html
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/attachment/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/attachment/message.html
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/attachment/video.html
--rw-r--r--   0 runner    (1001) docker     (123)    42106 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.168448 InteractionsChatExporter-2.5.3/chat_exporter/html/component/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/component/component_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/component/component_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/component/component_menu_options.html
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/component/component_menu_options_emoji.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.172448 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/author.html
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/author_icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/body.html
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/description.html
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/field-inline.html
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/field.html
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/footer_image.html
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/thumbnail.html
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/embed/title.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.172448 InteractionsChatExporter-2.5.3/chat_exporter/html/message/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/bot-tag-verified.html
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/bot-tag.html
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/content.html
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/end.html
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/interaction.html
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/message.html
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/meta.html
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/pin.html
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/reference.html
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/reference_unknown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/start.html
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/message/thread.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.172448 InteractionsChatExporter-2.5.3/chat_exporter/html/reaction/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/reaction/custom_emoji.html
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/reaction/emoji.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.172448 InteractionsChatExporter-2.5.3/chat_exporter/html/script/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/script/channel_subject.html
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/script/channel_topic.html
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/html/script/fancy_time.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:18.176448 InteractionsChatExporter-2.5.3/chat_exporter/parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/parse/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/chat_exporter/parse/mention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-22 22:14:05.000000 InteractionsChatExporter-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 22:14:18.176448 InteractionsChatExporter-2.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.941440 InteractionsChatExporter-2.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.921440 InteractionsChatExporter-2.5.4/InteractionsChatExporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-22 23:42:55.000000 InteractionsChatExporter-2.5.4/InteractionsChatExporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-22 23:42:55.000000 InteractionsChatExporter-2.5.4/InteractionsChatExporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 23:42:55.000000 InteractionsChatExporter-2.5.4/InteractionsChatExporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-22 23:42:55.000000 InteractionsChatExporter-2.5.4/InteractionsChatExporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 23:42:55.000000 InteractionsChatExporter-2.5.4/InteractionsChatExporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-22 23:42:55.941440 InteractionsChatExporter-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.921440 InteractionsChatExporter-2.5.4/chat_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/chat_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.925440 InteractionsChatExporter-2.5.4/chat_exporter/construct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/construct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.925440 InteractionsChatExporter-2.5.4/chat_exporter/construct/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/construct/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/construct/assets/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/construct/assets/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/construct/assets/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/construct/assets/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/construct/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/construct/transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.929440 InteractionsChatExporter-2.5.4/chat_exporter/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/ext/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/ext/discord_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/ext/emoji_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/ext/html_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.929440 InteractionsChatExporter-2.5.4/chat_exporter/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.929440 InteractionsChatExporter-2.5.4/chat_exporter/html/attachment/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/attachment/audio.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/attachment/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/attachment/message.html
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/attachment/video.html
+-rw-r--r--   0 runner    (1001) docker     (123)    42106 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.929440 InteractionsChatExporter-2.5.4/chat_exporter/html/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/component/component_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/component/component_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/component/component_menu_options.html
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/component/component_menu_options_emoji.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.933440 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/author.html
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/author_icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/body.html
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/description.html
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/field-inline.html
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/footer_image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/thumbnail.html
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/embed/title.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.937440 InteractionsChatExporter-2.5.4/chat_exporter/html/message/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/bot-tag-verified.html
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/bot-tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/end.html
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/interaction.html
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/message.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/meta.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/pin.html
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/reference.html
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/reference_unknown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/start.html
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/message/thread.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.941440 InteractionsChatExporter-2.5.4/chat_exporter/html/reaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/reaction/custom_emoji.html
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/reaction/emoji.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.941440 InteractionsChatExporter-2.5.4/chat_exporter/html/script/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/script/channel_subject.html
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/script/channel_topic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/html/script/fancy_time.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:55.941440 InteractionsChatExporter-2.5.4/chat_exporter/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/parse/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/chat_exporter/parse/mention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-22 23:42:41.000000 InteractionsChatExporter-2.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 23:42:55.941440 InteractionsChatExporter-2.5.4/setup.cfg
```

### Comparing `InteractionsChatExporter-2.5.3/InteractionsChatExporter.egg-info/PKG-INFO` & `InteractionsChatExporter-2.5.4/InteractionsChatExporter.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InteractionsChatExporter
-Version: 2.5.3
+Version: 2.5.4
 Summary: A simple Discord chat exporter for Interactions.py Discord bots.
 Author-email: mahtoid <info@mahto.id>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/DylZZZ/InteractionsChatExporter
 Project-URL: Discord, https://discord.gg/2uhHBQDwcc
 Project-URL: Donate, https://ko-fi.com/mahtoid
 Keywords: chat exporter,discord chat exporter,discord,discordpy,disnake,pycord,nextcord
@@ -25,54 +25,41 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
-[![Version][pypi-version]][pypi-url]
-[![Language][language-dom]][github-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![GPL License][license-shield]][license-url]
-
-
-  <h2>DiscordChatExporterPy</h2>
+  <h2>InteractionsChatExporter</h2>
 
   <p>
-    Export Discord chats with your discord.py (or fork) bots!
+    Export Discord chats with your interactions.py bots!
     <br />
-    <a href="https://discord.gg/2uhHBQDwcc">Join Discord</a>
-    ·
-    <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=bug&template=bug-report.yml">Report Bug</a>
-    ·
-    <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=enhancement&template=feature-request.yml">Request Feature</a>
   </p>
 </div>
 
 ---
 ## Installation
 
 To install the library to your virtual environment, for bot usage, run the command:
 ```sh 
-pip install chat-exporter
+pip install InteractionsChatExporter
 ```
 
 To clone the repository locally, run the command:
 ```sh
-git clone https://github.com/mahtoid/DiscordChatExporterPy
+git clone https://github.com/DylZZZ/InteractionsChatExporter
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ---
 ## Usage
 
-There are currently 3 methods (functions) to `chat-exporter` which you can use to export your chat.<br/>
+There are currently 3 methods (functions) to `InteractionsChatExporter` which you can use to export your chat.<br/>
 _Expand the blocks below to learn the functions, arguments and usages._
 <details><summary><b>Basic Usage</b></summary>
 
 `.quick_export()` is the simplest way of using chat-exporter.
 
 Using the _quick_export_ function will gather the history of the channel you give, build the transcript then post the file and embed directly to the channel - returning a message object gathered from the message it posted.
 
@@ -299,24 +286,12 @@
 It simply makes a request to the given URL and echos (prints) the content for you to be able to view it._
 
 </details>
 
 ---
 ## Attributions
 
+*This is a fork of [DiscordChatExporterPy](https://github.com/mahtoid/DiscordChatExporterPy) full credits go to him.*
 *This project borrows CSS and HTML code from [Tyrrrz's C# DiscordChatExporter](https://github.com/Tyrrrz/DiscordChatExporter/) repository.*
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-<!-- LINK DUMP -->
-[pypi-version]: https://img.shields.io/pypi/v/chat-exporter?style=for-the-badge
-[pypi-url]: https://pypi.org/project/chat-exporter/
-[language-dom]: https://img.shields.io/github/languages/top/mahtoid/discordchatexporterpy?style=for-the-badge
-[forks-shield]: https://img.shields.io/github/forks/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[forks-url]: https://github.com/mahtoid/DiscordChatExporterPy/
-[stars-shield]: https://img.shields.io/github/stars/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[stars-url]: https://github.com/mahtoid/DiscordChatExporterPy/stargazers
-[issues-shield]: https://img.shields.io/github/issues/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[issues-url]: https://github.com/mahtoid/DiscordChatExporterPy/issues
-[license-shield]: https://img.shields.io/github/license/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[license-url]: https://github.com/mahtoid/DiscordChatExporterPy/blob/master/LICENSE
-[github-url]: https://github.com/mahtoid/DiscordChatExporterPy/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: InteractionsChatExporter Version: 2.5.3 Summary: A
+Metadata-Version: 2.1 Name: InteractionsChatExporter Version: 2.5.4 Summary: A
 simple Discord chat exporter for Interactions.py Discord bots. Author-email:
 mahtoid
 mahto.id> License: GPL-3.0-only Project-URL: Homepage, https://github.com/
 DylZZZ/InteractionsChatExporter Project-URL: Discord, https://discord.gg/
 2uhHBQDwcc Project-URL: Donate, https://ko-fi.com/mahtoid Keywords: chat
 exporter,discord chat exporter,discord,discordpy,disnake,pycord,nextcord
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
@@ -12,28 +12,23 @@
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Topic :: Internet Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Topic :: Utilities Classifier: Typing
 :: Typed Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
-[![Version][pypi-version]][pypi-url] [![Language][language-dom]][github-url] [!
- [Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
-[Issues][issues-shield]][issues-url] [![GPL License][license-shield]][license-
-                                     url]
-                       ***** DiscordChatExporterPy *****
-          Export Discord chats with your discord.py (or fork) bots!
-                 Join_Discord Â· Report_Bug Â· Request_Feature
+                     ***** InteractionsChatExporter *****
+             Export Discord chats with your interactions.py bots!
 --- ## Installation To install the library to your virtual environment, for bot
-usage, run the command: ```sh pip install chat-exporter ``` To clone the
-repository locally, run the command: ```sh git clone https://github.com/
-mahtoid/DiscordChatExporterPy ```
+usage, run the command: ```sh pip install InteractionsChatExporter ``` To clone
+the repository locally, run the command: ```sh git clone https://github.com/
+DylZZZ/InteractionsChatExporter ```
                                                                   (back_to_top)
---- ## Usage There are currently 3 methods (functions) to `chat-exporter` which
-you can use to export your chat.
+--- ## Usage There are currently 3 methods (functions) to
+`InteractionsChatExporter` which you can use to export your chat.
 _Expand the blocks below to learn the functions, arguments and usages._ Basic
 Usage `.quick_export()` is the simplest way of using chat-exporter. Using the
 _quick_export_ function will gather the history of the channel you give, build
 the transcript then post the file and embed directly to the channel - returning
 a message object gathered from the message it posted. This is mostly seen as a
 demo function, as opposed to a command you should actually use. **Required
 Argument(s):**
@@ -134,25 +129,13 @@
       (ctx.channel) if transcript is None: return transcript_file =
       discord.File( io.BytesIO(transcript.encode()), filename=f"transcript-
       {ctx.channel.name}.html", ) message = await ctx.send
       (file=transcript_file) link = await chat_exporter.link(message) await
       ctx.send("Click this link to view the transcript online: " + link) ```
 _Please note that the PHP script does NOT store any information.
 It simply makes a request to the given URL and echos (prints) the content for
-you to be able to view it._  --- ## Attributions *This project borrows CSS and
-HTML code from [Tyrrrz's C# DiscordChatExporter](https://github.com/Tyrrrz/
-DiscordChatExporter/) repository.*
+you to be able to view it._  --- ## Attributions *This is a fork of
+[DiscordChatExporterPy](https://github.com/mahtoid/DiscordChatExporterPy) full
+credits go to him.* *This project borrows CSS and HTML code from [Tyrrrz's C#
+DiscordChatExporter](https://github.com/Tyrrrz/DiscordChatExporter/
+) repository.*
                                                                   (back_to_top)
- [pypi-version]: https://img.shields.io/pypi/v/chat-exporter?style=for-the-
-badge [pypi-url]: https://pypi.org/project/chat-exporter/ [language-dom]:
-https://img.shields.io/github/languages/top/mahtoid/
-discordchatexporterpy?style=for-the-badge [forks-shield]: https://
-img.shields.io/github/forks/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[forks-url]: https://github.com/mahtoid/DiscordChatExporterPy/ [stars-shield]:
-https://img.shields.io/github/stars/mahtoid/DiscordChatExporterPy?style=for-
-the-badge [stars-url]: https://github.com/mahtoid/DiscordChatExporterPy/
-stargazers [issues-shield]: https://img.shields.io/github/issues/mahtoid/
-DiscordChatExporterPy?style=for-the-badge [issues-url]: https://github.com/
-mahtoid/DiscordChatExporterPy/issues [license-shield]: https://img.shields.io/
-github/license/mahtoid/DiscordChatExporterPy?style=for-the-badge [license-url]:
-https://github.com/mahtoid/DiscordChatExporterPy/blob/master/LICENSE [github-
-url]: https://github.com/mahtoid/DiscordChatExporterPy/
```

### Comparing `InteractionsChatExporter-2.5.3/InteractionsChatExporter.egg-info/SOURCES.txt` & `InteractionsChatExporter-2.5.4/InteractionsChatExporter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 chat_exporter/construct/assets/__init__.py
 chat_exporter/construct/assets/attachment.py
 chat_exporter/construct/assets/component.py
 chat_exporter/construct/assets/embed.py
 chat_exporter/construct/assets/reaction.py
 chat_exporter/ext/__init__.py
 chat_exporter/ext/cache.py
-chat_exporter/ext/discord_import.py
 chat_exporter/ext/discord_utils.py
 chat_exporter/ext/emoji_convert.py
 chat_exporter/ext/html_generator.py
 chat_exporter/html/__init__.py
 chat_exporter/html/base.html
 chat_exporter/html/attachment/audio.html
 chat_exporter/html/attachment/image.html
```

### Comparing `InteractionsChatExporter-2.5.3/LICENSE` & `InteractionsChatExporter-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/PKG-INFO` & `InteractionsChatExporter-2.5.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InteractionsChatExporter
-Version: 2.5.3
+Version: 2.5.4
 Summary: A simple Discord chat exporter for Interactions.py Discord bots.
 Author-email: mahtoid <info@mahto.id>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/DylZZZ/InteractionsChatExporter
 Project-URL: Discord, https://discord.gg/2uhHBQDwcc
 Project-URL: Donate, https://ko-fi.com/mahtoid
 Keywords: chat exporter,discord chat exporter,discord,discordpy,disnake,pycord,nextcord
@@ -25,54 +25,41 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
-[![Version][pypi-version]][pypi-url]
-[![Language][language-dom]][github-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![GPL License][license-shield]][license-url]
-
-
-  <h2>DiscordChatExporterPy</h2>
+  <h2>InteractionsChatExporter</h2>
 
   <p>
-    Export Discord chats with your discord.py (or fork) bots!
+    Export Discord chats with your interactions.py bots!
     <br />
-    <a href="https://discord.gg/2uhHBQDwcc">Join Discord</a>
-    ·
-    <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=bug&template=bug-report.yml">Report Bug</a>
-    ·
-    <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=enhancement&template=feature-request.yml">Request Feature</a>
   </p>
 </div>
 
 ---
 ## Installation
 
 To install the library to your virtual environment, for bot usage, run the command:
 ```sh 
-pip install chat-exporter
+pip install InteractionsChatExporter
 ```
 
 To clone the repository locally, run the command:
 ```sh
-git clone https://github.com/mahtoid/DiscordChatExporterPy
+git clone https://github.com/DylZZZ/InteractionsChatExporter
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ---
 ## Usage
 
-There are currently 3 methods (functions) to `chat-exporter` which you can use to export your chat.<br/>
+There are currently 3 methods (functions) to `InteractionsChatExporter` which you can use to export your chat.<br/>
 _Expand the blocks below to learn the functions, arguments and usages._
 <details><summary><b>Basic Usage</b></summary>
 
 `.quick_export()` is the simplest way of using chat-exporter.
 
 Using the _quick_export_ function will gather the history of the channel you give, build the transcript then post the file and embed directly to the channel - returning a message object gathered from the message it posted.
 
@@ -299,24 +286,12 @@
 It simply makes a request to the given URL and echos (prints) the content for you to be able to view it._
 
 </details>
 
 ---
 ## Attributions
 
+*This is a fork of [DiscordChatExporterPy](https://github.com/mahtoid/DiscordChatExporterPy) full credits go to him.*
 *This project borrows CSS and HTML code from [Tyrrrz's C# DiscordChatExporter](https://github.com/Tyrrrz/DiscordChatExporter/) repository.*
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-<!-- LINK DUMP -->
-[pypi-version]: https://img.shields.io/pypi/v/chat-exporter?style=for-the-badge
-[pypi-url]: https://pypi.org/project/chat-exporter/
-[language-dom]: https://img.shields.io/github/languages/top/mahtoid/discordchatexporterpy?style=for-the-badge
-[forks-shield]: https://img.shields.io/github/forks/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[forks-url]: https://github.com/mahtoid/DiscordChatExporterPy/
-[stars-shield]: https://img.shields.io/github/stars/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[stars-url]: https://github.com/mahtoid/DiscordChatExporterPy/stargazers
-[issues-shield]: https://img.shields.io/github/issues/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[issues-url]: https://github.com/mahtoid/DiscordChatExporterPy/issues
-[license-shield]: https://img.shields.io/github/license/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[license-url]: https://github.com/mahtoid/DiscordChatExporterPy/blob/master/LICENSE
-[github-url]: https://github.com/mahtoid/DiscordChatExporterPy/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: InteractionsChatExporter Version: 2.5.3 Summary: A
+Metadata-Version: 2.1 Name: InteractionsChatExporter Version: 2.5.4 Summary: A
 simple Discord chat exporter for Interactions.py Discord bots. Author-email:
 mahtoid
 mahto.id> License: GPL-3.0-only Project-URL: Homepage, https://github.com/
 DylZZZ/InteractionsChatExporter Project-URL: Discord, https://discord.gg/
 2uhHBQDwcc Project-URL: Donate, https://ko-fi.com/mahtoid Keywords: chat
 exporter,discord chat exporter,discord,discordpy,disnake,pycord,nextcord
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
@@ -12,28 +12,23 @@
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Topic :: Internet Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Topic :: Utilities Classifier: Typing
 :: Typed Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE
-[![Version][pypi-version]][pypi-url] [![Language][language-dom]][github-url] [!
- [Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
-[Issues][issues-shield]][issues-url] [![GPL License][license-shield]][license-
-                                     url]
-                       ***** DiscordChatExporterPy *****
-          Export Discord chats with your discord.py (or fork) bots!
-                 Join_Discord Â· Report_Bug Â· Request_Feature
+                     ***** InteractionsChatExporter *****
+             Export Discord chats with your interactions.py bots!
 --- ## Installation To install the library to your virtual environment, for bot
-usage, run the command: ```sh pip install chat-exporter ``` To clone the
-repository locally, run the command: ```sh git clone https://github.com/
-mahtoid/DiscordChatExporterPy ```
+usage, run the command: ```sh pip install InteractionsChatExporter ``` To clone
+the repository locally, run the command: ```sh git clone https://github.com/
+DylZZZ/InteractionsChatExporter ```
                                                                   (back_to_top)
---- ## Usage There are currently 3 methods (functions) to `chat-exporter` which
-you can use to export your chat.
+--- ## Usage There are currently 3 methods (functions) to
+`InteractionsChatExporter` which you can use to export your chat.
 _Expand the blocks below to learn the functions, arguments and usages._ Basic
 Usage `.quick_export()` is the simplest way of using chat-exporter. Using the
 _quick_export_ function will gather the history of the channel you give, build
 the transcript then post the file and embed directly to the channel - returning
 a message object gathered from the message it posted. This is mostly seen as a
 demo function, as opposed to a command you should actually use. **Required
 Argument(s):**
@@ -134,25 +129,13 @@
       (ctx.channel) if transcript is None: return transcript_file =
       discord.File( io.BytesIO(transcript.encode()), filename=f"transcript-
       {ctx.channel.name}.html", ) message = await ctx.send
       (file=transcript_file) link = await chat_exporter.link(message) await
       ctx.send("Click this link to view the transcript online: " + link) ```
 _Please note that the PHP script does NOT store any information.
 It simply makes a request to the given URL and echos (prints) the content for
-you to be able to view it._  --- ## Attributions *This project borrows CSS and
-HTML code from [Tyrrrz's C# DiscordChatExporter](https://github.com/Tyrrrz/
-DiscordChatExporter/) repository.*
+you to be able to view it._  --- ## Attributions *This is a fork of
+[DiscordChatExporterPy](https://github.com/mahtoid/DiscordChatExporterPy) full
+credits go to him.* *This project borrows CSS and HTML code from [Tyrrrz's C#
+DiscordChatExporter](https://github.com/Tyrrrz/DiscordChatExporter/
+) repository.*
                                                                   (back_to_top)
- [pypi-version]: https://img.shields.io/pypi/v/chat-exporter?style=for-the-
-badge [pypi-url]: https://pypi.org/project/chat-exporter/ [language-dom]:
-https://img.shields.io/github/languages/top/mahtoid/
-discordchatexporterpy?style=for-the-badge [forks-shield]: https://
-img.shields.io/github/forks/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[forks-url]: https://github.com/mahtoid/DiscordChatExporterPy/ [stars-shield]:
-https://img.shields.io/github/stars/mahtoid/DiscordChatExporterPy?style=for-
-the-badge [stars-url]: https://github.com/mahtoid/DiscordChatExporterPy/
-stargazers [issues-shield]: https://img.shields.io/github/issues/mahtoid/
-DiscordChatExporterPy?style=for-the-badge [issues-url]: https://github.com/
-mahtoid/DiscordChatExporterPy/issues [license-shield]: https://img.shields.io/
-github/license/mahtoid/DiscordChatExporterPy?style=for-the-badge [license-url]:
-https://github.com/mahtoid/DiscordChatExporterPy/blob/master/LICENSE [github-
-url]: https://github.com/mahtoid/DiscordChatExporterPy/
```

### Comparing `InteractionsChatExporter-2.5.3/README.md` & `InteractionsChatExporter-2.5.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,36 @@
 <div align="center">
 
-[![Version][pypi-version]][pypi-url]
-[![Language][language-dom]][github-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![GPL License][license-shield]][license-url]
-
-
-  <h2>DiscordChatExporterPy</h2>
+  <h2>InteractionsChatExporter</h2>
 
   <p>
-    Export Discord chats with your discord.py (or fork) bots!
+    Export Discord chats with your interactions.py bots!
     <br />
-    <a href="https://discord.gg/2uhHBQDwcc">Join Discord</a>
-    ·
-    <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=bug&template=bug-report.yml">Report Bug</a>
-    ·
-    <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=enhancement&template=feature-request.yml">Request Feature</a>
   </p>
 </div>
 
 ---
 ## Installation
 
 To install the library to your virtual environment, for bot usage, run the command:
 ```sh 
-pip install chat-exporter
+pip install InteractionsChatExporter
 ```
 
 To clone the repository locally, run the command:
 ```sh
-git clone https://github.com/mahtoid/DiscordChatExporterPy
+git clone https://github.com/DylZZZ/InteractionsChatExporter
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ---
 ## Usage
 
-There are currently 3 methods (functions) to `chat-exporter` which you can use to export your chat.<br/>
+There are currently 3 methods (functions) to `InteractionsChatExporter` which you can use to export your chat.<br/>
 _Expand the blocks below to learn the functions, arguments and usages._
 <details><summary><b>Basic Usage</b></summary>
 
 `.quick_export()` is the simplest way of using chat-exporter.
 
 Using the _quick_export_ function will gather the history of the channel you give, build the transcript then post the file and embed directly to the channel - returning a message object gathered from the message it posted.
 
@@ -270,24 +257,12 @@
 It simply makes a request to the given URL and echos (prints) the content for you to be able to view it._
 
 </details>
 
 ---
 ## Attributions
 
+*This is a fork of [DiscordChatExporterPy](https://github.com/mahtoid/DiscordChatExporterPy) full credits go to him.*
 *This project borrows CSS and HTML code from [Tyrrrz's C# DiscordChatExporter](https://github.com/Tyrrrz/DiscordChatExporter/) repository.*
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-<!-- LINK DUMP -->
-[pypi-version]: https://img.shields.io/pypi/v/chat-exporter?style=for-the-badge
-[pypi-url]: https://pypi.org/project/chat-exporter/
-[language-dom]: https://img.shields.io/github/languages/top/mahtoid/discordchatexporterpy?style=for-the-badge
-[forks-shield]: https://img.shields.io/github/forks/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[forks-url]: https://github.com/mahtoid/DiscordChatExporterPy/
-[stars-shield]: https://img.shields.io/github/stars/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[stars-url]: https://github.com/mahtoid/DiscordChatExporterPy/stargazers
-[issues-shield]: https://img.shields.io/github/issues/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[issues-url]: https://github.com/mahtoid/DiscordChatExporterPy/issues
-[license-shield]: https://img.shields.io/github/license/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[license-url]: https://github.com/mahtoid/DiscordChatExporterPy/blob/master/LICENSE
-[github-url]: https://github.com/mahtoid/DiscordChatExporterPy/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,21 +1,16 @@
-[![Version][pypi-version]][pypi-url] [![Language][language-dom]][github-url] [!
- [Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
-[Issues][issues-shield]][issues-url] [![GPL License][license-shield]][license-
-                                     url]
-                       ***** DiscordChatExporterPy *****
-          Export Discord chats with your discord.py (or fork) bots!
-                 Join_Discord Â· Report_Bug Â· Request_Feature
+                     ***** InteractionsChatExporter *****
+             Export Discord chats with your interactions.py bots!
 --- ## Installation To install the library to your virtual environment, for bot
-usage, run the command: ```sh pip install chat-exporter ``` To clone the
-repository locally, run the command: ```sh git clone https://github.com/
-mahtoid/DiscordChatExporterPy ```
+usage, run the command: ```sh pip install InteractionsChatExporter ``` To clone
+the repository locally, run the command: ```sh git clone https://github.com/
+DylZZZ/InteractionsChatExporter ```
                                                                   (back_to_top)
---- ## Usage There are currently 3 methods (functions) to `chat-exporter` which
-you can use to export your chat.
+--- ## Usage There are currently 3 methods (functions) to
+`InteractionsChatExporter` which you can use to export your chat.
 _Expand the blocks below to learn the functions, arguments and usages._ Basic
 Usage `.quick_export()` is the simplest way of using chat-exporter. Using the
 _quick_export_ function will gather the history of the channel you give, build
 the transcript then post the file and embed directly to the channel - returning
 a message object gathered from the message it posted. This is mostly seen as a
 demo function, as opposed to a command you should actually use. **Required
 Argument(s):**
@@ -116,25 +111,13 @@
       (ctx.channel) if transcript is None: return transcript_file =
       discord.File( io.BytesIO(transcript.encode()), filename=f"transcript-
       {ctx.channel.name}.html", ) message = await ctx.send
       (file=transcript_file) link = await chat_exporter.link(message) await
       ctx.send("Click this link to view the transcript online: " + link) ```
 _Please note that the PHP script does NOT store any information.
 It simply makes a request to the given URL and echos (prints) the content for
-you to be able to view it._  --- ## Attributions *This project borrows CSS and
-HTML code from [Tyrrrz's C# DiscordChatExporter](https://github.com/Tyrrrz/
-DiscordChatExporter/) repository.*
+you to be able to view it._  --- ## Attributions *This is a fork of
+[DiscordChatExporterPy](https://github.com/mahtoid/DiscordChatExporterPy) full
+credits go to him.* *This project borrows CSS and HTML code from [Tyrrrz's C#
+DiscordChatExporter](https://github.com/Tyrrrz/DiscordChatExporter/
+) repository.*
                                                                   (back_to_top)
- [pypi-version]: https://img.shields.io/pypi/v/chat-exporter?style=for-the-
-badge [pypi-url]: https://pypi.org/project/chat-exporter/ [language-dom]:
-https://img.shields.io/github/languages/top/mahtoid/
-discordchatexporterpy?style=for-the-badge [forks-shield]: https://
-img.shields.io/github/forks/mahtoid/DiscordChatExporterPy?style=for-the-badge
-[forks-url]: https://github.com/mahtoid/DiscordChatExporterPy/ [stars-shield]:
-https://img.shields.io/github/stars/mahtoid/DiscordChatExporterPy?style=for-
-the-badge [stars-url]: https://github.com/mahtoid/DiscordChatExporterPy/
-stargazers [issues-shield]: https://img.shields.io/github/issues/mahtoid/
-DiscordChatExporterPy?style=for-the-badge [issues-url]: https://github.com/
-mahtoid/DiscordChatExporterPy/issues [license-shield]: https://img.shields.io/
-github/license/mahtoid/DiscordChatExporterPy?style=for-the-badge [license-url]:
-https://github.com/mahtoid/DiscordChatExporterPy/blob/master/LICENSE [github-
-url]: https://github.com/mahtoid/DiscordChatExporterPy/
```

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/chat_exporter.py` & `InteractionsChatExporter-2.5.4/chat_exporter/chat_exporter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import datetime
 import io
 from typing import List, Optional
 
 from chat_exporter.construct.transcript import Transcript
-from chat_exporter.ext.discord_import import discord
+import interactions
 
 
 async def quick_export(
-    channel: discord.TextChannel,
-    guild: Optional[discord.Guild] = None,
-    bot: Optional[discord.Client] = None,
+    channel: interactions.GuildChannel,
+    guild: Optional[interactions.Guild] = None,
+    bot: Optional[interactions.Client] = None,
 ):
     """
     Create a quick export of your Discord channel.
     This function will produce the transcript and post it back in to your channel.
-    :param channel: discord.TextChannel
-    :param guild: (optional) discord.Guild
-    :param bot: (optional) discord.Client
-    :return: discord.Message (posted transcript)
+    :param channel: interactions.GuildChannel
+    :param guild: (optional) interactions.Guild
+    :param bot: (optional) interactions.Client
+    :return: interactions.Message (posted transcript)
     """
-
+    
     if guild:
         channel.guild = guild
 
     transcript = (
         await Transcript(
             channel=channel,
             limit=None,
@@ -37,43 +37,45 @@
             bot=bot,
             ).export()
         ).html
 
     if not transcript:
         return
 
-    transcript_embed = discord.Embed(
+    transcript_embed = interactions.Embed(
         description=f"**Transcript Name:** transcript-{channel.name}\n\n",
-        colour=discord.Colour.blurple()
+        colour=interactions.Color.from_rgb(88, 101, 242),
     )
-
-    transcript_file = discord.File(io.BytesIO(transcript.encode()), filename=f"transcript-{channel.name}.html")
+    
+    transcript_file = interactions.File()
+    transcript_file.filename = f"transcript-{channel.name}.html"
+    transcript_file.file = io.BytesIO(transcript.encode("utf-8"))
     return await channel.send(embed=transcript_embed, file=transcript_file)
 
 
 async def export(
-    channel: discord.TextChannel,
+    channel: interactions.GuildChannel,
     limit: Optional[int] = None,
     tz_info="UTC",
-    guild: Optional[discord.Guild] = None,
-    bot: Optional[discord.Client] = None,
+    guild: Optional[interactions.Guild] = None,
+    bot: Optional[interactions.Client] = None,
     military_time: Optional[bool] = True,
     fancy_times: Optional[bool] = True,
     before: Optional[datetime.datetime] = None,
     after: Optional[datetime.datetime] = None,
     support_dev: Optional[bool] = True,
 ):
     """
     Create a customised transcript of your Discord channel.
     This function will return the transcript which you can then turn in to a file to post wherever.
-    :param channel: discord.TextChannel - channel to Export
+    :param channel: interactions.GuildChannel - channel to Export
     :param limit: (optional) integer - limit of messages to capture
     :param tz_info: (optional) TZ Database Name - set the timezone of your transcript
-    :param guild: (optional) discord.Guild - solution for edpy
-    :param bot: (optional) discord.Client - set getting member role colour
+    :param guild: (optional) interactions.Guild - solution for edpy
+    :param bot: (optional) interactions.Client - set getting member role colour
     :param military_time: (optional) boolean - set military time (24hour clock)
     :param fancy_times: (optional) boolean - set javascript around time display
     :param before: (optional) datetime.datetime - allows before time for history
     :param after: (optional) datetime.datetime - allows after time for history
     :return: string - transcript file make up
     """
     if guild:
@@ -92,31 +94,31 @@
             support_dev=support_dev,
             bot=bot,
         ).export()
     ).html
 
 
 async def raw_export(
-    channel: discord.TextChannel,
-    messages: List[discord.Message],
+    channel: interactions.GuildChannel,
+    messages: List[interactions.Message],
     tz_info="UTC",
-    guild: Optional[discord.Guild] = None,
-    bot: Optional[discord.Client] = None,
+    guild: Optional[interactions.Guild] = None,
+    bot: Optional[interactions.Client] = None,
     military_time: Optional[bool] = False,
     fancy_times: Optional[bool] = True,
     support_dev: Optional[bool] = True,
 ):
     """
     Create a customised transcript with your own captured Discord messages
     This function will return the transcript which you can then turn in to a file to post wherever.
-    :param channel: discord.TextChannel - channel to Export
-    :param messages: List[discord.Message] - list of Discord messages to export
+    :param channel: interactions.GuildChannel - channel to Export
+    :param messages: List[interactions.Message] - list of Discord messages to export
     :param tz_info: (optional) TZ Database Name - set the timezone of your transcript
-    :param guild: (optional) discord.Guild - solution for edpy
-    :param bot: (optional) discord.Client - set getting member role colour
+    :param guild: (optional) interactions.Guild - solution for edpy
+    :param bot: (optional) interactions.Client - set getting member role colour
     :param military_time: (optional) boolean - set military time (24hour clock)
     :param fancy_times: (optional) boolean - set javascript around time display
     :return: string - transcript file make up
     """
     if guild:
         channel.guild = guild
 
@@ -133,38 +135,38 @@
             support_dev=support_dev,
             bot=bot,
         ).export()
     ).html
 
 
 async def quick_link(
-    channel: discord.TextChannel,
-    message: discord.Message
+    channel: interactions.GuildChannel,
+    message: interactions.Message
 ):
     """
     Create a quick link for your transcript file.
     This function will return an embed with a link to view the transcript online.
-    :param channel: discord.TextChannel
-    :param message: discord.Message
-    :return: discord.Message (posted link)
+    :param channel: interactions.GuildChannel
+    :param message: interactions.Message
+    :return: interactions.Message (posted link)
     """
-    embed = discord.Embed(
+    embed = interactions.Embed(
         title="Transcript Link",
         description=(
             f"[Click here to view the transcript](https://mahto.id/chat-exporter?url={message.attachments[0].url})"
         ),
-        colour=discord.Colour.blurple(),
+        colour=interactions.Color.from_rgb(88, 101, 242),
     )
 
     return await channel.send(embed=embed)
 
 
 async def link(
-    message: discord.Message
+    message: interactions.Message
 ):
     """
     Returns a link which you can use to display in a message.
     This function will return a string of the link.
-    :param message: discord.Message
+    :param message: interactions.Message
     :return: string (link: https://mahto.id/chat-exporter?url=ATTACHMENT_URL)
     """
     return "https://mahto.id/chat-exporter?url=" + message.attachments[0].url
```

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/construct/assets/attachment.py` & `InteractionsChatExporter-2.5.4/chat_exporter/construct/assets/attachment.py`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/construct/assets/component.py` & `InteractionsChatExporter-2.5.4/chat_exporter/construct/assets/component.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from chat_exporter.ext.discord_import import discord
+import interactions
 
 from chat_exporter.ext.discord_utils import DiscordUtils
 from chat_exporter.ext.html_generator import (
     fill_out,
     component_button,
     component_menu,
     component_menu_options,
@@ -33,21 +33,21 @@
     menu_div_id: int = 0
 
     def __init__(self, component, guild):
         self.component = component
         self.guild = guild
 
     async def build_component(self, c):
-        if isinstance(c, discord.Button):
+        if isinstance(c, interactions.Button):
             await self.build_button(c)
-        elif isinstance(c, discord.SelectMenu):
+        elif isinstance(c, tuple([interactions.BaseSelectMenu, interactions.StringSelectMenu, interactions.UserSelectMenu, interactions.ChannelSelectMenu, interactions.RoleSelectMenu])):
             await self.build_menu(c)
             Component.menu_div_id += 1
 
-    async def build_button(self, c):
+    async def build_button(self, c: interactions.Button):
         url = c.url if c.url else ""
         label = c.label if c.label else ""
         style = self.styles[str(c.style).split(".")[1]]
         icon = DiscordUtils.button_external_link if url else ""
         emoji = str(c.emoji) if c.emoji else ""
 
         self.buttons += await fill_out(self.guild, component_button, [
@@ -55,15 +55,15 @@
             ("URL", str(url), PARSE_MODE_NONE),
             ("LABEL", str(label), PARSE_MODE_MARKDOWN),
             ("EMOJI", str(emoji), PARSE_MODE_EMOJI),
             ("ICON", str(icon), PARSE_MODE_NONE),
             ("STYLE", style, PARSE_MODE_NONE)
         ])
 
-    async def build_menu(self, c):
+    async def build_menu(self, c: interactions.BaseSelectMenu):
         placeholder = c.placeholder if c.placeholder else ""
         options = c.options
         content = ""
 
         if not c.disabled:
             content = await self.build_menu_options(options)
```

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/construct/assets/embed.py` & `InteractionsChatExporter-2.5.4/chat_exporter/construct/assets/embed.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import html
 
-from chat_exporter.ext.discord_import import discord
+import interactions
 
 from chat_exporter.ext.html_generator import (
     fill_out,
     embed_body,
     embed_title,
     embed_description,
     embed_field,
@@ -21,16 +21,14 @@
     PARSE_MODE_SPECIAL_EMBED,
 )
 
 modules_which_use_none = ["nextcord", "disnake"]
 
 
 def _gather_checker():
-    if discord.module not in modules_which_use_none and hasattr(discord.Embed, "Empty"):
-        return discord.Embed.Empty
     return None
 
 
 class Embed:
     r: str
     g: str
     b: str
@@ -41,16 +39,16 @@
     thumbnail: str
     footer: str
     fields: str
 
     check_against = None
 
     def __init__(self, embed, guild):
-        self.embed: discord.Embed = embed
-        self.guild: discord.Guild = guild
+        self.embed: interactions.Embed = embed
+        self.guild: interactions.Guild = guild
 
     async def flow(self):
         self.check_against = _gather_checker()
         self.build_colour()
         await self.build_title()
         await self.build_description()
         await self.build_fields()
```

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/construct/assets/reaction.py` & `InteractionsChatExporter-2.5.4/chat_exporter/construct/assets/reaction.py`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/construct/message.py` & `InteractionsChatExporter-2.5.4/chat_exporter/construct/message.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import html
 from typing import List, Optional, Union
 
 from pytz import timezone
 from datetime import timedelta
 
-from chat_exporter.ext.discord_import import discord
+import interactions
 
 from chat_exporter.construct.assets import Attachment, Component, Embed, Reaction
 from chat_exporter.ext.discord_utils import DiscordUtils
 from chat_exporter.ext.html_generator import (
     fill_out,
     bot_tag,
     bot_tag_verified,
@@ -24,15 +24,15 @@
     end_message,
     PARSE_MODE_NONE,
     PARSE_MODE_MARKDOWN,
     PARSE_MODE_REFERENCE,
 )
 
 
-def _gather_user_bot(author: discord.Member):
+def _gather_user_bot(author: interactions.Member):
     if author.bot and author.public_flags.verified_bot:
         return bot_tag_verified
     elif author.bot:
         return bot_tag
     return ""
 
 
@@ -48,19 +48,19 @@
     reactions: str = ""
     components: str = ""
     attachments: str = ""
     time_format: str = ""
 
     def __init__(
         self,
-        message: discord.Message,
-        previous_message: Optional[discord.Message],
+        message: interactions.Message,
+        previous_message: Optional[interactions.Message],
         pytz_timezone,
         military_time: bool,
-        guild: discord.Guild,
+        guild: interactions.Guild,
         meta_data: dict
     ):
         self.message = message
         self.previous_message = previous_message
         self.pytz_timezone = pytz_timezone
         self.military_time = military_time
         self.guild = guild
@@ -70,18 +70,18 @@
             self.time_format = "%A, %e %B %Y %H:%M"
 
         self.message_created_at, self.message_edited_at = self.set_time()
         self.meta_data = meta_data
 
     async def construct_message(
         self,
-    ) -> (str, dict):
-        if discord.MessageType.pins_add == self.message.type:
+    ):
+        if self.message.pinned:
             await self.build_pin()
-        elif discord.MessageType.thread_created == self.message.type:
+        elif self.message.thread:
             await self.build_thread()
         else:
             await self.build_message()
         return self.message_html, self.meta_data
 
     async def build_message(self):
         await self.build_content()
@@ -139,18 +139,18 @@
 
     async def build_reference(self):
         if not self.message.reference:
             self.message.reference = ""
             return
 
         try:
-            message: discord.Message = await self.message.channel.fetch_message(self.message.reference.message_id)
-        except (discord.NotFound, discord.HTTPException) as e:
+            message: interactions.Message = await self.message.channel.fetch_message(self.message.reference.message_id)
+        except (interactions.errors.NotFound, interactions.errors.HTTPException) as e:
             self.message.reference = ""
-            if isinstance(e, discord.NotFound):
+            if isinstance(e, interactions.errors.NotFound):
                 self.message.reference = message_reference_unknown
             return
 
         is_bot = _gather_user_bot(message.author)
         user_colour = await self._gather_user_colour(message.author)
 
         if not message.content and not message.interaction:
@@ -184,15 +184,15 @@
         ])
 
     async def build_interaction(self):
         if not self.message.interaction:
             self.message.interaction = ""
             return
 
-        user: Union[discord.Member, discord.User] = self.message.interaction.user
+        user: Union[interactions.Member, interactions.User] = self.message.interaction.user
         is_bot = _gather_user_bot(user)
         user_colour = await self._gather_user_colour(user)
         avatar_url = user.display_avatar if user.display_avatar else DiscordUtils.default_avatar
         self.message.interaction = await fill_out(self.guild, message_interaction, [
             ("AVATAR_URL", str(avatar_url), PARSE_MODE_NONE),
             ("BOT_TAG", is_bot, PARSE_MODE_NONE),
             ("NAME_TAG", "%s#%s" % (user.name, user.discriminator), PARSE_MODE_NONE),
@@ -204,26 +204,27 @@
             ("INTERACTION_ID", str(self.message.interaction.id), PARSE_MODE_NONE),
         ])
 
     async def build_sticker(self):
         if not self.message.stickers or not hasattr(self.message.stickers[0], "url"):
             return
 
-        sticker_image_url = self.message.stickers[0].url
-
-        if sticker_image_url.endswith(".json"):
-            sticker = await self.message.stickers[0].fetch()
-            sticker_image_url = (
-                f"https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/stickers/{sticker.pack_id}/{sticker.id}.gif"
-            )
+        return
+        # sticker_image_url = self.message.stickers[0].url
 
-        self.message.content = await fill_out(self.guild, img_attachment, [
-            ("ATTACH_URL", str(sticker_image_url), PARSE_MODE_NONE),
-            ("ATTACH_URL_THUMB", str(sticker_image_url), PARSE_MODE_NONE)
-        ])
+        # if sticker_image_url.endswith(".json"):
+        #     sticker = self.message.sticker_items[0].format_type.
+        #     sticker_image_url = (
+        #         f"https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/stickers/{sticker.pack_id}/{sticker.id}.gif"
+        #     )
+
+        # self.message.content = await fill_out(self.guild, img_attachment, [
+        #     ("ATTACH_URL", str(sticker_image_url), PARSE_MODE_NONE),
+        #     ("ATTACH_URL_THUMB", str(sticker_image_url), PARSE_MODE_NONE)
+        # ])
 
     async def build_assets(self):
         for e in self.message.embeds:
             self.embeds += await Embed(e, self.guild).flow()
 
         for a in self.message.attachments:
             self.attachments += await Attachment(a, self.guild).flow()
@@ -324,43 +325,43 @@
             ("THREAD_NAME", self.message.content, PARSE_MODE_NONE),
             ("USER_COLOUR", await self._gather_user_colour(self.message.author)),
             ("NAME", str(html.escape(self.message.author.display_name))),
             ("NAME_TAG", "%s#%s" % (self.message.author.name, self.message.author.discriminator), PARSE_MODE_NONE),
             ("MESSAGE_ID", str(self.message.id), PARSE_MODE_NONE),
         ])
 
-    async def _gather_member(self, author: discord.Member):
+    async def _gather_member(self, author: interactions.Member):
         member = self.guild.get_member(author.id)
 
         if member:
             return member
 
         try:
             return await self.guild.fetch_member(author.id)
         except Exception:
             return None
 
-    async def _gather_user_colour(self, author: discord.Member):
+    async def _gather_user_colour(self, author: interactions.Member):
         member = await self._gather_member(author)
         user_colour = member.colour if member and str(member.colour) != "#000000" else "#FFFFFF"
         return f"color: {user_colour};"
 
-    async def _gather_user_icon(self, author: discord.Member):
+    async def _gather_user_icon(self, author: interactions.Member):
         member = await self._gather_member(author)
 
         if not member:
             return ""
 
         if hasattr(member, "display_icon") and member.display_icon:
             return f"<img class='chatlog__role-icon' src='{member.display_icon}' alt='Role Icon'>"
         elif hasattr(member, "top_role") and member.top_role and member.top_role.icon:
             return f"<img class='chatlog__role-icon' src='{member.top_role.icon}' alt='Role Icon'>"
         return ""
 
-    def set_time(self, message: Optional[discord.Message] = None):
+    def set_time(self, message: Optional[interactions.Message] = None):
         message = message if message else self.message
         created_at_str = self.to_local_time_str(message.created_at)
         edited_at_str = self.to_local_time_str(message.edited_at) if message.edited_at else ""
 
         return created_at_str, edited_at_str
 
     def to_local_time_str(self, time):
@@ -372,22 +373,22 @@
         if self.military_time:
             return local_time.strftime(self.time_format)
 
         return local_time.strftime(self.time_format)
 
 
 async def gather_messages(
-    messages: List[discord.Message],
-    guild: discord.Guild,
+    messages: List[interactions.Message],
+    guild: interactions.Guild,
     pytz_timezone,
     military_time,
-) -> (str, dict):
+):
     message_html: str = ""
     meta_data: dict = {}
-    previous_message: Optional[discord.Message] = None
+    previous_message: Optional[interactions.Message] = None
 
     for message in messages:
         content_html, meta_data = await MessageConstruct(
             message,
             previous_message,
             pytz_timezone,
             military_time,
```

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/construct/transcript.py` & `InteractionsChatExporter-2.5.4/chat_exporter/construct/transcript.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import html
 import traceback
 
 from typing import List, Optional
 
 import pytz
 
-from chat_exporter.ext.discord_import import discord
+import interactions
 
 from chat_exporter.construct.message import gather_messages
 from chat_exporter.construct.assets.component import Component
 
 from chat_exporter.ext.cache import clear_cache
 from chat_exporter.parse.mention import pass_bot
 from chat_exporter.ext.discord_utils import DiscordUtils
@@ -20,37 +20,37 @@
 
 
 class TranscriptDAO:
     html: str
 
     def __init__(
         self,
-        channel: discord.TextChannel,
+        channel: interactions.GuildChannel,
         limit: Optional[int],
-        messages: Optional[List[discord.Message]],
+        messages: Optional[List[interactions.Message]],
         pytz_timezone,
         military_time: bool,
         fancy_times: bool,
         before: Optional[datetime.datetime],
         after: Optional[datetime.datetime],
         support_dev: bool,
-        bot: Optional[discord.Client],
+        bot: Optional[interactions.Client],
     ):
         self.channel = channel
         self.messages = messages
         self.limit = int(limit) if limit else None
         self.military_time = military_time
         self.fancy_times = fancy_times
         self.before = before
         self.after = after
         self.support_dev = support_dev
         self.pytz_timezone = pytz_timezone
 
         # This is to pass timezone in to mention.py without rewriting
-        setattr(discord.Guild, "timezone", self.pytz_timezone)
+        setattr(interactions.Guild, "timezone", self.pytz_timezone)
 
         if bot:
             pass_bot(bot)
 
     async def build_transcript(self):
         message_html, meta_data = await gather_messages(
             self.messages,
@@ -95,15 +95,15 @@
                 ("DISPLAY", str(meta_data[int(data)][6]), PARSE_MODE_NONE),
                 ("MESSAGE_COUNT", str(meta_data[int(data)][4]))
             ])
 
         channel_creation_time = self.channel.created_at.astimezone(timezone).strftime("%b %d, %Y (%T)")
 
         raw_channel_topic = (
-            self.channel.topic if isinstance(self.channel, discord.TextChannel) and self.channel.topic else ""
+            self.channel.topic if isinstance(self.channel, interactions.GuildChannel) and self.channel.topic else ""
         )
 
         channel_topic_html = ""
         if raw_channel_topic:
             channel_topic_html = await fill_out(self.channel.guild, channel_topic, [
                 ("CHANNEL_TOPIC", raw_channel_topic)
             ])
```

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/ext/cache.py` & `InteractionsChatExporter-2.5.4/chat_exporter/ext/cache.py`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/ext/discord_utils.py` & `InteractionsChatExporter-2.5.4/chat_exporter/ext/discord_utils.py`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/ext/emoji_convert.py` & `InteractionsChatExporter-2.5.4/chat_exporter/ext/emoji_convert.py`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/ext/html_generator.py` & `InteractionsChatExporter-2.5.4/chat_exporter/ext/html_generator.py`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/attachment/audio.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/attachment/audio.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/attachment/message.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/attachment/message.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/base.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/base.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/embed/body.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/embed/body.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/message/interaction.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/message/interaction.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/message/message.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/message/message.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/message/meta.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/message/meta.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/message/pin.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/message/pin.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/message/reference.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/message/reference.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/message/start.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/message/start.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/message/thread.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/message/thread.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/html/script/fancy_time.html` & `InteractionsChatExporter-2.5.4/chat_exporter/html/script/fancy_time.html`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/parse/markdown.py` & `InteractionsChatExporter-2.5.4/chat_exporter/parse/markdown.py`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/chat_exporter/parse/mention.py` & `InteractionsChatExporter-2.5.4/chat_exporter/parse/mention.py`

 * *Files identical despite different names*

### Comparing `InteractionsChatExporter-2.5.3/pyproject.toml` & `InteractionsChatExporter-2.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "InteractionsChatExporter"
 description = "A simple Discord chat exporter for Interactions.py Discord bots."
-version = "2.5.3"
+version = "2.5.4"
 readme = "README.md"
 authors = [
     { name="mahtoid", email="info@mahto.id" }
 ]
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-only" }
 classifiers = [
@@ -31,8 +31,8 @@
 ]
 dependencies = ["aiohttp", "pytz", "grapheme", "emoji"]
 keywords = ["chat exporter", "discord chat exporter", "discord", "discordpy", "disnake", "pycord", "nextcord"]
 
 [project.urls]
 Homepage = "https://github.com/DylZZZ/InteractionsChatExporter"
 Discord = "https://discord.gg/2uhHBQDwcc"
-Donate = "https://ko-fi.com/mahtoid"
+Donate = "https://ko-fi.com/mahtoid"
```

