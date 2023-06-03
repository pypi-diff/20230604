# Comparing `tmp/jiggybase-0.0.35.tar.gz` & `tmp/jiggybase-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.35.tar", last modified: Thu May 25 02:08:18 2023, max compression
+gzip compressed data, was "jiggybase-0.0.36.tar", last modified: Sat Jun  3 22:17:29 2023, max compression
```

## Comparing `jiggybase-0.0.35.tar` & `jiggybase-0.0.36.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.427770 jiggybase-0.0.35/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.35/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-25 02:08:18.427331 jiggybase-0.0.35/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.0.35/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.417723 jiggybase-0.0.35/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.35/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.0.35/jiggybase/chat_stream.py
--rw-r--r--   0 wsk        (501) staff       (20)     4078 2023-05-25 02:03:37.000000 jiggybase-0.0.35/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)    11142 2023-05-25 02:00:12.000000 jiggybase-0.0.35/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.420574 jiggybase-0.0.35/jiggybase/examples/
--rw-r--r--   0 wsk        (501) staff       (20)     1378 2023-05-15 15:42:51.000000 jiggybase-0.0.35/jiggybase/examples/chat_completion.py
--rw-r--r--   0 wsk        (501) staff       (20)      295 2023-05-25 02:00:08.000000 jiggybase-0.0.35/jiggybase/examples/chat_completion_stream.py
--rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.35/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.35/jiggybase/examples/upload_email_example.py
--rw-r--r--   0 wsk        (501) staff       (20)      449 2023-05-21 02:08:21.000000 jiggybase-0.0.35/jiggybase/ipython.py
--rwxr-xr-x   0 wsk        (501) staff       (20)      648 2023-05-21 02:24:20.000000 jiggybase-0.0.35/jiggybase/jiggybase_ipython.py
--rw-r--r--   0 wsk        (501) staff       (20)     5681 2023-05-25 01:30:49.000000 jiggybase-0.0.35/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.35/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.425932 jiggybase-0.0.35/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.35/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.35/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     2955 2023-05-25 00:41:27.000000 jiggybase-0.0.35/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.0.35/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.35/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.35/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.35/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.35/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.35/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     3206 2023-05-20 00:39:05.000000 jiggybase-0.0.35/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.35/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.35/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.35/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.35/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.35/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.419414 jiggybase-0.0.35/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     1050 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-25 02:08:18.000000 jiggybase-0.0.35/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-25 02:06:37.000000 jiggybase-0.0.35/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-25 02:08:18.427891 jiggybase-0.0.35/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-25 02:08:18.426801 jiggybase-0.0.35/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.35/test/test.py
--rw-r--r--   0 wsk        (501) staff       (20)    12115 2023-05-25 01:50:31.000000 jiggybase-0.0.35/test/test_extract_typed_completion.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.885012 jiggybase-0.0.36/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.36/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-06-03 22:17:29.884597 jiggybase-0.0.36/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6279 2023-05-15 02:51:01.000000 jiggybase-0.0.36/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.875492 jiggybase-0.0.36/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.36/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)      989 2023-05-15 14:54:50.000000 jiggybase-0.0.36/jiggybase/chat_stream.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4078 2023-05-25 02:03:37.000000 jiggybase-0.0.36/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)    11142 2023-05-25 02:00:12.000000 jiggybase-0.0.36/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.878914 jiggybase-0.0.36/jiggybase/examples/
+-rw-r--r--   0 wsk        (501) staff       (20)     1378 2023-05-15 15:42:51.000000 jiggybase-0.0.36/jiggybase/examples/chat_completion.py
+-rw-r--r--   0 wsk        (501) staff       (20)      295 2023-05-25 02:00:08.000000 jiggybase-0.0.36/jiggybase/examples/chat_completion_stream.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.36/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.36/jiggybase/examples/upload_email_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)      449 2023-05-21 02:08:21.000000 jiggybase-0.0.36/jiggybase/ipython.py
+-rwxr-xr-x   0 wsk        (501) staff       (20)      648 2023-05-21 02:24:20.000000 jiggybase-0.0.36/jiggybase/jiggybase_ipython.py
+-rw-r--r--   0 wsk        (501) staff       (20)     5681 2023-05-28 04:35:07.000000 jiggybase-0.0.36/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.36/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.883082 jiggybase-0.0.36/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.36/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.36/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2955 2023-05-25 00:41:27.000000 jiggybase-0.0.36/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-05-15 03:37:46.000000 jiggybase-0.0.36/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.36/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.36/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.36/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.36/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2845 2023-06-03 22:11:35.000000 jiggybase-0.0.36/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3206 2023-05-20 00:39:05.000000 jiggybase-0.0.36/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.36/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.36/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.36/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.36/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.36/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.877458 jiggybase-0.0.36/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     6813 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     1050 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       78 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-06-03 22:17:29.000000 jiggybase-0.0.36/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      752 2023-06-03 22:11:12.000000 jiggybase-0.0.36/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-06-03 22:17:29.885131 jiggybase-0.0.36/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-06-03 22:17:29.884029 jiggybase-0.0.36/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.36/test/test.py
+-rw-r--r--   0 wsk        (501) staff       (20)    12115 2023-05-25 01:50:31.000000 jiggybase-0.0.36/test/test_extract_typed_completion.py
```

### Comparing `jiggybase-0.0.35/LICENSE` & `jiggybase-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/PKG-INFO` & `jiggybase-0.0.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.35
+Version: 0.0.36
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.35/README.md` & `jiggybase-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/chat_stream.py` & `jiggybase-0.0.36/jiggybase/chat_stream.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/client.py` & `jiggybase-0.0.36/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/collection.py` & `jiggybase-0.0.36/jiggybase/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/examples/chat_completion.py` & `jiggybase-0.0.36/jiggybase/examples/chat_completion.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.0.36/jiggybase/examples/jiggybase_upload.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/examples/upload_email_example.py` & `jiggybase-0.0.36/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/jiggybase_ipython.py` & `jiggybase-0.0.36/jiggybase/jiggybase_ipython.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/jiggybase_session.py` & `jiggybase-0.0.36/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/login.py` & `jiggybase-0.0.36/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/models/auth.py` & `jiggybase-0.0.36/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/models/chat.py` & `jiggybase-0.0.36/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/models/chunk.py` & `jiggybase-0.0.36/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/models/collection.py` & `jiggybase-0.0.36/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/models/metadata.py` & `jiggybase-0.0.36/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/models/org.py` & `jiggybase-0.0.36/jiggybase/models/org.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,27 +16,34 @@
     description: Optional[str] = Field(default=None, description='Optional user supplied description.')
 
 class OrgPatchRequest(BaseModel):
     name:        Optional[str] = Field(max_length=39, description='Unique name for this org.')
     description: Optional[str] = Field(max_length=255, description='Optional user supplied description.')
 
 class OrgMemberPostRequest(BaseModel):
-    email:  EmailStr          = Field(description='The user_id of a member to invite to the org.')
-    role:        OrgRole      = Field(description='The users role in the org')
+    email:  EmailStr     = Field(description='The user_id of a member to invite to the org.')
+    role:   OrgRole      = Field(description='The users role in the org')
 
 class OrgMember(BaseModel):
     id:                  int      = Field(description="Unique membership id")
     name:                str      = Field(description="Member name")
-    email:               EmailStr  = Field(description="Member email")    
+    email:               EmailStr = Field(description="Member email")    
     created_at:          float    = Field(description='The epoch timestamp when the membership was created.')
     updated_at:          float    = Field(description='The epoch timestamp when the membership was updated.')
-    invited_by_name: str      = Field(description="The name that invited this member to the org.")
-    role:                OrgRole = Field(description="The user's role in the org")
+    invited_by_name:     str      = Field(description="The name that invited this member to the org.")
+    role:                OrgRole  = Field(description="The user's role in the org")
     accepted:            bool     = Field(description='True if the user has accepted the org membership.')
     
-     
+
+
 class Org(BaseModel):
-    id:          int           = Field(description='Internal org id')
-    name:        str           = Field(min_length=1, max_length=39, description='Unique name for this org.')
-    description: Optional[str] = Field(default=None, description='Optional user supplied description.')
-    created_at:  float         = Field(description='The epoch timestamp when the org was created.')
-    updated_at:  float         = Field(description='The epoch timestamp when the org was updated.')
+    id:                  int           = Field(escription="Internal org id")
+    name:                str           = Field(max_length=39, description='Unique name for this org.')
+    description:         Optional[str] = Field(max_length=255, description='Optional user supplied description.')
+    created_at:          float         = Field(description='The epoch timestamp when the org was created.')
+    updated_at:          float         = Field(description='The epoch timestamp when the org was updated.')
+    created_by:          int           = Field(description='The user_id of the user that created the org.')
+    subscription_id:     str           = Field(description='The subscription_id for the org.')    
+    gpt4_credits:        int           = Field(description='The number of GPT-4 message credits currently available to the org users for chat.jiggy.ai.')
+    gpt3_5_credits:      int           = Field(description='The number of GPT-3 message credits currently available to the org users for chat.jiggy.ai.')
+    subscription_status: Optional[str] = Field(description='The stripe subscription status.')
+
```

### Comparing `jiggybase-0.0.35/jiggybase/models/plugin.py` & `jiggybase-0.0.36/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/models/plugin_config.py` & `jiggybase-0.0.36/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/models/prompt.py` & `jiggybase-0.0.36/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/models/providers.py` & `jiggybase-0.0.36/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/models/user.py` & `jiggybase-0.0.36/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase/org.py` & `jiggybase-0.0.36/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.36/jiggybase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.35
+Version: 0.0.36
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.35/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.36/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/pyproject.toml` & `jiggybase-0.0.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.35"
+version = "0.0.36"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.35/test/test.py` & `jiggybase-0.0.36/test/test.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.35/test/test_extract_typed_completion.py` & `jiggybase-0.0.36/test/test_extract_typed_completion.py`

 * *Files identical despite different names*

