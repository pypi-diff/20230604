# Comparing `tmp/commandsgpt-1.4.0.tar.gz` & `tmp/commandsgpt-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandsgpt-1.4.0.tar", last modified: Sun Jun  4 21:09:21 2023, max compression
+gzip compressed data, was "commandsgpt-1.4.1.tar", last modified: Sun Jun  4 21:12:46 2023, max compression
```

## Comparing `commandsgpt-1.4.0.tar` & `commandsgpt-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:21.152691 commandsgpt-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-06-04 21:09:21.152691 commandsgpt-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:21.148691 commandsgpt-1.4.0/commands_gpt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:21.148691 commandsgpt-1.4.0/commands_gpt/commands_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:21.148691 commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/commands_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/recognizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/commands_gpt/commands_gpt/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:09:21.152691 commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-06-04 21:09:21.000000 commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-04 21:09:21.000000 commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:09:21.000000 commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 21:09:21.000000 commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-04 21:09:08.000000 commandsgpt-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-04 21:09:21.152691 commandsgpt-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:12:46.463716 commandsgpt-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-06-04 21:12:46.463716 commandsgpt-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:12:46.459716 commandsgpt-1.4.1/commands_gpt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:12:46.463716 commandsgpt-1.4.1/commands_gpt/commands_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/commands_gpt/commands_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/commands_gpt/commands_gpt/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:12:46.463716 commandsgpt-1.4.1/commands_gpt/commands_gpt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/commands_gpt/commands_gpt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/commands_gpt/commands_gpt/commands/commands_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/commands_gpt/commands_gpt/commands/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/commands_gpt/commands_gpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/commands_gpt/commands_gpt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/commands_gpt/commands_gpt/recognizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/commands_gpt/commands_gpt/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:12:46.463716 commandsgpt-1.4.1/commands_gpt/commandsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-06-04 21:12:46.000000 commandsgpt-1.4.1/commands_gpt/commandsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-04 21:12:46.000000 commandsgpt-1.4.1/commands_gpt/commandsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:12:46.000000 commandsgpt-1.4.1/commands_gpt/commandsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 21:12:46.000000 commandsgpt-1.4.1/commands_gpt/commandsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-04 21:12:34.000000 commandsgpt-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-04 21:12:46.463716 commandsgpt-1.4.1/setup.cfg
```

### Comparing `commandsgpt-1.4.0/LICENSE` & `commandsgpt-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.4.0/PKG-INFO` & `commandsgpt-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.4.0
+Version: 1.4.1
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: BSD License
@@ -224,15 +224,16 @@
     "WRITE_FILE": write_file_command,
     "CONCATENATE_STRINGS": concatenate_strings_command,
 }
 ```
 
 ## main.py
 ```python
-from commands_gpt.instruction_recognition import recognize_instruction_and_create_graph
+from commands_gpt.recognizers import ComplexRecognizer
+from commands_gpt.commands.graphs import Graph
 from commands_gpt.config import Config
 from custom_commands import commands, command_name_to_func
 
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 
 chat_model = "gpt-4-0314"
```

### Comparing `commandsgpt-1.4.0/README.md` & `commandsgpt-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,16 @@
     "WRITE_FILE": write_file_command,
     "CONCATENATE_STRINGS": concatenate_strings_command,
 }
 ```
 
 ## main.py
 ```python
-from commands_gpt.instruction_recognition import recognize_instruction_and_create_graph
+from commands_gpt.recognizers import ComplexRecognizer
+from commands_gpt.commands.graphs import Graph
 from commands_gpt.config import Config
 from custom_commands import commands, command_name_to_func
 
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 
 chat_model = "gpt-4-0314"
```

### Comparing `commandsgpt-1.4.0/commands_gpt/commands_gpt/chat.py` & `commandsgpt-1.4.1/commands_gpt/commands_gpt/chat.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/commands_funcs.py` & `commandsgpt-1.4.1/commands_gpt/commands_gpt/commands/commands_funcs.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.4.0/commands_gpt/commands_gpt/commands/graphs.py` & `commandsgpt-1.4.1/commands_gpt/commands_gpt/commands/graphs.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.4.0/commands_gpt/commands_gpt/config.py` & `commandsgpt-1.4.1/commands_gpt/commands_gpt/config.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.4.0/commands_gpt/commands_gpt/recognizers.py` & `commandsgpt-1.4.1/commands_gpt/commands_gpt/recognizers.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.4.0/commands_gpt/commands_gpt/regex.py` & `commandsgpt-1.4.1/commands_gpt/commands_gpt/regex.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/PKG-INFO` & `commandsgpt-1.4.1/commands_gpt/commandsgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.4.0
+Version: 1.4.1
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: BSD License
@@ -224,15 +224,16 @@
     "WRITE_FILE": write_file_command,
     "CONCATENATE_STRINGS": concatenate_strings_command,
 }
 ```
 
 ## main.py
 ```python
-from commands_gpt.instruction_recognition import recognize_instruction_and_create_graph
+from commands_gpt.recognizers import ComplexRecognizer
+from commands_gpt.commands.graphs import Graph
 from commands_gpt.config import Config
 from custom_commands import commands, command_name_to_func
 
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 
 chat_model = "gpt-4-0314"
```

### Comparing `commandsgpt-1.4.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt` & `commandsgpt-1.4.1/commands_gpt/commandsgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.4.0/setup.cfg` & `commandsgpt-1.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = commandsgpt
-version = 1.4.0
+version = 1.4.1
 author = Martín Alexis Martínez Andrade
 author_email = alexis.martinez.contacto@gmail.com
 description = An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/AlexisAndradeDev/CommandsGPT
 project_urls =
```

