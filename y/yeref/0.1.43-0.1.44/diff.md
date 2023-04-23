# Comparing `tmp/yeref-0.1.43.tar.gz` & `tmp/yeref-0.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.43.tar", last modified: Sun Apr 23 12:00:06 2023, max compression
+gzip compressed data, was "yeref-0.1.44.tar", last modified: Sun Apr 23 12:51:50 2023, max compression
```

## Comparing `yeref-0.1.43.tar` & `yeref-0.1.44.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 12:00:06.084806 yeref-0.1.43/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 12:00:06.085033 yeref-0.1.43/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-23 12:00:06.086382 yeref-0.1.43/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-23 11:59:53.000000 yeref-0.1.43/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 12:00:06.078307 yeref-0.1.43/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.43/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)    95328 2023-04-23 11:50:56.000000 yeref-0.1.43/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   184285 2023-04-23 11:14:41.000000 yeref-0.1.43/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 12:00:06.084299 yeref-0.1.43/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 12:00:06.000000 yeref-0.1.43/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-23 12:00:06.000000 yeref-0.1.43/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-23 12:00:06.000000 yeref-0.1.43/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-23 12:00:06.000000 yeref-0.1.43/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 12:51:50.318570 yeref-0.1.44/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 12:51:50.318809 yeref-0.1.44/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-23 12:51:50.319693 yeref-0.1.44/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-23 12:51:43.000000 yeref-0.1.44/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 12:51:50.305374 yeref-0.1.44/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.44/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   101605 2023-04-23 12:10:51.000000 yeref-0.1.44/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   184283 2023-04-23 12:18:06.000000 yeref-0.1.44/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 12:51:50.314306 yeref-0.1.44/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 12:51:50.000000 yeref-0.1.44/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-23 12:51:50.000000 yeref-0.1.44/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-23 12:51:50.000000 yeref-0.1.44/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-23 12:51:50.000000 yeref-0.1.44/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.43/setup.py` & `yeref-0.1.44/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.43',
+      version='0.1.44',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,10 +39,10 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.43-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.44-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
```

### Comparing `yeref-0.1.43/yeref/l_.py` & `yeref-0.1.44/yeref/l_.py`

 * *Files 3% similar despite different names*

```diff
@@ -1202,15 +1202,15 @@
 }
 
 # endregion
 
 
 # region FereyVPNBot
 l_vpn_btn1 = {
-    'ru': '⛰️ Нейросети',
+    'ru': '⛰️ VPN',
     'en': '⛰️ Projects',
     'es': '⛰️ Projects',
     'fr': '⛰️ Projects',
     'zh': '⛰️ 團體',
     'ar': '⛰️ مجموعات',
 }
 l_vpn_btn2 = {
@@ -1218,15 +1218,15 @@
     'en': '🌬 Subcribe',
     'es': '🌬 Sobre',
     'fr': '🌬 À propos de',
     'zh': '🌬 關於',
     'ar': '🌬 حول',
 }
 l_vpn_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>генерации</code> контента:\n\n▪️<b>текст</b>\n▪️<b>изображение</b>\n▪️<b>анализ Telegram-канала</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> проекта Ferey:\n\n▪️<b>openvpn</b>\n▪️<b>wireguard</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
     'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
     'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
     'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
     'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
     'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
 }
 l_vpn_1 = {
@@ -1246,15 +1246,15 @@
     'ar': '👇🏽 اختر الاتجاه',
 }
 # endregion
 
 
 # region FereyToolsBot
 l_tools_btn1 = {
-    'ru': '⛰️ Нейросети',
+    'ru': '⛰️ Инструменты',
     'en': '⛰️ Projects',
     'es': '⛰️ Projects',
     'fr': '⛰️ Projects',
     'zh': '⛰️ 團體',
     'ar': '⛰️ مجموعات',
 }
 l_tools_btn2 = {
@@ -1262,15 +1262,15 @@
     'en': '🌬 Subcribe',
     'es': '🌬 Sobre',
     'fr': '🌬 À propos de',
     'zh': '🌬 關於',
     'ar': '🌬 حول',
 }
 l_tools_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>генерации</code> контента:\n\n▪️<b>текст</b>\n▪️<b>изображение</b>\n▪️<b>анализ Telegram-канала</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> Telegram-<code>инструментов</code>:\n\n▪️<b>преобразование</b> контента\n▪️<b>получение</b> информации о сообщении\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
     'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
     'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
     'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
     'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
     'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
 }
 l_image_text = {
@@ -1706,8 +1706,133 @@
     'ru': "👩🏽‍💻 <b>Прикрепи</b> любое сообщение или сделай пересылку",
     'en': '⿴ Bot Desc Pic',
     'es': '👇🏽 Elige la dirección',
     'fr': '👇🏽 Choisissez l\'orientation',
     'zh': '👇🏽 選擇方向',
     'ar': '👇🏽 اختر الاتجاه',
 }
+# endregion
+
+
+# region FereyMediaBot
+l_media_btn1 = {
+    'ru': '⛰️ Медиа',
+    'en': '⛰️ Projects',
+    'es': '⛰️ Projects',
+    'fr': '⛰️ Projects',
+    'zh': '⛰️ 團體',
+    'ar': '⛰️ مجموعات',
+}
+l_media_btn2 = {
+    'ru': '🌬 Подписка',
+    'en': '🌬 Subcribe',
+    'es': '🌬 Sobre',
+    'fr': '🌬 À propos de',
+    'zh': '🌬 關於',
+    'ar': '🌬 حول',
+}
+l_media_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>медиа</code>-заметок:\n\n▪️<b>стикеры</b> из текста и фото\n▪️<b>аудио-звуки</b>\n▪️<b>видео-заметки</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
+    'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
+}
+
+l_media_text = {
+    'ru': "👩🏽‍💻 <b>Здесь</b> можно выбрать тип выпадающих media-заметок (/add | /del)",
+    'en': "🌏 Choose language",
+    'es': "🌏 Elige idioma",
+    'fr': "🌏 Choisissez la langue",
+    'zh': "🌏 選擇語言",
+    'ar': "🌏 اختر اللغة",
+}
+l_media_del = {
+    'ru': "👩🏽‍💻 <b>Выбери</b> media-заметку для удаления",
+    'en': "🌏 Choose language",
+    'es': "🌏 Elige idioma",
+    'fr': "🌏 Choisissez la langue",
+    'zh': "🌏 選擇語言",
+    'ar': "🌏 اختر اللغة",
+}
+l_media_file = {
+    'ru': "👩🏽‍💻 1/2. <b>Прикрепи</b> audio/video, text/photo контент для создания media-заметки",
+    'en': "🌏 Choose language",
+    'es': "🌏 Elige idioma",
+    'fr': "🌏 Choisissez la langue",
+    'zh': "🌏 選擇語言",
+    'ar': "🌏 اختر اللغة",
+}
+l_media_title1 = {
+    'ru': "👩🏽‍💻 2/2. <b>Введи</b> <code>ключевые_слова</code> для твоей media-заметки\n[изменить <code>ключевые_слова</code> нельзя]",
+    'en': "🌏 Choose language",
+    'es': "🌏 Elige idioma",
+    'fr': "🌏 Choisissez la langue",
+    'zh': "🌏 選擇語言",
+    'ar': "🌏 اختر اللغة",
+}
+l_media_title2 = {
+    'ru': "👩🏽‍💻 2/2. <b>Текущие</b> <code>ключевые_слова</code> для твоей media-заметки\n\n{0}\n\n[пришли новые или нажми {1}]",
+    'en': "🌏 Choose language",
+    'es': "🌏 Elige idioma",
+    'fr': "🌏 Choisissez la langue",
+    'zh': "🌏 選擇語言",
+    'ar': "🌏 اختر اللغة",
+}
+l_media_confirm = {
+    'ru': "🏁 Завершить",
+    'en': "🌏 Choose language",
+    'es': "🌏 Elige idioma",
+    'fr': "🌏 Choisissez la langue",
+    'zh': "🌏 選擇語言",
+    'ar': "🌏 اختر اللغة",
+}
+l_media_error = {
+    'ru': "👩🏽‍💻 <b>Ошибка</b> (попробуйте позже или загрузите другое media)",
+    'en': "🌏 Choose language",
+    'es': "🌏 Elige idioma",
+    'fr': "🌏 Choisissez la langue",
+    'zh': "🌏 選擇語言",
+    'ar': "🌏 اختر اللغة",
+}
+l_media_finish = {
+    'ru': "👩🏽‍💻 <b>Media</b>-заметка успешно создана",
+    'en': "🌏 Choose language",
+    'es': "🌏 Elige idioma",
+    'fr': "🌏 Choisissez la langue",
+    'zh': "🌏 選擇語言",
+    'ar': "🌏 اختر اللغة",
+}
+l_media_publish = {
+    'ru': "🔗 Список",
+    'en': "🔗 Publish",
+    'es': "🔗 Publicar",
+    'fr': "🔗 Publier",
+    'zh': "🔗 發布",
+    'ar': "🔗 نشر",
+}
+l_media_check = {
+    'ru': "🔗 Проверка",
+    'en': "🔗 Publish",
+    'es': "🔗 Publicar",
+    'fr': "🔗 Publier",
+    'zh': "🔗 發布",
+    'ar': "🔗 نشر",
+}
+l_media_hasdeleted = {
+    'ru': "👩🏽‍💻 <b>Media</b>-заметка удалена",
+    'en': "🔗 Publish",
+    'es': "🔗 Publicar",
+    'fr': "🔗 Publier",
+    'zh': "🔗 發布",
+    'ar': "🔗 نشر",
+}
+l_media_delprepare = {
+    'ru': "🔗 Выбрать",
+    'en': "🔗 Publish",
+    'es': "🔗 Publicar",
+    'fr': "🔗 Publier",
+    'zh': "🔗 發布",
+    'ar': "🔗 نشر",
+}
 # endregion
```

### Comparing `yeref-0.1.43/yeref/yeref.py` & `yeref-0.1.44/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -2437,15 +2437,15 @@
 
 
 async def read_likes(BASE_D, POST_ID=1):
     cnt = '⁰'
     try:
         sql = "SELECT USER_ID FROM LIKE WHERE POST_ID = ?"
         data = await db_select(sql, (POST_ID,), BASE_D)
-        cnt = str(100 + len(data))
+        cnt = str(0 + len(data))
         cnt = cnt.replace('0', '⁰').replace('1', '¹').replace('2', '²').replace('3', '³').replace('4', '⁴') \
             .replace('5', '⁵').replace('6', '⁶').replace('7', '⁷').replace('8', '⁸').replace('9', '⁹')
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return cnt
```

