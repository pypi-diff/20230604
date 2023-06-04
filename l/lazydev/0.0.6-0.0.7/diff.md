# Comparing `tmp/lazydev-0.0.6.tar.gz` & `tmp/lazydev-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazydev-0.0.6.tar", last modified: Fri Jun  2 22:13:42 2023, max compression
+gzip compressed data, was "lazydev-0.0.7.tar", last modified: Sun Jun  4 17:58:33 2023, max compression
```

## Comparing `lazydev-0.0.6.tar` & `lazydev-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 22:13:42.192264 lazydev-0.0.6/
--rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.6/LICENSE
--rw-r--r--   0 anirbankar   (501) staff       (20)     4559 2023-06-02 22:13:42.192111 lazydev-0.0.6/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)     3889 2023-06-02 22:13:23.000000 lazydev-0.0.6/README.md
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 22:13:42.189807 lazydev-0.0.6/lazydev/
--rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.6/lazydev/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1280 2023-06-02 20:51:59.000000 lazydev-0.0.6/lazydev/develop.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 22:13:42.191686 lazydev-0.0.6/lazydev/modules/
--rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.6/lazydev/modules/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     6177 2023-06-02 22:08:19.000000 lazydev-0.0.6/lazydev/modules/developer.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     4556 2023-06-02 21:07:12.000000 lazydev-0.0.6/lazydev/modules/prompts.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1679 2023-06-02 11:49:48.000000 lazydev-0.0.6/lazydev/modules/utils.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 22:13:42.190755 lazydev-0.0.6/lazydev.egg-info/
--rw-r--r--   0 anirbankar   (501) staff       (20)     4559 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/SOURCES.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/dependency_links.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/entry_points.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/requires.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/top_level.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-02 22:13:42.192303 lazydev-0.0.6/setup.cfg
--rw-r--r--   0 anirbankar   (501) staff       (20)     1478 2023-06-02 22:09:23.000000 lazydev-0.0.6/setup.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-04 17:58:33.652992 lazydev-0.0.7/
+-rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.7/LICENSE
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4553 2023-06-04 17:58:33.652843 lazydev-0.0.7/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)     3883 2023-06-03 08:10:06.000000 lazydev-0.0.7/README.md
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-04 17:58:33.650654 lazydev-0.0.7/lazydev/
+-rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.7/lazydev/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1280 2023-06-02 20:51:59.000000 lazydev-0.0.7/lazydev/develop.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-04 17:58:33.652532 lazydev-0.0.7/lazydev/modules/
+-rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.7/lazydev/modules/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     7279 2023-06-04 17:01:33.000000 lazydev-0.0.7/lazydev/modules/developer.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     6118 2023-06-04 08:58:14.000000 lazydev-0.0.7/lazydev/modules/prompts.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1807 2023-06-04 16:51:17.000000 lazydev-0.0.7/lazydev/modules/utils.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-04 17:58:33.651639 lazydev-0.0.7/lazydev.egg-info/
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4553 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/SOURCES.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/dependency_links.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/entry_points.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/requires.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-04 17:58:33.000000 lazydev-0.0.7/lazydev.egg-info/top_level.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-04 17:58:33.653034 lazydev-0.0.7/setup.cfg
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1482 2023-06-04 17:58:23.000000 lazydev-0.0.7/setup.py
```

### Comparing `lazydev-0.0.6/LICENSE` & `lazydev-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.6/PKG-INFO` & `lazydev-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.6
+Version: 0.0.7
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 Lazyness is the mother of invention 😉
 ```
 
 LazyDev is a Python module that utilizes GPT models to create entire coding projects for you. With just a few simple commands, LazyDev can generate a project file tree, write the necessary code, and even test the project for you. Say goodbye to the hassle of setting up projects from scratch and let LazyDev do the heavy lifting for you.
 
 ## Features
 
-- **Effortless project initialization**: Simply use the `python -m lazydev.develop -r <what you want to do>` command to kickstart the project generation process.
+- **Effortless project initialization**: Simply use the `lazydev develop -r "I want to develop a game"` command to kickstart the project generation process.
 - **Interactive question-based approach**: LazyDev asks relevant questions to gather essential information before starting the coding process, ensuring that the generated project meets your specific requirements.
 - **Complete project planning**: LazyDev plans the entire project structure based on the gathered information, setting up the necessary directories and files for you.
 - **Automated code generation**: The module automatically generates the code based on the project plan, saving you time and effort.
 - **Built-in testing functionality**: LazyDev even includes an automated testing phase to ensure that the generated code performs as expected.
 
 ## Installation
 
@@ -89,14 +89,14 @@
 
 This project is licensed under the Apache-2.0 License. See the [LICENSE](https://github.com/thecodacus/lazy-dev/blob/master/LICENSE) file for more details.
 
 ## Acknowledgements
 
 LazyDev was inspired by the desire to automate the initial setup and coding process for various projects. The underlying GPT models used in this module were developed by OpenAI.
 
-It is inspired by the project [smol-ai/developer](https://github.com/smol-ai/developer), and the principle `Build the thing that builds all the things.`
+It is inspired by the project [smol-ai/developer](https://github.com/smol-ai/developer), and the principle `Build the thing that builds all the things`
 
 ## Contact
 
 If you have any questions or suggestions, feel free to reach out to us at thecodacus@gmail.com.
 
 Happy coding with LazyDev!
```

### Comparing `lazydev-0.0.6/README.md` & `lazydev-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Lazyness is the mother of invention 😉
 ```
 
 LazyDev is a Python module that utilizes GPT models to create entire coding projects for you. With just a few simple commands, LazyDev can generate a project file tree, write the necessary code, and even test the project for you. Say goodbye to the hassle of setting up projects from scratch and let LazyDev do the heavy lifting for you.
 
 ## Features
 
-- **Effortless project initialization**: Simply use the `python -m lazydev.develop -r <what you want to do>` command to kickstart the project generation process.
+- **Effortless project initialization**: Simply use the `lazydev develop -r "I want to develop a game"` command to kickstart the project generation process.
 - **Interactive question-based approach**: LazyDev asks relevant questions to gather essential information before starting the coding process, ensuring that the generated project meets your specific requirements.
 - **Complete project planning**: LazyDev plans the entire project structure based on the gathered information, setting up the necessary directories and files for you.
 - **Automated code generation**: The module automatically generates the code based on the project plan, saving you time and effort.
 - **Built-in testing functionality**: LazyDev even includes an automated testing phase to ensure that the generated code performs as expected.
 
 ## Installation
 
@@ -71,14 +71,14 @@
 
 This project is licensed under the Apache-2.0 License. See the [LICENSE](https://github.com/thecodacus/lazy-dev/blob/master/LICENSE) file for more details.
 
 ## Acknowledgements
 
 LazyDev was inspired by the desire to automate the initial setup and coding process for various projects. The underlying GPT models used in this module were developed by OpenAI.
 
-It is inspired by the project [smol-ai/developer](https://github.com/smol-ai/developer), and the principle `Build the thing that builds all the things.`
+It is inspired by the project [smol-ai/developer](https://github.com/smol-ai/developer), and the principle `Build the thing that builds all the things`
 
 ## Contact
 
 If you have any questions or suggestions, feel free to reach out to us at thecodacus@gmail.com.
 
 Happy coding with LazyDev!
```

### Comparing `lazydev-0.0.6/lazydev/develop.py` & `lazydev-0.0.7/lazydev/develop.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.6/lazydev/modules/developer.py` & `lazydev-0.0.7/lazydev/modules/developer.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,159 +17,179 @@
     SystemMessage
 )
 
 import json
 
 from .utils import Utilities
 
+
 class Developer():
-    def __init__(self, requirement:str,root_dir:str, openai_api_key:str,model:str):
-        self.requirement=requirement
-        self.root_dir=root_dir
-        self.api_key=openai_api_key
-        self.files_written=[]
+    def __init__(self, requirement: str, root_dir: str, openai_api_key: str, model: str):
+        self.requirement = requirement
+        self.root_dir = root_dir
+        self.api_key = openai_api_key
+        self.files_written = []
         self.brain = ChatOpenAI(
             model=model,
             openai_api_key=self.api_key,
             temperature=0.1,
             streaming=False
-            )
-    
+        )
 
-    def brain_storm(self,prompt:str,step_name="prompt")->str:
+    def brain_storm(self, prompt: str, step_name="prompt") -> str:
         messages = [
             SystemMessage(content="you are a senior software developer"),
             HumanMessage(content=prompt)
         ]
-        aiMessage:AIMessage= self.brain(messages=messages)
+        aiMessage: AIMessage = self.brain(messages=messages)
         if not os.path.exists("./thoughts"):
             os.makedirs("./thoughts")
         if os.path.exists(f"./thoughts/{step_name}.md"):
             os.remove(f"./thoughts/{step_name}.md")
-        Utilities.write_to_file(f"{prompt}\n\n{aiMessage.content}",f"./thoughts/{step_name}.md")
+        Utilities.write_to_file(
+            f"{prompt}\n\n{aiMessage.content}", f"./thoughts/{step_name}.md")
         return aiMessage.content
-    
+
     def get_doubts(self):
-        prompt=PromptBook.expand_requirements(self.requirement)
-        doubts=self.brain_storm(prompt,'clear-doubts')
-        doubt_list:List[str]=doubts.split("\n")
-        doubt_list=[doubt.strip() for doubt in doubt_list if doubt.strip()!=""]
+        prompt = PromptBook.expand_requirements(self.requirement)
+        doubts = self.brain_storm(prompt, 'clear-doubts')
+        doubt_list: List[str] = doubts.split("\n")
+        doubt_list = [doubt.strip()
+                      for doubt in doubt_list if doubt.strip() != ""]
         return doubt_list
-    
-    def get_clarifications(self,doubts:List[str],answers:List[str]):
-        clarifications=""
+
+    def get_clarifications(self, doubts: List[str], answers: List[str]):
+        clarifications = ""
         for i in range(len(doubts)):
-            clarifications=f"{clarifications}\n\n{i+1}. {doubts[i]}\n Ans: {answers[i]}"
-        self.clarifications=clarifications
+            clarifications = f"{clarifications}\n\n{i+1}. {doubts[i]}\n Ans: {answers[i]}"
+        self.clarifications = clarifications
         return clarifications
-    
 
     def clear_doubts(self):
-        doubt_list=self.get_doubts()
+        doubt_list = self.get_doubts()
         print("""
 Hey there! 😄 It's Lazy Dev, your friendly neighborhood programmer, here to make your awesome project's dreams come true! 🎉 
 But before I dive into coding magic, I have a few fun and important questions for you. 
 So, grab a cup of coffee ☕️, sit back, and let's clarify some details, shall we? Here we go! 🚀
         """)
-        answer_list=[]
+        answer_list = []
         for doubt in doubt_list:
             answer = input(f"{doubt}\n>>")
             answer_list.append(answer)
 
         print("""
 Thats all I need! 😄
 
 Sit back and relax while I work my coding magic for you! ✨✨✨
 
 🚀 I've got this! 🎉
 
 Cheers! 👨‍💻
         """)
-        return doubt_list,answer_list
-    
+        return doubt_list, answer_list
+
     def plan_project(self):
-        prompt=PromptBook.plan_project(self.requirement,self.clarifications)
-        plannings:str=self.brain_storm(prompt,'plan-project')
-        self.plannings=plannings
+        prompt = PromptBook.plan_project(self.requirement, self.clarifications)
+        plannings: str = self.brain_storm(prompt, 'plan-project')
+        self.plannings = plannings
         return plannings
-    
+
     def generate_folder_structure(self):
-        prompt=PromptBook.design_folder_structure(
+        prompt = PromptBook.design_folder_structure(
             question=self.requirement,
             plan=self.plannings,
             clarifications=self.clarifications
-            )
-        retry_count=3
-        while retry_count>0:
+        )
+        retry_count = 3
+        while retry_count > 0:
             try:
 
-                folder_tree_str:str=self.brain_storm(prompt,"generate-filders")
-                folder_tree:dict=json.loads(folder_tree_str.strip().strip("`"))
+                folder_tree_str: str = self.brain_storm(
+                    prompt, "generate-filders")
+                folder_tree: dict = json.loads(
+                    folder_tree_str.strip().strip("`"))
                 break
             except:
                 print("Opps messed up the json format, let me try again")
-                retry_count=retry_count-1
-        
-        if retry_count==0:
+                retry_count = retry_count-1
+
+        if retry_count == 0:
             print("Sorry I was not able to create the folder structure in json correct format, check my instructions and try to refine it sothat i can understan the task better")
-            sys.exit()       
-        self.root_folder_name, self.file_paths = Utilities.generate_files_and_folders(structure=folder_tree,root_dir=self.root_dir)
+            sys.exit()
+        self.root_folder_name, self.file_paths = Utilities.generate_files_and_folders(
+            structure=folder_tree, root_dir=self.root_dir)
         return self.root_folder_name, self.file_paths
 
-
     def prioratize_files(self):
-        prompt=PromptBook.prioritise_file_list(self.file_paths)
-        retry_count=3
-        while retry_count>0:
+        prompt = PromptBook.prioritise_file_list(self.file_paths)
+        retry_count = 3
+        while retry_count > 0:
             try:
-                file_paths_str=self.brain_storm(prompt,'prioratize_files') 
+                file_paths_str = self.brain_storm(prompt, 'prioratize_files')
                 break
             except:
                 print("Opps messed up the json format, let me try again")
-                retry_count=retry_count-1
-        if retry_count==0:
+                retry_count = retry_count-1
+        if retry_count == 0:
             print("Sorry I was not able to create the file list in correct format, check my instructions and try to refine it sothat i can understan the task better")
-            sys.exit()       
-        self.file_paths=file_paths_str.split("\n")
+            sys.exit()
+        self.file_paths = file_paths_str.split("\n")
         return self.file_paths
-    
-    def write_file_content(self,file_path):
-        prompt=PromptBook.write_file(
+
+    def write_file_content(self, file_path, review_iteration: int = 1):
+        prompt = PromptBook.write_file(
             question=self.requirement,
             clarifications=self.clarifications,
             plan=self.plannings,
             files_written=self.files_written,
             file_path_to_write=file_path,
             file_paths=self.file_paths
-            )
-        code=self.brain_storm(prompt,f'code-{file_path.split("/")[-1]}') 
-        Utilities.write_to_file(code,file_path=file_path)
+        )
+        filename = file_path.split("/")[-1]
+        code = self.brain_storm(prompt, f'code-{filename}')
+        if (review_iteration > 1):
+            print(f"Reviewing the code {filename}")
+            for i in range(review_iteration-1):
+                review_prompt = PromptBook.get_code_feedback(
+                    draft=code,
+                    question=self.requirement,
+                    clarifications=self.clarifications,
+                    plan=self.plannings,
+                    files_written=self.files_written,
+                    file_path_to_write=file_path,
+                    file_paths=self.file_paths
+                )
+                response = self.brain_storm(
+                    review_prompt, f'code-{file_path.split("/")[-1]}')
+                response = response.strip('"\'`-\n')
+                if (response.strip('"\'`-\n') == "NONE"):
+                    break
+                code = response
+
+        Utilities.write_to_file(code, file_path=file_path)
         self.files_written.append((
             file_path,
             code
         ))
 
     def develop(self):
         # clearing all doubts
-        doubts,answers=self.clear_doubts()
-        self.clarifications=self.get_clarifications(doubts=doubts,answers=answers)
+        doubts, answers = self.clear_doubts()
+        self.clarifications = self.get_clarifications(
+            doubts=doubts, answers=answers)
         # planning the project
-        print("Planning...")
+        print("Brainstorming ideas...")
         self.plan_project()
         print(self.plannings)
         print("\n\n")
         # creating files and folders for the project
-        print("Creating files...")
-        self.generate_folder_structure()
+        print("Creating folder structure...")
+        root_folder_name, file_paths = self.generate_folder_structure()
+
         self.prioratize_files()
-        self.files_written=[]
+        self.files_written = []
         for file_path in self.file_paths:
-            file_name=file_path.split("/")[-1]
-            if(file_name.split(".")[-1] in ["png","jpg","jpeg","bimp"]):
+            file_name = file_path.split("/")[-1]
+            if (file_name.split(".")[-1] in ["png", "jpg", "jpeg", "bimp", "lock"]):
                 continue
             print(f"\nWriting Code for :{file_name}")
-            self.write_file_content(file_path)
-
-
-
-
-        
+            self.write_file_content(file_path, review_iteration=2)
```

### Comparing `lazydev-0.0.6/lazydev/modules/prompts.py` & `lazydev-0.0.7/lazydev/modules/prompts.py`

 * *Files 15% similar despite different names*

```diff
@@ -131,7 +131,50 @@
 * keep in mind there wont be any additional files other then the full files list given above, only use files that are mentioned in that list
 Begin!
 
 File:{file_path_to_write}
 Content:
 """
 
+    def get_code_feedback(draft:str,question,clarifications:str,plan:str,files_written:List[List[str]], file_path_to_write:str,file_paths:List[str])->str:
+        file_with_conent="\n\n".join([f"File:{file_path}\nContent:\n{content}" for file_path,content in files_written])
+        all_files_list="\n".join(file_paths)
+        return f"""
+you are a senior programmer below is what your client have asked you to do:
+---
+{question}
+---
+here are some clarrification on the requirements
+---
+{clarifications}
+---
+below is the what you have already planed what to do:
+---
+{plan}
+---
+Below are the full files list that already has been or will be written
+--
+{all_files_list}
+--
+
+you are now writing the code below are the files that already written with content as follows:
+---
+{file_with_conent}
+---
+
+now you are about to write content the following file:
+{file_path_to_write}
+
+below is one of the draft version of the code:
+---
+{draft}
+---
+
+your job is to find problems with the code and refine it. 
+
+As your response will go to an automated parser, things to keep in mind all the time:
+* if no refinement is required then just say NONE, and nothing else
+* only write the file content, no expiation, no pretext as this will directly go as code.
+* if the language support, add comments at steps, which expains what you are about to do, dont add comment if comment is not supported by the file type example json file
+* keep in mind there wont be any additional files other then the full files list given above, only use files that are mentioned in that list
+Begin!
+"""
```

### Comparing `lazydev-0.0.6/lazydev/modules/utils.py` & `lazydev-0.0.7/lazydev/modules/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 import os
 from typing import List, Dict
 
+
 class Utilities:
     @staticmethod
     def touch(path):
         with open(path, 'a'):
             os.utime(path, None)
 
     @staticmethod
-    def generate_files_recursively(files:List[Dict],cur_dir:str):
-        file_paths=[]
+    def generate_files_recursively(files: List[Dict], cur_dir: str):
+        file_paths = []
         for file in files:
-            name=file['name']
-            type=file['type']
-            item_path=os.path.join(cur_dir,name)
-            if type=="file":
+            name = file['name']
+            type = file['type']
+            item_path = os.path.join(cur_dir, name)
+            if type == "file":
                 Utilities.touch(item_path)
                 file_paths.append(item_path)
                 print(f"Created File: {item_path}")
             else:
                 if not os.path.exists(item_path):
                     os.makedirs(item_path)
                     print(f"Created Directory: {item_path}")
-                subfiles:List[Dict]=file['files']
-                sub_file_paths=Utilities.generate_files_recursively(subfiles,item_path)
-                file_paths=file_paths+sub_file_paths
+                if 'files' in file:
+                    subfiles: List[Dict] = file['files']
+                    sub_file_paths = Utilities.generate_files_recursively(
+                        subfiles, item_path)
+                    file_paths = file_paths+sub_file_paths
         return file_paths
 
     @staticmethod
-    def generate_files_and_folders(structure:dict,root_dir:str):
-        root_dir_name=structure['root_dir_name']
-        cur_dir=os.path.join(root_dir,root_dir_name)
-        root_dir_path=cur_dir
+    def generate_files_and_folders(structure: dict, root_dir: str):
+        root_dir_name = structure['root_dir_name']
+        cur_dir = os.path.join(root_dir, root_dir_name)
+        root_dir_path = cur_dir
         if not os.path.exists(cur_dir):
             os.makedirs(cur_dir)
             print(f"Created Directory: {cur_dir}")
-        files:List[Dict]=structure['files']
-        file_paths=Utilities.generate_files_recursively(files=files,cur_dir=cur_dir)
+        files: List[Dict] = structure['files']
+        file_paths = Utilities.generate_files_recursively(
+            files=files, cur_dir=cur_dir)
         return root_dir_path, file_paths
 
-    def write_to_file(content:str,file_path:str):
+    def write_to_file(content: str, file_path: str):
         # Open the file in write mode
         with open(file_path, "w") as file:
             # Write the content to the file
             file.write(content)
```

### Comparing `lazydev-0.0.6/lazydev.egg-info/PKG-INFO` & `lazydev-0.0.7/lazydev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.6
+Version: 0.0.7
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 Lazyness is the mother of invention 😉
 ```
 
 LazyDev is a Python module that utilizes GPT models to create entire coding projects for you. With just a few simple commands, LazyDev can generate a project file tree, write the necessary code, and even test the project for you. Say goodbye to the hassle of setting up projects from scratch and let LazyDev do the heavy lifting for you.
 
 ## Features
 
-- **Effortless project initialization**: Simply use the `python -m lazydev.develop -r <what you want to do>` command to kickstart the project generation process.
+- **Effortless project initialization**: Simply use the `lazydev develop -r "I want to develop a game"` command to kickstart the project generation process.
 - **Interactive question-based approach**: LazyDev asks relevant questions to gather essential information before starting the coding process, ensuring that the generated project meets your specific requirements.
 - **Complete project planning**: LazyDev plans the entire project structure based on the gathered information, setting up the necessary directories and files for you.
 - **Automated code generation**: The module automatically generates the code based on the project plan, saving you time and effort.
 - **Built-in testing functionality**: LazyDev even includes an automated testing phase to ensure that the generated code performs as expected.
 
 ## Installation
 
@@ -89,14 +89,14 @@
 
 This project is licensed under the Apache-2.0 License. See the [LICENSE](https://github.com/thecodacus/lazy-dev/blob/master/LICENSE) file for more details.
 
 ## Acknowledgements
 
 LazyDev was inspired by the desire to automate the initial setup and coding process for various projects. The underlying GPT models used in this module were developed by OpenAI.
 
-It is inspired by the project [smol-ai/developer](https://github.com/smol-ai/developer), and the principle `Build the thing that builds all the things.`
+It is inspired by the project [smol-ai/developer](https://github.com/smol-ai/developer), and the principle `Build the thing that builds all the things`
 
 ## Contact
 
 If you have any questions or suggestions, feel free to reach out to us at thecodacus@gmail.com.
 
 Happy coding with LazyDev!
```

### Comparing `lazydev-0.0.6/setup.py` & `lazydev-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name="lazydev",
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     install_requires=[
         "langchain>=0.0.188",
         "openai>=0.27.7"
     ],
     entry_points={
         'console_scripts': [
             'lazydev = lazydev:run',
         ],
     },
     author='Anirban Kat',
     author_email='thecodacus@gmail.com',
     description='AI developer for lazy programmer',
     long_description=readme,  # Assign the contents of README.md to long_description
-    long_description_content_type='text/markdown',  # Specify the type of long description
+    # Specify the type of long description
+    long_description_content_type='text/markdown',
     url='https://github.com/thecodacus/lazy-dev',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
@@ -40,8 +41,8 @@
     # },
 
     # # You can also specify additional non-package data files
     # data_files=[
     #     ('config', ['config.ini']),
     # ],
 
-)
+)
```

