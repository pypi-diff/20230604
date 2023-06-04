# Comparing `tmp/dibug-0.2.0.tar.gz` & `tmp/dibug-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dibug-0.2.0.tar", max compression
+gzip compressed data, was "dibug-0.3.0.tar", max compression
```

## Comparing `dibug-0.2.0.tar` & `dibug-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1076 2023-06-04 03:44:41.322614 dibug-0.2.0/LICENSE
--rw-r--r--   0        0        0      651 2023-06-04 03:44:41.322614 dibug-0.2.0/README.md
--rw-r--r--   0        0        0       66 2023-06-04 03:44:41.322614 dibug-0.2.0/dibug/__init__.py
--rw-r--r--   0        0        0       62 2023-06-04 03:44:41.322614 dibug-0.2.0/dibug/abc/__init__.py
--rw-r--r--   0        0        0      283 2023-06-04 03:44:41.322614 dibug-0.2.0/dibug/abc/command.py
--rw-r--r--   0        0        0      105 2023-06-04 03:44:41.322614 dibug-0.2.0/dibug/commands/__init__.py
--rw-r--r--   0        0        0     1732 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/commands/eval.py
--rw-r--r--   0        0        0     1387 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/commands/shell.py
--rw-r--r--   0        0        0     1398 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/dibugger.py
--rw-r--r--   0        0        0        0 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/py.typed
--rw-r--r--   0        0        0      144 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/utils/__init__.py
--rw-r--r--   0        0        0      439 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/utils/chunk.py
--rw-r--r--   0        0        0      628 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/utils/embed.py
--rw-r--r--   0        0        0      808 2023-06-04 03:44:41.326614 dibug-0.2.0/dibug/utils/inspect.py
--rw-r--r--   0        0        0      620 2023-06-04 03:44:41.326614 dibug-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 dibug-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-04 09:00:55.995692 dibug-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1190 2023-06-04 09:00:55.995692 dibug-0.3.0/README.md
+-rw-r--r--   0        0        0       66 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/abc/__init__.py
+-rw-r--r--   0        0        0      283 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/abc/command.py
+-rw-r--r--   0        0        0      150 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/commands/__init__.py
+-rw-r--r--   0        0        0     1734 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/commands/eval.py
+-rw-r--r--   0        0        0     1682 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/commands/info.py
+-rw-r--r--   0        0        0     1384 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/commands/shell.py
+-rw-r--r--   0        0        0     1624 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/dibugger.py
+-rw-r--r--   0        0        0        0 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/py.typed
+-rw-r--r--   0        0        0      144 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/utils/__init__.py
+-rw-r--r--   0        0        0      470 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/utils/chunk.py
+-rw-r--r--   0        0        0      628 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/utils/embed.py
+-rw-r--r--   0        0        0      808 2023-06-04 09:00:55.995692 dibug-0.3.0/dibug/utils/inspect.py
+-rw-r--r--   0        0        0      696 2023-06-04 09:00:55.995692 dibug-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 dibug-0.3.0/PKG-INFO
```

### Comparing `dibug-0.2.0/LICENSE` & `dibug-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dibug-0.2.0/dibug/commands/eval.py` & `dibug-0.3.0/dibug/commands/eval.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 from ..abc import DibugCommand
 from ..utils import DibugEmbed, inspect
 
 
 class EvalCommand(DibugCommand):
     def __init__(self, name: list[str], client: Client) -> None:
         self.name = name
-        self.client = client
+
+        self.__client = client
 
     async def execute(self, msg: Message, args: str) -> None:
         if not args:
-            await msg.channel.send("No codes")
+            await msg.reply("Missing code")
             return
 
         res = await msg.reply("Running...")
 
         if args.startswith("```py") and args.endswith("```"):
-            args = args[5:-3]
+            args = args[6:-3]
 
         try:
-            result = eval(args, {"client": self.client, "msg": msg})
+            result = eval(args, {"client": self.__client, "msg": msg})
 
             embed = (
                 DibugEmbed("Eval")
                 .chunked_fields(
                     "Input",
                     args,
                     "py",
```

### Comparing `dibug-0.2.0/dibug/commands/shell.py` & `dibug-0.3.0/dibug/commands/shell.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 class ShellCommand(DibugCommand):
     def __init__(self, name: list[str]) -> None:
         self.name = name
 
     async def execute(self, msg: Message, args: str) -> None:
         if not args:
-            await msg.channel.send("No codes")
+            await msg.reply("Missing code")
             return
 
         res = await msg.reply("Running...")
 
         if args.startswith("```sh") and args.endswith("```"):
-            args = args[5:-3]
+            args = args[6:-3]
 
         result = run(args, capture_output=True, shell=True, text=True)
 
         if result.stderr:
             embed = (
                 DibugEmbed("Shell", True)
                 .chunked_fields(
```

### Comparing `dibug-0.2.0/dibug/dibugger.py` & `dibug-0.3.0/dibug/dibugger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-from typing import Any, Callable, Type
+from typing import Any, Callable, Literal, Type
 
 from discord import Client, Message
 
 from .abc import DibugCommand
-from .commands import EvalCommand, ShellCommand
+from .commands import EvalCommand, InfoCommand, ShellCommand
 
 
 class Dibugger:
     def __init__(
         self,
         client: Client,
         is_owner: Callable[[int], bool],
         no_perm_msg: str = "No Permission",
-        prefix: str = "!dbg ",
+        prefix: str = "!dbg",
+        default: Literal["info"] = "info",
     ):
         self.client = client
         self.is_owner = is_owner
         self.no_perm_msg = no_perm_msg
         self.prefix = prefix
+        self.default = default
 
         self.__commands: list[DibugCommand] = []
 
-        self.__register_command(EvalCommand, ["eval", "e", "python", "py"], client)
+        self.__register_command(EvalCommand, ["eval", "e", "python", "py"], self.client)
+        self.__register_command(InfoCommand, ["info", "i"], self.client)
         self.__register_command(ShellCommand, ["shell", "sh"])
 
     def __register_command(
         self, command: Type[DibugCommand], name: list[str], *args: Any, **kwargs: Any
     ) -> None:
         self.__commands.append(command(name, *args, **kwargs))
 
@@ -33,14 +36,17 @@
         if msg.author.bot or not msg.content.startswith(self.prefix):
             return
 
         if not self.is_owner(msg.author.id):
             await msg.channel.send(self.no_perm_msg)
             return
 
-        cmd = msg.content[len(self.prefix) :]
+        cmd = msg.content[len(self.prefix) :].split()
+
+        if not cmd:
+            cmd = [self.default]
 
         for command in self.__commands:
             for name in command.name:
-                if cmd.startswith(name):
-                    await command.execute(msg, cmd[len(name) + 1 :])
+                if cmd[0] == name:
+                    await command.execute(msg, " ".join(cmd[1:]))
                     return
```

### Comparing `dibug-0.2.0/dibug/utils/embed.py` & `dibug-0.3.0/dibug/utils/embed.py`

 * *Files identical despite different names*

### Comparing `dibug-0.2.0/dibug/utils/inspect.py` & `dibug-0.3.0/dibug/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `dibug-0.2.0/pyproject.toml` & `dibug-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "dibug"
-version = "0.2.0"
+version = "0.3.0"
 description = "Debugging Tool for discord.py"
 authors = ["Starcea <stardev.uwu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/star0202/dibug"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 discord-py = ">=2.0.0"
 async-eval = "^0.1.11"
+psutil = "^5.9.5"
 
 [tool.poetry.group.style.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 
 [tool.poetry.group.type.dependencies]
 mypy = "^1.3.0"
+types-setuptools = "^67.8.0.0"
+types-psutil = "^5.9.5.13"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 files = ["dibug", "typings"]
 strict = true
```

