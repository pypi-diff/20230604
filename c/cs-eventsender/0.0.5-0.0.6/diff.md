# Comparing `tmp/cs-eventsender-0.0.5.tar.gz` & `tmp/cs-eventsender-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-eventsender-0.0.5.tar", last modified: Mon May 29 19:30:56 2023, max compression
+gzip compressed data, was "cs-eventsender-0.0.6.tar", last modified: Sun Jun  4 20:26:32 2023, max compression
```

## Comparing `cs-eventsender-0.0.5.tar` & `cs-eventsender-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:30:56.816009 cs-eventsender-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-29 19:30:56.816009 cs-eventsender-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 19:30:45.000000 cs-eventsender-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:30:56.816009 cs-eventsender-0.0.5/cs_eventsender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-29 19:30:56.000000 cs-eventsender-0.0.5/cs_eventsender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-29 19:30:56.000000 cs-eventsender-0.0.5/cs_eventsender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:30:56.000000 cs-eventsender-0.0.5/cs_eventsender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 19:30:56.000000 cs-eventsender-0.0.5/cs_eventsender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 19:30:56.000000 cs-eventsender-0.0.5/cs_eventsender.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:30:56.816009 cs-eventsender-0.0.5/eventsender/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 19:30:45.000000 cs-eventsender-0.0.5/eventsender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-29 19:30:45.000000 cs-eventsender-0.0.5/eventsender/event_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:30:56.816009 cs-eventsender-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 19:30:45.000000 cs-eventsender-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:32.764109 cs-eventsender-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-04 20:26:32.764109 cs-eventsender-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 20:26:18.000000 cs-eventsender-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:32.764109 cs-eventsender-0.0.6/cs_eventsender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-04 20:26:32.000000 cs-eventsender-0.0.6/cs_eventsender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-04 20:26:32.000000 cs-eventsender-0.0.6/cs_eventsender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:26:32.000000 cs-eventsender-0.0.6/cs_eventsender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-04 20:26:32.000000 cs-eventsender-0.0.6/cs_eventsender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 20:26:32.000000 cs-eventsender-0.0.6/cs_eventsender.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:32.764109 cs-eventsender-0.0.6/eventsender/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-04 20:26:18.000000 cs-eventsender-0.0.6/eventsender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-04 20:26:18.000000 cs-eventsender-0.0.6/eventsender/event_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:26:32.764109 cs-eventsender-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-04 20:26:18.000000 cs-eventsender-0.0.6/setup.py
```

### Comparing `cs-eventsender-0.0.5/eventsender/event_sender.py` & `cs-eventsender-0.0.6/eventsender/event_sender.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import logging
 import os
 import requests
+from secrets_loader import load_secret
 from datetime import datetime
 import json
 from cs_telegram_bot import TelegramClient
 
 
 class EventSender:
     def __init__(self, server_url=None, api_key=None):
-        self.server_url = server_url or os.getenv("REACT_APP_API_URL")
+        self.server_url = server_url or load_secret("REACT_APP_API_URL")
         if not self.server_url:
             raise ValueError(
                 "Server URL is not set. It must be provided during initialization or set in the environment variables.")
 
-        self.api_key = api_key or os.getenv("FLASK_APP_API_KEY")
+        self.api_key = api_key or load_secret("FLASK_APP_API_KEY")
         if not self.api_key:
             raise ValueError(
                 "API key is not set. It must be provided during initialization or set in the environment variables.")
 
         self.telegram_client = TelegramClient()
 
     def _datetime_handler(self, obj):
```

### Comparing `cs-eventsender-0.0.5/setup.py` & `cs-eventsender-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'A package for sending event notifications.'
 LONG_DESCRIPTION = 'A package for sending event notifications.'
 
 # Setting up
 setup(
     name="cs-eventsender",
     version=VERSION,
```

