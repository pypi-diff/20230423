# Comparing `tmp/yeref-0.1.40.tar.gz` & `tmp/yeref-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.40.tar", last modified: Sat Apr 22 08:45:55 2023, max compression
+gzip compressed data, was "yeref-0.1.41.tar", last modified: Sun Apr 23 10:46:54 2023, max compression
```

## Comparing `yeref-0.1.40.tar` & `yeref-0.1.41.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:45:55.764639 yeref-0.1.40/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:45:55.764877 yeref-0.1.40/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-22 08:45:55.765781 yeref-0.1.40/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-22 08:41:08.000000 yeref-0.1.40/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:45:55.758082 yeref-0.1.40/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.40/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)    53630 2023-04-22 08:39:39.000000 yeref-0.1.40/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   205201 2023-04-22 08:26:22.000000 yeref-0.1.40/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-22 08:45:55.763940 yeref-0.1.40/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-22 08:45:55.000000 yeref-0.1.40/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-22 08:45:55.000000 yeref-0.1.40/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-22 08:45:55.000000 yeref-0.1.40/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-22 08:45:55.000000 yeref-0.1.40/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 10:46:54.813516 yeref-0.1.41/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 10:46:54.813762 yeref-0.1.41/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-23 10:46:54.814895 yeref-0.1.41/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-23 10:46:51.000000 yeref-0.1.41/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 10:46:54.807421 yeref-0.1.41/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.41/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)    69861 2023-04-23 10:46:01.000000 yeref-0.1.41/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   183551 2023-04-23 10:34:36.000000 yeref-0.1.41/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 10:46:54.812554 yeref-0.1.41/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 10:46:54.000000 yeref-0.1.41/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-23 10:46:54.000000 yeref-0.1.41/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-23 10:46:54.000000 yeref-0.1.41/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-23 10:46:54.000000 yeref-0.1.41/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.40/setup.py` & `yeref-0.1.41/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.40',
+      version='0.1.41',
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
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.40-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.41-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
```

### Comparing `yeref-0.1.40/yeref/l_.py` & `yeref-0.1.41/yeref/l_.py`

 * *Files 14% similar despite different names*

```diff
@@ -137,315 +137,14 @@
     'fr': "💔 Like",
     'zh': "💔 Like",
     'ar': "💔 Like",
 }
 # endregion
 
 
-# region FereyDemoBot
-l_demo_btn1 = {
-    'ru': '⛰️ Проекты',
-    'en': '⛰️ Projects',
-    'es': '⛰️ Projects',
-    'fr': '⛰️ Projects',
-    'zh': '⛰️ 團體',
-    'ar': '⛰️ مجموعات',
-}
-l_demo_btn2 = {
-    'ru': '🌬 Подписка',
-    'en': '🌬 Subcribe',
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_demo_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>информация</b> обо всех проектах\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
-    'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
-    'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
-    'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
-    'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
-    'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
-}
-
-l_kind_1 = {
-    'ru': '<b>👩🏽‍💻@FereyDemoBot</b>\n\nДемонстрационный бот всех проектов',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_2 = {
-    'ru': '<b>👩🏽‍💻@FereyBotBot</b>\n\nКонструктор ботов:\n▪️авто-генерация бота\n▪️авто-генерация контента (open-ai)\n▪️авто-бан/авто-перевод',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_3 = {
-    'ru': '<b>👩🏽‍💻@FereyChannelBot</b>\n\nАдминистратор каналов:\n▪️авто-постинг\n▪️авто-декор',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_4 = {
-    'ru': '<b>👩🏽‍💻@FereyGroupBot</b>\n\nАдминистратор групп:\n▪️авто-постинг\n▪️модерация',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_5 = {
-    'ru': '<b>👩🏽‍💻@FereyUserBot</b>\n\nАдминистратор пользователей:\n▪️авто-постинг\n▪️авто-декор',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_6 = {
-    'ru': '<b>👩🏽‍💻@FereyPostBot</b>\n\nБыстрое создание и публикация постов:\n▪️превью\n▪️галерея',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_7 = {
-    'ru': '<b>👩🏽‍💻@FereyFindBot</b>\n\nПоиск по каналам/группам/пользователям/ботам:\n▪️отслеживание постов\n▪️гео-поиск',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_8 = {
-    'ru': '<b>👩🏽‍💻@FereyMediaBot</b>\n\nБот с популярными креативами:\n▪️аудио-заметки\n▪️видео-заметки',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_9 = {
-    'ru': '<b>👩🏽‍💻@FereyVpnBot</b>\n\nВсе о VPN',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_10 = {
-    'ru': '<b>👩🏽‍💻@FereyTargetBot</b>\n\nТаргетированная рассылка',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_11 = {
-    'ru': '<b>👩🏽‍💻@FereyToolsBot</b>\n\nБот инструментов:\n▪️конвертация\n▪️загрузка',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_12 = {
-    'ru': '<b>👩🏽‍💻@FereyAIBot</b>\n\nБот генерации контента (open-ai):\n▪️chat-gpt\n▪️dalli·e',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_13 = {
-    'ru': '<b>👩🏽‍💻@FereyAdsBot</b>\n\nБот рекламы в:\n▪️ботах\n▪️каналах',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_kind_14 = {
-    'ru':  '<b>👩🏽‍💻@FereyWorkBot</b>\n\nБот информации о:\n▪️вакансиях\n▪️соревнованиях',
-    'en': '👇🏽 Choose direction',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-# endregion
-
-
-# region FereyWorkBot
-l_work_btn1 = {
-    'ru': '⛰️ Вакансии',
-    'en': '⛰️ Projects',
-    'es': '⛰️ Projects',
-    'fr': '⛰️ Projects',
-    'zh': '⛰️ 團體',
-    'ar': '⛰️ مجموعات',
-}
-l_work_btn2 = {
-    'ru': '🌬 Подписка',
-    'en': '🌬 Subcribe',
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_work_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>вакансии</b> нашего стартапа\n▪️конкурсы и <b>мероприятия</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
-    'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
-    'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
-    'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
-    'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
-    'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
-}
-l_vacancy_1 = {
-    'ru': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
-    'en': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
-    'es': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
-    'fr': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
-    'zh': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
-    'ar': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
-}
-l_vacancy_2 = {
-    'ru': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
-    'en': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
-    'es': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
-    'fr': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
-    'zh': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
-    'ar': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
-}
-l_vacancy_3 = {
-    'ru': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
-    'en': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
-    'es': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
-    'fr': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
-    'zh':'👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
-    'ar': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
-}
-# endregion
-
-
-# region FereyAIBot
-l_ai_btn1 = {
-    'ru': '⛰️ Вакансии',
-    'en': '⛰️ Projects',
-    'es': '⛰️ Projects',
-    'fr': '⛰️ Projects',
-    'zh': '⛰️ 團體',
-    'ar': '⛰️ مجموعات',
-}
-l_ai_btn2 = {
-    'ru': '🌬 Подписка',
-    'en': '🌬 Subcribe',
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_ai_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>вакансии</b> нашего стартапа\n▪️конкурсы и <b>мероприятия</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
-    'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
-    'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
-    'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
-    'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
-    'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
-}
-l_gen_txt = {
-    'ru': "📘 Текст{0}",
-    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_gen_img = {
-    'ru': "🌌 Образ",
-    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_gen_tlg = {
-    'ru': "👩🏽‍💻 Анализ Telegram-канала",
-    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_generate_main = {
-    'ru': '👩🏽‍💻 <b>Выбери режим</b>',
-    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_generate_prompt = {
-    'ru': '👩🏽‍💻 <b>Введи</b> запрос для <b>{0}</b> 👇🏼..',
-    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_generate_chn = {
-    'ru': '👩🏽‍💻 <b>Вставь</b> ссылку на Telegram канал для анализа финансовых показателей',
-    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_generate_wait = {
-    'ru': '👩🏽‍💻 <b>Дождитесь</b> окончания генерации..',
-    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_generate_subcribe = {
-    'ru': '👩🏽‍💻 Подождите {0}сек или оформите подписку',
-    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_generate_error = {
-    'ru': '👩🏽‍💻 <b>Ошибка</b> генерации',
-    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-l_generate_errchn = {
-    'ru': '👩🏽‍💻 <b>Ошибка</b> доступа к каналу (попробуйте позже или сделайте канал публичным)',
-    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
-    'es': '👇🏽 Elige la dirección',
-    'fr': '👇🏽 Choisissez l\'orientation',
-    'zh': '👇🏽 選擇方向',
-    'ar': '👇🏽 اختر الاتجاه',
-}
-# endregion
-
-
 # region post
 l_post_text = {
     'ru': "✏️ 1. Напиши мне <b>текст</b> для нового поста (не забудь использовать <i>форматирование</i>)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 1. Send me <b>text</b> for new post for (don't forget to use <i>formatting</i>)\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
     'es': "✏️ 1. Envíame <b>texto</b> para una nueva publicación (no olvides usar <i>formato</i>)\n\n(<i>o haz clic en «➡️️ /Next» para omitir este paso</i>)",
     'fr': "✏️ 1. Envoyez-moi un <b>texte</b> pour un nouveau message (n'oubliez pas d'utiliser le <i>formatage</i>)\n\n(<i>ou cliquez sur le «➡️️ /Next» pour ignorer cette étape</i>)",
     'zh': "✏️ 1. 給我 <b>文本</b> 對於新職位 (不要忘記使用 <i>格式化</i>)\n\n(<i>或單擊 «➡️️/Next» 跳過這一步</i>)",
@@ -472,15 +171,15 @@
     'en': "✏️ 1. Send changed <b>text</b> for current post\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
     'es': "✏️ 1. Envía el <b>texto</b> modificado para la publicación actual\n\n(<i>o haz clic en «➡️️/Next» para omitir este paso</i>)",
     'fr': "✏️ 1. Envoyez le <b>texte</b> modifié pour le message actuel\n\n(<i>ou cliquez sur « ➡️️/Next» pour ignorer cette étape</i>) ",
     'zh': "✏️ 1. 發送更改 <b>文本</b>對於當前職位\n\n(<i>或單擊 «➡️️/Next» 跳過這一步</i>)",
     'ar': "✏️ 1/3. إرسال <b> النص </b> المتغير للمشاركة الحالية \n\n (<i> أو انقر فوق« ➡️️ /Next التالي »لتخطي هذه الخطوة </i>)",
 }
 l_post_media = {
-    'ru': "✏️ 2. Прикрепи <b>медиа</b> контент: фото/гиф/видео/аудио/документ или запиши голосовое/видео-заметку в кружке\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'ru': "✏️ 2. Прикрепи <b>медиа</b> контент: фото/гиф/видео/аудио/документ/стикер или запиши голосовое/видео-заметку в кружке\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 2. Attach <b>media</b> content: photo/giff/video/audio/document or record voice/video-note\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
     'es': "✏️ 2. Adjunte contenido <b>medios</b>: foto/giff/video/audio/documento o grabe voz/video-nota\n\n(<i>o haz clic en «➡️️/Next» para omitir este paso</i>)",
     'fr': "✏️ 2. Joindre du contenu <b>média</b> : photo/gif/vidéo/audio/document ou enregistrer voix/vidéo-note\n\n(<i>ou cliquer sur « ➡️️/Next » pour ignorer cette étape</i>)",
     'zh': "✏️ 2. 附 <b>媒體</b> 內容: 照片/gif/視頻/音頻/文件 或記錄 嗓音/視頻筆記\n\n(<i>或單擊 «➡️️/Next» 跳過這一步</i>)",
     'ar': "✏️ 2/3. أرفق محتوى <b> الوسائط </b>: صورة / giff / فيديو / صوت / مستند أو سجل ملاحظة صوتية / فيديو \n\n (<i> أو انقر فوق« ➡️️ /Next التالي » لتخطي هذه الخطوة </i>) ",
 }
 l_post_media_wait = {
@@ -552,15 +251,15 @@
     'en': "✏️ 4. Send <b>button-names</b> & <b>links</b> for buttons (1 or more; click on the example below to copy):\n\n<code>[🐳 My profile | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ Very interesting][💔 Do not disturb]</code>\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
     'es': "✏️ 4. Envía nombres de botones y enlaces para botones (1 o más; haz clic en el siguiente ejemplo para copiar):\n\n<code>[🐳 Mi perfil | https://t.me/XXXXX] </code>\n\n\n\n<code>[❤️ Muy interesante][💔 No molestar]</code>\n\n(<i>o haga clic en «➡️️/Next» para omitir esto paso</i>)",
     'fr': "✏️ 4. Envoyez les noms des boutons et les liens pour les boutons (1 ou plusieurs ; cliquez sur l'exemple ci-dessous pour copier) :\n\n<code>[🐳 Mon profil | https://t.me/XXXXX] </code>\n\nили\n\n<code>[❤️ Très intéressant][💔 Ne pas déranger]</code>\n\n(<i>ou cliquez sur « ➡️️/Next » pour ignorer cette étape</i>)",
     'zh': "✏️ 4. 發送按鈕名稱 & 按鈕鏈接 (1 或者更多; 單擊下面的示例進行複制):\n\n<code>[🐳 我的簡歷 | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ 很有意思][💔 請勿打擾]</code>\n\n(<i>或單擊 «➡️️/Next» to skip this step</i>)",
     'ar': "✏️ 3/3. أرسل أسماء الأزرار والروابط للأزرار (1 أو أكثر ؛ انقر على المثال أدناه لنسخه): \n\n <code> [🐳 ملفي الشخصي | https://t.me/XXXXX] </code> \n \n or \n\n <code> [ممتع جدًا] [💔 عدم الإزعاج] </code> \n\n (<i> أو انقر فوق «➡️️ /Next التالي» لتخطي ذلك الخطوة </i>) ",
 }
 l_post_finish = {
-    'ru': "✅ <b>пост готов</b>\n\n<i>Нажми «➡️️/Next», чтобы подтвердить, а затем на кнопку 🔗 Опубликовать</i>",
+    'ru': "✅ <b>Пост готов</b>\n\n<i>Нажми «➡️️/Next», чтобы подтвердить, а затем на кнопку 🔗 Опубликовать</i>",
     'en': "✅ <b>Post is ready</b>\n\n<i>Click the «➡️️/Next» to confirm. Then click the [🔗 Publish]-button</i>",
     'es': "✅ <b>La publicación está lista</b>\n\n<i>Haz clic en «➡️️/Next» para confirmar. Luego haz clic en el botón [🔗 Publicar]</i>",
     'fr': "✅ <b>La publication est prête</b>\n\n<i>Cliquez sur «➡️️/Next» pour confirmer. Cliquez ensuite sur le bouton [🔗 Publier]</i>",
     'zh': "✅ <b>帖子準備好了</b>\n\n<i>點擊 «➡️️/Next» 確認. 然後點擊 [🔗 發布]-按鈕</i>",
     'ar': "✅ <b> النشر جاهز </b> \n\n <i> انقر فوق« ➡️️ /Next التالي »للتأكيد. ثم انقر فوق الزر [🔗 نشر] </i>",
 }
 l_switch_pm_text = {
@@ -591,14 +290,23 @@
     'ru': "♻️ Изменить",
     'en': "♻️ Edit",
     'es': "♻️ Editar",
     'fr': "♻️ Éditer",
     'zh': "♻️ 編輯",
     'ar': "♻️ تعديل",
 }
+l_post_creation = {
+    'ru': "<b>Дата создания</b>",
+    'en': "<b>Publication Datetime</b>",
+    'es': "<b>Creación</b>",
+    'fr': "<b>Création</b>",
+    'zh': "<b>創建</b>",
+    'ar': "<b> إنشاء </b>",
+}
+
 l_post_publish = {
     'ru': "🔗 Опубликовать",
     'en': "🔗 Publish",
     'es': "🔗 Publicar",
     'fr': "🔗 Publier",
     'zh': "🔗 發布",
     'ar': "🔗 نشر",
@@ -607,38 +315,14 @@
     'ru': "👩🏽‍💻 Пост опубликован в канале",
     'en': "🔗 Publish",
     'es': "🔗 Publicar",
     'fr': "🔗 Publier",
     'zh': "🔗 發布",
     'ar': "🔗 نشر",
 }
-l_broadcast_start = {
-    'ru': "🗝️ Start..\n#duration {0}min",
-    'en': "🗝️ Sending is starting..\n#duration {0}min",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_broadcast_process = {
-    'ru': "🗝️ Рассылка..{0}%",
-    'en': "🗝️ Sending..{0}%",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_broadcast_send_finish = {
-    'ru': "🏁 <b>Рассылка</b> завершена\n\n🗝️ число пользователей, получивших сообщение: <u>{0}</u>",
-    'en': "🏁 <b>Sending</b> is finished\n\n🗝️ User count of getting message: <u>{0}</u>",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
 l_post_btn_answer = {
     'ru': "✅ Пользователь <b>{0}</b> (username={1}, id=<code>{2}</code>) <i>нажал</i> на [<b>{3}</b>] в посте #<u>{4}</u>",
     'en': "✅ The user <b>{0}</b> (username={1}, id=<code>{2}</code>) <i>click</i> the [<b>{3}</b>] of post #<u>{4}</u>",
     'es': "✅ El usuario <b>{0}</b> (username={1}, id=<code>{2}</code>) <i>haga clic</i> en [<b>{3}</b>] de la publicación #<u>{4}</u>",
     'fr': "✅ L'utilisateur <b>{0}</b> (username={1}, id=<code>{2}</code>) <i>clique</i> sur le [<b>{3}</b>] du message #<u>{4}</u>",
     'zh': "✅ 用戶 <b>{0}</b> (username={1}, id=<code>{2}</code>) <i>點擊</i> 上 [<b>{3}</b>] 報價的 #<u>{4}</u>",
     'ar': "✅ المستخدم <b>{0}</b> (اسم المستخدم = {1} ، المعرف = <code>{2}</code>) <i> انقر </i> على [<b>{3}</b>] من المشاركة # <u>{4}</u>",
@@ -776,8 +460,745 @@
     'ru': "🕒 Укажи время в будущем",
     'en': "🕒 Specify a time in the future",
     'es': "🕒 Especificar un tiempo en el futuro",
     'fr': "🕒 Spécifiez une heure dans le futur",
     'zh': "🕒 指定未來的時間",
     'ar': "🕒 حدد وقتًا في المستقبل",
 }
+l_me = {
+    'ru': "👤 Себе",
+    'en': "👤 Me",
+    'es': "en",
+    'fr': "sur",
+    'zh': "上",
+    'ar': "على",
+}
+l_all = {
+    'ru': "👥 Всем",
+    'en': "👥 All",
+    'es': "en",
+    'fr': "sur",
+    'zh': "上",
+    'ar': "على",
+}
+l_ids = {
+    'ru': "🙌🏽 По id",
+    'en': "🙌🏽 By id",
+    'es': "en",
+    'fr': "sur",
+    'zh': "上",
+    'ar': "على",
+}
+l_recipient = {
+    'ru': "👩🏽‍💻 <b>Выбери</b> получателя",
+    'en': "👩🏽‍💻 Choose recipient",
+    'es': "en",
+    'fr': "sur",
+    'zh': "上",
+    'ar': "على",
+}
+l_enter = {
+    'ru': "👩🏽‍💻 <b>Введи</b> Ids получателей через пробельные или разделительные символы",
+    'en': "👩🏽‍💻 Введи Ids получателей через пробельные или разделительные символы",
+    'es': "en",
+    'fr': "sur",
+    'zh': "上",
+    'ar': "على",
+}
+offer_has_restricted = {
+    'ru': "👩🏽‍💻 В настройках <b>[Конфиденциальность]</b> добавь @{0} в <i>исключения</i> для <b>[Голосовые сообщения]</b>, чтобы отобразить <code>видео-заметку</code>/<code>голосовое</code>",
+    'en': "off",
+    'es': "apagada",
+    'fr': "à l'arrêt",
+    'zh': "離開",
+    'ar': "إيقاف",
+}
+offer_time_zone = {
+    'ru': "📍 <b>Часовой пояс</b> геопозиции установлен\n\n🕐 Текущее время: <u>{0}</u> ({1}{2} по Гринвичу)",
+    'en': "no",
+    'es': "no",
+    'fr': "non",
+    'zh': "不",
+    'ar': "رقم",
+}
+offer_time_future = {
+    'ru': "🕒 <b>Укажи</b> время в будущем",
+    'en': "🕒 Specify a time in the future",
+    'es': "🕒 Especificar un tiempo en el futuro",
+    'fr': "🕒 Spécifiez une heure dans le futur",
+    'zh': "🕒 指定未來的時間",
+    'ar': "🕒 حدد وقتًا في المستقبل",
+}
+l_broadcast_plan = {
+    'ru': "🗝️ <b>Готово!</b> Рассылка запланирована",
+    'en': "🗝️ Sending is starting..\n#duration {0}min",
+    'es': "🔙 Volver..",
+    'fr': "🔙 Retour..",
+    'zh': "🔙 回來..",
+    'ar': "🔙 رجوع ..",
+}
+l_broadcast_start = {
+    'ru': "🗝️ <b>Старт</b> рассылки..\n#длительность {0}min",
+    'en': "🗝️ Sending is starting..\n#duration {0}min",
+    'es': "🔙 Volver..",
+    'fr': "🔙 Retour..",
+    'zh': "🔙 回來..",
+    'ar': "🔙 رجوع ..",
+}
+l_broadcast_process = {
+    'ru': "🗝️ <b>Рассылка</b>..{0}%",
+    'en': "🗝️ Sending..{0}%",
+    'es': "🔙 Volver..",
+    'fr': "🔙 Retour..",
+    'zh': "🔙 回來..",
+    'ar': "🔙 رجوع ..",
+}
+l_broadcast_finish = {
+    'ru': "🏁 <b>Рассылка</b> завершена\n\n🗝️ Число пользователей, получивших сообщение: <u>{0}</u>",
+    'en': "🏁 <b>Sending</b> is finished\n\n🗝️ User count of getting message: <u>{0}</u>",
+    'es': "🔙 Volver..",
+    'fr': "🔙 Retour..",
+    'zh': "🔙 回來..",
+    'ar': "🔙 رجوع ..",
+}
+
+l_generate_calendar_time = {
+    'ru': "🕒 Отправь <b>время</b> поста на {0} в формате <code>{1}</code>. Текущее время: <u>{2}</u> ({3} по Гринвичу)\n\n🔗 Пришли <b>геопозицию</b>, чтобы <i>автоматически</i> определить часовой пояс",
+    'en': "🕒 Send <b>time</b> for post (<i>in hours and minutes on UTC-Greenwich</i>) for {0} in format <code>{1}</code> (current time: {2})",
+    'es': "🕒 Enviar <b>hora</b> para la publicación (<i>en horas y minutos en UTC-Greenwich</i>) para {0} en formato <code>{1}</code> (hora actual: {2})",
+    'fr': "🕒 Envoyer <b>heure</b> pour la poste (<i>en heures et minutes sur UTC-Greenwich</i>) pour {0} au format <code>{1}</code> (heure actuelle : {2})",
+    'zh': "🕒 以 <code>{1}</code> 格式發送 {0} 的 <b>時間</b> （<i>UTC-格林威治的小時和分鐘</i>）（當前時間：{2}）",
+    'ar': "🕒 أرسل <b> الوقت </b> للنشر (<i> بالساعات والدقائق على UTC-Greenwich </i>) لـ {0} بالتنسيق <code>{1}</code> (الوقت الحالي: {2})",
+}
+l_month_1 = {
+    'ru': "Янв",
+    'en': "Jan",
+    'es': "enero",
+    'fr': "janvier",
+    'zh': "一月",
+    'ar': "كانون الثاني",
+}
+l_month_2 = {
+    'ru': "Фев",
+    'en': "Feb",
+    'es': "febrero",
+    'fr': "février",
+    'zh': "二月",
+    'ar': "كانون الثاني",
+}
+l_month_3 = {
+    'ru': "Мар",
+    'en': "Mar",
+    'es': "Marzo",
+    'fr': "Mars",
+    'zh': "行進",
+    'ar': "يمشي",
+}
+l_month_4 = {
+    'ru': "Апр",
+    'en': "april",
+    'es': "abril",
+    'fr': "avril",
+    'zh': "四月",
+    'ar': "أبريل",
+}
+l_month_5 = {
+    'ru': "Май",
+    'en': "May",
+    'es': "Mayo",
+    'fr': "Peut",
+    'zh': "可能",
+    'ar': "مايو",
+}
+l_month_6 = {
+    'ru': "Июн",
+    'en': "Jun",
+    'es': "Junio",
+    'fr': "Juin",
+    'zh': "六月",
+    'ar': "يونيو",
+}
+l_month_7 = {
+    'ru': "Июл",
+    'en': "Jul",
+    'es': "Julio",
+    'fr': "Juillet",
+    'zh': "七月",
+    'ar': "يوليو",
+}
+l_month_8 = {
+    'ru': "Авг",
+    'en': "Aug",
+    'es': "agosto",
+    'fr': "août",
+    'zh': "八月",
+    'ar': "شهر اغسطس",
+}
+l_month_9 = {
+    'ru': "Сен",
+    'en': "Sep",
+    'es': "septiembre",
+    'fr': "septembre",
+    'zh': "九月",
+    'ar': "شهر سبتمبر",
+}
+l_month_10 = {
+    'ru': "Окт",
+    'en': "Oct",
+    'es': "octubre",
+    'fr': "octobre",
+    'zh': "十月",
+    'ar': "اكتوبر",
+}
+l_month_11 = {
+    'ru': "Ноя",
+    'en': "Nov",
+    'es': "noviembre",
+    'fr': "novembre",
+    'zh': "十一月",
+    'ar': "شهر نوفمبر",
+}
+l_month_12 = {
+    'ru': "Дек",
+    'en': "Dec",
+    'es': "diciembre",
+    'fr': "décembre",
+    'zh': "十二月",
+    'ar': "ديسمبر",
+}
+
+l_weekday_1 = {
+    'ru': "пн",
+    'en': "Dec",
+    'es': "diciembre",
+    'fr': "décembre",
+    'zh': "十二月",
+    'ar': "ديسمبر",
+}
+l_weekday_2 = {
+    'ru': "вт",
+    'en': "Dec",
+    'es': "diciembre",
+    'fr': "décembre",
+    'zh': "十二月",
+    'ar': "ديسمبر",
+}
+l_weekday_3 = {
+    'ru': "ср",
+    'en': "Dec",
+    'es': "diciembre",
+    'fr': "décembre",
+    'zh': "十二月",
+    'ar': "ديسمبر",
+}
+l_weekday_4 = {
+    'ru': "чт",
+    'en': "Dec",
+    'es': "diciembre",
+    'fr': "décembre",
+    'zh': "十二月",
+    'ar': "ديسمبر",
+}
+l_weekday_5 = {
+    'ru': "пт",
+    'en': "Dec",
+    'es': "diciembre",
+    'fr': "décembre",
+    'zh': "十二月",
+    'ar': "ديسمبر",
+}
+l_weekday_6 = {
+    'ru': "сб",
+    'en': "Dec",
+    'es': "diciembre",
+    'fr': "décembre",
+    'zh': "十二月",
+    'ar': "ديسمبر",
+}
+l_weekday_7 = {
+    'ru': "вс",
+    'en': "Dec",
+    'es': "diciembre",
+    'fr': "décembre",
+    'zh': "十二月",
+    'ar': "ديسمبر",
+}
+
+l_inline_demo = {
+    'ru': "обо всех проектах",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_bot = {
+    'ru': "конструктор ботов",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_post = {
+    'ru': "конструктор офферов",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_media = {
+    'ru': "конструктор медиа-заметок",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_channel = {
+    'ru': "администратор каналов",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_group = {
+    'ru': "администратор групп",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_find = {
+    'ru': "бот для поиска",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_ai = {
+    'ru': "бот с нейросетью",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_ads = {
+    'ru': "рекламный бот",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_vpn = {
+    'ru': "vpn-бот",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_target = {
+    'ru': "таргет-бот",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_user = {
+    'ru': "администратор пользователя",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_tools = {
+    'ru': "Telegram-инструменты",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+l_inline_work = {
+    'ru': "вакансии/конкурсы",
+    'en': "forever",
+    'es': "siempre",
+    'fr': "toujours",
+    'zh': "永遠",
+    'ar': "إلى الأبد",
+}
+# endregion
+
+
+# region FereyDemoBot
+l_demo_btn1 = {
+    'ru': '⛰️ Проекты',
+    'en': '⛰️ Projects',
+    'es': '⛰️ Projects',
+    'fr': '⛰️ Projects',
+    'zh': '⛰️ 團體',
+    'ar': '⛰️ مجموعات',
+}
+l_demo_btn2 = {
+    'ru': '🌬 Подписка',
+    'en': '🌬 Subcribe',
+    'es': '🌬 Sobre',
+    'fr': '🌬 À propos de',
+    'zh': '🌬 關於',
+    'ar': '🌬 حول',
+}
+l_demo_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>информация</b> обо всех проектах\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
+    'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
+}
+
+l_kind_1 = {
+    'ru': '<b>👩🏽‍💻@FereyDemoBot</b>\n\nДемонстрационный бот всех проектов',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_2 = {
+    'ru': '<b>👩🏽‍💻@FereyBotBot</b>\n\nКонструктор ботов:\n▪️авто-генерация бота\n▪️авто-генерация контента (open-ai)\n▪️авто-бан/авто-перевод',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_3 = {
+    'ru': '<b>👩🏽‍💻@FereyChannelBot</b>\n\nАдминистратор каналов:\n▪️авто-постинг\n▪️авто-декор',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_4 = {
+    'ru': '<b>👩🏽‍💻@FereyGroupBot</b>\n\nАдминистратор групп:\n▪️авто-постинг\n▪️модерация',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_5 = {
+    'ru': '<b>👩🏽‍💻@FereyUserBot</b>\n\nАдминистратор пользователей:\n▪️авто-постинг\n▪️авто-декор',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_6 = {
+    'ru': '<b>👩🏽‍💻@FereyPostBot</b>\n\nБыстрое создание и публикация постов:\n▪️превью\n▪️галерея',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_7 = {
+    'ru': '<b>👩🏽‍💻@FereyFindBot</b>\n\nПоиск по каналам/группам/пользователям/ботам:\n▪️отслеживание постов\n▪️гео-поиск',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_8 = {
+    'ru': '<b>👩🏽‍💻@FereyMediaBot</b>\n\nБот с популярными креативами:\n▪️аудио-заметки\n▪️видео-заметки',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_9 = {
+    'ru': '<b>👩🏽‍💻@FereyVpnBot</b>\n\nВсе о VPN',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_10 = {
+    'ru': '<b>👩🏽‍💻@FereyTargetBot</b>\n\nТаргетированная рассылка',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_11 = {
+    'ru': '<b>👩🏽‍💻@FereyToolsBot</b>\n\nБот инструментов:\n▪️конвертация\n▪️загрузка',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_12 = {
+    'ru': '<b>👩🏽‍💻@FereyAIBot</b>\n\nБот генерации контента (open-ai):\n▪️chat-gpt\n▪️dalli·e',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_13 = {
+    'ru': '<b>👩🏽‍💻@FereyAdsBot</b>\n\nБот рекламы в:\n▪️ботах\n▪️каналах',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_kind_14 = {
+    'ru':  '<b>👩🏽‍💻@FereyWorkBot</b>\n\nБот информации о:\n▪️вакансиях\n▪️соревнованиях',
+    'en': '👇🏽 Choose direction',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+# endregion
+
+
+# region FereyWorkBot
+l_work_btn1 = {
+    'ru': '⛰️ Вакансии',
+    'en': '⛰️ Projects',
+    'es': '⛰️ Projects',
+    'fr': '⛰️ Projects',
+    'zh': '⛰️ 團體',
+    'ar': '⛰️ مجموعات',
+}
+l_work_btn2 = {
+    'ru': '🌬 Подписка',
+    'en': '🌬 Subcribe',
+    'es': '🌬 Sobre',
+    'fr': '🌬 À propos de',
+    'zh': '🌬 關於',
+    'ar': '🌬 حول',
+}
+l_work_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>вакансии</b> нашего стартапа\n▪️конкурсы и <b>мероприятия</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
+    'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
+}
+l_vacancy_1 = {
+    'ru': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'en': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'es': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'fr': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'zh': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'ar': '👩🏽‍💻 <b>Text to video ai-designer</b>\n\nTasks: create ferey-masks (realistic video) for any human\nGender: girl\nAge: less than 30\nPay: share of the company',
+}
+l_vacancy_2 = {
+    'ru': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+    'en': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+    'es': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+    'fr': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+    'zh': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+    'ar': '👩🏽‍💻 <b>Content/video maker</b>\n\nTasks: generate creatives for all socials\nGender: girl\nAge: less than 30\nPay: 1 TON per 1 post for all socials',
+}
+l_vacancy_3 = {
+    'ru': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'en': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'es': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'fr': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'zh':'👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+    'ar': '👩🏽‍💻 <b>Aio/pyro-gram developer</b>\n\nTasks: dev and support all projects\nGender: girl\nAge: less than 30\nPay: share of the company',
+}
+# endregion
+
+
+# region FereyAIBot
+l_ai_btn1 = {
+    'ru': '⛰️ Нейросети',
+    'en': '⛰️ Projects',
+    'es': '⛰️ Projects',
+    'fr': '⛰️ Projects',
+    'zh': '⛰️ 團體',
+    'ar': '⛰️ مجموعات',
+}
+l_ai_btn2 = {
+    'ru': '🌬 Подписка',
+    'en': '🌬 Subcribe',
+    'es': '🌬 Sobre',
+    'fr': '🌬 À propos de',
+    'zh': '🌬 關於',
+    'ar': '🌬 حول',
+}
+l_ai_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>генерации</code> контента:\n\n▪️<b>текст</b>\n▪️<b>изображение</b>\n▪️<b>анализ Telegram-канала</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
+    'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
+}
+l_gen_txt = {
+    'ru': "📘 Текст{0}",
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_gen_img = {
+    'ru': "🌌 Образ",
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_gen_tlg = {
+    'ru': "👩🏽‍💻 Анализ Telegram-канала",
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_main = {
+    'ru': '👩🏽‍💻 <b>Выбери режим</b>',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_prompt = {
+    'ru': '👩🏽‍💻 <b>Введи</b> запрос для <b>{0}</b> 👇🏼..',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_chn = {
+    'ru': '👩🏽‍💻 <b>Вставь</b> ссылку на Telegram канал для анализа финансовых показателей',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_wait = {
+    'ru': '👩🏽‍💻 <b>Дождитесь</b> окончания генерации..',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_subcribe = {
+    'ru': '👩🏽‍💻 Подождите {0}сек или оформите подписку',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_error = {
+    'ru': '👩🏽‍💻 <b>Ошибка</b> генерации',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+l_generate_errchn = {
+    'ru': '👩🏽‍💻 <b>Ошибка</b> доступа к каналу (попробуйте позже или сделайте канал публичным)',
+    'en': '👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link',
+    'es': '👇🏽 Elige la dirección',
+    'fr': '👇🏽 Choisissez l\'orientation',
+    'zh': '👇🏽 選擇方向',
+    'ar': '👇🏽 اختر الاتجاه',
+}
+# endregion
+
+
+# region FereyAdsBot
+l_ads_btn1 = {
+    'ru': '⛰️ Посты',
+    'en': '⛰️ Projects',
+    'es': '⛰️ Projects',
+    'fr': '⛰️ Projects',
+    'zh': '⛰️ 團體',
+    'ar': '⛰️ مجموعات',
+}
+l_ads_btn2 = {
+    'ru': '🌬 Подписка',
+    'en': '🌬 Subcribe',
+    'es': '🌬 Sobre',
+    'fr': '🌬 À propos de',
+    'zh': '🌬 關於',
+    'ar': '🌬 حول',
+}
+l_ads_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных <code>постов</code> <b>Ferey</b>\n\n▪️️реклама во всех Ferey-ботах\n▪️️заказ рекламы на канале\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
+    'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
+}
+l_post_media_ads = {
+    'ru': "✏️ 2. Прикрепи <b>медиа</b> контент: фото/гиф/видео до 5Mb\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'en': "✏️ 2. Attach <b>media</b> content: photo/giff/video/audio/document or record voice/video-note\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
+    'es': "✏️ 2. Adjunte contenido <b>medios</b>: foto/giff/video/audio/documento o grabe voz/video-nota\n\n(<i>o haz clic en «➡️️/Next» para omitir este paso</i>)",
+    'fr': "✏️ 2. Joindre du contenu <b>média</b> : photo/gif/vidéo/audio/document ou enregistrer voix/vidéo-note\n\n(<i>ou cliquer sur « ➡️️/Next » pour ignorer cette étape</i>)",
+    'zh': "✏️ 2. 附 <b>媒體</b> 內容: 照片/gif/視頻/音頻/文件 或記錄 嗓音/視頻筆記\n\n(<i>或單擊 «➡️️/Next» 跳過這一步</i>)",
+    'ar': "✏️ 2/3. أرفق محتوى <b> الوسائط </b>: صورة / giff / فيديو / صوت / مستند أو سجل ملاحظة صوتية / فيديو \n\n (<i> أو انقر فوق« ➡️️ /Next التالي » لتخطي هذه الخطوة </i>) ",
+}
+# endregion
+
+
+# region FereyPostBot
+l_post_btn1 = {
+    'ru': '⛰️ Посты',
+    'en': '⛰️ Projects',
+    'es': '⛰️ Projects',
+    'fr': '⛰️ Projects',
+    'zh': '⛰️ 團體',
+    'ar': '⛰️ مجموعات',
+}
+l_post_btn2 = {
+    'ru': '🌬 Подписка',
+    'en': '🌬 Subcribe',
+    'es': '🌬 Sobre',
+    'fr': '🌬 À propos de',
+    'zh': '🌬 關於',
+    'ar': '🌬 حول',
+}
+l_post_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных <code>постов</code> <b>Ferey</b>\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'en': "🌱 {0}, welcome to <i>landing-bot</i> for <code>administration</code> <b>Telegram</b>-channels:\n\n▪️<b>pretecting</b> channel from spy-joining of\n▪️store offers in <b>unique</b> space\n▪️defend offers form <b>auto</b> deleted* \n(*even it has stop-words)\n\n❗️to order chat-bot-development go to <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'es': "🌱 {0}, Bienvenida(o) a <i>lugar de aterrizaje-bot</i> por <code>creando & publicando</code> <b>Telegram</b>-Grupos:\n\n▪️️crear <b>cualquier</b> tipo de oferta (con botones)\n▪️almacenar ofertas en un espacio <b>único</b>\n▪️️defend ofrece formulario <b>auto</b> borrado* \n(*incluso tiene palabras vacías)\n\n❗️para ordenar chat-bot-desarrollo vaya a <a href='https://t.me/{1}'>Ferey</a>-estudio",
+    'fr': "🌱 {0}, bienvenue sur <i>landing-bot</i> pour la <code>création et publication</code> <b>Télégramme</b>-channeles:\n\n▪️créer <b>tout </b> type d'offre (avec boutons)\n▪️stocker les offres dans un espace <b>unique</b>\n▪️défendre les offres sous forme <b>auto</b> supprimées* \n(*même si elles ont cessé -words)\n\n❗️pour commander le développement de chat-bot, rendez-vous sur <a href='https://t.me/{1}'>Ferey</a>-studio",
+    'zh': "🌱 {0}, 歡迎來到 <i>著陸點-bot</i> 為了 <code>創造 & 張貼</code> <b>Telegram</b>-團體:\n\n▪️️創造 <b>任何</b> 報價類型 (帶按鈕)\n▪️商店優惠在 <b>獨特的</b> 獨特的\n▪️捍衛報價表格自動刪除* \n(*捍衛自動刪除的提議)\n\n❗️訂購 Telegram-bot 去 <a href='https://t.me/{1}'>Ferey</a>-工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i> برنامج التتبع </i> من أجل الإنشاء والنش Telegram - مجموعات: \n\n▪️ إنشاء <b> أي </b> نوع العرض (مع الأزرار) \n▪️ عروض المتجر في مساحة فريدة \n▪️ الدفاع عن نموذج عروض <b> تلقائي </b> محذوفة * \n (* حتى إذا توقفت -كلمات) \n\n لطلب تطوير chat-bot-انتقل إلى <a href='https://t.me/{1}'>Ferey</a>-studio"
+}
+
 # endregion
```

### Comparing `yeref-0.1.40/yeref/yeref.py` & `yeref-0.1.41/yeref/yeref.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/python3
 # region data
 import ast
 import asyncio
 import datetime
 import io
+import json
 import logging
 import mimetypes
 import os
 import random
 import re
 import shutil
 import sqlite3
@@ -55,18 +56,22 @@
     '6281795468',
 ]
 old_tid = 4_000_000_000
 lat_company = 59.395881
 long_company = 24.658980
 lkjhgfdsa_channel_id = -1001657854832
 lkjhgfdsa_channel_un = "lkjhgfdsa_channel"
+tg_ch_ads_un = 'kiejakn3_djdjn4m_ads'
+tg_ch_ads_id = -1001921910898
 price_one = 200
 price_all = 500
 
 TGPH_TOKEN_BAN = 'a9335172886eae62ec0743bf8a4e195286ec30cff067da5fd1db2899d008'
+TGPH_TOKEN_BROADCAST = 'b348a7a3964bbb4df2b66f8dbcd142e9dbf22ce58478a96bab3761dba51c'
+pp = 'https://telegra.ph/broadcasting-04-22'
 SECTION = 'CONFIG'
 LINES_ON_PAGE = 5
 short_name = 'me'
 const_url = 'https://t.me/'
 phone_number = '79999999999'
 vk_group = 'https://vk.com'
 vk_account = 'https://vk.com'
@@ -208,14 +213,20 @@
 
                     if str(chat_id) in ban_ids:
                         return True
                     break
             except Exception as e:
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
+
+        # telegraph_ = Telegraph(access_token=TGPH_TOKEN_BAN)
+        # html_ = {'one': '1', 'two': '2'}
+        # html_ = json.dumps(html_, ensure_ascii=False)
+        # page_ = telegraph_.create_page(title='broadcasting', html_content=html_, author_name='bot_username', author_url='https://t.me/bot_username', return_content=True)
+        # page_url = page_['url']
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
@@ -290,34 +301,115 @@
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
+async def check_tgph_posts(bot_username, BASE_D):
+    try:
+        telegraph_ = Telegraph(access_token=TGPH_TOKEN_BAN)
+        pages = telegraph_.get_page_list()
+
+        for item in pages['pages']:
+            try:
+                if item['path'] == 'broadcasting-04-22':
+                    page = telegraph_.get_page(path=item['path'], return_content=True, return_html=False)
+                    content_json = json.loads(str(page['content'][0]))
+
+                    for OFFER_USERTID, v in content_json.items():
+                        if bot_username in v['bots']:
+                            bots_, OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, \
+                                OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, \
+                                OFFER_ISGALLERY, OFFER_DT, OFFER_TZ = v
+
+                            sql = "INSERT OR IGNORE INTO OFFER (OFFER_USERTID, OFFER_TEXT, OFFER_MEDIATYPE, " \
+                                  "OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, OFFER_ISTGPH, " \
+                                  "OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT, " \
+                                  "OFFER_TZ) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)"
+                            await db_change(sql, (int(OFFER_USERTID), v[OFFER_TEXT], v[OFFER_MEDIATYPE],
+                                                  v[OFFER_FILEID], v[OFFER_BUTTON], v[OFFER_ISBUTTON],
+                                                  v[OFFER_TGPHLINK], v[OFFER_ISTGPH], v[OFFER_ISSPOILER],
+                                                  v[OFFER_ISPIN], v[OFFER_ISSILENCE], v[OFFER_ISGALLERY],
+                                                  v[OFFER_DT], v[OFFER_TZ],), BASE_D)
+
+                            v['bots'].remove(bot_username)
+                            if not len(v['bots']):
+                                del content_json[str(OFFER_USERTID)]
+                            else:
+                                content_json[str(OFFER_USERTID)] = v
+
+                            post_dumps = json.dumps(content_json, ensure_ascii=False)
+                            telegraph_.edit_page(path=item['path'], title="broadcasting", html_content=post_dumps)
+                    break
+            except Exception as e:
+                logger.info(log_ % str(e))
+                await asyncio.sleep(round(random.uniform(0, 1), 2))
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
+        await asyncio.sleep(e.retry_after + 1)
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+
+
+async def post_offer(bot, data, BASE_D):
+    try:
+        for item in data:
+            try:
+                OFFER_ID, OFFER_USERTID, OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_FILEIDNOTE, OFFER_BUTTON, OFFER_ISBUTTON, \
+                    OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, \
+                    OFFER_DT, OFFER_TZ = item
+
+                sign_ = OFFER_TZ[0]
+                h_, m_ = OFFER_TZ.strip(sign_).split(':')
+                dt_now = datetime.datetime.utcnow()
+                if sign_ == "+":
+                    dt_cur = dt_now + datetime.timedelta(hours=int(h_), minutes=int(m_))
+                else:
+                    dt_cur = dt_now - datetime.timedelta(hours=int(h_), minutes=int(m_))
+                timedelta_ = (dt_cur - datetime.datetime.strptime(OFFER_DT, "%d-%m-%Y %H:%M"))
+
+                if timedelta_.days >= 0 and timedelta_.seconds >= 0:
+                    sql = "UPDATE OFFER SET OFFER_DT=NULL, OFFER_STATUS=0 WHERE OFFER_ID=?"
+                    await db_change(sql, (OFFER_ID,), BASE_D)
+
+                    loop_minute = asyncio.get_event_loop()
+                    loop_minute.create_task(broadcast_send_admin(bot, OFFER_USERTID, 'en', OFFER_ID, BASE_D, []))
+            except Exception as e:
+                logger.info(log_ % str(e))
+                await asyncio.sleep(round(random.uniform(0, 1), 2))
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
+        await asyncio.sleep(e.retry_after + 1)
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(0, 1), 2))
+
+
 async def bots_by_inline(chat_id, message, BASE_D):
     result = []
     try:
         lz = await lz_code(chat_id, message.from_user.language_code, BASE_D)
 
         data = [
-            ['👩🏽‍💻 @FereyDemoBot', l_inline_demo[lz], 'https://t.me/FereyDemoBot'],
-            ['👩🏽‍💻 @FereyBotBot', l_inline_bot[lz], 'https://t.me/FereyBotBot'],
-            ['👩🏽‍💻 @FereyPostBot', l_inline_post[lz], 'https://t.me/FereyPostBot'],
-            ['👩🏽‍💻 @FereyMediaBot', l_inline_media[lz], 'https://t.me/FereyMediaBot'],
-            ['👩🏽‍💻 @FereyChannelBot', l_inline_channel[lz], 'https://t.me/FereyChannelBot'],
-            ['👩🏽‍💻 @FereyGroupBot', l_inline_group[lz], 'https://t.me/FereyGroupBot'],
-            ['👩🏽‍💻 @FereyFindBot', l_inline_find[lz], 'https://t.me/FereyFindBot'],
-            ['👩🏽‍💻 @FereyAIBot', l_inline_ai[lz], 'https://t.me/FereyAIBot'],
-            ['👩🏽‍💻 @FereyAdsBot', l_inline_ads[lz], 'https://t.me/FereyAdsBot'],
-            ['👩🏽‍💻 @FereyVPNBot', l_inline_vpn[lz], 'https://t.me/FereyVPNBot'],
-            ['👩🏽‍💻 @FereyTargetBot', l_inline_target[lz], 'https://t.me/FereyTargetBot'],
-            ['👩🏽‍💻 @FereyUserBot', l_inline_user[lz], 'https://t.me/FereyUserBot'],
-            ['👩🏽‍💻 @FereyToolsBot', l_inline_tools[lz], 'https://t.me/FereyToolsBot'],
-            ['👩🏽‍💻 @FereyWorkBot', l_inline_work[lz], 'https://t.me/FereyWorkBot'],
+            ['👩🏽‍💻 @FereyDemoBot', yeref.l_inline_demo[lz], 'https://t.me/FereyDemoBot'],
+            ['👩🏽‍💻 @FereyBotBot', yeref.l_inline_bot[lz], 'https://t.me/FereyBotBot'],
+            ['👩🏽‍💻 @FereyPostBot', yeref.l_inline_post[lz], 'https://t.me/FereyPostBot'],
+            ['👩🏽‍💻 @FereyMediaBot', yeref.l_inline_media[lz], 'https://t.me/FereyMediaBot'],
+            ['👩🏽‍💻 @FereyChannelBot', yeref.l_inline_channel[lz], 'https://t.me/FereyChannelBot'],
+            ['👩🏽‍💻 @FereyGroupBot', yeref.l_inline_group[lz], 'https://t.me/FereyGroupBot'],
+            ['👩🏽‍💻 @FereyFindBot', yeref.l_inline_find[lz], 'https://t.me/FereyFindBot'],
+            ['👩🏽‍💻 @FereyAIBot', yeref.l_inline_ai[lz], 'https://t.me/FereyAIBot'],
+            ['👩🏽‍💻 @FereyAdsBot', yeref.l_inline_ads[lz], 'https://t.me/FereyAdsBot'],
+            ['👩🏽‍💻 @FereyVPNBot', yeref.l_inline_vpn[lz], 'https://t.me/FereyVPNBot'],
+            ['👩🏽‍💻 @FereyTargetBot', yeref.l_inline_target[lz], 'https://t.me/FereyTargetBot'],
+            ['👩🏽‍💻 @FereyUserBot', yeref.l_inline_user[lz], 'https://t.me/FereyUserBot'],
+            ['👩🏽‍💻 @FereyToolsBot', yeref.l_inline_tools[lz], 'https://t.me/FereyToolsBot'],
+            ['👩🏽‍💻 @FereyWorkBot', yeref.l_inline_work[lz], 'https://t.me/FereyWorkBot'],
         ]
 
         for i in range(0, len(data)):
             title, desc, text = data[i]
 
             input_message_content = types.InputTextMessageContent(message_text=text, disable_web_page_preview=False)
             result.append(types.InlineQueryResultArticle(id=str(uuid4()),
@@ -350,617 +442,14 @@
     finally:
         return result
 
 
 # endregion
 
 
-# region l_
-l_offer_text = {
-    'ru': "✏️ 1/4. Напиши мне <b>текст</b> для нового оффера (не забудь использовать <i>форматирование</i>)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
-    'en': "✏️ 1/4. Send me <b>text</b> for new post for (don't forget to use <i>formatting</i>)\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
-    'es': "✏️ 1/4. Envíame <b>texto</b> para una nueva publicación (no olvides usar <i>formato</i>)\n\n(<i>o haz clic en «➡️️ /Next» para omitir este paso</i>)",
-    'fr': "✏️ 1/4. Envoyez-moi un <b>texte</b> pour un nouveau message (n'oubliez pas d'utiliser le <i>formatage</i>)\n\n(<i>ou cliquez sur le «➡️️ /Next» pour ignorer cette étape</i>)",
-    'zh': "✏️ 1/4. 給我 <b>文本</b> 對於新職位 (不要忘記使用 <i>格式化</i>)\n\n(<i>或單擊 «➡️️/Next» 跳過這一步</i>)",
-    'ar': "✏️ 1/3. أرسل لي <b> نصًا </b> للنشر الجديد إلى عن على (لا تنس استخدام <i> تنسيق </i>) \n\n (<i> أو انقر فوق« ➡️️ /Next التالي »لتخطي هذه الخطوة </i>)",
-}
-l_offer_text_limit = {
-    'ru': "❗️ Количество <b>символов</b> текста (<i>включая форматирование</i>): <u>{0}</u> больше допустимых 1024",
-    'en': "❗️ Number of text-symbols (<i>include formatting</i>): <u>{0}</u> more allowed 1024",
-    'es': "❗️ Recuento de símbolos de texto (<i>incluye formato</i>): <u>{0}</u> más 1024 permitidos",
-    'fr': "❗️ Nombre de symboles textuels (<i>inclure la mise en forme</i>) : <u>{0}</u> plus autorisé 1024",
-    'zh': "❗️ 文本符號數 (<i>包括格式</i>): <u>{0}</u> 更多允許 1024",
-    'ar': "❗️ عدد رموز النص (<i> تضمين التنسيق </i>): <u>{0}</u> أكثر مسموحًا بـ 1024",
-}
-l_offer_text_empty = {
-    'ru': "❗️ Оффер пустой, попробуй сначала\n\n{0}",
-    'en': "❗️ The post is empty! Please, try again\n\n{0}",
-    'es': "❗️ ¡La publicación está vacía! Inténtalo de nuevo\n\n{0}",
-    'fr': "❗️ La publication est vide ! Veuillez réessayer\n\n{0}",
-    'zh': "❗️ 帖子為空! 請再試一次\n\n{0}",
-    'ar': "❗️ المنشور فارغ! من فضلك ، حاول مرة أخرى \n\n{0}",
-}
-l_offer_edit = {
-    'ru': "✏️ 1/4. Отправь измененный <b>текст</b> для текущего оффера\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
-    'en': "✏️ 1/4. Send changed <b>text</b> for current post\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
-    'es': "✏️ 1/4. Envía el <b>texto</b> modificado para la publicación actual\n\n(<i>o haz clic en «➡️️/Next» para omitir este paso</i>)",
-    'fr': "✏️ 1/4. Envoyez le <b>texte</b> modifié pour le message actuel\n\n(<i>ou cliquez sur « ➡️️/Next» pour ignorer cette étape</i>) ",
-    'zh': "✏️ 1/4. 發送更改 <b>文本</b>對於當前職位\n\n(<i>或單擊 «➡️️/Next» 跳過這一步</i>)",
-    'ar': "✏️ 1/3. إرسال <b> النص </b> المتغير للمشاركة الحالية \n\n (<i> أو انقر فوق« ➡️️ /Next التالي »لتخطي هذه الخطوة </i>)",
-}
-l_offer_media = {
-    'ru': "✏️ 2/4. Прикрепи <b>медиа</b> контент: фото/гиф/видео/аудио/документ или запиши голосовое/видео-заметку в кружке\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
-    'en': "✏️ 2/4. Attach <b>media</b> content: photo/giff/video/audio/document or record voice/video-note\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
-    'es': "✏️ 2/4. Adjunte contenido <b>medios</b>: foto/giff/video/audio/documento o grabe voz/video-nota\n\n(<i>o haz clic en «➡️️/Next» para omitir este paso</i>)",
-    'fr': "✏️ 2/4. Joindre du contenu <b>média</b> : photo/gif/vidéo/audio/document ou enregistrer voix/vidéo-note\n\n(<i>ou cliquer sur « ➡️️/Next » pour ignorer cette étape</i>)",
-    'zh': "✏️ 2/4. 附 <b>媒體</b> 內容: 照片/gif/視頻/音頻/文件 或記錄 嗓音/視頻筆記\n\n(<i>或單擊 «➡️️/Next» 跳過這一步</i>)",
-    'ar': "✏️ 2/3. أرفق محتوى <b> الوسائط </b>: صورة / giff / فيديو / صوت / مستند أو سجل ملاحظة صوتية / فيديو \n\n (<i> أو انقر فوق« ➡️️ /Next التالي » لتخطي هذه الخطوة </i>) ",
-}
-l_offer_media_wait = {
-    'ru': "🎥 Ожидайте обработки {0}..\n#длительность {1}мин",
-    'en': "🎥 Processing {0}..\n#duration {1}min",
-    'es': "🎥 Procesando {0}..\n#duración {1}min",
-    'fr': "🎥 Traitement {0}..\n#durée {1}min",
-    'zh': "🎥 加工 {0}..\n#期間 {1}min",
-    'ar': "🎥 معالجة {0} .. \n # مدة {1} دقيقة",
-}
-l_offer_media_toobig = {
-    'ru': f"📨️ Файл больше 20 Мб, загрузи меньший обьем",
-    'en': f"📨️ File more than 20 Mb. Please, reduce size of file",
-    'es': f"📨️ Archivo de más de 20 Mb. Por favor, reduzca el tamaño del archivo",
-    'fr': f"📨️ Fichier de plus de 20 Mo. Veuillez réduire la taille du fichier",
-    'zh': f"📨️ 文件超過 20 Mb. 請減小文件大小",
-    'ar': f"📨️ الملف أكبر من 20 ميغا بايت. الرجاء تقليل حجم الملف",
-}
-l_offer_button = {
-    'ru': "✏️ 3/4. Отправь <b>названия</b> для кнопок и <b>ссылки</b> в формате (одну или несколько; кликни на образец ниже, чтобы скопировать):\n\n<code>[🐳 Ссылка | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ Интересно][💔 Не пишите]</code>\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
-    'en': "✏️ 3/4. Send <b>button-names</b> & <b>links</b> for buttons (1 or more; click on the example below to copy):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ Very interesting][💔 Do not disturb]</code>\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
-    'es': "✏️ 3/4. Envía nombres de botones y enlaces para botones (1 o más; haz clic en el siguiente ejemplo para copiar):\n\n<code>[🐳 Enlace | https://t.me/XXXXX] </code>\n\n\n\n<code>[❤️ Muy interesante][💔 No molestar]</code>\n\n(<i>o haga clic en «➡️️/Next» para omitir esto paso</i>)",
-    'fr': "✏️ 3/4. Envoyez les noms des boutons et les liens pour les boutons (1 ou plusieurs ; cliquez sur l'exemple ci-dessous pour copier) :\n\n<code>[🐳 Lien | https://t.me/XXXXX] </code>\n\nили\n\n<code>[❤️ Très intéressant][💔 Ne pas déranger]</code>\n\n(<i>ou cliquez sur « ➡️️/Next » pour ignorer cette étape</i>)",
-    'zh': "✏️ 3/4. 發送按鈕名稱 & 按鈕鏈接 (1 或者更多; 單擊下面的示例進行複制):\n\n<code>[🐳 關聯 | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ 很有意思][💔 請勿打擾]</code>\n\n(<i>或單擊 «➡️️/Next» to skip this step</i>)",
-    'ar': "✏️ 3/3. أرسل أسماء الأزرار والروابط للأزرار (1 أو أكثر ؛ انقر على المثال أدناه لنسخه): \n\n <code> [🐳 صلة | https://t.me/XXXXX] </code> \n \n or \n\n <code> [ممتع جدًا] [💔 عدم الإزعاج] </code> \n\n (<i> أو انقر فوق «➡️️ /Next التالي» لتخطي ذلك الخطوة </i>) ",
-}
-l_offer_button_urlinvalid = {
-    'ru': "🔗 Ссылка {0} не действительна",
-    'en': "🔗 Url {0} is invalid",
-    'es': "🔗 URL {0} no es válida",
-    'fr': "🔗L'URL {0} n'est pas valide",
-    'zh': "🔗 網址 {0} 無效",
-    'ar': "🔗 عنوان {0} غير صالح",
-}
-l_offer_date = {
-    'ru': "✏️ 4/4. Выбери дату на календаре\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
-    'en': "✏️ 4/4. Send <b>button-names</b> & <b>links</b> for buttons (1 or more; click on the example below to copy):\n\n<code>[🐳 My profile | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ Very interesting][💔 Do not disturb]</code>\n\n(<i>or click the «➡️️/Next» to skip this step</i>)",
-    'es': "✏️ 4/4. Envía nombres de botones y enlaces para botones (1 o más; haz clic en el siguiente ejemplo para copiar):\n\n<code>[🐳 Mi perfil | https://t.me/XXXXX] </code>\n\n\n\n<code>[❤️ Muy interesante][💔 No molestar]</code>\n\n(<i>o haga clic en «➡️️/Next» para omitir esto paso</i>)",
-    'fr': "✏️ 4/4. Envoyez les noms des boutons et les liens pour les boutons (1 ou plusieurs ; cliquez sur l'exemple ci-dessous pour copier) :\n\n<code>[🐳 Mon profil | https://t.me/XXXXX] </code>\n\nили\n\n<code>[❤️ Très intéressant][💔 Ne pas déranger]</code>\n\n(<i>ou cliquez sur « ➡️️/Next » pour ignorer cette étape</i>)",
-    'zh': "✏️ 4/4. 發送按鈕名稱 & 按鈕鏈接 (1 或者更多; 單擊下面的示例進行複制):\n\n<code>[🐳 我的簡歷 | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ 很有意思][💔 請勿打擾]</code>\n\n(<i>或單擊 «➡️️/Next» to skip this step</i>)",
-    'ar': "✏️ 3/3. أرسل أسماء الأزرار والروابط للأزرار (1 أو أكثر ؛ انقر على المثال أدناه لنسخه): \n\n <code> [🐳 ملفي الشخصي | https://t.me/XXXXX] </code> \n \n or \n\n <code> [ممتع جدًا] [💔 عدم الإزعاج] </code> \n\n (<i> أو انقر فوق «➡️️ /Next التالي» لتخطي ذلك الخطوة </i>) ",
-}
-l_offer_finish = {
-    'ru': "✅ <b>Оффер готов</b>\n\n<i>Нажми «➡️️/Next», чтобы подтвердить, а затем на кнопку 🔗 Опубликовать</i>",
-    'en': "✅ <b>Post is ready</b>\n\n<i>Click the «➡️️/Next» to confirm. Then click the [🔗 Publish]-button</i>",
-    'es': "✅ <b>La publicación está lista</b>\n\n<i>Haz clic en «➡️️/Next» para confirmar. Luego haz clic en el botón [🔗 Publicar]</i>",
-    'fr': "✅ <b>La publication est prête</b>\n\n<i>Cliquez sur «➡️️/Next» pour confirmer. Cliquez ensuite sur le bouton [🔗 Publier]</i>",
-    'zh': "✅ <b>帖子準備好了</b>\n\n<i>點擊 «➡️️/Next» 確認. 然後點擊 [🔗 發布]-按鈕</i>",
-    'ar': "✅ <b> النشر جاهز </b> \n\n <i> انقر فوق« ➡️️ /Next التالي »للتأكيد. ثم انقر فوق الزر [🔗 نشر] </i>",
-}
-l_offer_new = {
-    'ru': "⛰ Создать",
-    'en': "⛰ New",
-    'es': "⛰ nueva",
-    'fr': "⛰ nouvelle",
-    'zh': "⛰ 新的",
-    'ar': "⛰ الجديد",
-}
-l_offer_delete = {
-    'ru': "🚫 Удалить",
-    'en': "🚫 Delete",
-    'es': "🚫 Borrar",
-    'fr': "🚫 Effacer",
-    'zh': "🚫 刪除",
-    'ar': "🚫 حذف",
-}
-l_offer_change = {
-    'ru': "♻️ Изменить",
-    'en': "♻️ Edit",
-    'es': "♻️ Editar",
-    'fr': "♻️ Éditer",
-    'zh': "♻️ 編輯",
-    'ar': "♻️ تعديل",
-}
-l_offer_publish = {
-    'ru': "🔗 Опубликовать",
-    'en': "🔗 Publish",
-    'es': "🔗 Publicar",
-    'fr': "🔗 Publier",
-    'zh': "🔗 發布",
-    'ar': "🔗 نشر",
-}
-l_broadcast_start = {
-    'ru': "🗝️ Start..\n#duration {0}min",
-    'en': "🗝️ Sending is starting..\n#duration {0}min",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_broadcast_process = {
-    'ru': "🗝️ Рассылка..{0}%",
-    'en': "🗝️ Sending..{0}%",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_broadcast_finish = {
-    'ru': "🏁 <b>Рассылка</b> завершена\n\n🗝️ Число пользователей, получивших сообщение: <u>{0}</u>",
-    'en': "🏁 <b>Sending</b> is finished\n\n🗝️ User count of getting message: <u>{0}</u>",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_offer_datetime = {
-    'ru': "<b>Дата публикации</b>",
-    'en': "<b>Publication Datetime</b>",
-    'es': "<b>Creación</b>",
-    'fr': "<b>Création</b>",
-    'zh': "<b>創建</b>",
-    'ar': "<b> إنشاء </b>",
-}
-l_offer_buttons = {
-    'ru': "<b>Кнопки</b>",
-    'en': "<b>Buttons</b>",
-    'es': "<b>Botones</b>",
-    'fr': "<b>Boutons</b>",
-    'zh': "<b>鈕扣</b>",
-    'ar': "<b> الأزرار </b>",
-}
-
-l_btn = {
-    'ru': "кнопки",
-    'en': "buttons",
-    'es': "<b>Enlace</b>",
-    'fr': "<b>Lien</b>",
-    'zh': "<b>關聯</b>",
-    'ar': "<b> ارتباط </b>",
-}
-l_pin = {
-    'ru': "закреп",
-    'en': "pin",
-    'es': "<b>Enlace</b>",
-    'fr': "<b>Lien</b>",
-    'zh': "<b>關聯</b>",
-    'ar': "<b> ارتباط </b>",
-}
-l_silence = {
-    'ru': "тихо",
-    'en': "silence",
-    'es': "<b>Enlace</b>",
-    'fr': "<b>Lien</b>",
-    'zh': "<b>關聯</b>",
-    'ar': "<b> ارتباط </b>",
-}
-l_gallery = {
-    'ru': "галерея",
-    'en': "preview",
-    'es': "<b>Enlace</b>",
-    'fr': "<b>Lien</b>",
-    'zh': "<b>關聯</b>",
-    'ar': "<b> ارتباط </b>",
-}
-l_preview = {
-    'ru': "превью",
-    'en': "preview",
-    'es': "<b>Enlace</b>",
-    'fr': "<b>Lien</b>",
-    'zh': "<b>關聯</b>",
-    'ar': "<b> ارتباط </b>",
-}
-l_spoiler = {
-    'ru': "спойлер",
-    'en': "preview",
-    'es': "<b>Enlace</b>",
-    'fr': "<b>Lien</b>",
-    'zh': "<b>關聯</b>",
-    'ar': "<b> ارتباط </b>",
-}
-l_buttons_text = {
-    'ru': "👩🏽‍💻 Режим [кнопки] доступен, если создана хотя бы 1 кнопка",
-    'en': "👩🏽‍💻 [preview] mode isavailable only with unique jpg|png|gif|mp4-files before 5Mb",
-    'es': "<b>Enlace</b>",
-    'fr': "<b>Lien</b>",
-    'zh': "<b>關聯</b>",
-    'ar': "<b> ارتباط </b>",
-}
-l_preview_text = {
-    'ru': "👩🏽‍💻 Режим [превью] используется с одиночными jpg|png|gif|mp4-файлами до 5Mb",
-    'en': "👩🏽‍💻 [preview] mode isavailable only with unique jpg|png|gif|mp4-files before 5Mb",
-    'es': "<b>Enlace</b>",
-    'fr': "<b>Lien</b>",
-    'zh': "<b>關聯</b>",
-    'ar': "<b> ارتباط </b>",
-}
-l_gallery_text = {
-    'ru': "👩🏽‍💻 Режим [галерея] доступен для 2 и более медиа файлов",
-    'en': "👩🏽‍💻 [preview] mode isavailable only with unique jpg|png|gif|mp4-files before 5Mb",
-    'es': "<b>Enlace</b>",
-    'fr': "<b>Lien</b>",
-    'zh': "<b>關聯</b>",
-    'ar': "<b> ارتباط </b>",
-}
-l_spoiler_text = {
-    'ru': "👩🏽‍💻 Режим [спойлер] доступен для photo/gif/video",
-    'en': "👩🏽‍💻 [preview] mode isavailable only with unique jpg|png|gif|mp4-files before 5Mb",
-    'es': "<b>Enlace</b>",
-    'fr': "<b>Lien</b>",
-    'zh': "<b>關聯</b>",
-    'ar': "<b> ارتباط </b>",
-}
-offer_has_restricted = {
-    'ru': "👩🏽‍💻 В настройках <b>[Конфиденциальность]</b> добавь @{0} в <i>исключения</i> для <b>[Голосовые сообщения]</b>, чтобы отобразить <code>видео-заметку</code>/<code>голосовое</code>",
-    'en': "off",
-    'es': "apagada",
-    'fr': "à l'arrêt",
-    'zh': "離開",
-    'ar': "إيقاف",
-}
-offer_time_zone = {
-    'ru': "📍 <b>Часовой пояс</b> геопозиции установлен\n\n🕐 Текущее время: <u>{0}</u> ({1}{2} по Гринвичу)",
-    'en': "no",
-    'es': "no",
-    'fr': "non",
-    'zh': "不",
-    'ar': "رقم",
-}
-offer_time_future = {
-    'ru': "🕒 Укажи время в будущем",
-    'en': "🕒 Specify a time in the future",
-    'es': "🕒 Especificar un tiempo en el futuro",
-    'fr': "🕒 Spécifiez une heure dans le futur",
-    'zh': "🕒 指定未來的時間",
-    'ar': "🕒 حدد وقتًا في المستقبل",
-}
-
-generate_calendar_time = {
-    'ru': "🕒 Отправь <b>время</b> поста на {0} в формате <code>{1}</code>. Текущее время: <u>{2}</u> ({3} по Гринвичу)\n\n🔗 Пришли <b>геопозицию</b>, чтобы <i>автоматически</i> определить часовой пояс",
-    'en': "🕒 Send <b>time</b> for post (<i>in hours and minutes on UTC-Greenwich</i>) for {0} in format <code>{1}</code> (current time: {2})",
-    'es': "🕒 Enviar <b>hora</b> para la publicación (<i>en horas y minutos en UTC-Greenwich</i>) para {0} en formato <code>{1}</code> (hora actual: {2})",
-    'fr': "🕒 Envoyer <b>heure</b> pour la poste (<i>en heures et minutes sur UTC-Greenwich</i>) pour {0} au format <code>{1}</code> (heure actuelle : {2})",
-    'zh': "🕒 以 <code>{1}</code> 格式發送 {0} 的 <b>時間</b> （<i>UTC-格林威治的小時和分鐘</i>）（當前時間：{2}）",
-    'ar': "🕒 أرسل <b> الوقت </b> للنشر (<i> بالساعات والدقائق على UTC-Greenwich </i>) لـ {0} بالتنسيق <code>{1}</code> (الوقت الحالي: {2})",
-}
-month_1 = {
-    'ru': "Янв",
-    'en': "Jan",
-    'es': "enero",
-    'fr': "janvier",
-    'zh': "一月",
-    'ar': "كانون الثاني",
-}
-month_2 = {
-    'ru': "Фев",
-    'en': "Feb",
-    'es': "febrero",
-    'fr': "février",
-    'zh': "二月",
-    'ar': "كانون الثاني",
-}
-month_3 = {
-    'ru': "Мар",
-    'en': "Mar",
-    'es': "Marzo",
-    'fr': "Mars",
-    'zh': "行進",
-    'ar': "يمشي",
-}
-month_4 = {
-    'ru': "Апр",
-    'en': "april",
-    'es': "abril",
-    'fr': "avril",
-    'zh': "四月",
-    'ar': "أبريل",
-}
-month_5 = {
-    'ru': "Май",
-    'en': "May",
-    'es': "Mayo",
-    'fr': "Peut",
-    'zh': "可能",
-    'ar': "مايو",
-}
-month_6 = {
-    'ru': "Июн",
-    'en': "Jun",
-    'es': "Junio",
-    'fr': "Juin",
-    'zh': "六月",
-    'ar': "يونيو",
-}
-month_7 = {
-    'ru': "Июл",
-    'en': "Jul",
-    'es': "Julio",
-    'fr': "Juillet",
-    'zh': "七月",
-    'ar': "يوليو",
-}
-month_8 = {
-    'ru': "Авг",
-    'en': "Aug",
-    'es': "agosto",
-    'fr': "août",
-    'zh': "八月",
-    'ar': "شهر اغسطس",
-}
-month_9 = {
-    'ru': "Сен",
-    'en': "Sep",
-    'es': "septiembre",
-    'fr': "septembre",
-    'zh': "九月",
-    'ar': "شهر سبتمبر",
-}
-month_10 = {
-    'ru': "Окт",
-    'en': "Oct",
-    'es': "octubre",
-    'fr': "octobre",
-    'zh': "十月",
-    'ar': "اكتوبر",
-}
-month_11 = {
-    'ru': "Ноя",
-    'en': "Nov",
-    'es': "noviembre",
-    'fr': "novembre",
-    'zh': "十一月",
-    'ar': "شهر نوفمبر",
-}
-month_12 = {
-    'ru': "Дек",
-    'en': "Dec",
-    'es': "diciembre",
-    'fr': "décembre",
-    'zh': "十二月",
-    'ar': "ديسمبر",
-}
-
-weekday_1 = {
-    'ru': "пн",
-    'en': "Dec",
-    'es': "diciembre",
-    'fr': "décembre",
-    'zh': "十二月",
-    'ar': "ديسمبر",
-}
-weekday_2 = {
-    'ru': "вт",
-    'en': "Dec",
-    'es': "diciembre",
-    'fr': "décembre",
-    'zh': "十二月",
-    'ar': "ديسمبر",
-}
-weekday_3 = {
-    'ru': "ср",
-    'en': "Dec",
-    'es': "diciembre",
-    'fr': "décembre",
-    'zh': "十二月",
-    'ar': "ديسمبر",
-}
-weekday_4 = {
-    'ru': "чт",
-    'en': "Dec",
-    'es': "diciembre",
-    'fr': "décembre",
-    'zh': "十二月",
-    'ar': "ديسمبر",
-}
-weekday_5 = {
-    'ru': "пт",
-    'en': "Dec",
-    'es': "diciembre",
-    'fr': "décembre",
-    'zh': "十二月",
-    'ar': "ديسمبر",
-}
-weekday_6 = {
-    'ru': "сб",
-    'en': "Dec",
-    'es': "diciembre",
-    'fr': "décembre",
-    'zh': "十二月",
-    'ar': "ديسمبر",
-}
-weekday_7 = {
-    'ru': "вс",
-    'en': "Dec",
-    'es': "diciembre",
-    'fr': "décembre",
-    'zh': "十二月",
-    'ar': "ديسمبر",
-}
-
-on = {
-    'ru': "вкл",
-    'en': "on",
-    'es': "en",
-    'fr': "sur",
-    'zh': "上",
-    'ar': "على",
-}
-off = {
-    'ru': "выкл",
-    'en': "off",
-    'es': "apagado",
-    'fr': "à l'arrêt",
-    'zh': "離開",
-    'ar': "إيقاف",
-}
-l_me = {
-    'ru': "👤 Себе",
-    'en': "👤 Me",
-    'es': "en",
-    'fr': "sur",
-    'zh': "上",
-    'ar': "على",
-}
-l_all = {
-    'ru': "👥 Всем",
-    'en': "👥 All",
-    'es': "en",
-    'fr': "sur",
-    'zh': "上",
-    'ar': "على",
-}
-l_ids = {
-    'ru': "🙌🏽 По id",
-    'en': "🙌🏽 By id",
-    'es': "en",
-    'fr': "sur",
-    'zh': "上",
-    'ar': "على",
-}
-l_recipient = {
-    'ru': "👩🏽‍💻 <b>Выбери</b> получателя",
-    'en': "👩🏽‍💻 Choose recipient",
-    'es': "en",
-    'fr': "sur",
-    'zh': "上",
-    'ar': "على",
-}
-l_enter = {
-    'ru': "👩🏽‍💻 <b>Введи</b> Ids получателей через пробельные или разделительные символы",
-    'en': "👩🏽‍💻 Введи Ids получателей через пробельные или разделительные символы",
-    'es': "en",
-    'fr': "sur",
-    'zh': "上",
-    'ar': "على",
-}
-
-l_inline_demo = {
-    'ru': "обо всех проектах",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_bot = {
-    'ru': "конструктор ботов",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_post = {
-    'ru': "конструктор офферов",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_media = {
-    'ru': "конструктор медиа-заметок",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_channel = {
-    'ru': "администратор каналов",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_group = {
-    'ru': "администратор групп",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_find = {
-    'ru': "бот для поиска",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_ai = {
-    'ru': "бот с нейросетью",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_ads = {
-    'ru': "рекламный бот",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_vpn = {
-    'ru': "vpn-бот",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_target = {
-    'ru': "таргет-бот",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_user = {
-    'ru': "администратор пользователя",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_tools = {
-    'ru': "Telegram-инструменты",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-l_inline_work = {
-    'ru': "вакансии/конкурсы",
-    'en': "forever",
-    'es': "siempre",
-    'fr': "toujours",
-    'zh': "永遠",
-    'ar': "إلى الأبد",
-}
-
-
-# endregion
-
-
 # region admin
 async def pre_upload(bot, chat_id, media_name, media_type, EXTRA_D, BASE_D):
     result = None
     try:
         sql = "SELECT FILE_FILEID FROM FILE WHERE FILE_FILENAME=?"
         data = await db_select(sql, (media_name,), BASE_D)
 
@@ -1028,69 +517,69 @@
                             call=None):
     try:
         sql = "SELECT OFFER_ID, OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, " \
               "OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT FROM OFFER"
         data_offers = await db_select(sql, (), BASE_D)
         if not data_offers:
             if call: await call.message.delete()
-            await bot.send_message(chat_id, l_offer_text[lz], reply_markup=markupAdmin)
+            await bot.send_message(chat_id, yeref.l_post_text[lz], reply_markup=markupAdmin)
             await state.set_state(FsmOffer.text)
             return
 
         # region config
         post_id = 1 if post_id < 1 else post_id
         item = data_offers[post_id - 1]
         OFFER_ID, OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_ISTGPH, \
             OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT = item
-        show_offers_datetime = l_offer_datetime[lz]
-        show_offers_button = l_offer_buttons[lz]
-        show_offers_off = off[lz]
+        show_offers_datetime = yeref.l_post_datetime[lz]
+        show_offers_button = yeref.l_post_buttons[lz]
+        show_offers_off = yeref.l_off[lz]
 
         extra = f"\n\n{show_offers_datetime}: {OFFER_DT if OFFER_DT else show_offers_off}\n" \
                 f"{show_offers_button}: {OFFER_BUTTON if OFFER_BUTTON else show_offers_off}\n"
         OFFER_TEXT = OFFER_TEXT or ''
         OFFER_TEXT = '' if OFFER_MEDIATYPE == 'video_note' or OFFER_MEDIATYPE == 'sticker' else OFFER_TEXT
         moment = 1020 - len(OFFER_TEXT) - len(extra)
-        OFFER_TEXT = await correct_tag(f"{l_offer_text[0:(len(OFFER_TEXT) + moment)]}") if moment <= 0 else OFFER_TEXT
+        OFFER_TEXT = await correct_tag(f"{yeref.l_post_text[0:(len(OFFER_TEXT) + moment)]}") if moment <= 0 else OFFER_TEXT
 
         # endregion
         # region reply_markup
         reply_markup = get_keyboard_admin(data_offers, 'offers', post_id)
 
         buttons = [
-            types.InlineKeyboardButton(text=f"✅ {l_btn[lz]}" if OFFER_ISBUTTON else f"☑️ {l_btn[lz]}",
+            types.InlineKeyboardButton(text=f"✅ {yeref.l_btn[lz]}" if OFFER_ISBUTTON else f"☑️ {yeref.l_btn[lz]}",
                                        callback_data=f'ofr_isbtn_{OFFER_ID}_{post_id}'),
-            types.InlineKeyboardButton(text=f"✅ {l_pin[lz]}" if OFFER_ISPIN else f"☑️ {l_pin[lz]}",
+            types.InlineKeyboardButton(text=f"✅ {yeref.l_pin[lz]}" if OFFER_ISPIN else f"☑️ {yeref.l_pin[lz]}",
                                        callback_data=f'ofr_ispin_{OFFER_ID}_{post_id}'),
-            types.InlineKeyboardButton(text=f"✅ {l_silence[lz]}" if OFFER_ISSILENCE else f"☑️ {l_silence[lz]}",
+            types.InlineKeyboardButton(text=f"✅ {yeref.l_silence[lz]}" if OFFER_ISSILENCE else f"☑️ {yeref.l_silence[lz]}",
                                        callback_data=f'ofr_issilence_{OFFER_ID}_{post_id}'),
         ]
         reply_markup.row(*buttons)
 
         buttons = [
-            types.InlineKeyboardButton(text=f"✅ {l_gallery[lz]}" if OFFER_ISGALLERY else f"☑️ {l_gallery[lz]}",
+            types.InlineKeyboardButton(text=f"✅ {yeref.l_gallery[lz]}" if OFFER_ISGALLERY else f"☑️ {yeref.l_gallery[lz]}",
                                        callback_data=f'ofr_isgallery_{OFFER_ID}_{post_id}'),
-            types.InlineKeyboardButton(text=f"✅ {l_preview[lz]}" if OFFER_ISTGPH else f"☑️ {l_preview[lz]}",
+            types.InlineKeyboardButton(text=f"✅ {yeref.l_preview[lz]}" if OFFER_ISTGPH else f"☑️ {yeref.l_preview[lz]}",
                                        callback_data=f'ofr_ispreview_{OFFER_ID}_{post_id}'),
-            types.InlineKeyboardButton(text=f"✅ {l_spoiler[lz]}" if OFFER_ISSPOILER else f"☑️ {l_spoiler[lz]}",
+            types.InlineKeyboardButton(text=f"✅ {yeref.l_spoiler[lz]}" if OFFER_ISSPOILER else f"☑️ {yeref.l_spoiler[lz]}",
                                        callback_data=f'ofr_isspoiler_{OFFER_ID}_{post_id}'),
         ]
         reply_markup.row(*buttons)
 
         buttons = [
-            types.InlineKeyboardButton(text=l_offer_new[lz],
+            types.InlineKeyboardButton(text=yeref.l_post_new[lz],
                                        callback_data=f'ofr_new_{OFFER_ID}_{post_id}'),
-            types.InlineKeyboardButton(text=l_offer_delete[lz],
+            types.InlineKeyboardButton(text=yeref.l_post_delete[lz],
                                        callback_data=f'ofr_del_{OFFER_ID}_{post_id}'),
-            types.InlineKeyboardButton(text=l_offer_change[lz],
+            types.InlineKeyboardButton(text=yeref.l_post_change[lz],
                                        callback_data=f'ofr_edit_{OFFER_ID}_{post_id}'),
         ]
         reply_markup.row(*buttons)
 
-        reply_markup.row(types.InlineKeyboardButton(text=l_offer_publish[lz],
+        reply_markup.row(types.InlineKeyboardButton(text=yeref.l_post_publish[lz],
                                                     callback_data=f'ofr_pub_{OFFER_ID}_{post_id}'))
 
         # endregion
         # region show
         if OFFER_FILEID and '[' not in OFFER_FILEID:
             OFFER_TEXT = OFFER_TEXT + extra
             if not call:
@@ -1112,24 +601,24 @@
                                             reply_markup=reply_markup.as_markup())
                 elif OFFER_MEDIATYPE == 'sticker':
                     await bot.send_sticker(chat_id=chat_id, sticker=OFFER_FILEID)
                     await bot.send_message(chat_id, OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                            disable_web_page_preview=True)
                 elif OFFER_MEDIATYPE == 'voice':
                     if has_restricted:
-                        text = offer_has_restricted[lz].format(bot_un)
+                        text = yeref.offer_has_restricted[lz].format(bot_un)
                         await bot.send_message(chat_id, text, disable_web_page_preview=True)
                         await bot.send_message(chat_id, OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                                disable_web_page_preview=True)
                     else:
                         await bot.send_voice(chat_id, OFFER_FILEID, caption=OFFER_TEXT,
                                              reply_markup=reply_markup.as_markup())
                 elif OFFER_MEDIATYPE == 'video_note':
                     if has_restricted:
-                        text = offer_has_restricted[lz].format(bot_un)
+                        text = yeref.offer_has_restricted[lz].format(bot_un)
                         await bot.send_message(chat_id, text, disable_web_page_preview=True)
                     else:
                         await bot.send_video_note(chat_id=chat_id, video_note=OFFER_FILEID)
                     await bot.send_message(chat_id, OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                            disable_web_page_preview=True)
             else:
                 if OFFER_MEDIATYPE == 'photo' or OFFER_MEDIATYPE == 'text':
@@ -1174,33 +663,33 @@
                         await call.message.edit_media(media=media, reply_markup=reply_markup.as_markup())
                 elif OFFER_MEDIATYPE == 'sticker':
                     await bot.send_sticker(chat_id, OFFER_FILEID)
                     await bot.send_message(chat_id=chat_id, text=OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                            disable_web_page_preview=True)
                 elif OFFER_MEDIATYPE == 'video_note':
                     if has_restricted:
-                        text = offer_has_restricted[lz].format(bot_un)
+                        text = yeref.offer_has_restricted[lz].format(bot_un)
                         await bot.send_message(chat_id, text, disable_web_page_preview=True)
                     else:
                         await bot.send_video_note(chat_id=chat_id, video_note=OFFER_FILEID)
                     await bot.send_message(chat_id, OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                            disable_web_page_preview=True)
                 elif OFFER_MEDIATYPE == 'voice':
                     if has_restricted:
-                        text = offer_has_restricted[lz].format(bot_un)
+                        text = yeref.offer_has_restricted[lz].format(bot_un)
                         await bot.send_message(chat_id, text, disable_web_page_preview=True)
                         await bot.send_message(chat_id, OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                                disable_web_page_preview=True)
                     else:
                         await bot.send_voice(chat_id, OFFER_FILEID, caption=OFFER_TEXT,
                                              reply_markup=reply_markup.as_markup())
         else:
             if call and str(post_id) == await get_current_page_number(call):
                 await call.message.edit_reply_markup(reply_markup=reply_markup.as_markup())
-            else:
+            elif OFFER_FILEID:
                 OFFER_FILEID = ast.literal_eval(OFFER_FILEID) if OFFER_FILEID and '[' in OFFER_FILEID else OFFER_FILEID
                 OFFER_MEDIATYPE = ast.literal_eval(
                     OFFER_MEDIATYPE) if OFFER_MEDIATYPE and '[' in OFFER_MEDIATYPE else OFFER_MEDIATYPE
 
                 media = []
                 for i in range(0, len(OFFER_FILEID)):
                     caption = OFFER_TEXT if i == 0 else None
@@ -1245,30 +734,31 @@
         return result
 
 
 async def broadcast_send_admin(bot, chat_id, lz, offer_id, BASE_D, ids):
     try:
         if ids == 'me':
             user_ids = [chat_id]
-        elif ids == 'all':
+        elif not ids or ids == 'all':
             sql = "SELECT USER_TID FROM USER"
             data = await db_select(sql, (), BASE_D)
             user_ids = [item[0] for item in data]
         else:
             sql = "SELECT USER_TID FROM USER"
             data = await db_select(sql, (), BASE_D)
             user_ids = [item[0] for item in data]
             user_ids = [item for item in user_ids if str(item) in ids]
 
         duration = 0 if len(user_ids) < 50 else int(len(user_ids) / 50)
-        text = l_broadcast_start[lz].format(duration)
-        await bot.send_message(chat_id, text, parse_mode=ParseMode.HTML)
+        if str(chat_id) in my_tids:
+            text = yeref.l_broadcast_start[lz].format(duration)
+            await bot.send_message(chat_id, text, parse_mode=ParseMode.HTML)
         all_len = len(user_ids)
-        # max_size = 20  # 1
-        max_size = 1  # 1
+        max_size = 20  # 1
+        # max_size = 1  # 1
         fact_len = 0
 
         while True:
             try:
                 random.shuffle(user_ids)
                 await asyncio.sleep(0.05)
                 tmp_user_ids = [user_ids.pop() for _ in range(0, max_size) if len(user_ids)]
@@ -1277,21 +767,27 @@
 
                 for result in results:
                     if result:
                         fact_len += 1
 
                 if not len(user_ids): break
                 per = int(float(len(user_ids)) / float(all_len) * 100.0)
-                text = l_broadcast_process[lz].format(100 - per)
-                await bot.send_message(chat_id, text, parse_mode=ParseMode.HTML)
+
+                if str(chat_id) in my_tids:
+                    text = yeref.l_broadcast_process[lz].format(100 - per)
+                    await bot.send_message(chat_id, text, parse_mode=ParseMode.HTML)
             except Exception as e:
                 logger.info(log_ % {str(e)})
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
 
-        text = l_broadcast_finish[lz].format(fact_len)
+        if str(chat_id) not in my_tids:
+            sql = "DELETE FROM OFFER WHERE OFFER_ID=?"
+            await db_change(sql, (offer_id,), BASE_D)
+
+        text = yeref.l_broadcast_finish[lz].format(fact_len)
         await bot.send_message(chat_id, text, parse_mode=ParseMode.HTML)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def send_user(bot, chat_id, offer_id, BASE_D, message_id=None, current=1):
@@ -1443,45 +939,45 @@
         shift_month = data.get('shift_month', 0)
 
         dt_ = datetime.datetime.utcnow() + datetime.timedelta(hours=0) + datetime.timedelta(days=32 * shift_month)
         if shift_month:
             dt_ = datetime.datetime(year=dt_.year, month=dt_.month, day=1)
 
         month_dic = {
-            1: month_1[lz],
-            2: month_2[lz],
-            3: month_3[lz],
-            4: month_4[lz],
-            5: month_5[lz],
-            6: month_6[lz],
-            7: month_7[lz],
-            8: month_8[lz],
-            9: month_9[lz],
-            10: month_10[lz],
-            11: month_11[lz],
-            12: month_12[lz]
+            1: yeref.l_month_1[lz],
+            2: yeref.l_month_2[lz],
+            3: yeref.l_month_3[lz],
+            4: yeref.l_month_4[lz],
+            5: yeref.l_month_5[lz],
+            6: yeref.l_month_6[lz],
+            7: yeref.l_month_7[lz],
+            8: yeref.l_month_8[lz],
+            9: yeref.l_month_9[lz],
+            10: yeref.l_month_10[lz],
+            11: yeref.l_month_11[lz],
+            12: yeref.l_month_12[lz]
         }
         month = month_dic[dt_.month]
 
         reply_markup = InlineKeyboardBuilder()
         buttons = [
             types.InlineKeyboardButton(text="«", callback_data=f'calendar_left'),
             types.InlineKeyboardButton(text=f"{month} {dt_.year}", callback_data='cb_99'),
             types.InlineKeyboardButton(text="»", callback_data=f'calendar_right'),
         ]
         reply_markup.row(*buttons)
 
         buttons_ = [
-            types.InlineKeyboardButton(text=weekday_1[lz], callback_data='cb_99'),
-            types.InlineKeyboardButton(text=weekday_2[lz], callback_data='cb_99'),
-            types.InlineKeyboardButton(text=weekday_3[lz], callback_data='cb_99'),
-            types.InlineKeyboardButton(text=weekday_4[lz], callback_data='cb_99'),
-            types.InlineKeyboardButton(text=weekday_5[lz], callback_data='cb_99'),
-            types.InlineKeyboardButton(text=weekday_6[lz], callback_data='cb_99'),
-            types.InlineKeyboardButton(text=weekday_7[lz], callback_data='cb_99'),
+            types.InlineKeyboardButton(text=yeref.l_weekday_1[lz], callback_data='cb_99'),
+            types.InlineKeyboardButton(text=yeref.l_weekday_2[lz], callback_data='cb_99'),
+            types.InlineKeyboardButton(text=yeref.l_weekday_3[lz], callback_data='cb_99'),
+            types.InlineKeyboardButton(text=yeref.l_weekday_4[lz], callback_data='cb_99'),
+            types.InlineKeyboardButton(text=yeref.l_weekday_5[lz], callback_data='cb_99'),
+            types.InlineKeyboardButton(text=yeref.l_weekday_6[lz], callback_data='cb_99'),
+            types.InlineKeyboardButton(text=yeref.l_weekday_7[lz], callback_data='cb_99'),
         ]
         reply_markup.row(*buttons_)
 
         week_first_day = datetime.datetime(year=dt_.year, month=dt_.month, day=1).weekday() + 1
         buttons_ = []
         for i in range(0, 6 * 7):
             buttons_.append(types.InlineKeyboardButton(text=" ", callback_data=f'cb_99'))
@@ -1495,17 +991,17 @@
         for i in range(0, len(buttons_)):
             tmp.append(buttons_[i])
             if len(tmp) >= 7:
                 reply_markup.row(*tmp)
                 tmp = []
 
         if is_new:
-            await bot.send_message(chat_id=chat_id, text=l_offer_date[lz], reply_markup=reply_markup.as_markup())
+            await bot.send_message(chat_id=chat_id, text=yeref.l_post_date[lz], reply_markup=reply_markup.as_markup())
         else:
-            await bot.edit_message_text(chat_id=chat_id, text=l_offer_date[lz], message_id=message_id,
+            await bot.edit_message_text(chat_id=chat_id, text=yeref.l_post_date[lz], message_id=message_id,
                                         reply_markup=reply_markup.as_markup())
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
@@ -1521,41 +1017,41 @@
         has_restricted = (await bot.get_chat(chat_id)).has_restricted_voice_and_video_messages
 
         if cmd == 'new':
             await state.clear()
 
             await state.set_state(FsmOffer.text)
 
-            await bot.send_message(call.from_user.id, l_offer_text[lz], reply_markup=markupAdmin)
+            await bot.send_message(call.from_user.id, yeref.l_post_text[lz], reply_markup=markupAdmin)
         elif cmd == 'del':
             await state.clear()
 
             sql = "DELETE FROM OFFER WHERE OFFER_ID=?"
             await db_change(sql, (offer_id,), BASE_D)
 
             await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id - 1, call)
         elif cmd == 'edit':
             await state.clear()
 
             await state.set_state(FsmOffer.text)
             await state.update_data(offer_id=offer_id)
 
-            await bot.send_message(call.from_user.id, l_offer_edit[lz], reply_markup=markupAdmin)
+            await bot.send_message(call.from_user.id, yeref.l_post_edit[lz], reply_markup=markupAdmin)
         elif cmd == 'isbtn':
             sql = "SELECT OFFER_BUTTON, OFFER_ISBUTTON FROM OFFER WHERE OFFER_ID=?"
             data = await db_select(sql, (offer_id,), BASE_D)
             OFFER_BUTTON, OFFER_ISBUTTON = data[0]
 
             if OFFER_BUTTON:
                 OFFER_ISBUTTON = 0 if OFFER_ISBUTTON else 1
                 sql = "UPDATE OFFER SET OFFER_ISBUTTON=? WHERE OFFER_ID=?"
                 await db_change(sql, (OFFER_ISBUTTON, offer_id,), BASE_D)
                 await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id, call)
             else:
-                text = l_buttons_text[lz]
+                text = yeref.l_buttons_text[lz]
                 await call.answer(text=text, show_alert=True)
         elif cmd == 'ispin':
             sql = "SELECT OFFER_ISPIN FROM OFFER WHERE OFFER_ID=?"
             data = await db_select(sql, (offer_id,), BASE_D)
             OFFER_ISPIN = 0 if data[0][0] else 1
             sql = "UPDATE OFFER SET OFFER_ISPIN=? WHERE OFFER_ID=?"
             await db_change(sql, (OFFER_ISPIN, offer_id,), BASE_D)
@@ -1574,23 +1070,23 @@
 
             if OFFER_FILEID and '[' in OFFER_FILEID:
                 OFFER_ISGALLERY = 0 if data[0][0] else 1
                 sql = "UPDATE OFFER SET OFFER_ISGALLERY=? WHERE OFFER_ID=?"
                 await db_change(sql, (OFFER_ISGALLERY, offer_id,), BASE_D)
                 await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id, call)
             else:
-                text = l_gallery_text[lz]
+                text = yeref.l_gallery_text[lz]
                 await call.answer(text=text, show_alert=True)
         elif cmd == 'ispreview':
             sql = "SELECT OFFER_ISTGPH, OFFER_TGPHLINK FROM OFFER WHERE OFFER_ID=?"
             data = await db_select(sql, (offer_id,), BASE_D)
             OFFER_ISTGPH, OFFER_TGPHLINK = data[0]
 
             if not OFFER_TGPHLINK:
-                text = l_preview_text[lz]
+                text = yeref.l_preview_text[lz]
                 await call.answer(text=text, show_alert=True)
 
             OFFER_ISTGPH = 0 if OFFER_ISTGPH else 1
             sql = "UPDATE OFFER SET OFFER_ISTGPH=? WHERE OFFER_ID=?"
             await db_change(sql, (OFFER_ISTGPH, offer_id,), BASE_D)
             await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id, call)
         elif cmd == 'isspoiler':
@@ -1600,29 +1096,29 @@
 
             if OFFER_MEDIATYPE and OFFER_MEDIATYPE in ['photo', 'animation', 'video'] or '[' in OFFER_MEDIATYPE:
                 OFFER_ISSPOILER = 0 if data[0][0] else 1
                 sql = "UPDATE OFFER SET OFFER_ISSPOILER=? WHERE OFFER_ID=?"
                 await db_change(sql, (OFFER_ISSPOILER, offer_id,), BASE_D)
                 await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id, call)
             else:
-                text = l_spoiler_text[lz]
+                text = yeref.l_spoiler_text[lz]
                 await call.answer(text=text, show_alert=True)
         elif cmd == 'pub':
             await state.clear()
             await call.answer()
 
             reply_markup = InlineKeyboardBuilder()
             buttons = [
-                types.InlineKeyboardButton(text=l_me[lz], callback_data=f"pub_me_{offer_id}"),
-                types.InlineKeyboardButton(text=l_all[lz], callback_data=f"pub_all_{offer_id}"),
-                types.InlineKeyboardButton(text=l_ids[lz], callback_data=f"pub_ids_{offer_id}"),
+                types.InlineKeyboardButton(text=yeref.l_me[lz], callback_data=f"pub_me_{offer_id}"),
+                types.InlineKeyboardButton(text=yeref.l_all[lz], callback_data=f"pub_all_{offer_id}"),
+                types.InlineKeyboardButton(text=yeref.l_ids[lz], callback_data=f"pub_ids_{offer_id}"),
             ]
             reply_markup.add(*buttons).adjust(1)
 
-            text = l_recipient[lz]
+            text = yeref.l_recipient[lz]
             await bot.send_message(chat_id, text, reply_markup=reply_markup.as_markup())
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
@@ -1640,15 +1136,15 @@
         elif option == 'all':
             loop = asyncio.get_event_loop()
             loop.create_task(broadcast_send_admin(bot, chat_id, lz, offer_id, BASE_D, 'all'))
         elif option == 'ids':
             await state.set_state(FsmIds.start)
             await state.update_data(offer_id=offer_id)
 
-            text = l_enter[lz]
+            text = yeref.l_enter[lz]
             await bot.send_message(chat_id, text)
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
@@ -1676,27 +1172,27 @@
 
 async def fsm_text_admin(bot, FsmOffer, message, state, BASE_D):
     try:
         chat_id = message.from_user.id
         lz = await lz_code(chat_id, message.from_user.language_code, BASE_D)
 
         if message.text == '⬅️ Prev':
-            await bot.send_message(chat_id, l_offer_text[lz])
+            await bot.send_message(chat_id, yeref.l_post_text[lz])
             await state.set_state(FsmOffer.text)
         elif message.text in ['➡️️ Next', '/Next']:
-            await bot.send_message(chat_id, l_offer_media[lz])
+            await bot.send_message(chat_id, yeref.l_post_media[lz])
             await state.set_state(FsmOffer.media)
         else:
             if len(message.html_text) >= 1024:
-                text = l_offer_text_limit[lz].format(len(message.html_text))
+                text = yeref.l_post_text_limit[lz].format(len(message.html_text))
                 await bot.send_message(chat_id, text)
                 return
 
             await state.update_data(offer_text=message.html_text)
-            await bot.send_message(chat_id=chat_id, text=l_offer_media[lz])
+            await bot.send_message(chat_id=chat_id, text=yeref.l_post_media[lz])
             await state.set_state(FsmOffer.media)
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
@@ -1710,25 +1206,25 @@
         offer_text = None
         offer_file_id = None
         offer_file_type = None
         offer_tgph_link = None
         file_name_part = None
 
         if message.text == '⬅️ Prev':
-            await bot.send_message(chat_id, l_offer_text[lz])
+            await bot.send_message(chat_id, yeref.l_post_text[lz])
             await state.set_state(FsmOffer.text)
         elif message.text in ['➡️️ Next', '/Next']:
             if not offer_text:
-                await bot.send_message(chat_id, l_offer_text_empty[lz].format(l_offer_text[lz]))
+                await bot.send_message(chat_id, yeref.l_post_text_empty[lz].format(yeref.l_post_text[lz]))
                 await state.set_state(FsmOffer.text)
             else:
                 await generate_calendar_admin(bot, state, lz, chat_id)
                 await state.set_state(FsmOffer.date_)
         else:
-            await bot.send_message(chat_id, l_offer_media_wait[lz].format('album', 1))
+            await bot.send_message(chat_id, yeref.l_post_media_wait[lz].format('album', 1))
 
             for obj in album:
                 if obj.photo:
                     media_id = obj.photo[-1].file_id
                     media_type = 'photo'
                     dt_ = datetime.datetime.utcnow().strftime('%d-%m-%Y_%H-%M-%S-%f.jpg')
                     file_name_part_new = f"{dt_}"
@@ -1770,15 +1266,15 @@
                 await state.update_data(offer_file_id=str(offer_file_id),
                                         offer_file_type=str(offer_file_type),
                                         offer_tgph_link=str(offer_tgph_link),
                                         file_name_part=str(file_name_part))
                 await asyncio.sleep(0.05)
 
             if len(ast.literal_eval(str(offer_file_id))) < 2:
-                await bot.send_message(chat_id=chat_id, text=l_offer_media[lz])
+                await bot.send_message(chat_id=chat_id, text=yeref.l_post_media[lz])
                 await state.set_state(FsmOffer.media)
                 return
 
             await generate_calendar_admin(bot, state, lz, chat_id)
             await state.set_state(FsmOffer.date_)
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
@@ -1793,39 +1289,39 @@
     lz = await lz_code(chat_id, message.from_user.language_code, BASE_D)
 
     try:
         data = await state.get_data()
         offer_text = data.get('offer_text', None)
 
         if message.text == '⬅️ Prev':
-            await bot.send_message(chat_id, l_offer_text[lz])
+            await bot.send_message(chat_id, yeref.l_post_text[lz])
             await state.set_state(FsmOffer.text)
         elif message.text in ['➡️️ Next', '/Next']:
             if not offer_text:
-                await bot.send_message(chat_id, l_offer_text_empty[lz].format(l_offer_text[lz]))
+                await bot.send_message(chat_id, yeref.l_post_text_empty[lz].format(yeref.l_post_text[lz]))
                 await state.set_state(FsmOffer.text)
             else:
-                text = l_offer_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
-                    l_offer_button[lz].replace('XXXXX', '')
+                text = yeref.l_post_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
+                    yeref.l_post_button[lz].replace('XXXXX', '')
                 await bot.send_message(chat_id, text)
                 await state.set_state(FsmOffer.button)
         else:
             file_name = file_name_part = file_id = file_id_note = file_type = offer_tgph_link = None
             if message.text:
-                await bot.send_message(chat_id=chat_id, text=l_offer_media[lz])
+                await bot.send_message(chat_id=chat_id, text=yeref.l_post_media[lz])
                 return
             elif message.photo:
                 file_id = message.photo[-1].file_id
                 file_name_part = f"{datetime.datetime.utcnow().strftime('%d-%m-%Y_%H-%M-%S-%f.jpg')}"
                 file_name = os.path.join(MEDIA_D, file_name_part)
                 file = await bot.get_file(file_id)
                 await bot.download_file(file.file_path, file_name)
                 file_type = 'photo'
             elif message.animation:
-                await bot.send_message(chat_id, l_offer_media_wait[lz].format('giff', 1))
+                await bot.send_message(chat_id, yeref.l_post_media_wait[lz].format('giff', 1))
                 file_id = message.animation.file_id
                 file_name_part = f"{message.animation.file_name}"
                 file_name = os.path.join(MEDIA_D, file_name_part)
                 file = await bot.get_file(file_id)
                 await bot.download_file(file.file_path, file_name)
                 file_type = 'animation'
 
@@ -1838,27 +1334,27 @@
 
                     if os.path.exists(file_name): os.remove(file_name)
                     file_name = os.path.join(os.path.dirname(file_name), get_name_without_ext(file_name) + '.mp4')
                     file_name_part = os.path.basename(file_name)
                     if os.path.exists(tmp_name): os.rename(tmp_name, file_name)
             elif message.sticker:
                 if message.sticker.is_animated or message.sticker.is_video:
-                    await bot.send_message(chat_id=chat_id, text=l_offer_media[lz])
+                    await bot.send_message(chat_id=chat_id, text=yeref.yeref.l_post_media[lz])
                     await state.set_state(FsmOffer.media)
                     return
 
                 file_id = message.sticker.file_id
                 dt_ = datetime.datetime.utcnow().strftime('%d-%m-%Y_%H-%M-%S-%f.webp')
                 file_name_part = f"{dt_}"
                 file_name = os.path.join(MEDIA_D, file_name_part)
                 file = await bot.get_file(file_id)
                 await bot.download_file(file.file_path, file_name)
                 file_type = 'sticker'
             elif message.video:
-                await bot.send_message(chat_id, l_offer_media_wait[lz].format('video', 1))
+                await bot.send_message(chat_id, yeref.l_post_media_wait[lz].format('video', 1))
                 file_id = message.video.file_id
                 file_name_part = f"{message.video.file_name}"
                 file_name = os.path.join(MEDIA_D, file_name_part)
                 file = await bot.get_file(file_id)
                 await bot.download_file(file.file_path, file_name)
 
                 await asyncio.sleep(0.05)
@@ -1879,15 +1375,15 @@
                 title = message.from_user.first_name
                 thumbnail = types.InputFile(os.path.join(EXTRA_D, 'img.jpg'))
                 res = await bot.send_audio(chat_id=chat_id, audio=types.FSInputFile(file_name), thumbnail=thumbnail,
                                            title=title, performer=performer)
                 file_id = res.audio.file_id
                 await bot.delete_message(chat_id, res.message_id)
             elif message.voice:
-                await bot.send_message(chat_id, l_offer_media_wait[lz].format('voice', 1))
+                await bot.send_message(chat_id, yeref.l_post_media_wait[lz].format('voice', 1))
                 file_id = message.voice.file_id
                 dt_ = datetime.datetime.utcnow().strftime('%d-%m-%Y_%H-%M-%S-%f.ogg')
                 file_name_part = f"{dt_}"
                 file_name = os.path.join(MEDIA_D, file_name_part)
                 file = await bot.get_file(file_id)
                 await bot.download_file(file.file_path, file_name)
                 file_type = 'voice'
@@ -1928,49 +1424,49 @@
                 except Exception as e:
                     logger.info(log_ % f"Telegraph: {str(e)}")
                     await asyncio.sleep(round(random.uniform(0, 1), 2))
             if file_name and os.path.exists(file_name): os.remove(file_name)
             await state.update_data(offer_file_id=file_id, offer_file_id_note=file_id_note, offer_file_type=file_type,
                                     offer_tgph_link=offer_tgph_link, file_name_part=file_name_part)
 
-            text = l_offer_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
-                l_offer_button[lz].replace('XXXXX', '')
+            text = yeref.l_post_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
+                yeref.l_post_button[lz].replace('XXXXX', '')
             await bot.send_message(chat_id, text)
             await state.set_state(FsmOffer.button)
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     # except FileIsTooBig as e:
     #     logger.info(log_ % str(e))
     #     await asyncio.sleep(round(random.uniform(0, 1), 2))
-    #     await bot.send_message(chat_id, l_offer_media_toobig[lz])
+    #     await bot.send_message(chat_id, yeref.l_post_media_toobig[lz])
     except Exception as e:
         if 'too big' in str(e):
             await bot.send_message(chat_id, yeref.l_post_media_toobig[lz])
         else:
             logger.info(log_ % str(e))
             await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def fsm_button_admin(bot, FsmOffer, message, state, BASE_D):
     try:
         chat_id = message.from_user.id
         lz = await lz_code(chat_id, message.from_user.language_code, BASE_D)
 
         if message.text == '⬅️ Prev':
-            await bot.send_message(message.from_user.id, l_offer_media[lz])
+            await bot.send_message(message.from_user.id, yeref.l_post_media[lz])
             await state.set_state(FsmOffer.media)
         elif message.text in ['➡️️ Next', '/Next']:
             await generate_calendar_admin(bot, state, lz, chat_id)
             await state.set_state(FsmOffer.date_)
         else:
             res_ = await check_buttons(bot, chat_id, message.text.strip())
             if len(res_) == 0:
-                text = l_offer_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
-                    l_offer_button[lz].replace('XXXXX', '')
+                text = yeref.l_post_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
+                    yeref.l_post_button[lz].replace('XXXXX', '')
                 await bot.send_message(chat_id, text)
                 await state.set_state(FsmOffer.button)
                 return
 
             await state.update_data(offer_button=message.text.strip())
             await generate_calendar_admin(bot, state, lz, chat_id)
             await state.set_state(FsmOffer.date_)
@@ -2006,15 +1502,15 @@
             dt_cur = dt_now + datetime.timedelta(hours=int(h_), minutes=int(m_))
         else:
             dt_cur = dt_now - datetime.timedelta(hours=int(h_), minutes=int(m_))
 
         datetime_plus = (dt_cur + datetime.timedelta(hours=1)).strftime("%H:%M")
         datetime_current = dt_cur.strftime("%H:%M")
 
-        text = generate_calendar_time[lz].format(dt_user, datetime_plus, datetime_current, USER_TZ)
+        text = yeref.l_generate_calendar_time[lz].format(dt_user, datetime_plus, datetime_current, USER_TZ)
         await bot.send_message(chat_id, text)
         await state.set_state(FsmOffer.time_)
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
@@ -2048,20 +1544,20 @@
 
 async def fsm_date_admin(bot, FsmOffer, message, state, BASE_D):
     try:
         chat_id = message.from_user.id
         lz = await lz_code(chat_id, message.from_user.language_code, BASE_D)
 
         if message.text == '⬅️ Prev':
-            text = l_offer_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
-                l_offer_button[lz].replace('XXXXX', '')
+            text = yeref.l_post_button[lz].replace('XXXXX', message.chat.username) if message.chat.username else \
+                yeref.l_post_button[lz].replace('XXXXX', '')
             await bot.send_message(chat_id, text)
             await state.set_state(FsmOffer.button)
         else:
-            await bot.send_message(chat_id, l_offer_finish[lz])
+            await bot.send_message(chat_id, yeref.l_post_finish[lz])
             await state.set_state(FsmOffer.finish)
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
@@ -2078,15 +1574,15 @@
         day_, month_, year_ = offer_date.split('..')
         dt_user = datetime.datetime(year=int(year_), month=int(month_), day=int(day_))
 
         if message.text == '⬅️ Prev':
             await generate_calendar_admin(bot, state, lz, chat_id)
             await state.set_state(FsmOffer.date_)
         elif message.text in ['➡️️ Next', '/Next']:
-            await bot.send_message(chat_id, l_offer_finish[lz])
+            await bot.send_message(chat_id, yeref.l_post_finish[lz])
             await state.set_state(FsmOffer.finish)
         else:
             sql = "SELECT USER_TZ FROM USER WHERE USER_TID=?"
             data = await db_select(sql, (chat_id,), BASE_D)
             USER_TZ = data[0][0] if data[0][0] else "+00:00"
             offer_tz = USER_TZ
             await state.update_data(offer_tz=offer_tz)
@@ -2101,27 +1597,27 @@
             datetime_current = dt_cur.strftime("%H:%M")
 
             try:
                 arr = text.strip().split(':')
                 dt_user_new = datetime.datetime(year=int(year_), month=int(month_), day=int(day_), hour=int(arr[0]),
                                                 minute=int(arr[1]))
                 if dt_user_new < dt_cur:
-                    await message.answer(text=offer_time_future[lz])
+                    await message.answer(text=yeref.offer_time_future[lz])
                     return
             except Exception as e:
                 logger.info(log_ % str(e))
-                text = generate_calendar_time[lz].format(dt_user.strftime("%d-%m-%Y"), datetime_plus,
+                text = yeref.l_generate_calendar_time[lz].format(dt_user.strftime("%d-%m-%Y"), datetime_plus,
                                                          datetime_current, USER_TZ)
                 await bot.send_message(chat_id, text)
                 return
 
             offer_dt = dt_user_new.strftime('%d-%m-%Y %H:%M')
             await state.update_data(offer_dt=offer_dt)
 
-            await bot.send_message(chat_id, l_offer_finish[lz])
+            await bot.send_message(chat_id, yeref.l_post_finish[lz])
             await state.set_state(FsmOffer.finish)
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
@@ -2201,15 +1697,15 @@
 
     return reply_markup
 
 
 async def callbacks_offers_admin(bot, FsmOffer, call, state, BASE_D, bot_un):
     try:
         chat_id = call.from_user.id
-        src = call.data.split("_")[1]
+        # src = call.data.split("_")[1]
         post_id = int(call.data.split("_")[-1])
         lz = await lz_code(chat_id, call.from_user.language_code, BASE_D)
         has_restricted = (await bot.get_chat(chat_id)).has_restricted_voice_and_video_messages
 
         await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id, call)
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
@@ -3151,73 +2647,14 @@
 
 def cleanhtml(raw_html):
     cleanr = re.compile('<.*?>')
     cleantext = re.sub(cleanr, '', raw_html.strip())
     return cleantext
 
 
-async def init_bot(dp, bot, ref, message, CONF_P, EXTRA_D, MEDIA_D, BASE_D, fields_1):
-    await dp.bot.set_my_commands([
-        types.BotCommand("start", "⚙️ Restart"),
-        types.BotCommand("lang", "🇫🇷 Language"),
-        types.BotCommand("happy", "🐈 Happy"),
-    ])
-    os.makedirs(MEDIA_D, exist_ok=True, mode=0o777)
-
-    # add and sync USER to db
-    if not message.from_user.is_bot:
-        dt_ = datetime.datetime.utcnow().strftime("%d-%m-%Y %H:%M")
-        sql = "INSERT OR IGNORE INTO USER (USER_TID, USER_USERNAME, USER_FULLNAME, USER_DT) " \
-              "VALUES (?, ?, ?, ?)"
-        await db_change(sql, (message.from_user.id, message.from_user.username, message.from_user.full_name,
-                              dt_,), BASE_D)
-    if ref != '' and ref != str(message.from_user.id):
-        sql = "UPDATE USER SET USER_UTM = ? WHERE USER_TID = ?"
-        await db_change(sql, (ref, message.from_user.id,), BASE_D)
-    sql = f"SELECT {fields_1} FROM USER"
-    value_many = await db_select(sql, (), BASE_D)
-    spreadsheet_id = (r_conf('db_file_id', CONF_P))[0]
-    await api_sync_all(value_many, spreadsheet_id, CONF_P, EXTRA_D)
-
-    # pre-upload
-    sql = "SELECT * FROM FILE"
-    data = await db_select(sql, (), BASE_D)
-    if not data:
-        scopes = r_conf('scopes', CONF_P)
-        credential_file = os.path.join(EXTRA_D, (r_conf('credential_file', CONF_P))[0])
-        credentials = ServiceAccountCredentials.from_json_keyfile_name(credential_file, scopes)
-        http_auth = credentials.authorize(httplib2.Http())
-        drive_service = build('drive', 'v3', http=http_auth, cache_discovery=False)
-        file_list_dic = await api_get_file_list(drive_service, (r_conf('static_folder_id', CONF_P))[0], {})
-
-        for k, v in file_list_dic.items():
-            try:
-                result = None
-                fl_post = await get_from_media(CONF_P, EXTRA_D, MEDIA_D, BASE_D, v[0], re_write=True)
-                post = types.InputFile(fl_post) if fl_post and '/' in fl_post else fl_post
-                mimetype_folder = 'application/vnd.google-apps.folder'
-                if await is_video(fl_post) and v[1] != mimetype_folder and not str(v[0]).endswith('_note.mp4'):
-                    result = await bot.send_video(chat_id=my_tid, video=post, caption="")
-                elif await is_image(fl_post) and v[1] != mimetype_folder:
-                    result = await bot.send_photo(chat_id=my_tid, photo=post, caption="")
-                elif str(v[0]).endswith('.ogg') and v[1] != mimetype_folder:
-                    result = await bot.send_voice(chat_id=my_tid, voice=post, caption="")
-                elif str(v[0]).endswith('.mp3') and v[1] != mimetype_folder:
-                    result = await bot.send_audio(chat_id=my_tid, audio=post, caption="")
-                elif str(v[0]).endswith('_note.mp4') and v[1] != mimetype_folder:
-                    result = await bot.send_video_note(chat_id=my_tid, video_note=post)
-                if result:
-                    await save_fileid(result, v[0], BASE_D)
-            except Exception as e:
-                logger.info(log_ % str(e))
-                await asyncio.sleep(round(random.uniform(1, 2), 2))
-                print(e)
-        logger.info(log_ % "pre upload end")
-
-
 def get_post_of_dict(dicti_, pos=1):
     tmp = 1
     for k, v in dicti_.items():
         if tmp == pos:
             return k, v
         tmp += 1
     return None, None
@@ -3864,15 +3301,15 @@
         if os.path.exists(SESSION_NAME):
             os.remove(SESSION_NAME)
         await bot.send_message(my_tid, f"✅ deleteAccount {SESSION_TID} ok")
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
-        await log(e)
+        await log(e, CONF_P)
         await asyncio.sleep(round(random.uniform(1, 2), 2))
 
 
 async def delete_invalid_chat(chat, BASE_E):
     sql = "DELETE FROM CHANNEL WHERE CHANNEL_USERNAME=?"
     await db_change(sql, (chat,), BASE_E)
 
@@ -3926,16 +3363,16 @@
 
             if diff.days >= 0:
                 sql = "UPDATE SESSION SET SESSION_STATUS = ? WHERE SESSION_TID = ?"
                 await db_change(sql, (None, SESSION_TID,), BASE_S)
                 result = SESSION_TID
             else:
                 result = None
-    except Exception:
-        # await log(e)
+    except Exception as e:
+        await log(e)
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
 async def check_session_limit(SESSION_TID, LIMIT_NAME, LIMIT, BASE_S):
     result = SESSION_TID
```

