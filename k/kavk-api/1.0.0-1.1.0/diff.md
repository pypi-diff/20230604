# Comparing `tmp/kavk_api-1.0.0.tar.gz` & `tmp/kavk_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kavk_api-1.0.0.tar", max compression
+gzip compressed data, was "kavk_api-1.1.0.tar", max compression
```

## Comparing `kavk_api-1.0.0.tar` & `kavk_api-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-04-24 13:58:38.368151 kavk_api-1.0.0/LICENSE
--rw-r--r--   0        0        0     1082 2023-04-25 14:16:24.259940 kavk_api-1.0.0/README.rst
--rw-r--r--   0        0        0       51 2023-05-28 16:59:15.216341 kavk_api-1.0.0/kavk_api/__init__.py
--rw-r--r--   0        0        0     1396 2023-05-28 16:59:15.216341 kavk_api-1.0.0/kavk_api/api/base.py
--rw-r--r--   0        0        0   261638 2023-05-28 16:59:15.216341 kavk_api-1.0.0/kavk_api/api/methods.py
--rw-r--r--   0        0        0   133943 2023-05-28 16:59:15.217341 kavk_api-1.0.0/kavk_api/api/objects.py
--rw-r--r--   0        0        0    38178 2023-05-28 16:59:15.217341 kavk_api-1.0.0/kavk_api/api/responses.py
--rw-r--r--   0        0        0     9203 2023-05-28 16:59:15.217341 kavk_api-1.0.0/kavk_api/events/bot_events.py
--rw-r--r--   0        0        0     7453 2023-05-28 16:59:15.217341 kavk_api-1.0.0/kavk_api/events/enums.py
--rw-r--r--   0        0        0     4998 2023-05-28 16:59:15.217341 kavk_api-1.0.0/kavk_api/events/event_objects.py
--rw-r--r--   0        0        0     9872 2023-05-28 16:59:15.217341 kavk_api-1.0.0/kavk_api/events/user_events.py
--rw-r--r--   0        0        0      360 2023-05-28 16:59:15.217341 kavk_api-1.0.0/kavk_api/exceptions.py
--rw-r--r--   0        0        0     3875 2023-05-28 16:59:15.217341 kavk_api-1.0.0/kavk_api/kavk_api.py
--rw-r--r--   0        0        0      175 2023-05-28 16:47:07.471481 kavk_api-1.0.0/kavk_api/longpoll/__init__.py
--rw-r--r--   0        0        0     3187 2023-05-28 16:59:15.217341 kavk_api-1.0.0/kavk_api/longpoll/bot.py
--rw-r--r--   0        0        0     2800 2023-05-28 16:59:15.218341 kavk_api-1.0.0/kavk_api/longpoll/user.py
--rw-r--r--   0        0        0       27 2023-05-28 16:59:15.218341 kavk_api-1.0.0/kavk_api/upload/__init__.py
--rw-r--r--   0        0        0      153 2023-05-28 16:59:15.218341 kavk_api-1.0.0/kavk_api/upload/responses.py
--rw-r--r--   0        0        0     8009 2023-05-28 16:59:15.218341 kavk_api-1.0.0/kavk_api/upload/upload.py
--rw-r--r--   0        0        0      123 2023-05-28 16:49:03.045855 kavk_api-1.0.0/kavk_api/utils.py
--rw-r--r--   0        0        0      421 2023-05-28 16:59:15.218341 kavk_api-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 kavk_api-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-24 13:58:38.368151 kavk_api-1.1.0/LICENSE
+-rw-r--r--   0        0        0      746 2023-06-04 11:07:23.757250 kavk_api-1.1.0/README.md
+-rw-r--r--   0        0        0       51 2023-05-28 16:59:15.216341 kavk_api-1.1.0/kavk_api/__init__.py
+-rw-r--r--   0        0        0     1396 2023-05-29 08:21:39.810966 kavk_api-1.1.0/kavk_api/api/base.py
+-rw-r--r--   0        0        0   261638 2023-05-29 08:21:39.811965 kavk_api-1.1.0/kavk_api/api/methods.py
+-rw-r--r--   0        0        0   133943 2023-05-29 08:21:39.812965 kavk_api-1.1.0/kavk_api/api/objects.py
+-rw-r--r--   0        0        0    38178 2023-05-29 08:21:39.812965 kavk_api-1.1.0/kavk_api/api/responses.py
+-rw-r--r--   0        0        0     6477 2023-06-04 11:08:56.689008 kavk_api-1.1.0/kavk_api/events/bot_events.py
+-rw-r--r--   0        0        0     7453 2023-05-29 08:21:39.813965 kavk_api-1.1.0/kavk_api/events/enums.py
+-rw-r--r--   0        0        0     4998 2023-05-29 08:21:39.813965 kavk_api-1.1.0/kavk_api/events/event_objects.py
+-rw-r--r--   0        0        0    10205 2023-06-04 11:08:56.690008 kavk_api-1.1.0/kavk_api/events/user_events.py
+-rw-r--r--   0        0        0      360 2023-05-29 08:21:39.813965 kavk_api-1.1.0/kavk_api/exceptions.py
+-rw-r--r--   0        0        0     3875 2023-05-29 08:21:39.813965 kavk_api-1.1.0/kavk_api/kavk_api.py
+-rw-r--r--   0        0        0      189 2023-06-04 11:08:56.690008 kavk_api-1.1.0/kavk_api/longpoll/__init__.py
+-rw-r--r--   0        0        0     3175 2023-06-04 11:08:56.690008 kavk_api-1.1.0/kavk_api/longpoll/bot.py
+-rw-r--r--   0        0        0     3017 2023-06-04 11:08:56.691007 kavk_api-1.1.0/kavk_api/longpoll/user.py
+-rw-r--r--   0        0        0       27 2023-05-28 16:59:15.218341 kavk_api-1.1.0/kavk_api/upload/__init__.py
+-rw-r--r--   0        0        0      153 2023-05-29 08:21:39.814965 kavk_api-1.1.0/kavk_api/upload/responses.py
+-rw-r--r--   0        0        0     8009 2023-05-29 08:21:39.814965 kavk_api-1.1.0/kavk_api/upload/upload.py
+-rw-r--r--   0        0        0      123 2023-05-29 08:21:39.814965 kavk_api-1.1.0/kavk_api/utils.py
+-rw-r--r--   0        0        0      420 2023-06-04 11:08:31.805017 kavk_api-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 kavk_api-1.1.0/PKG-INFO
```

### Comparing `kavk_api-1.0.0/LICENSE` & `kavk_api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kavk_api-1.0.0/kavk_api/api/base.py` & `kavk_api-1.1.0/kavk_api/api/base.py`

 * *Files identical despite different names*

### Comparing `kavk_api-1.0.0/kavk_api/api/methods.py` & `kavk_api-1.1.0/kavk_api/api/methods.py`

 * *Files identical despite different names*

### Comparing `kavk_api-1.0.0/kavk_api/api/objects.py` & `kavk_api-1.1.0/kavk_api/api/objects.py`

 * *Files identical despite different names*

### Comparing `kavk_api-1.0.0/kavk_api/api/responses.py` & `kavk_api-1.1.0/kavk_api/api/responses.py`

 * *Files identical despite different names*

### Comparing `kavk_api-1.0.0/kavk_api/events/enums.py` & `kavk_api-1.1.0/kavk_api/events/enums.py`

 * *Files identical despite different names*

### Comparing `kavk_api-1.0.0/kavk_api/events/event_objects.py` & `kavk_api-1.1.0/kavk_api/events/event_objects.py`

 * *Files identical despite different names*

### Comparing `kavk_api-1.0.0/kavk_api/events/user_events.py` & `kavk_api-1.1.0/kavk_api/events/user_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pydantic import BaseModel
 from pydantic.fields import ModelField
 from typing import Optional, Any, Union
 from .enums import VkMessageFlag, VkEventType
 from ..api.objects import MessagesKeyboard
 
 class WrongTypeException(Exception): pass
+class WrongEventTypeException(Exception): pass
+class WrongEventHandlerTypeException(Exception): pass
 
 class Additional(BaseModel):
     title:str = '...'
     emoji:bool = False
     from_:int = 0
     has_template:bool = False
     marked_users:Optional[list[list]] = None
@@ -62,21 +64,21 @@
     raw:list = []
     type:VkEventType
 
     def __init__(self, **data) -> None:
         type = self.__class__.__dict__.get('__fields__',{}).get('type')
         try: 
             data_type = VkEventType(data.get('type'))
-        except: raise WrongTypeException('type {} not found in EventsType!'.format(data.get('type')))
+        except: raise WrongEventTypeException('type {} not found in EventsType!'.format(data.get('type')))
         if isinstance(type, ModelField):
             if not isinstance(type.default, VkEventType):
-                raise WrongTypeException('{} class doesn\'t have default type!'.format(self.__class__.__name__))
+                raise WrongEventHandlerTypeException('{} class doesn\'t have default type!'.format(self.__class__.__name__))
             elif type.default != data_type:
                 raise WrongTypeException('{} class doesn\'t support {} type'.format(self.__class__.__name__, data.get('type')))
-        else: raise WrongTypeException('{} class doesn\'t have default type!'.format(self.__class__.__name__))
+        else: raise WrongEventHandlerTypeException('{} class doesn\'t have default type!'.format(self.__class__.__name__))
         if isinstance(data.get('message', None), str):
             data.update({'message': data['message'].replace('&lt;', '<') \
             .replace('&gt;', '>') \
             .replace('&quot;', '"') \
             .replace('&amp;', '&') \
             .replace('<br>', '\n')
                          })
@@ -277,21 +279,30 @@
 
 class NotificationChange(BaseEvent):
     type = VkEventType.FRIEND_STATE_CHANGE
     peer_id:int
     sound:int
     disabled_until:int
 
-class MessageReactionNew(BaseEvent):
-    type = VkEventType.MESSAGE_REACTION_NEW
-    
+class UnknowEvent:
+    def __init__(self, raw:list):
+        self.type = None
+        self.raw = raw
+
+AnyUserEvent = Union[ReplaceMessageFlags, SetMessageFlags, ResetMessageFlags, MessageNew, MessageEdit, ReadIncomingMessages, ReadOutgoingMessages, FriendOnline, FriendOffline, ResetDialogFlags, ReplaceDialogFlags, SetDialogFlags, DeleteDialogMessages, RestoreDialogMessages, ChangeMajorId, ChangeMinorId, ChatSettingsChange, ChatInfoChanged, UserTypingInDialog, UserTypingInChat, UsersTypingInChat, UserVoiceRecording, UserUploadPhoto, UserUploadVideo, UserUploadFile, UserCall, ChangeCountOfUnreadDialogs, ChangeInvisible, FriendStateChange, NotificationChange]
 
-def _get_event(raw:list) -> Union[ReplaceMessageFlags, SetMessageFlags, ResetMessageFlags, MessageNew, MessageEdit, ReadIncomingMessages, ReadOutgoingMessages, FriendOnline, FriendOffline, ResetDialogFlags, ReplaceDialogFlags, SetDialogFlags, DeleteDialogMessages, RestoreDialogMessages, ChangeMajorId, ChangeMinorId, ChatSettingsChange, ChatInfoChanged, UserTypingInDialog, UserTypingInChat, UsersTypingInChat, UserVoiceRecording, UserUploadPhoto, UserUploadVideo, UserUploadFile, UserCall, ChangeCountOfUnreadDialogs, ChangeInvisible, FriendStateChange, NotificationChange]:
-    for e in EVENTS:
+def _get_event(raw:list) -> AnyUserEvent | UnknowEvent:
+    for e in AnyUserEvent.__args__:
         try:
             return e.from_list(raw)
-        except: pass
-
-    raise WrongTypeException('Wrong event! {}\nPlease report this event at github.com/kravandir/kavk_api/issues'.format(raw))
+        except: 
+            pass
 
+    return UnknowEvent(raw)
 
-EVENTS = [ReplaceMessageFlags, SetMessageFlags, ResetMessageFlags, MessageNew, MessageEdit, ReadIncomingMessages, ReadOutgoingMessages, FriendOnline, FriendOffline, ResetDialogFlags, ReplaceDialogFlags, SetDialogFlags, DeleteDialogMessages, RestoreDialogMessages, ChangeMajorId, ChangeMinorId, ChatSettingsChange, ChatInfoChanged, UserTypingInDialog, UserTypingInChat, UsersTypingInChat, UserVoiceRecording, UserUploadPhoto, UserUploadVideo, UserUploadFile, UserCall, ChangeCountOfUnreadDialogs, ChangeInvisible, FriendStateChange, NotificationChange]
+__all__ = (
+"WrongTypeException", "WrongEventTypeException", "WrongEventHandlerTypeException", "Additional", "Attachments", "BaseEvent", "ReplaceMessageFlags",
+"SetMessageFlags", "ResetMessageFlags", "MessageNew", "MessageEdit", "ReadIncomingMessages", "ReadOutgoingMessages", "FriendOnline", "FriendOffline",
+"ResetDialogFlags", "ReplaceDialogFlags", "SetDialogFlags", "DeleteDialogMessages", "RestoreDialogMessages", "ChangeMajorId", "ChangeMinorId",
+"ChatSettingsChange", "ChatInfoChanged", "UserTypingInDialog", "UserTypingInChat", "UsersTypingInChat", "UserVoiceRecording", "UserUploadPhoto",
+"UserUploadVideo", "UserUploadFile", "UserCall", "ChangeCountOfUnreadDialogs", "ChangeInvisible", "FriendStateChange", "NotificationChange",
+"UnknowEvent", "_get_event")
```

### Comparing `kavk_api-1.0.0/kavk_api/kavk_api.py` & `kavk_api-1.1.0/kavk_api/kavk_api.py`

 * *Files identical despite different names*

### Comparing `kavk_api-1.0.0/kavk_api/longpoll/bot.py` & `kavk_api-1.1.0/kavk_api/longpoll/bot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from ..kavk_api import Vk
-from ..events import bot_events as BotEvent
-
+from ..events import bot_events as BotEventType
+from typing import AsyncIterator
 
 class BotLongPoll:
     '''
         Класс для работы с BotLongPoll
 
         ...
-        
         vk:Vk
             Объект kavk_api.Vk
         wait:int = 25
             Время ожидания
     '''
     def __init__(self, vk:Vk, wait:int=25) -> None:
         self._vk:Vk = vk
         self._wait:int = wait
         self._server:str = ''
         self._params:dict = {}
         self._updates:list = []
 
-    async def listen(self):
+    async def listen(self) -> AsyncIterator[BotEventType.AnyBotEvent]:
         '''Генератор ивентов BotLongPoll'''
         while 1:
             async for event in BotLongPoll(self._vk, self._wait):
                 yield event
 
     async def _update_params(self) -> None:
         '''Обновление self._params и self._server'''
@@ -59,30 +58,29 @@
     # Что происходит дальше?
     # __aiter__ возвращает коду `async for e in LongPoll.listen()`
     # функцию __anext__.
     # Она же в свою очередь просто получает наш новый ивент и обрабатывает его
 
     def __aiter__(self): return self
 
-    async def __anext__(self):
+    async def __anext__(self) -> BotEventType.AnyBotEvent:
         if self._updates != []:
-            u:dict = self._updates.pop(0)
-            event = BotEvent._get_event(u.get('type',''))
-            return event(**u, raw=u)
+            update:dict = self._updates.pop(0)
+            return BotEventType._get_event(**update)
             
         updates = []
         while updates == []:
             '''
             Если событий за время self._wait не произойдёт, мы получим в ответ пустой список.
             Т.к. делать ивент из такого ответа хз как, мы просто ждем когда прийдет нормальный
             '''
             updates = await self._get_event() 
         
         if len(updates) > 0:
             self._updates = updates[1:]
             update:dict = updates[0]
-        else: update:dict = updates[0]
-        event_type = str(update.get('type', ''))
-        event = BotEvent._get_event(event_type)
-        return event(**update, raw=update)
+        else: 
+            update:dict = updates[0]
+
+        return BotEventType._get_event(**update)
 
-__all__ = ("BotLongPoll", 'BotEvent')
+__all__ = ("BotLongPoll", 'BotEventType')
```

### Comparing `kavk_api-1.0.0/kavk_api/longpoll/user.py` & `kavk_api-1.1.0/kavk_api/longpoll/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from ..events import user_events as UserEvents
+from ..events import user_events as UserEventType
 from ..events import enums as UserEnums
 from ..kavk_api import Vk
 from ..events.enums import DEFAULT_MODE
+from typing import AsyncIterator
 
 class UserLongPoll:
     def __init__(self, vk:Vk, _wait:int=25, _mode:int=DEFAULT_MODE, _v:int=3) -> None:
         self._vk = vk
         self._wait = _wait
         self._mode = _mode
         self._v = _v
         self._params = {}
         self._server = ''
         self._updates = []
 
-    async def listen(self):
+    async def listen(self) -> AsyncIterator[UserEventType.AnyUserEvent|UserEventType.UnknowEvent]:
         while 1:
             async for event in UserLongPoll(self._vk, self._wait, self._mode, self._v):
                 yield event 
 
     async def _get_event_raw(self, url:str, params:dict) -> dict:
         r = await self._vk.client.get(url=url, params=params)
         r = await r.json()
@@ -54,31 +55,28 @@
     # Что происходит дальше?
     # __aiter__ возвращает коду `async for e in UserLongPoll.listem()`
     # функцию __anext__.
     # Она же в свою очередь просто получает наш новый ивент
 
     def __aiter__(self): return self
 
-    async def __anext__(self):
+    async def __anext__(self) -> UserEventType.AnyUserEvent|UserEventType.UnknowEvent:
         if self._params == {}: 
             await self._update_params()
 
         if self._updates != []:
             u = self._updates.pop(0)
-            return UserEvents._get_event(u)
+            return UserEventType._get_event(u)
         
         updates = []
         while updates == []:
             updates = await self._get_event()
-            if len(updates) > 0:
-                if updates[0][0] > 600: # Игнорим ивенты реакций
-                    updates.clear()
         
-        if len(updates) > 0:
-            self._updates = updates[1:]
-            update = updates[0]
+        if len(updates) > 0: # Если пришло больше одного события
+            self._updates = updates[1:] # Оставляем все кроме первого чтобы потомих вернуть
+            update = updates[0] # работаем над первым
         else:
             update = updates
-        return UserEvents._get_event(update)
+        return UserEventType._get_event(update)
 
 
-__all__ = ("UserEvents", "UserLongPoll", "UserEnums")
+__all__ = ("UserEventType", "UserLongPoll", "UserEnums")
```

### Comparing `kavk_api-1.0.0/kavk_api/upload/upload.py` & `kavk_api-1.1.0/kavk_api/upload/upload.py`

 * *Files identical despite different names*

### Comparing `kavk_api-1.0.0/PKG-INFO` & `kavk_api-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,42 @@
 Metadata-Version: 2.1
 Name: kavk-api
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 License: MIT
 Author: Kravandir
 Author-email: kravandir@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-.. image :: https://i.imgur.com/yqfZiRG.png
-   :align: center
-   :alt: KAVK_API logo
+# KAVK_API
+[![](https://img.shields.io/pypi/v/kavk_api?style=for-the-badge)](https://pypi.org/project/kavk-api/)
+[![](https://img.shields.io/pypi/l/kavk_api?style=for-the-badge)](https://pypi.org/project/kavk-api/)
+[![](https://img.shields.io/badge/VK-Contact-blue?style=for-the-badge)](https://vk.com/klm_ahmed)
+
+## Установка
+`pip install kavk_api`
+
+## Пример
+``` python
+import asyncio
+from kavk_api import Vk
+from kavk_api.longpoll import BotLongPoll
+
+async def main():
+    vk = Vk('token')
+    longpoll = LongPoll(vk)
+    await vk.wall.post(message="Привет kavk_api!")
+    async for event in longpoll.listen():
+        print(event.type, event.object)
+        
+asyncio.run(main())
+```
 
-
-.. image :: https://img.shields.io/pypi/v/kavk_api?style=for-the-badge
-   :alt: PyPi version
-   :target: https://pypi.python.org/pypi/kavk_api
-
-.. image :: https://img.shields.io/pypi/l/kavk_api?style=for-the-badge
-   :alt: MIT License
-   :target: https://pypi.python.org/pypi/kavk_api
-
-.. image :: https://img.shields.io/badge/VK-Contact-blue?style=for-the-badge
-   :alt: https://vk.com/klm_ahmed
-   :target: https://vk.com/klm_ahmed
-
-=========
-
-Установка
----------
-``pip install kavk_api``
-
-TODO:
--------
-* замена asyncio.run()
-
-
-Пример:
--------
-.. code-block:: python
-
-        import asyncio
-        from kavk_api import Vk
-        from kavk_api.longpoll.bot import BotLongPoll
-
-        async def main():
-            vk = Vk('token')
-            longpoll = LongPoll(vk)
-            await vk.wall.post(message="Привет kavk_api!")
-            async for event in longpoll.listen():
-                print(event.type, event.object)
-      
-  
-        asyncio.run(main())
+## TODO
+- Замена asyncio.run()
```

