# Comparing `tmp/yeref-0.1.79.tar.gz` & `tmp/yeref-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.79.tar", last modified: Sat Jun  3 13:52:09 2023, max compression
+gzip compressed data, was "yeref-0.1.80.tar", last modified: Sun Jun  4 09:24:15 2023, max compression
```

## Comparing `yeref-0.1.79.tar` & `yeref-0.1.80.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-03 13:52:09.108363 yeref-0.1.79/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-03 13:52:09.108518 yeref-0.1.79/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-03 13:52:09.109118 yeref-0.1.79/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-03 13:51:57.000000 yeref-0.1.79/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-03 13:52:09.102951 yeref-0.1.79/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.79/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   533336 2023-06-03 13:51:24.000000 yeref-0.1.79/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   208414 2023-06-02 10:26:58.000000 yeref-0.1.79/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-03 13:52:09.107926 yeref-0.1.79/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-03 13:52:09.000000 yeref-0.1.79/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-03 13:52:09.000000 yeref-0.1.79/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-03 13:52:09.000000 yeref-0.1.79/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-03 13:52:09.000000 yeref-0.1.79/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-04 09:24:15.859728 yeref-0.1.80/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-04 09:24:15.859881 yeref-0.1.80/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-04 09:24:15.860490 yeref-0.1.80/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-04 09:24:01.000000 yeref-0.1.80/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-04 09:24:15.847750 yeref-0.1.80/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.80/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   533408 2023-06-04 09:12:57.000000 yeref-0.1.80/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   208832 2023-06-04 07:17:18.000000 yeref-0.1.80/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-04 09:24:15.859277 yeref-0.1.80/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-04 09:24:15.000000 yeref-0.1.80/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-04 09:24:15.000000 yeref-0.1.80/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-04 09:24:15.000000 yeref-0.1.80/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-04 09:24:15.000000 yeref-0.1.80/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.79/setup.py` & `yeref-0.1.80/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.79',
+      version='0.1.80',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.79/yeref/l_.py` & `yeref-0.1.80/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -909,119 +909,119 @@
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>información</b> sobre todos los proyectos\n\n❗️ también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>informations</b> sur tous les projets\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
     'zh': "🌱 {0}，欢迎来到<b>Ferey</b> <code>проекта</code>的<i>落地机器人</i>：\n\n▪️ 所有项目的<b>信息</b>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>معلومات</b> حول جميع المشاريع\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 
 l_kind_1 = {
-    'ru': "<b>👩🏽‍💻@FereyDemoBot</b>\n\nДемонстрационный бот всех проектов",
+    'ru': "<b>👩🏽‍💻@FereyDemoBot</b>\n\n<b>Демо</b> бот всех проектов",
     'en': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nDemo bot of all projects",
     'es': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nBot de demostración de todos los proyectos",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\nDemo bot de tous les projets",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyDemoBot</b>\n\n所有项目的演示机器人",
     'ar': "<b>👩🏽‍💻FereyDemoBot</b>\n\nروبوت تجريبي <b>@FereyDemoBot</b> المشاريع",
 }
 l_kind_2 = {
-    'ru': "<b>👩🏽‍💻@FereyBotBot</b>\n\nКонструктор ботов:\n▪️авто-генерация бота\n▪️авто-генерация контента (open-ai)\n▪️авто-бан/авто-перевод",
+    'ru': "<b>👩🏽‍💻@FereyBotBot</b>\n\n<b>Конструктор</b> ботов:\n▪️авто-генерация бота\n▪️авто-генерация контента (open-ai)\n▪️авто-бан/перевод/рассылка",
     'en': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nBot Builder:\n▪️auto-generate bot\n▪️auto-generate content (open-ai)\n▪️auto-ban/auto-translate",
     'es': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nGenerador de bots:\n▪️generación automática de bot\n▪️generación automática de contenido (open-ai)\n▪️prohibición automática/traducción automática",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nBot Builder :\n▪️auto-génère le bot\n▪️auto-génère le contenu (open-ai)\n▪️auto-ban/auto-translate",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyBotBot</b>\n\nBot Builder：\n▪️自动生成机器人\n▪️自动生成内容（open-ai）\n▪️自动禁止/自动翻译",
     'ar': "<b>👩🏽‍💻FereyBotBot</b>\n\nBot Builder:\n▪️ إنشاء روبوت تلقائيًا <b>@FereyBotBot</b> n▪️ إنشاء محتوى تلقائيًا (فتح ai)\n▪️ حظر تلقائي / ترجمة آلية",
 }
 l_kind_3 = {
-    'ru': "<b>👩🏽‍💻@FereyChannelBot</b>\n\nАдминистратор каналов:\n▪️авто-постинг\n▪️авто-декор",
+    'ru': "<b>👩🏽‍💻@FereyChannelBot</b>\n\n<b>Администрирование</b> каналов:\n▪️авто-постинг\n▪️авто-декор",
     'en': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\nChannel admin:\n▪️auto-posting\n▪️auto-decor",
     'es': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\nAdministrador del canal:\n▪️publicación automática\n▪️decoración automática",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\nAdministrateur de la chaîne :\n▪️publication automatique\n▪️décoration automatique",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyChannelBot</b>\n\n频道管理员：\n▪️自动发布\n▪️自动装饰",
     'ar': "<b>👩🏽‍💻FereyChannelBot</b>\n\nمسؤول القناة:\nنشر تلقائي <b>@FereyChannelBot</b> n ديكور تلقائي",
 }
 l_kind_4 = {
-    'ru': "<b>👩🏽‍💻@FereyGroupBot</b>\n\nАдминистратор групп:\n▪️авто-постинг\n▪️модерация",
+    'ru': "<b>👩🏽‍💻@FereyGroupBot</b>\n\n<b>Модерация</b> групп:\n▪️авто-постинг\n▪️модерация",
     'en': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\nGroup admin:\n▪️auto-posting\n▪️moderation",
     'es': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\nAdministrador del grupo:\n▪️publicación automática\n▪️moderación",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\nAdministrateur du groupe :\n▪️publication automatique\n▪️modération",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyGroupBot</b>\n\n群组管理员：\n▪️自动发布\n▪️审核",
     'ar': "<b>👩🏽‍💻FereyGroupBot</b>\n\n<b>@FereyGroupBot</b> المجموعة:\nنشر تلقائي\n▪️ تعديل",
 }
 l_kind_5 = {
-    'ru': "<b>👩🏽‍💻@FereyUserBot</b>\n\nАдминистратор пользователей:\n▪️авто-постинг\n▪️авто-декор",
+    'ru': "<b>👩🏽‍💻@FereyUserBot</b>\n\n<b>Автоматизация</b> пользователей:\n▪️авто-постинг\n▪️авто-декор",
     'en': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\nUser Admin:\n▪️auto-posting\n▪️auto-decor",
     'es': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\nAdministrador de usuarios:\n▪️publicación automática\n▪️decoración automática",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\nAdministrateur utilisateur :\n▪️publication automatique\n▪️décoration automatique",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyUserBot</b>\n\n用户管理员：\n▪️自动发布\n▪️自动装饰",
     'ar': "<b>👩🏽‍💻FereyUserBot</b>\n\nمسؤول المستخدم:\nنشر <b>@FereyUserBot</b>\nديكور تلقائي",
 }
 l_kind_6 = {
-    'ru': "<b>👩🏽‍💻@FereyPostBot</b>\n\nБыстрое создание и публикация постов:\n▪️превью\n▪️галерея",
+    'ru': "<b>👩🏽‍💻@FereyPostBot</b>\n\n<b>Приватные посты</b>:\n▪️превью\n▪️галерея",
     'en': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\nQuick post creation and publishing:\n▪️preview\n▪️gallery",
     'es': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\nCreación y publicación rápidas de publicaciones:\n▪️vista previa\n▪️galería",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\nCréation et publication rapides d'articles :\n▪️aperçu\n▪️galerie",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyPostBot</b>\n\n快速创建和发布帖子：\n▪️预览\n▪️图库",
     'ar': "<b>👩🏽‍💻FereyPostBot</b>\n\nإنشاء منشور سريع <b>@FereyPostBot</b> :\nمعاينة\n▪️ معرض",
 }
 l_kind_7 = {
-    'ru': "<b>👩🏽‍💻@FereyFindBot</b>\n\nПоиск по каналам/группам/пользователям/ботам:\n▪️отслеживание постов\n▪️гео-поиск",
+    'ru': "<b>👩🏽‍💻@FereyFindBot</b>\n\n<b>Поиск</b> по каналам/группам/пользователям/ботам:\n▪️отслеживание постов\n▪️гео-поиск",
     'en': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\nSearch by channels/groups/users/bots:\n▪️post tracking\n▪️geo-search",
     'es': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\nBuscar por canales/grupos/usuarios/bots:\n▪️seguimiento de publicaciones\n▪️búsqueda geográfica",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\nRecherche par canaux/groupes/utilisateurs/bots :\n▪️suivi des publications\n▪️géo-recherche",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyFindBot</b>\n\n按频道/群组/用户/机器人搜索：\n▪️post tracking\n▪️geo-search",
     'ar': "<b>👩🏽‍💻FereyFindBot</b>\n\nالبحث عن طريق القنوات / المجموعات <b>@FereyFindBot</b> المستخدمين / الروبوتات:\n▪️ تتبع المنشور\n▪️ البحث الجيو",
 }
 l_kind_8 = {
-    'ru': "<b>👩🏽‍💻@FereyMediaBot</b>\n\nБот с популярными креативами:\n▪️аудио-заметки\n▪️видео-заметки",
+    'ru': "<b>👩🏽‍💻@FereyMediaBot</b>\n\n<b>Медиа-заметки</b>:\n▪️аудио/️видео-заметки\n▪️текст/фото-стикеры",
     'en': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\nBot with popular creatives:\n▪️audio notes\n▪️video notes",
     'es': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\nBot con creatividades populares:\n▪️notas de audio\n▪️notas de video",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\nBot avec des créations populaires :\n▪️notes audio\n▪️notes vidéo",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyMediaBot</b>\n\n具有流行创意的机器人：\n▪️音频笔记\n▪️视频笔记",
     'ar': "<b>👩🏽‍💻FereyMediaBot</b>\n\nاستخدام التصميمات المشهورة:\n▪️ ملاحظات <b>@FereyMediaBot</b>\n▪️ ملاحظات الفيديو",
 }
 l_kind_9 = {
-    'ru': "<b>👩🏽‍💻@FereyVpnBot</b>\n\nВсе о VPN",
+    'ru': "<b>👩🏽‍💻@FereyVPNBot</b>\n\n<b>Настройка</b>VPN",
     'en': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\nAll about VPN",
     'es': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\nTodo sobre VPN",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\nTout sur le VPN",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyVpnBot</b>\n\n关于 VPN",
     'ar': "<b>👩🏽‍💻FereyVpnBot</b> <b>@FereyVpnBot</b> n\nكل شيء عن VPN",
 }
 l_kind_10 = {
-    'ru': "<b>👩🏽‍💻@FereyTargetBot</b>\n\nТаргетированная рассылка",
+    'ru': "<b>👩🏽‍💻@FereyTargetBot</b>\n\n<b>Таргет</b> сообщений/пользователей",
     'en': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\nTargeted email",
     'es': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\nCorreo electrónico dirigido",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\nE-mail ciblé",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyTargetBot</b>\n\n目标电子邮件",
     'ar': "<b>👩🏽‍💻FereyTargetBot</b> \ <b>@FereyTargetBot</b>\nالبريد الإلكتروني المستهدف",
 }
 l_kind_11 = {
-    'ru': "<b>👩🏽‍💻@FereyToolsBot</b>\n\nБот инструментов:\n▪️конвертация\n▪️загрузка",
+    'ru': "<b>👩🏽‍💻@FereyToolsBot</b>\n\n<b>Телеграм инструменты</b>:\n▪️конвертация файлов\n▪️шаблоны",
     'en': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\nTool bot:\n▪️convert\n▪️download",
     'es': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\nHerramienta bot:\n▪️convertir\n▪️descargar",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\nBot outil :\n▪️convertir\n▪️télécharger",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyToolsBot</b>\n\n工具机器人：\n▪️转换\n▪️下载",
     'ar': "<b>👩🏽‍💻FereyToolsBot</b>\n\ <b>@FereyToolsBot</b> بوت الأداة:\n▪️ تحويل\n▪️ تحميل",
 }
 l_kind_12 = {
-    'ru': "<b>👩🏽‍💻@FereyAIBot</b>\n\nБот генерации контента (open-ai):\n▪️chat-gpt\n▪️dalli·e",
+    'ru': "<b>👩🏽‍💻@FereyAIBot</b>\n\n<b>Нейросеть</b> генерации контента (open-ai):\n▪️chat-gpt\n▪️dalli·e",
     'en': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\nContent generation bot (open-ai):\n▪️chat-gpt\n▪️dalli e",
     'es': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\nBot de generación de contenido (open-ai):\n▪️chat-gpt\n▪️dalli e",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\nBot de génération de contenu (open-ai) :\n▪️chat-gpt\n▪️dalli e",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyAIBot</b>\n\n内容生成机器人（open-ai）：\n▪️chat-gpt\n▪️dalli e",
     'ar': "<b>👩🏽‍💻FereyAIBot</b>\n\nروبوت إنشاء المحتوى (open <b>@FereyAIBot</b> ai):\n▪️chat-gpt\n▪️dalli e",
 }
 l_kind_13 = {
-    'ru': "<b>👩🏽‍💻@FereyAdsBot</b>\n\nБот рекламы в:\n▪️ботах\n▪️каналах",
+    'ru': "<b>👩🏽‍💻@FereyAdsBot</b>\n\n<b>Реклама</b> в:\n▪️ботах",
     'en': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\nBot ads in:\n▪️bots\n▪️channels",
     'es': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\nAnuncios de bot en:\n▪️bots\n▪️canales",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\nAnnonces de robots dans :\n▪️bots\n▪️chaînes",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyAdsBot</b>\n\n机器人广告在：\n▪️bots\n▪️channels",
     'ar': "<b>👩🏽‍💻FereyAdsBot</b>\n\n<b>@FereyAdsBot</b> الإعلانات في:\n▪️ الروبوتات\n▪️ القنوات",
 }
 l_kind_14 = {
-    'ru': "<b>👩🏽‍💻@FereyWorkBot</b>\n\nБот информации о:\n▪️вакансиях\n▪️соревнованиях",
+    'ru': "<b>👩🏽‍💻@FereyWorkBot</b>\n\n<b>Рабочий</b> бот информации о:\n▪️вакансиях\n▪️соревнованиях",
     'en': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\nBot of information about:\n▪️vacancies\n▪️competitions",
     'es': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\nBot de información sobre:\n▪️vacantes\n▪️concursos",
     'fr': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\nBot d'informations sur :\n▪️offres d'emploi\n▪️concours",
     'zh': "<b>👩🏽‍💻</b> <b>@FereyWorkBot</b>\n\n有关以下信息的机器人：\n▪️职位空缺\n▪️比赛",
     'ar': "<b>👩🏽‍💻FereyWorkBot</b>\n\nبعض <b>@FereyWorkBot</b> حول:\n▪️ وظائف شاغرة\n▪️ مسابقات",
 }
 # endregion
@@ -6167,17 +6167,17 @@
 
 # endregion
 
 
 # region FereyBotBot
 l_bot_btn1 = {
     'ru': "⛰ Боты",
-    'en': "⛰ Boots",
-    'es': "⛰ Botas",
-    'fr': "⛰ Bottes",
+    'en': "⛰ Bots",
+    'es': "⛰ Bots",
+    'fr': "⛰ Bots",
     'zh': "⛰ 靴子",
     'ar': "⛰ أحذية",
 }
 l_bot_btn2 = {
     'ru': "🌬 Подписка",
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
@@ -7016,15 +7016,15 @@
     'en': "Export as >",
     'es': "Exportar como >",
     'fr': "Exporter sous >",
     'zh': "导出为 >",
     'ar': "تصدير باسم>",
 }
 l_burger_clear = {
-    'ru': "Очистка",
+    'ru': "Очистить",
     'en': "Cleaning",
     'es': "Limpieza",
     'fr': "Nettoyage",
     'zh': "打扫",
     'ar': "تنظيف",
 }
 l_burger_gen_alert = {
```

### Comparing `yeref-0.1.79/yeref/yeref.py` & `yeref-0.1.80/yeref/yeref.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,15 @@
                     if param:
                         cur.execute(sql, param)
                     else:
                         cur.execute(sql)
 
                     return cur.fetchall()
         except Exception as e:
-            await log(e)
+            logger.info(log_ % str(e))
             await asyncio.sleep(round(random.uniform(1, 2), 2))
             retry -= 1
     return []
 
 
 async def db_change(sql, param=None, db=None):
     retry = 2
@@ -207,15 +207,15 @@
                         cur.execute(sql, param)
                     else:
                         cur.execute(sql)
 
                     con.commit()
                     return cur.lastrowid
         except Exception as e:
-            await log(e)
+            logger.info(log_ % str(e))
             await asyncio.sleep(round(random.uniform(1, 2), 2))
             retry -= 1
     return 0
 
 
 async def db_bot_create(db):
     con = sqlite3.connect(db, timeout=10)
@@ -468,15 +468,15 @@
         return telegraph_, result
 
 
 async def tgph_change(access_token, url, json_):
     retry = 2
     while retry > 0:
         try:
-            await asyncio.sleep(round(random.uniform(0, 1), 2))
+            await asyncio.sleep(round(random.uniform(1, 2), 2))
             telegraph_ = Telegraph(access_token=access_token)
             pages_ = await telegraph_.get_page_list()
 
             for page_ in pages_['pages']:
                 if page_['url'] != url: continue
 
                 get_page_ = await telegraph_.get_page(path=page_['path'], return_content=True, return_html=False)
@@ -2374,15 +2374,15 @@
 
 async def fun_empty(txt):
     try:
         txt = str(txt)
         if '%' in txt:
             print(txt)
     except Exception as e:
-        await log(f'\033[95m%s\033[0m' % str(e))
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
 
 
 async def lz_code(chat_id, lan, BASE_D):
     result = 'en'
     try:
         sql = "SELECT USER_LZ FROM USER WHERE USER_TID=?"
@@ -2407,15 +2407,15 @@
                 result = 'ru'
 
             sql = "UPDATE USER SET USER_LZ=? WHERE USER_TID=?"
             await db_change(sql, (result, chat_id,), BASE_D)
         else:
             result = data[0][0]
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
 async def no_war_text(txt):
     result = txt
@@ -3252,15 +3252,15 @@
                     "hostname": hostname,
                     "port": int(port),
                     "username": username,
                     "password": password
                 }
                 break
             except Exception as e:
-                await log(e)
+                logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(1, 2), 2))
     except Exception as e:
         logger.info(log_ % f"{str(e)}, {identifier}, {server}")
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
@@ -3332,15 +3332,15 @@
                 if el not in string.ascii_letters + string.digits + "@_https://t.me/+ ":
                     link = link.replace(el, '')
         except Exception:
             pass
 
         result = link
     except Exception:
-        # await log(e)
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
 def is_names(phrase):
     # (?s)\bhello\b.*?\b
@@ -3567,15 +3567,15 @@
                         await bot.send_message(chat_id, txt_)
                         return
                     result = await app.get_chat(r.id)
                     if is_history:
                         try:
                             get_chat_history_count = await app.get_chat_history_count(r.id)
                         except Exception as e:
-                            await log(e)
+                            logger.info(log_ % str(e))
                             await asyncio.sleep(round(random.uniform(0, 1), 2))
 
                     await leave_my_chat(app, result, link)
                 break
             except (FloodWait, SlowmodeWait) as e:
                 wait_ = f"Wait: {datetime.datetime.utcfromtimestamp(e.value + 1).strftime('%H:%M:%S')}"
                 logger.info(log_ % wait_)
@@ -3595,15 +3595,15 @@
             except Exception as e:
                 logger.info(log_ % f"{SESSION_TID}: {str(e)}")
                 await asyncio.sleep(round(random.uniform(1, 2), 2))
             finally:
                 sql = "UPDATE SESSION SET SESSION_STATUS = ? WHERE SESSION_TID = ?"
                 await db_change(sql, (SESSION_STATUS, SESSION_TID,), BASE_S)
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result, get_chat_history_count
 
 
 async def is_invite_chat(bot, chat_id, link, SESSIONS_D, EXTRA_D, CONF_P, BASE_S, BASE_E):
     result = None
@@ -3643,15 +3643,15 @@
                         await bot.send_message(chat_id, text)
                         # await asyncio.sleep(r_conf('AWAIT_JOIN'))
 
                         try:
                             get_chat_member = await app.get_chat_member(chat_id=r.id, user_id=int(SESSION_TID))
                             result = True if get_chat_member and get_chat_member.status.value == 'member' else False
                         except Exception as e:
-                            await log(e)
+                            logger.info(log_ % str(e))
                             await asyncio.sleep(round(random.uniform(1, 2), 2))
 
                     # leave_chat
                     await leave_my_chat(app, r, link)
                 break
             except (FloodWait, SlowmodeWait) as e:
                 wait_ = f"Wait: {datetime.datetime.utcfromtimestamp(e.value + 1).strftime('%H:%M:%S')}"
@@ -3672,30 +3672,30 @@
             except Exception as e:
                 logger.info(log_ % f"{SESSION_TID}: {str(e)}")
                 await asyncio.sleep(round(random.uniform(1, 2), 2))
             finally:
                 sql = "UPDATE SESSION SET SESSION_STATUS = ? WHERE SESSION_TID = ?"
                 await db_change(sql, (SESSION_STATUS, SESSION_TID,), BASE_S)
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
 async def join_my_chat(bot, app, chat_id, link, SESSION_TID, BASE_S):
     result = None
     try:
         if 't.me/c/' in str(link):
             try:
                 tmp = link.strip('https://t.me/c/').split('/')[0]
                 peer_channel = await app.resolve_peer(int(f"-100{tmp}"))
                 result = await app.invoke(functions.channels.JoinChannel(channel=peer_channel))
             except Exception as e:
-                await log(e)
+                logger.info(log_ % str(e))
         else:
             result = await app.join_chat(link)
         await asyncio.sleep(1)
     except (FloodWait, SlowmodeWait) as e:
         text = log_ % f"Wait: {datetime.datetime.utcfromtimestamp(e.value + 1).strftime('%H:%M:%S')}"
         logger.info(text)
         await asyncio.sleep(round(random.uniform(5, 10), 2))
@@ -3707,33 +3707,33 @@
     except UserAlreadyParticipant as e:
         logger.info(log_ % f"UserAlreadyParticipant {link}: {str(e)}")
         try:
             result = await app.get_chat(link)
         except Exception:
             pass
     except (InviteHashExpired, InviteHashInvalid) as e:
-        await log(e)
+        logger.info(log_ % str(e))
         try:
             result = await app.join_chat(link)
         except Exception:
             await bot.send_message(chat_id, f"️👩🏽‍💻 Link {link} is invalid or try later")
     except (UsernameInvalid, UsernameNotOccupied, ChannelBanned) as e:
-        await log(e)
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
         await bot.send_message(chat_id, f"️👩🏽‍💻 Link {link} is invalid or try later")
     except BadRequest as e:
-        await log(e)
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(2, 3), 2))
 
         try:
             result = await app.join_chat(link)
         except Exception:
             result = -1
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
 async def leave_my_chat(app, r, link):
     try:
@@ -3783,19 +3783,19 @@
                     try:
                         async for member in app.get_chat_members(r.id, filter=enums.ChatMembersFilter.SEARCH):
                             if member.user.username and not member.user.is_bot and not member.user.is_deleted and \
                                     not member.user.is_scam and not member.user.is_fake and not member.user.is_support \
                                     and str(member.user.id) not in data_:
                                 tmp_members.append(member.user.username)
                     except ChatAdminRequired as e:
-                        await log(e)
+                        logger.info(log_ % str(e))
                         await bot.send_message(chat_id, f"🔺 Требуются права админа")
                         return
                     except Exception as e:
-                        await log(e)
+                        logger.info(log_ % str(e))
 
                     # leave chat
                     await leave_my_chat(app, r, link)
 
                     result = tmp_members
                     break
             except (FloodWait, SlowmodeWait) as e:
@@ -3817,15 +3817,15 @@
             except Exception as e:
                 logger.info(log_ % f"{SESSION_TID}: {str(e)}")
                 await asyncio.sleep(round(random.uniform(1, 2), 2))
             finally:
                 sql = "UPDATE SESSION SET SESSION_STATUS = ? WHERE SESSION_TID = ?"
                 await db_change(sql, (SESSION_STATUS, SESSION_TID,), BASE_S)
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
 async def delete_account(bot, SESSION_TID, SESSIONS_D, CONF_P, BASE_S):
     try:
@@ -3908,15 +3908,15 @@
             if diff.days >= 0:
                 sql = "UPDATE SESSION SET SESSION_STATUS = ? WHERE SESSION_TID = ?"
                 await db_change(sql, (None, SESSION_TID,), BASE_S)
                 result = SESSION_TID
             else:
                 result = None
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
 async def check_session_limit(SESSION_TID, LIMIT_NAME, LIMIT, BASE_S):
     result = SESSION_TID
@@ -3941,15 +3941,15 @@
                 sql = f"UPDATE SESSION SET {LIMIT_NAME} = ? WHERE SESSION_TID = ?"
                 await db_change(sql, (result, SESSION_TID,), BASE_S)
             elif msg_by_day < LIMIT:
                 result = SESSION_TID
             else:
                 result = None
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
 async def check_inviteday(CONF_P, BASE_S, threshold=0):
     result = 0
@@ -3963,22 +3963,22 @@
                 checkSessionLimit_ = await check_session_limit(SESSION_TID, 'SESSION_INVITEDAY', INVITEDAY_LIMIT_,
                                                                BASE_S)
                 if SESSION_INVITEDAY == '' or SESSION_INVITEDAY is None:
                     result += INVITEDAY_LIMIT_
                 elif await check_session_flood(SESSION_TID, BASE_S) and checkSessionLimit_:
                     result += r_conf('INVITEDAY_LIMIT', CONF_P) - int(SESSION_INVITEDAY.split()[0])
             except Exception as e:
-                await log(e)
+                logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(1, 2), 2))
 
         result = int(result * 0.6)
         if threshold:
             result = result if result < threshold else threshold
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
 # endregion
 
@@ -4015,15 +4015,15 @@
         convert_value = []
         for item in value_many:
             convert_value.append(list(item))
 
         await api_write_cells(sheets_service, convert_value, range_many, spreadsheet_id, sheet_id, value_input_option,
                               major_dimension)
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
 
 
 async def api_find_row_by_tid(USER_TID, CONF_P, EXTRA_D, sheet_id='Sheet1'):
     result = None
     try:
         scopes_ = r_conf('scopes', CONF_P)
         credential_file_ = os.path.join(EXTRA_D, (r_conf('credential_file', CONF_P))[0])
@@ -4054,44 +4054,44 @@
             "data": [{
                 "range": f"{sheet_id}!{range_many}",
                 "majorDimension": majorDimension,
                 "values": value_many,
             }]}).execute()
         logger.info(log_ % 'write to db ok')
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
     finally:
         return result
 
 
 async def api_append_cells(sheets_service, value_many, spreadsheet_id, valueInputOption):
     result = True
     try:
         sheets_service.spreadsheets().values().append(spreadsheetId=spreadsheet_id, range='A1',
                                                       valueInputOption=valueInputOption,
                                                       body={"values": value_many}).execute()
 
         logger.info(log_ % 'write to db ok')
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
         result = False
     return result
 
 
 async def api_read_cells(sheets_service, range_many, spreadsheet_id, sheet_id='Sheet1'):
     result = None
     try:
         r = sheets_service.spreadsheets().values().batchGet(
             spreadsheetId=spreadsheet_id, ranges=f"{sheet_id}!{range_many}"
         ).execute()
 
         result = r.get('valueRanges', [])[0]['values'] if len(r.get('valueRanges', [])) > 0 else None
         logger.info(log_ % 'read from db ok')
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
     finally:
         return result
 
 
 def get_random_color():
     """
     Создаю случайный цвет с альфа каном
@@ -4153,15 +4153,15 @@
         cnt += 1
         logger.info(log_ % f"\t{cnt}. send to user {USER_TID}-{USER_USERNAME} ok")
         await asyncio.sleep(0.05)
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
         logger.info(log_ % f"\tsend to user {USER_TID}-{USER_USERNAME} error")
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return cnt
 
 
 async def api_get_file_list(drive_service, folder_id, tmp_dic=None, parent_name='', is_file=False):
@@ -4179,15 +4179,15 @@
         try:
             if item['mimeType'] == 'application/vnd.google-apps.folder':
                 tmp_dic[item['id']] = [item['name'], item['mimeType'], parent_name, item['modifiedTime']]
                 await api_get_file_list(drive_service, item['id'], tmp_dic, item['name'])
             else:
                 tmp_dic[item['id']] = [item['name'], item['mimeType'], parent_name, item['modifiedTime']]
         except Exception as e:
-            await log(e)
+            logger.info(log_ % str(e))
 
     tmp_dic_2 = {}
     for k, v in reversed(tmp_dic.items()):
         tmp_dic_2[k] = v
 
     return tmp_dic_2
 
@@ -4206,15 +4206,15 @@
             status, response = request_.next_chunk()
             if status: logger.info(log_ % "Uploaded %d%%." % int(status.progress() * 100))
         logger.info(log_ % "Upload Complete!")
         # if os.path.exists(post_media_name):
         #     os.remove(post_media_name)
         result = True
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
     finally:
         return result
 
 
 async def api_dl_file(drive_service, id_, name, gdrive_mime_type, MEDIA_D):
     save_mime_type = None
     file_name = add = ''
@@ -4372,15 +4372,15 @@
         if ':' in range_many:
             result = r.get('valueRanges', [])[0]['values'] if len(r.get('valueRanges', [])) > 0 else None
             result = [item[0] for item in result]
         else:
             result = r.get('valueRanges', [])[0]['values'][0][0] if len(r.get('valueRanges', [])) > 0 else None
         logger.info(log_ % 'read from db ok')
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
     finally:
         return result
 
 
 async def get_list_of_send_folder(CONF_P, EXTRA_D):
     scopes = r_conf('scopes', CONF_P)
     credential_file = os.path.join(EXTRA_D, (r_conf('credential_file', CONF_P))[0])
@@ -4394,15 +4394,15 @@
         try:
             parent_folder = v[2]
             name_folder = v[0]
             datetime_ = datetime.datetime.now()
             if parent_folder == '' and datetime_ < datetime.datetime.strptime(name_folder, "%d-%m-%Y %H:%M"):
                 tmp.append([name_folder, k])
         except Exception as e:
-            await log(e)
+            logger.info(log_ % str(e))
 
     return tmp
 
 
 async def save_post_to_google_drive(CONF_P, EXTRA_D, post_txt, post_btn, post_url, post_media_name,
                                     post_media_type, post_pin, post_time, post_media_options, post_users='*'):
     try:
@@ -4453,15 +4453,15 @@
             CONF_P=CONF_P,
             EXTRA_D=EXTRA_D,
             range_many='B1',
             major_dimension="COLUMNS"
         )
         logger.info(log_ % 'save to google ok')
     except Exception as e:
-        await log(e)
+        logger.info(log_ % str(e))
 
 
 # endregion
 
 
 # region aiogram
 async def convert_domain_to_currency(domain):
```

