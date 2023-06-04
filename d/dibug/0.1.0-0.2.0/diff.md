# Comparing `tmp/dibug-0.1.0.tar.gz` & `tmp/dibug-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dibug-0.1.0.tar", max compression
+gzip compressed data, was "dibug-0.2.0.tar", max compression
```

## Comparing `dibug-0.1.0.tar` & `dibug-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0       66 2023-06-03 14:25:19.905509 dibug-0.1.0/dibug/__init__.py
--rw-r--r--   0        0        0       62 2023-06-03 14:45:27.624371 dibug-0.1.0/dibug/abc/__init__.py
--rw-r--r--   0        0        0      283 2023-06-04 02:33:21.091273 dibug-0.1.0/dibug/abc/command.py
--rw-r--r--   0        0        0       57 2023-06-04 02:12:35.211403 dibug-0.1.0/dibug/commands/__init__.py
--rw-r--r--   0        0        0     1896 2023-06-04 02:31:59.034951 dibug-0.1.0/dibug/commands/eval.py
--rw-r--r--   0        0        0     1294 2023-06-04 02:33:39.960648 dibug-0.1.0/dibug/dibugger.py
--rw-r--r--   0        0        0        0 2023-06-03 13:56:14.960755 dibug-0.1.0/dibug/py.typed
--rw-r--r--   0        0        0      144 2023-06-04 02:12:19.528535 dibug-0.1.0/dibug/utils/__init__.py
--rw-r--r--   0        0        0      439 2023-06-03 16:06:15.755868 dibug-0.1.0/dibug/utils/chunk.py
--rw-r--r--   0        0        0      241 2023-06-03 17:44:28.090087 dibug-0.1.0/dibug/utils/embed.py
--rw-r--r--   0        0        0      682 2023-06-04 02:34:26.427981 dibug-0.1.0/dibug/utils/inspect.py
--rw-r--r--   0        0        0     1076 2023-06-03 13:50:11.957369 dibug-0.1.0/LICENSE
--rw-r--r--   0        0        0      571 2023-06-04 02:35:11.299009 dibug-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      651 2023-06-04 02:29:12.190471 dibug-0.1.0/README.md
--rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 dibug-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-04 03:44:41.322614 dibug-0.2.0/LICENSE
+-rw-r--r--   0        0        0      651 2023-06-04 03:44:41.322614 dibug-0.2.0/README.md
+-rw-r--r--   0        0        0       66 2023-06-04 03:44:41.322614 dibug-0.2.0/dibug/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-04 03:44:41.322614 dibug-0.2.0/dibug/abc/__init__.py
+-rw-r--r--   0        0        0      283 2023-06-04 03:44:41.322614 dibug-0.2.0/dibug/abc/command.py
+-rw-r--r--   0        0        0      105 2023-06-04 03:44:41.322614 dibug-0.2.0/dibug/commands/__init__.py
+-rw-r--r--   0        0        0     1732 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/commands/eval.py
+-rw-r--r--   0        0        0     1387 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/commands/shell.py
+-rw-r--r--   0        0        0     1398 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/dibugger.py
+-rw-r--r--   0        0        0        0 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/py.typed
+-rw-r--r--   0        0        0      144 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/utils/__init__.py
+-rw-r--r--   0        0        0      439 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/utils/chunk.py
+-rw-r--r--   0        0        0      628 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/utils/embed.py
+-rw-r--r--   0        0        0      808 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/utils/inspect.py
+-rw-r--r--   0        0        0      620 2023-06-04 03:44:41.326614 dibug-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 dibug-0.2.0/PKG-INFO
```

### Comparing `dibug-0.1.0/dibug/dibugger.py` & `dibug-0.2.0/dibug/dibugger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Callable, Type
 
 from discord import Client, Message
 
 from .abc import DibugCommand
-from .commands import EvalCommand
+from .commands import EvalCommand, ShellCommand
 
 
 class Dibugger:
     def __init__(
         self,
         client: Client,
         is_owner: Callable[[int], bool],
@@ -18,14 +18,15 @@
         self.is_owner = is_owner
         self.no_perm_msg = no_perm_msg
         self.prefix = prefix
 
         self.__commands: list[DibugCommand] = []
 
         self.__register_command(EvalCommand, ["eval", "e", "python", "py"], client)
+        self.__register_command(ShellCommand, ["shell", "sh"])
 
     def __register_command(
         self, command: Type[DibugCommand], name: list[str], *args: Any, **kwargs: Any
     ) -> None:
         self.__commands.append(command(name, *args, **kwargs))
 
     async def handle_msg(self, msg: Message) -> None:
@@ -38,7 +39,8 @@
 
         cmd = msg.content[len(self.prefix) :]
 
         for command in self.__commands:
             for name in command.name:
                 if cmd.startswith(name):
                     await command.execute(msg, cmd[len(name) + 1 :])
+                    return
```

### Comparing `dibug-0.1.0/dibug/utils/inspect.py` & `dibug-0.2.0/dibug/utils/inspect.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,10 +16,13 @@
         for member in getmembers(obj)
         if member not in ignore and not member[0].startswith("_")
     ]
 
     for member in members:
         lines.append(" " * (indent + 2) + str(member))
 
-    lines.append(" " * indent + "]")
+    if not members and not isinstance(obj, Iterable) or isinstance(obj, (str, bytes)):
+        lines[-1] += "]"
+    else:
+        lines.append(" " * indent + "]")
 
     return lines
```

### Comparing `dibug-0.1.0/LICENSE` & `dibug-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dibug-0.1.0/pyproject.toml` & `dibug-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "dibug"
-version = "0.1.0"
+version = "0.2.0"
 description = "Debugging Tool for discord.py"
 authors = ["Starcea <stardev.uwu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+repository = "https://github.com/star0202/dibug"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 discord-py = ">=2.0.0"
 async-eval = "^0.1.11"
 
 [tool.poetry.group.style.dependencies]
```

### Comparing `dibug-0.1.0/README.md` & `dibug-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dibug-0.1.0/PKG-INFO` & `dibug-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: dibug
-Version: 0.1.0
+Version: 0.2.0
 Summary: Debugging Tool for discord.py
+Home-page: https://github.com/star0202/dibug
 License: MIT
 Author: Starcea
 Author-email: stardev.uwu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: async-eval (>=0.1.11,<0.2.0)
 Requires-Dist: discord-py (>=2.0.0)
+Project-URL: Repository, https://github.com/star0202/dibug
 Description-Content-Type: text/markdown
 
 # dibug
 
 Debugging Tool for discord.py
 
 # Usage
```

