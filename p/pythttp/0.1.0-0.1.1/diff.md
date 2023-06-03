# Comparing `tmp/pythttp-0.1.0.tar.gz` & `tmp/pythttp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.1.0.tar", last modified: Wed May 31 11:00:27 2023, max compression
+gzip compressed data, was "pythttp-0.1.1.tar", last modified: Sat Jun  3 23:41:43 2023, max compression
```

## Comparing `pythttp-0.1.0.tar` & `pythttp-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 11:00:27.348911 pythttp-0.1.0/
--rw-rw-rw-   0        0        0     1093 2023-05-31 11:00:27.348911 pythttp-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.0/README.md
--rw-rw-rw-   0        0        0      419 2023-05-31 11:00:25.000000 pythttp-0.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-31 11:00:27.327837 pythttp-0.1.0/pythttp/
--rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.1.0/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     3282 2023-05-31 10:51:06.000000 pythttp-0.1.0/pythttp/Protocol.py
--rw-rw-rw-   0        0        0     3885 2023-05-31 11:00:03.000000 pythttp-0.1.0/pythttp/RequestHandler.py
--rw-rw-rw-   0        0        0     2732 2023-05-31 10:59:28.000000 pythttp-0.1.0/pythttp/Structure.py
--rw-rw-rw-   0        0        0     3037 2023-05-30 15:45:28.000000 pythttp-0.1.0/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      139 2023-05-31 09:28:19.000000 pythttp-0.1.0/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 11:00:27.346906 pythttp-0.1.0/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-05-31 11:00:27.000000 pythttp-0.1.0/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-31 11:00:27.000000 pythttp-0.1.0/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 11:00:27.000000 pythttp-0.1.0/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 11:00:27.000000 pythttp-0.1.0/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 11:00:27.349911 pythttp-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-05-31 11:00:18.000000 pythttp-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:41:43.928562 pythttp-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2023-06-03 23:41:43.927586 pythttp-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.1.1/README.md
+-rw-rw-rw-   0        0        0      419 2023-06-03 23:41:39.000000 pythttp-0.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-03 23:41:43.911836 pythttp-0.1.1/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.1.1/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     3391 2023-06-03 23:41:07.000000 pythttp-0.1.1/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0    10102 2023-06-03 23:41:07.000000 pythttp-0.1.1/pythttp/RequestHandler.py
+-rw-rw-rw-   0        0        0     2936 2023-06-03 23:41:05.000000 pythttp-0.1.1/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3064 2023-06-03 23:41:04.000000 pythttp-0.1.1/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      139 2023-05-31 09:28:19.000000 pythttp-0.1.1/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:41:43.926610 pythttp-0.1.1/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-06-03 23:41:43.000000 pythttp-0.1.1/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-03 23:41:43.000000 pythttp-0.1.1/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 23:41:43.000000 pythttp-0.1.1/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 23:41:43.000000 pythttp-0.1.1/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 23:41:43.928562 pythttp-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-06-03 23:41:36.000000 pythttp-0.1.1/setup.py
```

### Comparing `pythttp-0.1.0/PKG-INFO` & `pythttp-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.0/README.md` & `pythttp-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.0/pythttp/Log_Manager.py` & `pythttp-0.1.1/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.1.0/pythttp/Protocol.py` & `pythttp-0.1.1/pythttp/Protocol.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import socket
+import select
 from urllib import request
 from urllib import parse
 from .Thread_Manager import *
 from .Structure import *
 from .Log_Manager import *
 
 class HyperTextTransferProtocol:
@@ -34,43 +35,49 @@
         self.s.listen(limit)
 
     def AcceptConnection(self):
         self.c, self.addr = self.s.accept()
         self.log(msg=f"[Connected with] ==> \033[32m{self.addr}\033[0m")
         return self.c, self.addr
     
-    def Receive(self,socket=None, addres=None, max_recv_size=1):
+    def Receive(self, socket=None, address=None, max_recv_size=1):
         received_data = b''
-        header_list=list()
+        header_list = []
+        sokt=self.c
+        if socket is not None:
+            sokt= socket[0]
         while b'\r\n\r\n' not in received_data:
-            if socket is None:
-                received_data += self.c.recv(max_recv_size)
-            received_data += socket[0].recv(max_recv_size)
-            header_list=parse.unquote(received_data).split('\r\n')
+            received_data += sokt.recv(max_recv_size)
+        header_list = parse.unquote(received_data).split('\r\n')
         if 'POST' in header_list[0]:
-            post_header=self.Receive(socket,addres)[1]
-            post_body=b''
-            for count in range(int(self.ExtractPostBodySize(header_list)/2048)):
-                post_body+=socket[0].recv(2048)
-            return 'POST',post_header,post_body
-        self.log(msg=f'[{parse.unquote(header_list[0])} request from] ==> \033[33m{addres}\033[0m')
-        return 'GET',header_list
+            post_body = b''
+            max_buf_size = self.ExtractPostBodySize(header_list)
+            buf_size = 2048
+            while True:
+                post_body += socket[0].recv(buf_size)
+                if max_buf_size == len(post_body):
+                    break
+                buf_size = buf_size * 2
+            return 'Body', post_body
+        self.log(msg=f"[{parse.unquote(header_list[0])} request from] ==> \033[33m{address}\033[0m")
+        return 'Header', header_list
     
+
     def ExtractPostBodySize(self, header):
         content_length_header = next((header for header in header if 'Content-Length' in header), None)
         if content_length_header:
             content_length_str = ''.join(filter(str.isdigit, content_length_header))
             return int(content_length_str)
         return 0
 
     def AssignUserThread(self,socket_and_addres):
         thread_name,thread = self.Thread.ThreadConstructor(target=self.Receive,args=socket_and_addres)
         self.Thread.USERS.append(socket_and_addres[1])
         self.Thread.USERS_COUNT+=1
-        self.Thread.SESSIONS[thread_name]=socket_and_addres[1]
+        self.Thread.ThreadSessions[thread_name]=socket_and_addres[1]
         self.Thread.user_socket_dict[socket_and_addres[1]]=socket_and_addres[0]
         return thread_name,thread
 
     def SendResponse(self,query,socket_and_addres):
         addr = f'\033[31m{socket_and_addres[1]}\033[0m'
         socket_and_addres[0][0].send(query)
         socket_and_addres[0][0].close()
```

### Comparing `pythttp-0.1.0/pythttp/Structure.py` & `pythttp-0.1.1/pythttp/Structure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import datetime as dt
+from dataclasses import dataclass, field
 import pickle
 
-class DBManager:
-    def __init__(self) -> None:
-        self.ServerDB={}
-
-    def SaveDB(self):
-        with open('ServerDB.DB','wb') as WDB:
-            pickle.dump(self.ServerDB,WDB)
-        return 'Done'
+
+
+@dataclass
+class StructDB:
+    UserUID: str
+    UserName: str
+    UserPw: str
+    UserEmail: str = None
+    UserUploadFiles: dict =field(default_factory=dict)
+    StructDBdict: dict =field(init=False,default_factory=dict)
+    def __post_init__(self):
+        self.StructDBdict['UserUID'] = self.UserUID
+        self.StructDBdict['UserName'] = self.UserName
+        self.StructDBdict['UserPw'] = self.UserPw
+        self.StructDBdict['UserEmail'] = self.UserEmail
+        self.StructDBdict['UserUploadFiles'] = self.UserUploadFiles
+
+class DBManger:
     
-    def loadDB(self):
-        with open('ServerDB.DB','rb') as RDB:
-            self.ServerDB=pickle.load(RDB)
-        return 'Done'
-
-    def CreatDB(self):
-        with open('ServerDB.DB','ab') as CDB:
-            pickle.dump(self.ServerDB,CDB)
-        return 'Done'
+    def PASS(self):
+        pass
+
+
 
 class PrepareHeader:
     def __init__(self, user_agent='127.0.0.1', body=None):
         self.body = body
         self.status_code="HTTP/1.1 200 OK"
         self.string_header = self.status_code + '\r\n'
         self.default_header = {}
@@ -40,21 +46,22 @@
         }
         if params:
             url += '?' + '&'.join([f'{key}={value}' for key, value in params.items()])
         return f'{method} {url} HTTP/1.1\r\n' + \
                '\r\n'.join([f'{key}: {value}' for key, value in headers.items()]) + \
                '\r\n\r\n'
 
-    def _response_headers(self,status_code,Content):
+    def _response_headers(self,status_code,Content,Cookie=None):
         headers = {
             'Date': HttpDateTime().http_date_time,
             'Server':'longinus',
             'Cache-Control': 'no-store, no-cache, must-revalidate, post-check=0, pre-check=0',
             'Pragma' : 'no-cache',
-            'Content-Length': len(Content)
+            'Content-Length': len(Content),
+            'Set-Cookie' : Cookie
         }
         return (f'HTTP/1.1 {status_code}\r\n' + \
         '\r\n'.join([f'{key}: {value}' for key, value in headers.items()]) + \
         '\r\n\r\n').encode()
 
 class HttpDateTime:
     def __init__(self):
```

### Comparing `pythttp-0.1.0/pythttp/Thread_Manager.py` & `pythttp-0.1.1/pythttp/Thread_Manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,64 +12,63 @@
 
     def run(self):
         self.result = self.target(*self.args)
 
 class Thread_DataManager:
     def __init__(self) -> None:
         self.USERS=[]
-        self.SESSIONS={}
+        self.ThreadSessions={}
         self.USERS_COUNT=0
         self.user_socket_dict={}
 
 class Thread:
     def __init__(self):
         self.ACTIVATED_THREADS={}
         self.USERS=Thread_DataManager().USERS
-        self.SESSIONS=Thread_DataManager().SESSIONS
+        self.ThreadSessions=Thread_DataManager().ThreadSessions
         self.USERS_COUNT=Thread_DataManager().USERS_COUNT
         self.user_socket_dict=Thread_DataManager().user_socket_dict
         self.THREADS_COUNT=0
         self.stopped_threads={}
         self.finished_users=[]
         self.log=Log().logging
 
     def display_variables(self):
         LIST_VARIABLES=f'''
-                            'SESSIONS':{self.SESSIONS},
+                            'SESSIONS':{self.ThreadSessions},
                             'USERS':{self.USERS},
                             'USERS_COUNT':{self.USERS_COUNT},
                             'ACTIVATED_THREADS':{self.ACTIVATED_THREADS},
                             'THREADS_COUNT':{self.THREADS_COUNT}
                             'user_thread_result_dict':{self.user_thread_result_dict}
                             'user_socket_dict':{self.user_socket_dict}
                             'stopped_threads':{self.stopped_threads}
                             'finished_users':{self.finished_users}
                         '''
         print(LIST_VARIABLES)
-
     def ThreadConstructor(self, target, args=(), daemon=False):
         thread_mutex=0
         while True:
             new_thread_name='THREAD_{}_{}'.format(target.__name__,thread_mutex)
             self.THREADS_COUNT+=1
             if new_thread_name not in self.ACTIVATED_THREADS.keys():
                 globals()[new_thread_name] = THREAD_PRESET(target=target,args=args,daemon=daemon)
                 new_thread=globals()[new_thread_name]
                 self.ACTIVATED_THREADS[new_thread_name]=new_thread
                 return new_thread_name,new_thread
             else:
                 thread_mutex+=1
 
-    def SessionDestructor(self,thread_name,user):
+    def ThreadDestructor(self,thread_name,user):
         thread=eval(thread_name)
         if (thread.is_alive()==False):
             del self.user_socket_dict[user]
             del self.finished_users[self.finished_users.index(user)]
             del self.USERS[self.USERS.index(user)]
-            del self.SESSIONS[thread_name]
+            del self.ThreadSessions[thread_name]
             self.USERS_COUNT-=1
         self.THREADS_COUNT-=1
 
     def find_stopped_thread(self):
         for activated_thread_name,thread in self.ACTIVATED_THREADS.copy().items():
             if 'stopped' in str(thread) :
                 del self.ACTIVATED_THREADS[activated_thread_name]
```

### Comparing `pythttp-0.1.0/pythttp.egg-info/PKG-INFO` & `pythttp-0.1.1/pythttp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.1.0/setup.py` & `pythttp-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.1.0",
+    version="0.1.1",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=[],
```

