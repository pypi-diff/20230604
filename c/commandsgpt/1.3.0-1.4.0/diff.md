# Comparing `tmp/commandsgpt-1.3.0.tar.gz` & `tmp/commandsgpt-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandsgpt-1.3.0.tar", last modified: Wed May 24 21:55:06 2023, max compression
+gzip compressed data, was "commandsgpt-1.4.0.tar", last modified: Sun Jun  4 21:09:21 2023, max compression
```

## Comparing `commandsgpt-1.3.0.tar` & `commandsgpt-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:55:06.625001 commandsgpt-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-24 21:55:06.625001 commandsgpt-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:55:06.621001 commandsgpt-1.3.0/commands_gpt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:55:06.621001 commandsgpt-1.3.0/commands_gpt/commands_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:55:06.621001 commandsgpt-1.3.0/commands_gpt/commands_gpt/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/commands/commands_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/commands/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/instruction_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/commands_gpt/commands_gpt/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:55:06.625001 commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-24 21:55:06.000000 commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-24 21:55:06.000000 commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:55:06.000000 commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 21:55:06.000000 commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 21:54:55.000000 commandsgpt-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-24 21:55:06.625001 commandsgpt-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:21.152691 commandsgpt-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-06-04 21:09:21.152691 commandsgpt-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:21.148691 commandsgpt-1.4.0/commands_gpt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:21.148691 commandsgpt-1.4.0/commands_gpt/commands_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:21.148691 commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/commands_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/recognizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:21.152691 commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-06-04 21:09:21.000000 commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-04 21:09:21.000000 commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:09:21.000000 commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 21:09:21.000000 commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-04 21:09:21.152691 commandsgpt-1.4.0/setup.cfg
```

### Comparing `commandsgpt-1.3.0/LICENSE` & `commandsgpt-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.3.0/PKG-INFO` & `commandsgpt-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.3.0
+Version: 1.4.0
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: BSD License
@@ -114,26 +114,30 @@
 
 Create an instruction:
 
 ```python
 instruction = input("Enter your instruction: ")
 ```
 
+Create a recognizer:
+
+```python
+recognizer = ComplexRecognizer(config, commands, command_name_to_func)
+```
+
 Pass your instruction to the recognizer model:
 
 ```python
-graph = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, commands, command_name_to_func,
-    verbosity=config.verbosity, save_graph_as_file=config.save_graph_as_file
-)
+commands_data_str = recognizer.recognize(instruction)
 ```
 
-Finally, execute the graph of commands:
+Create the graph of commands and execute it:
 
 ```python
+graph = Graph(recognizer, commands_data_str)
 graph.execute_commands(config)
 ```
 
 # Example
 
 Create two files: `custom_commands.py` and `main.py`.
 
@@ -232,18 +236,19 @@
 add_essential_commands(commands, command_name_to_func)
 
 chat_model = "gpt-4-0314"
 
 config = Config(chat_model, verbosity=2, explain_graph=False, save_graph_as_file=False)
 
 instruction = input("Enter your prompt: ")
-graph = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, commands, command_name_to_func,
-    verbosity=config.verbosity, save_graph_as_file=config.save_graph_as_file
-)
+
+recognizer = ComplexRecognizer(config, commands, command_name_to_func)
+
+commands_data_str = recognizer.recognize(instruction)
+graph = Graph(recognizer, commands_data_str)
 graph.execute_commands(config)
 ```
 
 Copyright (c) 2023, Martín Alexis Martínez Andrade.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

### Comparing `commandsgpt-1.3.0/README.md` & `commandsgpt-1.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -98,26 +98,30 @@
 
 Create an instruction:
 
 ```python
 instruction = input("Enter your instruction: ")
 ```
 
+Create a recognizer:
+
+```python
+recognizer = ComplexRecognizer(config, commands, command_name_to_func)
+```
+
 Pass your instruction to the recognizer model:
 
 ```python
-graph = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, commands, command_name_to_func,
-    verbosity=config.verbosity, save_graph_as_file=config.save_graph_as_file
-)
+commands_data_str = recognizer.recognize(instruction)
 ```
 
-Finally, execute the graph of commands:
+Create the graph of commands and execute it:
 
 ```python
+graph = Graph(recognizer, commands_data_str)
 graph.execute_commands(config)
 ```
 
 # Example
 
 Create two files: `custom_commands.py` and `main.py`.
 
@@ -216,13 +220,14 @@
 add_essential_commands(commands, command_name_to_func)
 
 chat_model = "gpt-4-0314"
 
 config = Config(chat_model, verbosity=2, explain_graph=False, save_graph_as_file=False)
 
 instruction = input("Enter your prompt: ")
-graph = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, commands, command_name_to_func,
-    verbosity=config.verbosity, save_graph_as_file=config.save_graph_as_file
-)
+
+recognizer = ComplexRecognizer(config, commands, command_name_to_func)
+
+commands_data_str = recognizer.recognize(instruction)
+graph = Graph(recognizer, commands_data_str)
 graph.execute_commands(config)
 ```
```

### Comparing `commandsgpt-1.3.0/commands_gpt/commands_gpt/chat.py` & `commandsgpt-1.4.0/commands_gpt/commands_gpt/chat.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.3.0/commands_gpt/commands_gpt/commands/commands_funcs.py` & `commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/commands_funcs.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # The return value must be a dictionary which keys must match the "generates_data" keys
 # The data types must match the ones declared in the ESSENTIAL_COMMANDS dictionary
 
 def think_command(config: Config, graph: Graph, about: str) -> dict[str, Any]:
     messages = [
         {
             "role": "system", 
-            "content": "You are a model used when executing a 'THINK' command, which function is to reflect, think, write, or ideate."
+            "content": "You are a model used when executing a 'THINK' command, which function is to reflect, think, write, or ideate. Only do what the prompt says; DO NOT add useless/extra information/irrelevant chat/irrelevant explanation."
         },
     ]
     thought = get_answer_from_model(about, config.chat_model, messages)
 
     results = {
         "thought": thought,
     }
@@ -76,19 +76,18 @@
     }
     return results
 
 def calculate_command(config: Config, graph: Graph, expression: str) -> dict[str, Any]:
     try:
         result = safe_eval_math_expr(expression)
     except ValueError:
-        # TODO: convert from natural language to math expression
         messages = [
             {
                 "role": "system",
-                "content": f"You are a model that takes a math expression in natural language and returns JUST the math expression, without any words. 'Negative one raised to the 1/2 plus eight' -> '(-1) ** (1/2) + 8'"
+                "content": f"You are a model that takes a math expression in natural language and returns ONLY the math expression, without any words. You can only use +, -, *, /, %, **, //. Example: 'Square root of negative one plus eight' -> '(-1) ** (1/2) + 8'"
             }
         ]
         expression_ = get_answer_from_model(expression, config.chat_model, messages)
         result = safe_eval_math_expr(expression_)
 
     results = {
         "result": result,
```

### Comparing `commandsgpt-1.3.0/commands_gpt/commands_gpt/commands/graphs.py` & `commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/graphs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import Any, Callable
 
+from ..recognizers import AbstractRecognizer
 from .. import regex
-from .. import instruction_recognition
 from ..config import Config
 
 # next commands field indexes
 NEXT_COMMAND_ID = 0
 DEPENDENT_ON_DATA = 1
 REQUIRED_VALUE = 2
 
@@ -46,30 +46,28 @@
                 next_commands_to_execute.append(next_command_id)
             else: # next command execution depends on the result of current node
                 if self.data_generated[dependent_on_data] == required_value:
                     next_commands_to_execute.append(next_command_id)
         return next_commands_to_execute
 
 class Graph:
-    def __init__(self, raw_commands_data: str, commands: dict[str, dict], 
-            command_name_to_func: dict[str, Callable]):
-        self.set_start_data(raw_commands_data, commands, command_name_to_func)
+    def __init__(self, recognizer: AbstractRecognizer, commands_data_str: str):
+        self.set_start_data(recognizer, commands_data_str)
         self.initialize()
 
-    def set_start_data(self, raw_commands_data: str, commands: dict[str, dict], 
-            command_name_to_func: dict[str, Callable]):
-        self.raw_commands_data = raw_commands_data
-        self.commands = commands
-        self.command_name_to_func = command_name_to_func
+    def set_start_data(self, recognizer: AbstractRecognizer, commands_data_str: str):
+        self.recognizer = recognizer
+        self.commands_data_str = commands_data_str
+        self.commands = recognizer.commands
+        self.command_name_to_func = recognizer.command_name_to_func
 
-    def build_graph(self, raw_commands_data: str, commands: dict[str, dict], 
-            command_name_to_func: dict[str, Callable]):
-        self.set_start_data(raw_commands_data, commands, command_name_to_func)
+    def build_graph(self, commands_data_str: str):
+        self.set_start_data(self.recognizer, commands_data_str)
 
-        graph_build_data = generate_graph_build_data(raw_commands_data)
+        graph_build_data = generate_graph_build_data(commands_data_str)
         (self.commands_data_str_by_node,
          self.commands_data,
          self.data_references_in_each_command) = graph_build_data
 
         self.build_nodes()
 
     def build_node(self, command_data: dict) -> CommandNode:
@@ -84,15 +82,15 @@
         for command_data in self.commands_data.values():
             node = self.build_node(command_data)
             self.nodes[node.id] = node
 
     def initialize(self):
         self.reached_nodes_ids: list[int] = []
         self.nodes: dict[str, CommandNode] = {}
-        self.build_graph(self.raw_commands_data, self.commands, self.command_name_to_func)
+        self.build_graph(self.commands_data_str)
             
     def execute_node(self, node_id: int, config: Config) -> list[int]:
         node = self.nodes[node_id]
 
         # inject data references to current node's arguments
         injected_command_data_str = self.commands_data_str_by_node[node.id]
         for node_to_inject_id in self.data_references_in_each_command[node.id]:
@@ -110,15 +108,15 @@
 
         node.execute_command(config, self, node.arguments)
         self.reached_nodes_ids.append(node.id)
         
         next_commands_to_execute = node.get_next_commands_to_execute()
         return next_commands_to_execute
 
-    def print_graph(self, explain_graph: bool, config: Config):
+    def print_graph(self, explain_graph: bool):
         print("\n\n--- Commands graph ---")
 
         print("\n~~ Graph ~~")
         for node in self.nodes.values():
             print(f"\n{node.id}. {node.command_name}")
             
             if node.next_commands:
@@ -127,23 +125,23 @@
                     next_node = self.nodes[next_command_id]
                     print(f"\t{next_node.id}. {next_node.command_name}")
                     if dependent_on_data is not None:
                         print(f"\t\tIf '{dependent_on_data}' generated data has value: {required_value}.")
 
         if explain_graph:
             print("\n~~ Explanation ~~")
-            explanation = instruction_recognition.explain_graph_in_natural_language(self.raw_commands_data, config.chat_model, self.commands)
+            explanation = self.recognizer.explain_graph_in_natural_language(self.commands_data_str)
             print(explanation)
 
         print("\n--- -------------- ---\n")
 
     def execute_commands(self, config: Config):
         self.initialize()
         if config.verbosity >= 1:
-            self.print_graph(config.explain_graph, config)
+            self.print_graph(config.explain_graph)
 
         first_node_id = sorted(self.nodes.keys())[0]
         next_commands_to_execute = self.execute_node(first_node_id, config)
         new_next_commands_to_execute = []
         while True:
             new_next_commands_to_execute.clear()
             for next_command_id in next_commands_to_execute:
@@ -188,44 +186,44 @@
         "name": name,
         "arguments": arguments,
         "next_commands": next_commands,
     }
 
     return command_data
 
-def generate_graph_build_data(raw_commands_data: str):
+def generate_graph_build_data(commands_data_str: str):
     """
     Parses a commands data string to a JSON to create the graph data
 
     Args:
-        raw_commands_data (str): A string containing raw commands data in JSON-Lines-like format that has not yet been converted to a JSON.
+        commands_data_str (str): A string containing the data to create a graph/command.
 
     Returns:
         a tuple: Containing:
-            raw_commands_data_by_node (dict of str): Commands data as a string.
+            commands_data_str_by_node (dict of str): Commands data as a string.
                 Keys are the ID of the commands; values are the commands data
                 as strings.
         
             commands_data: data of the commands as JSON (to create a graph).
 
             data_references_in_each_command: data references that appear inside of each command (data that will be injected).
                 A key is the ID of a command. The value stores a dictionary of data references inside of that particular command.
     """
     data_references_in_each_command = {}
 
     commands_data = {}
-    raw_commands_data_by_node = {}
-    for line_num, command_data_str in enumerate(raw_commands_data.splitlines(), start=1):
+    commands_data_str_by_node = {}
+    for line_num, command_data_str in enumerate(commands_data_str.splitlines(), start=1):
         data_references = get_node_data_references(command_data_str)
         try:
             command_data = get_node_command_data(command_data_str)
         except Exception as e:
             print(f"!!! Can't decode command data string to JSON in line {line_num}: {command_data_str}")
             raise e
 
         command_id = command_data["id"]
 
-        raw_commands_data_by_node[command_id] = command_data_str
+        commands_data_str_by_node[command_id] = command_data_str
         commands_data[command_id] = command_data
         data_references_in_each_command[command_id] = data_references
 
-    return raw_commands_data_by_node, commands_data, data_references_in_each_command
+    return commands_data_str_by_node, commands_data, data_references_in_each_command
```

### Comparing `commandsgpt-1.3.0/commands_gpt/commands_gpt/config.py` & `commandsgpt-1.4.0/commands_gpt/commands_gpt/config.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.3.0/commands_gpt/commands_gpt/regex.py` & `commandsgpt-1.4.0/commands_gpt/commands_gpt/regex.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,42 +44,42 @@
         value = generated_data_by_node[data_name]
 
     value_as_str = str(value)
     value_as_str = escape_str_for_json(value_as_str)
 
     return value_as_str
 
-def inject_node_data(raw_commands_data: str, node_id, generated_data_by_node: dict[str, Any]):
+def inject_node_data(commands_data_str: str, node_id, generated_data_by_node: dict[str, Any]):
     pattern = rf"__&{node_id}\.(\w+)__"
-    return re.sub(pattern, lambda m: replace_generated_data_by_node(m, generated_data_by_node), raw_commands_data)
+    return re.sub(pattern, lambda m: replace_generated_data_by_node(m, generated_data_by_node), commands_data_str)
 
-def nullify_all_data_references(raw_commands_data: str):
+def nullify_all_data_references(commands_data_str: str):
     """Replaces all __&i.data__ by null."""
     pattern = r"__&(\d+)\.(\w+(?:\[\d+\])*)__"
-    return re.sub(pattern, "null", raw_commands_data)
+    return re.sub(pattern, "null", commands_data_str)
 
-def find_data_references_indices(raw_commands_data: str) -> dict[int, dict[str, list[tuple]]]:
+def find_data_references_indices(commands_data_str: str) -> dict[int, dict[str, list[tuple]]]:
     """
     Returns a dictionary with the ID of each command and the name of the generated data, along with their start and end positions
     in the raw commands data string.
 
     Args:
-        raw_commands_data (str): A string containing raw commands data that has not yet been converted to JSON.
+        commands_data_str (str): A string containing the data to create a graph/command.
 
     Returns:
         A dictionary where the keys are command IDs and the values are dictionaries representing the generated data for that
         command. These inner dictionaries have keys that are names of generated data variables and values that are lists of tuples.
         Each tuple in these lists contains the starting and ending positions of the generated data variable within the
-        raw_commands_data input string.
+        commands_data_str input string.
 
     Example:
         {1: {'urls[0]': [(115, 129), (299, 313)]}, 2: {'text': [(214, 225)]}}
     """
     pattern = r"__&(\d+)\.(\w+(?:\[\d+\])*)__"
-    matches = re.finditer(pattern, raw_commands_data)
+    matches = re.finditer(pattern, commands_data_str)
     references = {}
     for match in matches:
         command_id = int(match.group(1))
         generated_data_name = match.group(2)
         start_index = match.start()
         end_index = match.end()
```

### Comparing `commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/PKG-INFO` & `commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.3.0
+Version: 1.4.0
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: BSD License
@@ -114,26 +114,30 @@
 
 Create an instruction:
 
 ```python
 instruction = input("Enter your instruction: ")
 ```
 
+Create a recognizer:
+
+```python
+recognizer = ComplexRecognizer(config, commands, command_name_to_func)
+```
+
 Pass your instruction to the recognizer model:
 
 ```python
-graph = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, commands, command_name_to_func,
-    verbosity=config.verbosity, save_graph_as_file=config.save_graph_as_file
-)
+commands_data_str = recognizer.recognize(instruction)
 ```
 
-Finally, execute the graph of commands:
+Create the graph of commands and execute it:
 
 ```python
+graph = Graph(recognizer, commands_data_str)
 graph.execute_commands(config)
 ```
 
 # Example
 
 Create two files: `custom_commands.py` and `main.py`.
 
@@ -232,18 +236,19 @@
 add_essential_commands(commands, command_name_to_func)
 
 chat_model = "gpt-4-0314"
 
 config = Config(chat_model, verbosity=2, explain_graph=False, save_graph_as_file=False)
 
 instruction = input("Enter your prompt: ")
-graph = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, commands, command_name_to_func,
-    verbosity=config.verbosity, save_graph_as_file=config.save_graph_as_file
-)
+
+recognizer = ComplexRecognizer(config, commands, command_name_to_func)
+
+commands_data_str = recognizer.recognize(instruction)
+graph = Graph(recognizer, commands_data_str)
 graph.execute_commands(config)
 ```
 
 Copyright (c) 2023, Martín Alexis Martínez Andrade.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

### Comparing `commandsgpt-1.3.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt` & `commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 commands_gpt/commands_gpt/__init__.py
 commands_gpt/commands_gpt/chat.py
 commands_gpt/commands_gpt/config.py
-commands_gpt/commands_gpt/instruction_recognition.py
 commands_gpt/commands_gpt/models.py
+commands_gpt/commands_gpt/recognizers.py
 commands_gpt/commands_gpt/regex.py
 commands_gpt/commands_gpt/commands/__init__.py
 commands_gpt/commands_gpt/commands/commands_funcs.py
 commands_gpt/commands_gpt/commands/graphs.py
 commands_gpt/commandsgpt.egg-info/PKG-INFO
 commands_gpt/commandsgpt.egg-info/SOURCES.txt
 commands_gpt/commandsgpt.egg-info/dependency_links.txt
```

### Comparing `commandsgpt-1.3.0/setup.cfg` & `commandsgpt-1.4.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = commandsgpt
-version = 1.3.0
+version = 1.4.0
 author = Martín Alexis Martínez Andrade
 author_email = alexis.martinez.contacto@gmail.com
 description = An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/AlexisAndradeDev/CommandsGPT
 project_urls =
```

