# Comparing `tmp/lollms-1.0.3.tar.gz` & `tmp/lollms-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-1.0.3.tar", last modified: Fri Jun  2 14:53:07 2023, max compression
+gzip compressed data, was "lollms-1.1.0.tar", last modified: Sun Jun  4 00:06:45 2023, max compression
```

## Comparing `lollms-1.0.3.tar` & `lollms-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 14:53:07.797795 lollms-1.0.3/
--rw-rw-rw-   0        0        0    11558 2023-06-02 10:47:30.000000 lollms-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     6748 2023-06-02 14:53:07.796796 lollms-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6232 2023-06-02 14:52:39.000000 lollms-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 14:53:07.778795 lollms-1.0.3/lollms/
--rw-rw-rw-   0        0        0    32012 2023-06-02 14:30:56.000000 lollms-1.0.3/lollms/__init__.py
--rw-rw-rw-   0        0        0     6608 2023-06-01 08:52:43.000000 lollms-1.0.3/lollms/binding.py
--rw-rw-rw-   0        0        0     9348 2023-06-02 14:30:56.000000 lollms-1.0.3/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7558 2023-06-02 11:00:49.000000 lollms-1.0.3/lollms/server.py
-drwxrwxrwx   0        0        0        0 2023-06-02 14:53:07.793797 lollms-1.0.3/lollms.egg-info/
--rw-rw-rw-   0        0        0     6748 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      143 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 14:53:07.000000 lollms-1.0.3/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 14:53:07.798797 lollms-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1178 2023-06-02 14:39:07.000000 lollms-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 00:06:45.271135 lollms-1.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4690 2023-06-04 00:06:45.271135 lollms-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4174 2023-06-03 23:58:22.000000 lollms-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 00:06:45.248046 lollms-1.1.0/lollms/
+-rw-rw-rw-   0        0        0    32532 2023-06-03 23:06:41.000000 lollms-1.1.0/lollms/__init__.py
+-rw-rw-rw-   0        0        0     8270 2023-06-03 23:04:42.000000 lollms-1.1.0/lollms/binding.py
+-rw-rw-rw-   0        0        0     9348 2023-06-03 19:43:42.000000 lollms-1.1.0/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     9734 2023-06-03 23:42:16.000000 lollms-1.1.0/lollms/server.py
+drwxrwxrwx   0        0        0        0 2023-06-04 00:06:45.270266 lollms-1.1.0/lollms.egg-info/
+-rw-rw-rw-   0        0        0     4690 2023-06-04 00:06:45.000000 lollms-1.1.0/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-06-04 00:06:45.000000 lollms-1.1.0/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 00:06:45.000000 lollms-1.1.0/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-04 00:06:45.000000 lollms-1.1.0/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      143 2023-06-04 00:06:45.000000 lollms-1.1.0/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-04 00:06:45.000000 lollms-1.1.0/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 00:06:45.271135 lollms-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1178 2023-06-03 20:37:56.000000 lollms-1.1.0/setup.py
```

### Comparing `lollms-1.0.3/LICENSE` & `lollms-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-1.0.3/lollms/__init__.py` & `lollms-1.1.0/lollms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 import subprocess
 import pkg_resources
 from enum import Enum
 
 from lollms.binding import BindingConfig, LLMBinding
 
+lollms_path = Path(__file__).parent
+
 class MSG_TYPE(Enum):
     MSG_TYPE_CHUNK=0
     MSG_TYPE_FULL=1
     MSG_TYPE_META=2
     MSG_TYPE_REF=3
     MSG_TYPE_CODE=4
     MSG_TYPE_UI=5
@@ -48,24 +50,24 @@
         # Install the package using pip
         subprocess.check_call(["pip", "install", package_name])
         
         print(f"{package_name} has been successfully installed.")
 
 
 
-class PAPScript:
+class APScript:
     """
-    Template class for implementing personality processor classes in the PAPScript framework.
+    Template class for implementing personality processor classes in the APScript framework.
 
     This class provides a basic structure and placeholder methods for processing model inputs and outputs.
     Personality-specific processor classes should inherit from this class and override the necessary methods.
 
     Methods:
         __init__():
-            Initializes the PAPScript object.
+            Initializes the APScript object.
 
         run_workflow(generate_fn, prompt):
             Runs the workflow for processing the model input and output.
 
         process_model_input(text):
             Process the model input.
 
@@ -73,16 +75,16 @@
             Process the model output.
 
     Attributes:
         None
 
     Usage:
     ```
-    # Create a personality-specific processor class that inherits from PAPScript
-    class MyPersonalityProcessor(PAPScript):
+    # Create a personality-specific processor class that inherits from APScript
+    class MyPersonalityProcessor(APScript):
         def __init__(self):
             super().__init__()
 
         def process_model_input(self, text):
             # Implement the desired behavior for processing the model input
             # and return the processed model input
 
@@ -102,14 +104,30 @@
 
     # Run the workflow
     my_processor.run_workflow(generate_fn, prompt)
     ```
     """
     def __init__(self) -> None:
         pass
+    
+    def load_config_file(self, path):
+        """
+        Load the content of config_local.yaml file.
+
+        The function reads the content of the config_local.yaml file and returns it as a Python dictionary.
+
+        Args:
+            None
+
+        Returns:
+            dict: A dictionary containing the loaded data from the config_local.yaml file.
+        """     
+        with open(path, 'r') as file:
+            data = yaml.safe_load(file)
+        return data
 
     def run_workflow(self, prompt, previous_discussion_text="", callback=None):
         """
         Runs the workflow for processing the model input and output.
 
         This method should be called to execute the processing workflow.
 
@@ -819,20 +837,20 @@
 
         Args:
             value (int): The new number of words value.
         """
         self._assets_list = value
 
     @property
-    def processor(self) -> PAPScript:
+    def processor(self) -> APScript:
         """Get the number of words to consider for repeat penalty."""
         return self._processor
 
     @processor.setter
-    def processor(self, value: PAPScript):
+    def processor(self, value: APScript):
         """Set the number of words to consider for repeat penalty.
 
         Args:
             value (int): The new number of words value.
         """
         self._processor = value
```

### Comparing `lollms-1.0.3/lollms/binding.py` & `lollms-1.1.0/lollms/binding.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,72 +12,92 @@
 import inspect
 import yaml
 import sys
 from tqdm import tqdm
 import urllib
 
 __author__ = "parisneo"
-__github__ = "https://github.com/ParisNeo/gpt4all-ui"
+__github__ = "https://github.com/ParisNeo/lollms_bindings_zoo"
 __copyright__ = "Copyright 2023, "
 __license__ = "Apache 2.0"
 
 
 import yaml
 
 DEFAULT_CONFIG = {
+    # =================== Lord Of Large Language Models Configuration file =========================== 
     "version": 5,
-    "user_name": "user",
-    "config": "default",
-    "ctx_size": 2048,
-    "n_gpu_layers": 20,
-    "db_path": "databases/database.db",
-    "debug": False,
-    "n_threads": 8,
+    "binding_name": "llama_cpp_official",
+    "model_name": "Wizard-Vicuna-7B-Uncensored.ggmlv3.q4_0.bin",
+
+    # Host information
     "host": "localhost",
-    "language": "en-US",
-    "binding": "gpt_4all",
-    "model": None,
-    "n_predict": 1024,
-    "nb_messages_to_remember": 5,
-    "personality_language": "english",
-    "personality_category": "default",
-    "personality": "gpt4all",
     "port": 9600,
-    "repeat_last_n": 40,
-    "repeat_penalty": 1.2,
+
+    # Genreration parameters 
     "seed": -1,
+    "n_predict": 1024,
+    "ctx_size": 2048,
     "temperature": 0.9,
     "top_k": 50,
     "top_p": 0.95,
-    "use_gpu": False,
-    "auto_read": False,
-    "use_avx2": True,
-    "override_personality_model_parameters": False
+    "repeat_last_n": 40,
+    "repeat_penalty": 1.2,
+
+    "n_threads": 8,
+
+    #Personality parameters
+    "personalities": ["english/generic/lollms"],
+    "default_personality_id": 0,
+    "override_personality_model_parameters": False, #if true the personality parameters are overriden by those of the configuration (may affect personality behaviour) 
+
+    "user_name": "user",
+
 }
 
 
 class BindingConfig:
-    def __init__(self, file_path=None):
+    def __init__(self, file_path=None, models_path = None, bindings_path = None, personalities_path = None):
         if file_path:
             self.file_path = Path(file_path)
+            if models_path is None:
+                self.models_path = self.file_path.parent.parent/"models"
+            if bindings_path is None:
+                self.bindings_path = self.file_path.parent.parent/"bindings_zoo"
+            if personalities_path is None:
+                self.personalities_path = self.file_path.parent.parent/"personalities_zoo"
+
+                
         else:
             self.file_path = None
+            self.models_path = None
+            self.bindings_path = None
+            self.personalities_path = None
+
+        if self.models_path is None:
+            self.models_path = Path("./models")
+        if self.bindings_path is None:
+            self.bindings_path = Path("./bindings_zoo")
+
+        if self.personalities_path is None:
+            self.personalities_path = Path("./personalities_zoo")
+
         self.config = None
         
         if file_path is not None:
             self.load_config(file_path)
         else:
             self.config = DEFAULT_CONFIG.copy()
 
     def check_model_existance(self):
-        model_path = Path("models")/self.binding/self.model
+        model_path = self.models_path/self.binding_name/self.model_name
         return model_path.exists()
     
     def download_model(self, url):
-        folder_path = Path("models")/self.binding
+        folder_path = self.models_path/self.binding_name
         model_name  = url.split("/")[-1]
         model_full_path = (folder_path / model_name)
 
         # Check if file already exists in folder
         if model_full_path.exists():
             print("File already exists in folder")
         else:
@@ -104,15 +124,15 @@
     def __getattr__(self, key):
         if self.config is None:
             raise ValueError("No configuration loaded.")
         return self.config[key]
 
 
     def __setattr__(self, key, value):
-        if key in ["file_path", "config"]:
+        if key in ["file_path", "config","models_path","bindings_path","personalities_path"]:
             super().__setattr__(key, value)
         else:
             if self.config is None:
                 raise ValueError("No configuration loaded.")
             self.config[key] = value
 
     def __setitem__(self, key, value):
@@ -132,22 +152,42 @@
     def save_config(self, file_path):
         if self.config is None:
             raise ValueError("No configuration loaded.")
         with open(file_path, "w") as f:
             yaml.dump(self.config, f)
 
 
+class BindingInstaller:
+    def __init__(self, config: BindingConfig) -> None:
+        self.config = config
+
 class LLMBinding:
    
     file_extension='*.bin'
     binding_path = Path(__file__).parent
     def __init__(self, config:BindingConfig, inline:bool) -> None:
         self.config = config
         self.inline = inline
 
+    def load_config_file(self, path):
+        """
+        Load the content of config_local.yaml file.
+
+        The function reads the content of the config_local.yaml file and returns it as a Python dictionary.
+
+        Args:
+            None
+
+        Returns:
+            dict: A dictionary containing the loaded data from the config_local.yaml file.
+        """     
+        with open(path, 'r') as file:
+            data = yaml.safe_load(file)
+        return data
+
 
     def generate(self, 
                  prompt:str,                  
                  n_predict: int = 128,
                  callback: Callable[[str], None] = None,
                  verbose: bool = False,
                  **gpt_params ):
```

### Comparing `lollms-1.0.3/lollms/langchain_integration.py` & `lollms-1.1.0/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-1.0.3/lollms/server.py` & `lollms-1.1.0/lollms/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from flask import Flask, render_template, request
 from flask_socketio import SocketIO, emit
 from flask_cors import CORS
-from pyaipersonality import AIPersonality, MSG_TYPE
-from pyaipersonality.binding import BindingConfig
+from lollms import AIPersonality, MSG_TYPE
+from lollms.binding import BindingConfig
 import importlib
 from pathlib import Path
 import argparse
 import logging
+import shutil
+
 
 # Reset
 color_reset = '\u001b[0m'
 
 # Regular colors
 color_black = '\u001b[30m'
 color_red = '\u001b[31m'
@@ -26,164 +28,192 @@
 color_bright_red = '\u001b[31;1m'
 color_bright_green = '\u001b[32;1m'
 color_bright_yellow = '\u001b[33;1m'
 color_bright_blue = '\u001b[34;1m'
 color_bright_magenta = '\u001b[35;1m'
 color_bright_cyan = '\u001b[36;1m'
 color_bright_white = '\u001b[37;1m'
-# Store connected clients
-clients = {}
-models = []
-personalities = {}
-answer = ['']
-
-def build_model(bindings_path:Path, cfg: BindingConfig):
-    binding_path = Path(bindings_path)/cfg["binding"]
-    # first find out if there is a requirements.txt file
-    install_file_name="install.py"
-    install_script_path = binding_path / install_file_name        
-    if install_script_path.exists():
-        module_name = install_file_name[:-3]  # Remove the ".py" extension
-        module_spec = importlib.util.spec_from_file_location(module_name, str(install_script_path))
-        module = importlib.util.module_from_spec(module_spec)
-        module_spec.loader.exec_module(module)
-        if hasattr(module, "Install"):
-            module.Install(None)
-    # define the full absolute path to the module
-    absolute_path = binding_path.resolve()            
-    # infer the module name from the file path
-    module_name = binding_path.stem    
-    # use importlib to load the module from the file path
-    loader = importlib.machinery.SourceFileLoader(module_name, str(absolute_path/"__init__.py"))
-    binding_module = loader.load_module()
-    binding_class = getattr(binding_module, binding_module.binding_name)
-
-    model = binding_class(cfg)
-    return model
-
-app = Flask("AIPersonality_Server")
-app.config['SECRET_KEY'] = 'your-secret-key'
-CORS(app)  # Enable CORS for all routes
-socketio = SocketIO(app)
-
-# Set log level to warning
-app.logger.setLevel(logging.WARNING)
-# Configure a custom logger for Flask-SocketIO
-socketio_log = logging.getLogger('socketio')
-socketio_log.setLevel(logging.WARNING)
-socketio_log.addHandler(logging.StreamHandler())
-
-
-@socketio.on('connect')
-def handle_connect():
-    client_id = request.sid
-    clients[client_id] = {"namespace":request.namespace,"full_discussion_blocks":[]}
-    print(f'Client connected with session ID: {client_id}')
-
-@socketio.on('disconnect')
-def handle_disconnect():
-    client_id = request.sid
-    if client_id in clients:
-        del clients[client_id]
-    print(f'Client disconnected with session ID: {client_id}')
-
-@socketio.on('list_personalities')
-def handle_list_personalities():
-    personality_names = list(personalities.keys())
-    emit('personalities_list', {'personalities': personality_names}, room=request.sid)
-
-@socketio.on('add_personality')
-def handle_add_personality(data):
-    personality_path = data['path']
-    try:
-        personality = AIPersonality(personality_path)
-        personalities[personality.name] = personality
-        emit('personality_added', {'name': personality.name}, room=request.sid)
-    except Exception as e:
-        error_message = str(e)
-        emit('personality_add_failed', {'error': error_message}, room=request.sid)
-
-
-@socketio.on('generate_text')
-def handle_generate_text(data):
-    model = models[0]
-    client_id = request.sid
-    prompt = data['prompt']
-    personality:AIPersonality = personalities[data['personality']]
-    # Placeholder code for text generation
-    # Replace this with your actual text generation logic
-    print(f"Text generation requested by client :{client_id}")
-
-    answer[0]=''
-    full_discussion_blocks = clients[client_id]["full_discussion_blocks"]
-    def callback(text, messsage_type:MSG_TYPE):
-        if messsage_type==MSG_TYPE.MSG_TYPE_CHUNK:
-            answer[0]  = answer[0] + text
-            emit('text_chunk', {'chunk': text}, room=client_id)
-        return True
-    
-    if personality.processor is not None and personality.processor_cfg["process_model_input"]:
-        preprocessed_prompt = personality.processor.process_model_input(prompt)
-    else:
-        preprocessed_prompt = prompt
-        
-    full_discussion_blocks.append(personality.user_message_prefix)
-    full_discussion_blocks.append(preprocessed_prompt)
-    full_discussion_blocks.append(personality.link_text)
-    full_discussion_blocks.append(personality.ai_message_prefix)
-        
-    full_discussion = personality.personality_conditioning + ''.join(full_discussion_blocks)
-    
-    print(f"---------------- Input prompt -------------------")
-    print(f"{color_green}{full_discussion}")
-    print(f"{color_reset}--------------------------------------------")
-    if personality.processor is not None and personality.processor_cfg["custom_workflow"]:
-        print("processing...",end="",flush=True)
-        generated_text = personality.processor.run_workflow(prompt, full_discussion, callback=callback)
-    else:
-        print("generating...",end="",flush=True)
-        generated_text = model.generate(full_discussion, n_predict=personality.model_n_predicts, callback=callback)
-    full_discussion_blocks.append(generated_text)
-    print(f"{color_green}ok{color_reset}",end="",flush=True)    
-
-    
-    # Emit the generated text to the client
-    emit('text_generated', {'text': generated_text}, room=client_id)
-
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('--host', '-hst', default="localhost", help='Host name')
-    parser.add_argument('--port', '-prt', default="9600", help='Port number')
-    parser.add_argument('--config', '-cfg', default="configs/config.yaml", help='Path to the configuration file')
-    parser.add_argument('--bindings_path', '-bp', default="bindings_zoo", help='Binding path')
-    parser.add_argument('--binding', '-b', default=None, help='Binding value')
-    parser.add_argument('--personalities', '-p', nargs='+', default=[], help='A list of path to the personalites folders')
-    parser.add_argument('--model_name', '-m', default="Manticore-13B.ggmlv3.q4_0.bin", help='Model name')
-    args = parser.parse_args()
-    path = Path(args.config)
-
-    print("█       █        █       █▄  ▄█▄  ▄█")
-    print("█       █        █       █ ▀▀   ▀▀ █")
-    print("█       █        █       █         █")
-    print("█▄▄▄▄   █▄▄▄▄▄   █▄▄▄▄   █         █")
-    if path.exists():
-        cfg = BindingConfig(args.config)
-    else:
-        cfg = BindingConfig()
-
-    if args.binding:
-        cfg.binding = args.binding
-
-    if args.model_name:
-        cfg.model = args.model_name
-    model = build_model(args.bindings_path, cfg)
-    models.append(model)
-
-    personalities["default_personality"]=AIPersonality()
-    for p in args.personalities:
-        personality = AIPersonality(p)
-        personalities[personality.name] = personality
-    print("running...")
-    socketio.run(app, host=args.host, port=args.port)
+
+
+
+class LoLLMsServer:
+    def __init__(self):
+        self.app = Flask("LoLLMsServer_Server")
+        self.app.config['SECRET_KEY'] = 'your-secret-key'
+        CORS(self.app)  # Enable CORS for all routes
+        self.socketio = SocketIO(self.app)
+        self.clients = {}
+        self.models = []
+        self.personalities = {}
+        self.answer = ['']
+
+        # Set log level to warning
+        self.app.logger.setLevel(logging.WARNING)
+        # Configure a custom logger for Flask-SocketIO
+        self.socketio_log = logging.getLogger('socketio')
+        self.socketio_log.setLevel(logging.WARNING)
+        self.socketio_log.addHandler(logging.StreamHandler())
+
+        self.initialize_routes()
+
+    def initialize_routes(self):
+        @self.socketio.on('connect')
+        def handle_connect():
+            client_id = request.sid
+            self.clients[client_id] = {"namespace": request.namespace, "full_discussion_blocks": []}
+            print(f'Client connected with session ID: {client_id}')
+
+        @self.socketio.on('disconnect')
+        def handle_disconnect():
+            client_id = request.sid
+            if client_id in self.clients:
+                del self.clients[client_id]
+            print(f'Client disconnected with session ID: {client_id}')
+
+        @self.socketio.on('list_personalities')
+        def handle_list_personalities():
+            personality_names = list(self.personalities.keys())
+            emit('personalities_list', {'personalities': personality_names}, room=request.sid)
+
+        @self.socketio.on('add_personality')
+        def handle_add_personality(data):
+            personality_path = data['path']
+            try:
+                personality = AIPersonality(personality_path)
+                self.personalities[personality.name] = personality
+                emit('personality_added', {'name': personality.name}, room=request.sid)
+            except Exception as e:
+                error_message = str(e)
+                emit('personality_add_failed', {'error': error_message}, room=request.sid)
+
+        @self.socketio.on('generate_text')
+        def handle_generate_text(data):
+            model = self.models[0]
+            client_id = request.sid
+            prompt = data['prompt']
+            personality: AIPersonality = self.personalities[data['personality']]
+            # Placeholder code for text generation
+            # Replace this with your actual text generation logic
+            print(f"Text generation requested by client: {client_id}")
+
+            self.answer[0] = ''
+            full_discussion_blocks = self.clients[client_id]["full_discussion_blocks"]
+
+            def callback(text, message_type: MSG_TYPE):
+                if message_type == MSG_TYPE.MSG_TYPE_CHUNK:
+                    self.answer[0] = self.answer[0] + text
+                    emit('text_chunk', {'chunk': text}, room=client_id)
+                return True
+
+            if personality.processor is not None and personality.processor_cfg["process_model_input"]:
+                preprocessed_prompt = personality.processor.process_model_input(prompt)
+            else:
+                preprocessed_prompt = prompt
+
+            full_discussion_blocks.append(personality.user_message_prefix)
+            full_discussion_blocks.append(preprocessed_prompt)
+            full_discussion_blocks.append(personality.link_text)
+            full_discussion_blocks.append(personality.ai_message_prefix)
+
+            full_discussion = personality.personality_conditioning + ''.join(full_discussion_blocks)
+
+            print(f"---------------- Input prompt -------------------")
+            print(f"{color_green}{full_discussion}")
+            print(f"{color_reset}--------------------------------------------")
+            if personality.processor is not None and personality.processor_cfg["custom_workflow"]:
+                print("processing...", end="", flush=True)
+                generated_text = personality.processor.run_workflow(prompt, full_discussion, callback=callback)
+            else:
+                print("generating...", end="", flush=True)
+                generated_text = model.generate(full_discussion, n_predict=personality.model_n_predicts,
+                                                callback=callback)
+            full_discussion_blocks.append(generated_text)
+            print(f"{color_green}ok{color_reset}", end="", flush=True)
+
+            # Emit the generated text to the client
+            emit('text_generated', {'text': generated_text}, room=client_id)
+
+    def build_model(self, bindings_path: Path, cfg: BindingConfig):
+        binding_path = Path(bindings_path) / cfg["binding_name"]
+        # first find out if there is a requirements.txt file
+        install_file_name = "install.py"
+        install_script_path = binding_path / install_file_name
+        if install_script_path.exists():
+            module_name = install_file_name[:-3]  # Remove the ".py" extension
+            module_spec = importlib.util.spec_from_file_location(module_name, str(install_script_path))
+            module = importlib.util.module_from_spec(module_spec)
+            module_spec.loader.exec_module(module)
+            if hasattr(module, "Install"):
+                module.Install(self.config)
+        # define the full absolute path to the module
+        absolute_path = binding_path.resolve()
+        # infer the module name from the file path
+        module_name = binding_path.stem
+        # use importlib to load the module from the file path
+        loader = importlib.machinery.SourceFileLoader(module_name, str(absolute_path / "__init__.py"))
+        binding_module = loader.load_module()
+        binding_class = getattr(binding_module, binding_module.binding_name)
+
+        model = binding_class(cfg)
+        return model
+
+    def run(self, host="localhost", port="9600"):
+        parser = argparse.ArgumentParser()
+        parser.add_argument('--host', '-hst', default=host, help='Host name')
+        parser.add_argument('--port', '-prt', default=port, help='Port number')
+
+        parser.add_argument('--config', '-cfg', default=None, help='Path to the configuration file')
+        parser.add_argument('--bindings_path', '-bp', default=str(Path(__file__).parent / "bindings_zoo"),
+                            help='The path to the Bindings folder')
+        parser.add_argument('--personalities_path', '-pp',
+                            default=str(Path(__file__).parent / "personalities_zoo"),
+                            help='The path to the personalities folder')
+        parser.add_argument('--models_path', '-mp', default=str(Path(__file__).parent / "models"),
+                            help='The path to the models folder')
+
+        parser.add_argument('--binding_name', '-b', default="llama_cpp_official",
+                            help='Binding to be used by default')
+        parser.add_argument('--model_name', '-m', default="Manticore-13B.ggmlv3.q4_0.bin",
+                            help='Model name')
+        parser.add_argument('--personality_full_name', '-p', default="personality",
+                            help='Personality path relative to the personalities folder (language/category/name)')
+
+        args = parser.parse_args()
+
+        if args.config is None:
+            original = Path(__file__).parent / "configs/config.yaml"
+            local = Path(__file__).parent / "configs/config_local.yaml"
+            if not local.exists():
+                shutil.copy(original, local)
+            cfg_path = local
+
+        print("█       █        █       █▄  ▄█▄  ▄█")
+        print("█       █        █       █ ▀▀   ▀▀ █")
+        print("█       █        █       █         █")
+        print("█▄▄▄▄   █▄▄▄▄▄   █▄▄▄▄   █         █")
+
+        if cfg_path.exists():
+            self.config = BindingConfig(cfg_path)
+        else:
+            self.config = BindingConfig()
+
+        if args.binding_name:
+            self.config.binding_name = args.binding_name
+
+        if args.model_name:
+            self.config.model_name = args.model_name
+
+        model = self.build_model(args.bindings_path, self.config)
+        self.models.append(model)
+
+        self.personalities["default_personality"] = AIPersonality()
+
+        for p in self.config.personalities:
+            personality = AIPersonality(self.config.personalities_path/p)
+            self.personalities[personality.name] = personality
+
+        print("running...")
+        self.socketio.run(self.app, host=args.host, port=args.port)
 
 if __name__ == '__main__':
-    main()
+    server = AIPersonalityServer()
+    server.run()
```

### Comparing `lollms-1.0.3/setup.py` & `lollms-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 requirements = read_requirements("requirements.txt")
 requirements_dev = read_requirements("requirements_dev.txt")
 
 setuptools.setup(
     name="lollms",
-    version="1.0.3",
+    version="1.1.0",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

