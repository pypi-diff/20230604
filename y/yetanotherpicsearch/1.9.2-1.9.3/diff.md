# Comparing `tmp/yetanotherpicsearch-1.9.2.tar.gz` & `tmp/yetanotherpicsearch-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetanotherpicsearch-1.9.2.tar", max compression
+gzip compressed data, was "yetanotherpicsearch-1.9.3.tar", max compression
```

## Comparing `yetanotherpicsearch-1.9.2.tar` & `yetanotherpicsearch-1.9.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/LICENSE
--rw-r--r--   0        0        0     2041 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/README.md
--rw-r--r--   0        0        0     9390 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/__init__.py
--rw-r--r--   0        0        0     2089 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/ascii2d.py
--rw-r--r--   0        0        0      657 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/baidu.py
--rw-r--r--   0        0        0     2781 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/config.py
--rw-r--r--   0        0        0     5086 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/ehentai.py
--rw-r--r--   0        0        0     1195 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/google.py
--rw-r--r--   0        0        0     1959 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/iqdb.py
--rw-r--r--   0        0        0     3132 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/nhentai.py
--rw-r--r--   0        0        0      924 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/nhentai_model.py
--rw-r--r--   0        0        0     6003 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/saucenao.py
--rw-r--r--   0        0        0     6751 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/utils.py
--rw-r--r--   0        0        0     1827 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/whatanime.py
--rw-r--r--   0        0        0     1075 2023-05-26 15:29:43.898918 yetanotherpicsearch-1.9.2/YetAnotherPicSearch/yandex.py
--rw-r--r--   0        0        0     1432 2023-05-26 15:29:43.906918 yetanotherpicsearch-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     3458 1970-01-01 00:00:00.000000 yetanotherpicsearch-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/LICENSE
+-rw-r--r--   0        0        0     2041 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/README.md
+-rw-r--r--   0        0        0     9390 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/__init__.py
+-rw-r--r--   0        0        0     2089 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/ascii2d.py
+-rw-r--r--   0        0        0      657 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/baidu.py
+-rw-r--r--   0        0        0     2781 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/config.py
+-rw-r--r--   0        0        0     5086 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/ehentai.py
+-rw-r--r--   0        0        0     1195 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/google.py
+-rw-r--r--   0        0        0     2003 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/iqdb.py
+-rw-r--r--   0        0        0     3132 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/nhentai.py
+-rw-r--r--   0        0        0      924 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/nhentai_model.py
+-rw-r--r--   0        0        0     6047 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/saucenao.py
+-rw-r--r--   0        0        0     7416 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/utils.py
+-rw-r--r--   0        0        0     1827 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/whatanime.py
+-rw-r--r--   0        0        0     1075 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/yandex.py
+-rw-r--r--   0        0        0     1427 2023-06-04 16:53:46.162186 yetanotherpicsearch-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     3453 1970-01-01 00:00:00.000000 yetanotherpicsearch-1.9.3/PKG-INFO
```

### Comparing `yetanotherpicsearch-1.9.2/LICENSE` & `yetanotherpicsearch-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/README.md` & `yetanotherpicsearch-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/__init__.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/__init__.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/ascii2d.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/ascii2d.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/baidu.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/baidu.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/config.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/config.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/ehentai.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/ehentai.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/google.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/google.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/iqdb.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/iqdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from typing import List, Optional, Tuple
 
-from httpx import URL, AsyncClient
+from httpx import AsyncClient
 from PicImageSearch import Iqdb
 
 from .ascii2d import ascii2d_search
 from .config import config
-from .utils import SEARCH_FUNCTION_TYPE, async_lock, get_source, handle_img, shorten_url
+from .utils import (
+    SEARCH_FUNCTION_TYPE,
+    async_lock,
+    get_source,
+    get_valid_url,
+    handle_img,
+    shorten_url,
+)
 
 
 @async_lock()
 async def iqdb_search(
     url: str, client: AsyncClient
 ) -> Tuple[List[str], Optional[SEARCH_FUNCTION_TYPE]]:
     iqdb = Iqdb(client=client)
@@ -33,15 +40,15 @@
         selected_res = danbooru_res_list[0]
     elif yandere_res_list:
         selected_res = yandere_res_list[0]
 
     thumbnail = await handle_img(selected_res.thumbnail, hide_img)
     source = await get_source(selected_res.url)
     if source:
-        if URL(source).host:
+        if get_valid_url(source):
             source = await shorten_url(source)
         source = f"来源：{source}"
     res_list = [
         f"Iqdb ({selected_res.similarity}%)",
         thumbnail,
         await shorten_url(selected_res.url),
         source,
```

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/nhentai.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/nhentai.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/nhentai_model.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/nhentai_model.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/saucenao.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/saucenao.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import re
 from typing import List, Optional, Tuple
 
-from httpx import URL, AsyncClient
+from httpx import AsyncClient
 from PicImageSearch import SauceNAO
 from PicImageSearch.model import SauceNAOItem, SauceNAOResponse
 
 from .ascii2d import ascii2d_search
 from .config import config
 from .ehentai import ehentai_title_search
 from .nhentai import nhentai_title_search
-from .utils import SEARCH_FUNCTION_TYPE, async_lock, get_source, handle_img, shorten_url
+from .utils import (
+    SEARCH_FUNCTION_TYPE,
+    async_lock,
+    get_source,
+    get_valid_url,
+    handle_img,
+    shorten_url,
+)
 from .whatanime import whatanime_search
 
 SAUCENAO_DB = {
     "all": 999,
     "pixiv": 5,
     "danbooru": 9,
     "anime": [21, 22],
@@ -99,15 +106,15 @@
 
     thumbnail = await handle_img(selected_res.thumbnail, hide_img)
 
     url = await shorten_url(selected_res.url)
     source = selected_res.source if selected_res.source != selected_res.title else ""
     if not source and selected_res.url:
         source = await get_source(selected_res.url)
-    if source and URL(source).host:
+    if source and get_valid_url(source):
         source = await shorten_url(source)
 
     author_link = (
         f"[{selected_res.author}]({await shorten_url(selected_res.author_url)})"
         if selected_res.author and selected_res.author_url
         else ""
     )
```

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/utils.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Optional,
     TypeVar,
     Union,
 )
 
 import arrow
 from cachetools import TTLCache
-from httpx import URL, AsyncClient
+from httpx import URL, AsyncClient, InvalidURL
 from nonebot.adapters.onebot.v11 import Bot
 from PicImageSearch.model.ehentai import EHentaiItem, EHentaiResponse
 from pyquery import PyQuery
 from shelved_cache import cachedasyncmethod
 
 from .config import config
 from .nhentai_model import NHentaiItem, NHentaiResponse
@@ -71,34 +71,56 @@
     return [i["user_id"] for i in friend_list]
 
 
 def handle_reply_msg(message_id: int) -> str:
     return f"[CQ:reply,id={message_id}]"
 
 
+def handle_source(source: str) -> str:
+    return (
+        source.replace("www.pixiv.net/en/artworks", "www.pixiv.net/artworks")
+        .replace(
+            "www.pixiv.net/member_illust.php?mode=medium&illust_id=",
+            "www.pixiv.net/artworks/",
+        )
+        .replace("http://", "https://")
+    )
+
+
+def parse_source(resp_text: str, host: str) -> Optional[str]:
+    if host in ["danbooru.donmai.us", "gelbooru.com"]:
+        return PyQuery(resp_text)(".image-container").attr("data-normalized-source")
+
+    elif host in ["yande.re", "konachan.com"]:
+        source = PyQuery(resp_text)("#post_source").attr("value")
+        return source or PyQuery(resp_text)('a[href^="/pool/show/"]').text()
+
+    return ""
+
+
 async def get_source(url: str) -> str:
-    source = url
-    if host := URL(source).host:
-        headers = None if host == "danbooru.donmai.us" else DEFAULT_HEADERS
-        async with AsyncClient(
-            headers=headers, proxies=config.proxy, follow_redirects=True
-        ) as session:
-            resp = await session.get(source)
-            if resp.status_code >= 400:
-                return ""
-
-            if host in ["danbooru.donmai.us", "gelbooru.com"]:
-                source = PyQuery(resp.text)(".image-container").attr(
-                    "data-normalized-source"
-                )
+    if not url:
+        return ""
 
-            elif host in ["yande.re", "konachan.com"]:
-                source = PyQuery(resp.text)("#post_source").attr("value")
-                if not source:
-                    source = PyQuery(resp.text)('a[href^="/pool/show/"]').text()
+    _url = get_valid_url(url)
+    if not _url:
+        return ""
+
+    host = _url.host
+    headers = None if host == "danbooru.donmai.us" else DEFAULT_HEADERS
+    async with AsyncClient(
+        headers=headers, proxies=config.proxy, follow_redirects=True
+    ) as session:
+        resp = await session.get(url)
+        if resp.status_code >= 400:
+            return ""
+
+        source = parse_source(resp.text, host)
+        if source and get_valid_url(source):
+            return handle_source(source)
 
     return source or ""
 
 
 def confuse_url(url: str) -> str:
     return next(
         (
@@ -117,18 +139,19 @@
     if pid_match := pid_search.search(url):
         return confuse_url(f"https://pixiv.net/i/{pid_match[1]}")
 
     uid_search = re.compile(r"pixiv.+(?:member\.php\?id=|users/)(\d+)")
     if uid_match := uid_search.search(url):
         return confuse_url(f"https://pixiv.net/u/{uid_match[1]}")
 
-    if URL(url).host == "danbooru.donmai.us":
+    host = URL(url).host
+    if host == "danbooru.donmai.us":
         return confuse_url(url.replace("/post/show/", "/posts/"))
 
-    if URL(url).host in [
+    elif host in [
         "e-hentai.org",
         "exhentai.org",
         "graph.baidu.com",
         "nhentai.net",
         "www.google.com",
         "yandex.com",
     ]:
@@ -211,7 +234,17 @@
     ]
     raw_with_ratio.sort(key=lambda x: x[1], reverse=True)
 
     if filtered := [i[0] for i in raw_with_ratio if i[1] > 0.65]:
         return filtered
 
     return [i[0] for i in raw_with_ratio]
+
+
+def get_valid_url(url: str) -> Optional[URL]:
+    try:
+        url = URL(url)
+        if url.host:
+            return url
+    except InvalidURL:
+        return None
+    return None
```

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/whatanime.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/whatanime.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/YetAnotherPicSearch/yandex.py` & `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/yandex.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.2/pyproject.toml` & `yetanotherpicsearch-1.9.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "YetAnotherPicSearch"
-version = "1.9.2"
+version = "1.9.3"
 description = "Yet Another Picture Search Nonebot Plugin"
 authors = ["NekoAria"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "YetAnotherPicSearch" },
 ]
 homepage = "https://github.com/NekoAria/YetAnotherPicSearch"
 repository = "https://github.com/NekoAria/YetAnotherPicSearch"
 keywords = ["nonebot", "ascii2d", "baidu", "e-hentai", "google", "iqdb", "saucenao", "tracemoe", "yandex", "anime", "danbooru", "doujin", "pixiv"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 arrow = "^1.2.3"
-cachetools = "^5.3.0"
+cachetools = "^5.3.1"
 httpx = "^0.24.1"
 lxml = "^4.9.2"
 nonebot-adapter-onebot = "^2.2.3"
-nonebot2 = "^2.0.0-rc.4"
+nonebot2 = "^2.0.0"
 PicImageSearch = "^3.9.2"
-pydantic = "^1.10.7"
+pydantic = "^1.10.8"
 pyquery = "^2.0.0"
-python-socks = {extras = ["asyncio"], version = "^2.2.0", optional = true}
+python-socks = {extras = ["asyncio"], version = "^2.3.0", optional = true}
 socksio = { version = "^1.0.0", optional = true }
 shelved-cache = "^0.3.1"
 tenacity = "^8.2.2"
 
 [tool.poetry.extras]
 socks = ["python-socks", "socksio"]
```

### Comparing `yetanotherpicsearch-1.9.2/PKG-INFO` & `yetanotherpicsearch-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetanotherpicsearch
-Version: 1.9.2
+Version: 1.9.3
 Summary: Yet Another Picture Search Nonebot Plugin
 Home-page: https://github.com/NekoAria/YetAnotherPicSearch
 License: GPL-3.0-only
 Keywords: nonebot,ascii2d,baidu,e-hentai,google,iqdb,saucenao,tracemoe,yandex,anime,danbooru,doujin,pixiv
 Author: NekoAria
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,22 +12,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: socks
 Requires-Dist: PicImageSearch (>=3.9.2,<4.0.0)
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
-Requires-Dist: cachetools (>=5.3.0,<6.0.0)
+Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
-Requires-Dist: nonebot2 (>=2.0.0-rc.4,<3.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pyquery (>=2.0.0,<3.0.0)
-Requires-Dist: python-socks[asyncio] (>=2.2.0,<3.0.0) ; extra == "socks"
+Requires-Dist: python-socks[asyncio] (>=2.3.0,<3.0.0) ; extra == "socks"
 Requires-Dist: shelved-cache (>=0.3.1,<0.4.0)
 Requires-Dist: socksio (>=1.0.0,<2.0.0) ; extra == "socks"
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Project-URL: Repository, https://github.com/NekoAria/YetAnotherPicSearch
 Description-Content-Type: text/markdown
 
 <div align="center">
```

