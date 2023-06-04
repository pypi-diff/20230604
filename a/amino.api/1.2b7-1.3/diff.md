# Comparing `tmp/amino.api-1.2b7.tar.gz` & `tmp/amino.api-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.api-1.2b7.tar", last modified: Tue May  2 19:00:37 2023, max compression
+gzip compressed data, was "amino.api-1.3.tar", last modified: Sun Jun  4 14:31:25 2023, max compression
```

## Comparing `amino.api-1.2b7.tar` & `amino.api-1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 19:00:37.454611 amino.api-1.2b7/
--rw-rw-rw-   0        0        0      773 2023-05-02 19:00:37.454611 amino.api-1.2b7/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.2b7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 19:00:37.397599 amino.api-1.2b7/amino/
--rw-rw-rw-   0        0        0      922 2023-05-01 20:02:04.000000 amino.api-1.2b7/amino/__init__.py
--rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b7/amino/async_client.py
--rw-rw-rw-   0        0        0       56 2023-04-21 21:48:51.000000 amino.api-1.2b7/amino/async_full_client.py
--rw-rw-rw-   0        0        0       59 2023-04-21 21:48:51.000000 amino.api-1.2b7/amino/async_local_client.py
--rw-rw-rw-   0        0        0       50 2023-04-21 21:48:51.000000 amino.api-1.2b7/amino/async_socket.py
--rw-rw-rw-   0        0        0    35999 2023-05-01 19:49:27.000000 amino.api-1.2b7/amino/client.py
--rw-rw-rw-   0        0        0    18667 2023-04-30 11:43:28.000000 amino.api-1.2b7/amino/full_client.py
--rw-rw-rw-   0        0        0    41536 2023-05-02 17:40:15.000000 amino.api-1.2b7/amino/local_client.py
--rw-rw-rw-   0        0        0    11535 2023-04-21 23:43:16.000000 amino.api-1.2b7/amino/socket.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:00:37.453625 amino.api-1.2b7/amino/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 21:48:51.000000 amino.api-1.2b7/amino/utils/__init__.py
--rw-rw-rw-   0        0        0     1099 2023-04-28 13:22:02.000000 amino.api-1.2b7/amino/utils/exceptions.py
--rw-rw-rw-   0        0        0     7429 2023-04-22 10:56:39.000000 amino.api-1.2b7/amino/utils/helpers.py
--rw-rw-rw-   0        0        0    14913 2023-05-02 17:39:22.000000 amino.api-1.2b7/amino/utils/objects.py
--rw-rw-rw-   0        0        0     2270 2023-04-22 10:51:46.000000 amino.api-1.2b7/amino/utils/requester.py
--rw-rw-rw-   0        0        0     3660 2023-04-26 13:04:41.000000 amino.api-1.2b7/amino/utils/snippetTools.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:00:37.431614 amino.api-1.2b7/amino.api.egg-info/
--rw-rw-rw-   0        0        0      773 2023-05-02 19:00:35.000000 amino.api-1.2b7/amino.api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2023-05-02 19:00:35.000000 amino.api-1.2b7/amino.api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 19:00:35.000000 amino.api-1.2b7/amino.api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-02 19:00:35.000000 amino.api-1.2b7/amino.api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 19:00:35.000000 amino.api-1.2b7/amino.api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 19:00:37.456626 amino.api-1.2b7/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-05-02 19:00:07.000000 amino.api-1.2b7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:31:25.019760 amino.api-1.3/
+-rw-rw-rw-   0        0        0      771 2023-06-04 14:31:25.019760 amino.api-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 14:31:24.958746 amino.api-1.3/amino/
+-rw-rw-rw-   0        0        0      920 2023-06-04 14:27:02.000000 amino.api-1.3/amino/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-05-28 18:51:42.000000 amino.api-1.3/amino/async_client.py
+-rw-rw-rw-   0        0        0       56 2023-05-28 18:51:42.000000 amino.api-1.3/amino/async_full_client.py
+-rw-rw-rw-   0        0        0       59 2023-05-28 18:51:42.000000 amino.api-1.3/amino/async_local_client.py
+-rw-rw-rw-   0        0        0       50 2023-05-28 18:51:42.000000 amino.api-1.3/amino/async_socket.py
+-rw-rw-rw-   0        0        0    35999 2023-05-29 20:44:24.000000 amino.api-1.3/amino/client.py
+-rw-rw-rw-   0        0        0    18958 2023-06-04 13:45:10.000000 amino.api-1.3/amino/full_client.py
+-rw-rw-rw-   0        0        0    67936 2023-05-28 18:51:42.000000 amino.api-1.3/amino/local_client.py
+-rw-rw-rw-   0        0        0    11538 2023-05-28 18:51:42.000000 amino.api-1.3/amino/socket.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:31:25.017747 amino.api-1.3/amino/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/exceptions.py
+-rw-rw-rw-   0        0        0     7429 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/helpers.py
+-rw-rw-rw-   0        0        0    14913 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/objects.py
+-rw-rw-rw-   0        0        0     2270 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/requester.py
+-rw-rw-rw-   0        0        0     3660 2023-05-28 18:51:42.000000 amino.api-1.3/amino/utils/snippetTools.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:31:24.989753 amino.api-1.3/amino.api.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-06-04 14:31:23.000000 amino.api-1.3/amino.api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-06-04 14:31:23.000000 amino.api-1.3/amino.api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:31:23.000000 amino.api-1.3/amino.api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-04 14:31:23.000000 amino.api-1.3/amino.api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-04 14:31:23.000000 amino.api-1.3/amino.api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 14:31:25.021754 amino.api-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2023-06-04 14:27:43.000000 amino.api-1.3/setup.py
```

### Comparing `amino.api-1.2b7/PKG-INFO` & `amino.api-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.2b7
+Version: 1.3
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.2b7/amino/__init__.py` & `amino.api-1.3/amino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from json import loads
 from requests import get
 
 __title__ = 'amino.api'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Xsarz'
-__version__ = '1.2b7'
+__version__ = '1.3'
 __newest__ = loads(get("https://pypi.org/pypi/amino.api/json").text)["info"]["version"]
 
 
 
 if __version__ != __newest__:
 	s('cls || clear')
 	print(f'\033[38;5;214m{__title__} made by {__author__}\nPlease update the library. Your version: {__version__}  A new version:{__newest__}\033[0m')
```

### Comparing `amino.api-1.2b7/amino/client.py` & `amino.api-1.3/amino/client.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b7/amino/full_client.py` & `amino.api-1.3/amino/full_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,8 +506,14 @@
 
 	def get_hall_of_fame(self, size: int = 25):
 		response = self.req.make_request(method="GET", endpoint=f"/g/s/topic/0/feed/community?size={size}&categoryKey=customized&type=discover&pagingType=t&moduleId=23ce695c-c4da-4da5-a6c4-7777ba23b7aa")
 		return response.json()
 	
 	def get_recommended_communities(self, size: int = 25):
 		response = self.req.make_request(method="GET", endpoint=f"/g/s/topic/0/feed/community?size={size}&categoryKey=recommendation&type=discover&pagingType=t")
-		return response.json()
+		return objects.communityList(response.json())
+
+
+	def get_user_info(self, userId: str, comId: str = None):
+
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/user-profile/{userId}" if comId else f"/g/s/user-profile/{userId}")
+		return objects.UserProfile(response.json()["userProfile"])
```

### Comparing `amino.api-1.2b7/amino/local_client.py` & `amino.api-1.3/amino/local_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1136,8 +1136,636 @@
 			url = f"/x{self.comId}/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}"
 		elif fileId:
 			url = f"/x{self.comId}/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}"
 		else:
 			raise exceptions.IncorrectType()
 
 		response = self.req.make_request(method="GET", endpoint=url)
-		return response.json()["commentList"]
+		return response.json()["commentList"]
+
+
+
+
+	def get_blog_categories(self, size: int = 25):
+
+
+		response = self.req.make_request(method="GET", endpoint=f"/x{self.comId}/s/blog-category?size={size}")
+		return response.json()["blogCategoryList"]
+
+	def get_blogs_by_category(self, categoryId: str,start: int = 0, size: int = 25):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/blog-category/{categoryId}/blog-list?start={start}&size={size}")
+		return response.json()["blogList"]
+
+
+	def get_quiz_rankings(self, quizId: str, start: int = 0, size: int = 25):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/blog/{quizId}/quiz/result?start={start}&size={size}")
+		return response.json()
+
+
+	def get_wall_comments(self, userId: str, sorting: str, start: int = 0, size: int = 25):
+
+		if sorting not in ["newest", "vote", "oldest"]: raise exceptions.IncorrectType(sorting)
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/user-profile/{userId}/comment?sort={sorting}&start={start}&size={size}")
+		return response.json()["commentList"]
+
+
+	def get_recent_blogs(self, pageToken: str = None, start: int = 0, size: int = 25):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/feed/blog-all?pagingType=t&{f'pageToken={pageToken}' if pageToken else f'start={start}'}&size={size}")
+		return response.json()
+
+
+	def get_chat_users(self, chatId: str, start: int = 0, size: int = 25):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2")
+		return objects.userProfileList(response.json()["memberList"])
+
+
+
+	def get_notifications(self, start: int = 0, size: int = 25):
+
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/notification?pagingType=t&start={start}&size={size}")
+		return response.json()["notificationList"]
+
+
+	def get_notices(self, start: int = 0, size: int = 25):
+
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/notice?type=usersV2&status=1&start={start}&size={size}")
+		return response.json()["noticeList"]
+
+
+	def get_sticker_pack_info(self, sticker_pack_id: str):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/sticker-collection/{sticker_pack_id}?includeStickers=true")
+		return response.json()["stickerCollection"]
+
+
+	def get_sticker_packs(self):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/sticker-collection?includeStickers=false&type=my-active-collection")
+		return response.json()["stickerCollection"]
+
+
+
+	def get_store_chat_bubbles(self, start: int = 0, size: int = 25):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/store/items?sectionGroupId=chat-bubble&start={start}&size={size}")
+		return response.json()
+
+
+
+	def get_store_stickers(self, start: int = 0, size: int = 25):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/store/items?sectionGroupId=sticker&start={start}&size={size}")
+		return response.json()
+
+
+
+	def get_community_stickers(self):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/sticker-collection?type=community-shared")
+		return response.json()
+
+
+	def get_sticker_collection(self, collectionId: str):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/sticker-collection/{collectionId}?includeStickers=true")
+		return response.json()["stickerCollection"]
+
+
+	def get_shared_folder_info(self):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/shared-folder/stats")
+		return response.json()["stats"]
+
+
+	def get_shared_folder_files(self, type: str = "latest", start: int = 0, size: int = 25):
+
+		response = self.req.make_request(method=f"GET", endpoint=f"/x{self.comId}/s/shared-folder/files?type={type}&start={start}&size={size}")
+		return response.json()["fileList"]
+
+
+
+
+	def moderation_history(self, userId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, size: int = 25):
+		if userId: url = f"/x{self.comId}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}"
+		elif blogId: url = f"/x{self.comId}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}"
+		elif quizId: url = f"/x{self.comId}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}"
+		elif wikiId: url = f"/x{self.comId}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}"
+		elif fileId: url = f"/x{self.comId}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}"
+		else: url = f"/x{self.comId}/s/admin/operation?pagingType=t&size={size}"
+
+		response = self.req.make_request(method=f"GET", endpoint=url)
+		return response.json()["adminLogList"]
+
+
+
+	def feature(self, time: int, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
+		if chatId:
+			if time == 1: time = 3600
+			if time == 1: time = 7200
+			if time == 1: time = 10800
+
+		else:
+			if time == 1: time = 86400
+			elif time == 2: time = 172800
+			elif time == 3: time = 259200
+			else: raise exceptions.WrongType(time)
+
+		data = {
+			"adminOpName": 114,
+			"adminOpValue": {
+				"featuredDuration": time
+			},
+			"timestamp": int(timestamp() * 1000)
+		}
+
+		if userId:
+			data["adminOpValue"] = {"featuredType": 4}
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif blogId:
+			data["adminOpValue"] = {"featuredType": 1}
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif wikiId:
+			data["adminOpValue"] = {"featuredType": 1}
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif chatId:
+			data["adminOpValue"] = {"featuredType": 5}
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		else: raise exceptions.SpecifyType()
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return json.loads(response.text)
+
+	def unfeature(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
+		data = {
+			"adminOpName": 114,
+			"adminOpValue": {},
+			"timestamp": int(timestamp() * 1000)
+		}
+
+		if userId:
+			data["adminOpValue"] = {"featuredType": 0}
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif blogId:
+			data["adminOpValue"] = {"featuredType": 0}
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif wikiId:
+			data["adminOpValue"] = {"featuredType": 0}
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif chatId:
+			data["adminOpValue"] = {"featuredType": 0}
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		else: raise exceptions.SpecifyType()
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return json.loads(response.text)
+
+	def hide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
+		data = {
+			"adminOpNote": {
+				"content": reason
+			},
+			"timestamp": int(timestamp() * 1000)
+		}
+
+		if userId:
+			data["adminOpName"] = 18
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif blogId:
+			data["adminOpName"] = 110
+			data["adminOpValue"] = 9
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif quizId:
+			data["adminOpName"] = 110
+			data["adminOpValue"] = 9
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif wikiId:
+			data["adminOpName"] = 110
+			data["adminOpValue"] = 9
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif chatId:
+			data["adminOpName"] = 110
+			data["adminOpValue"] = 9
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif fileId:
+			data["adminOpName"] = 110
+			data["adminOpValue"] = 9
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		else: raise exceptions.SpecifyType()
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return json.loads(response.text)
+
+	def unhide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
+		data = {
+			"adminOpNote": {
+				"content": reason
+			},
+			"timestamp": int(timestamp() * 1000)
+		}
+
+		if userId:
+			data["adminOpName"] = 19
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif blogId:
+			data["adminOpName"] = 110
+			data["adminOpValue"] = 0
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif quizId:
+			data["adminOpName"] = 110
+			data["adminOpValue"] = 0
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{quizId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif wikiId:
+			data["adminOpName"] = 110
+			data["adminOpValue"] = 0
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/item/{wikiId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif chatId:
+			data["adminOpName"] = 110
+			data["adminOpValue"] = 0
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		elif fileId:
+			data["adminOpName"] = 110
+			data["adminOpValue"] = 0
+			data = json.dumps(data)
+			response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/files/{fileId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+
+		else: raise exceptions.SpecifyType()
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return json.loads(response.text)
+
+	def edit_titles(self, userId: str, titles: list, colors: list):
+		tlt = []
+		for titles, colors in zip(titles, colors):
+			tlt.append({"title": titles, "color": colors})
+
+		data = json.dumps({
+			"adminOpName": 207,
+			"adminOpValue": {
+				"titles": tlt
+			},
+			"timestamp": int(timestamp() * 1000)
+		})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/admin", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return json.loads(response.text)
+
+	# TODO : List all warning texts
+	def warn(self, userId: str, reason: str = None):
+		data = json.dumps({
+			"uid": userId,
+			"title": "Custom",
+			"content": reason,
+			"attachedObject": {
+				"objectId": userId,
+				"objectType": 0
+			},
+			"penaltyType": 0,
+			"adminOpNote": {},
+			"noticeType": 7,
+			"timestamp": int(timestamp() * 1000)
+		})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/notice", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return json.loads(response.text)
+
+	# TODO : List all strike texts
+	def strike(self, userId: str, time: int, title: str = None, reason: str = None):
+		if time == 1: time = 86400
+		elif time == 2: time = 10800
+		elif time == 3: time = 21600
+		elif time == 4: time = 43200
+		elif time == 5: time = 86400
+		else: raise exceptions.WrongType(time)
+
+		data = json.dumps({
+			"uid": userId,
+			"title": title,
+			"content": reason,
+			"attachedObject": {
+				"objectId": userId,
+				"objectType": 0
+			},
+			"penaltyType": 1,
+			"penaltyValue": time,
+			"adminOpNote": {},
+			"noticeType": 4,
+			"timestamp": int(timestamp() * 1000)
+		})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/notice", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return json.loads(response.text)
+
+	def ban(self, userId: str, reason: str, banType: int = None):
+		data = json.dumps({
+			"reasonType": banType,
+			"note": {
+				"content": reason
+			},
+			"timestamp": int(timestamp() * 1000)
+		})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/ban", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return json.loads(response.text)
+
+	def unban(self, userId: str, reason: str):
+		data = json.dumps({
+			"note": {
+				"content": reason
+			},
+			"timestamp": int(timestamp() * 1000)
+		})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/{userId}/unban", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return json.loads(response.text)
+
+	def reorder_featured_users(self, userIds: list):
+		data = json.dumps({
+			"uidList": userIds,
+			"timestamp": int(timestamp() * 1000)
+		})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/user-profile/featured/reorder", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return json.loads(response.text)
+
+	def get_hidden_blogs(self, start: int = 0, size: int = 25):
+		response = self.session.get(f"{self.api}/x{self.comId}/s/feed/blog-disabled?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
+
+	def get_featured_users(self, start: int = 0, size: int = 25):
+		response = self.session.get(f"{self.api}/x{self.comId}/s/user-profile?type=featured&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return objects.UserProfileCountList(json.loads(response.text)).UserProfileCountList
+
+	def review_quiz_questions(self, quizId: str):
+		response = self.session.get(f"{self.api}/x{self.comId}/s/blog/{quizId}?action=review", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return objects.QuizQuestionList(json.loads(response.text)["blog"]["quizQuestionList"]).QuizQuestionList
+
+	def get_recent_quiz(self, start: int = 0, size: int = 25):
+		response = self.session.get(f"{self.api}/x{self.comId}/s/blog?type=quizzes-recent&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
+
+	def get_trending_quiz(self, start: int = 0, size: int = 25):
+		response = self.session.get(f"{self.api}/x{self.comId}/s/feed/quiz-trending?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
+
+	def get_best_quiz(self, start: int = 0, size: int = 25):
+		response = self.session.get(f"{self.api}/x{self.comId}/s/feed/quiz-best-quizzes?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return objects.BlogList(json.loads(response.text)["blogList"]).BlogList
+
+	def send_action(self, actions: list, blogId: str = None, quizId: str = None, lastAction: bool = False):
+		# Action List
+		# Browsing
+
+		if lastAction is True: t = 306
+		else: t = 304
+
+		data = {
+			"o": {
+				"actions": actions,
+				"target": f"ndc://x{self.comId}/",
+				"ndcId": int(self.comId),
+				"params": {"topicIds": [45841, 17254, 26542, 42031, 22542, 16371, 6059, 41542, 15852]},
+				"id": "831046"
+			},
+			"t": t
+		}
+
+		if blogId is not None or quizId is not None:
+			data["target"] = f"ndc://x{self.comId}/blog/{blogId}"
+			if blogId is not None: data["params"]["blogType"] = 0
+			if quizId is not None: data["params"]["blogType"] = 6
+
+		return self.send(json.dumps(data))
+
+	# Provided by "spectrum#4691"
+	def purchase(self, objectId: str, objectType: int, aminoPlus: bool = True, autoRenew: bool = False):
+		data = {'objectId': objectId,
+				'objectType': objectType,
+				'v': 1,
+				"timestamp": int(timestamp() * 1000)}
+
+		if aminoPlus: data['paymentContext'] = {'discountStatus': 1, 'discountValue': 1, 'isAutoRenew': autoRenew}
+		else: data['paymentContext'] = {'discountStatus': 0, 'discountValue': 1, 'isAutoRenew': autoRenew}
+
+		data = json.dumps(data)
+		response = self.session.post(f"{self.api}/x{self.comId}/s/store/purchase", headers=self.parse_headers(data=data), data=data)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return response.status_code
+
+	# Provided by "spectrum#4691"
+	def apply_avatar_frame(self, avatarId: str, applyToAll: bool = True):
+		"""
+		Apply avatar frame.
+
+		**Parameters**
+			- **avatarId** : ID of the avatar frame.
+			- **applyToAll** : Apply to all.
+
+		**Returns**
+			- **Success** : 200 (int)
+
+			- **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+
+		"""
+
+		data = {"frameId": avatarId,
+				"applyToAll": 0,
+				"timestamp": int(timestamp() * 1000)}
+
+		if applyToAll: data["applyToAll"] = 1
+
+		data = json.dumps(data)
+		response = self.session.post(f"{self.api}/x{self.comId}/s/avatar-frame/apply", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return response.status_code
+
+	def invite_to_vc(self, chatId: str, userId: str):
+		"""
+		Invite a User to a Voice Chat
+
+		**Parameters**
+			- **chatId** - ID of the Chat
+			- **userId** - ID of the User
+
+		**Returns**
+			- **Success** : 200 (int)
+
+			- **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+		"""
+
+		data = json.dumps({
+			"uid": userId
+		})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/{chatId}/vvchat-presenter/invite/", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return response.status_code
+
+	def add_poll_option(self, blogId: str, question: str):
+		data = json.dumps({
+			"mediaList": None,
+			"title": question,
+			"type": 0,
+			"timestamp": int(timestamp() * 1000)
+		})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/blog/{blogId}/poll/option", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return response.status_code
+
+	def create_wiki_category(self, title: str, parentCategoryId: str, content: str = None):
+		data = json.dumps({
+			"content": content,
+			"icon": None,
+			"label": title,
+			"mediaList": None,
+			"parentCategoryId": parentCategoryId,
+			"timestamp": int(timestamp() * 1000)
+		})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/item-category", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return response.status_code
+
+	def create_shared_folder(self,title: str):
+		data = json.dumps({
+				"title":title,
+				"timestamp":int(timestamp() * 1000)
+			})
+		response = self.session.post(f"{self.api}/x{self.comId}/s/shared-folder/folders", headers=self.parse_headers(data=data),data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return response.status_code
+
+	def submit_to_wiki(self, wikiId: str, message: str):
+		data = json.dumps({
+			"message": message,
+			"itemId": wikiId,
+			"timestamp": int(timestamp() * 1000)
+		})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return response.status_code
+
+	def accept_wiki_request(self, requestId: str, destinationCategoryIdList: list):
+		data = json.dumps({
+			"destinationCategoryIdList": destinationCategoryIdList,
+			"actionType": "create",
+			"timestamp": int(timestamp() * 1000)
+		})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request/{requestId}/approve", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return response.status_code
+
+	def reject_wiki_request(self, requestId: str):
+		data = json.dumps({})
+
+		response = self.session.post(f"{self.api}/x{self.comId}/s/knowledge-base-request/{requestId}/reject", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return response.status_code
+
+	def get_wiki_submissions(self, start: int = 0, size: int = 25):
+		response = self.session.get(f"{self.api}/x{self.comId}/s/knowledge-base-request?type=all&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return objects.WikiRequestList(json.loads(response.text)["knowledgeBaseRequestList"]).WikiRequestList
+
+	def get_live_layer(self):
+		response = self.session.get(f"{self.api}/x{self.comId}/s/live-layer/homepage?v=2", headers=self.parse_headers(), proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return objects.LiveLayer(json.loads(response.text)["liveLayerList"]).LiveLayer
+
+	def apply_bubble(self, bubbleId: str, chatId: str, applyToAll: bool = False):
+		data = {
+			"applyToAll": 0,
+			"bubbleId": bubbleId,
+			"threadId": chatId,
+			"timestamp": int(timestamp() * 1000)
+		}
+
+		if applyToAll is True:
+			data["applyToAll"] = 1
+
+		data = json.dumps(data)
+		response = self.session.post(f"{self.api}/x{self.comId}/s/chat/thread/apply-bubble", headers=self.parse_headers(data=data), data=data, proxies=self.proxies, verify=self.certificatePath)
+		if response.status_code != 200: 
+			return exceptions.CheckException(response.text)
+		else: return response.status_code
```

### Comparing `amino.api-1.2b7/amino/socket.py` & `amino.api-1.3/amino/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from traceback import format_exc
 
 from .utils import objects
 from .utils.exceptions import SocketNotStarted
 
 class SocketHandler:
 	def __init__(self, req, sock_trace: bool = False, debug: bool = False):
-		self.socket_url = "wss://ws1.narvii.com"
+		self.socket_url = "wss://ws1.aminoapps.com"
 		self.debug = debug
 		self.socket = None
 		self.reconnectTime = 60
 		self.active = False
 		self.socket_thread = None
 		self.req = req
 		if self.socket_enabled:
```

### Comparing `amino.api-1.2b7/amino/utils/exceptions.py` & `amino.api-1.3/amino/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b7/amino/utils/helpers.py` & `amino.api-1.3/amino/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b7/amino/utils/objects.py` & `amino.api-1.3/amino/utils/objects.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b7/amino/utils/requester.py` & `amino.api-1.3/amino/utils/requester.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b7/amino/utils/snippetTools.py` & `amino.api-1.3/amino/utils/snippetTools.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b7/amino.api.egg-info/PKG-INFO` & `amino.api-1.3/amino.api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.2b7
+Version: 1.3
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino.API</h1>
```

### Comparing `amino.api-1.2b7/amino.api.egg-info/SOURCES.txt` & `amino.api-1.3/amino.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b7/setup.py` & `amino.api-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 info = {
 	"name": "amino.api",
-	"version": "1.2b7",
+	"version": "1.3",
 	"github_page": "https://github.com/xXxCLOTIxXx/amino.api",
 	"download_link": "https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip",
 	"license": "MIT",
 	"author": "Xsarz",
 	"author_email": "xsarzy@gmail.com",
 	"description": "Library for creating amino bots and scripts.",
 	"long_description": None,
```

