# Comparing `tmp/python-tado-0.8.0.tar.gz` & `tmp/python-tado-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-tado-0.8.0.tar", last modified: Sat Apr 18 21:25:16 2020, max compression
+gzip compressed data, was "dist/python-tado-0.8.1.tar", last modified: Sat Apr 18 21:28:32 2020, max compression
```

## Comparing `python-tado-0.8.0.tar` & `python-tado-0.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2020-04-18 21:25:16.000000 python-tado-0.8.0/
--rw-r--r--   0 wolfgang   (501) staff       (20)    35141 2017-05-14 20:36:03.000000 python-tado-0.8.0/LICENSE
--rw-r--r--   0 wolfgang   (501) staff       (20)       59 2019-03-16 10:41:55.000000 python-tado-0.8.0/MANIFEST.in
--rw-r--r--   0 wolfgang   (501) staff       (20)     2928 2020-04-18 21:25:16.000000 python-tado-0.8.0/PKG-INFO
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2020-04-18 21:25:16.000000 python-tado-0.8.0/PyTado/
--rw-r--r--   0 wolfgang   (501) staff       (20)       42 2017-05-14 20:36:29.000000 python-tado-0.8.0/PyTado/__init__.py
--rw-r--r--   0 wolfgang   (501) staff       (20)     2597 2019-03-16 10:41:55.000000 python-tado-0.8.0/PyTado/__main__.py
--rw-r--r--   0 wolfgang   (501) staff       (20)     1901 2020-03-23 07:37:52.000000 python-tado-0.8.0/PyTado/const.py
--rw-r--r--   0 wolfgang   (501) staff       (20)    13421 2020-04-18 21:24:16.000000 python-tado-0.8.0/PyTado/interface.py
--rw-r--r--   0 wolfgang   (501) staff       (20)    10552 2020-04-18 21:24:16.000000 python-tado-0.8.0/PyTado/zone.py
--rw-r--r--   0 wolfgang   (501) staff       (20)     1805 2020-03-04 09:17:26.000000 python-tado-0.8.0/README.md
-drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2020-04-18 21:25:16.000000 python-tado-0.8.0/python_tado.egg-info/
--rw-r--r--   0 wolfgang   (501) staff       (20)     2928 2020-04-18 21:25:15.000000 python-tado-0.8.0/python_tado.egg-info/PKG-INFO
--rw-r--r--   0 wolfgang   (501) staff       (20)      400 2020-04-18 21:25:15.000000 python-tado-0.8.0/python_tado.egg-info/SOURCES.txt
--rw-r--r--   0 wolfgang   (501) staff       (20)        1 2020-04-18 21:25:15.000000 python-tado-0.8.0/python_tado.egg-info/dependency_links.txt
--rw-r--r--   0 wolfgang   (501) staff       (20)       49 2020-04-18 21:25:15.000000 python-tado-0.8.0/python_tado.egg-info/entry_points.txt
--rw-r--r--   0 wolfgang   (501) staff       (20)        1 2020-04-18 21:25:15.000000 python-tado-0.8.0/python_tado.egg-info/not-zip-safe
--rw-r--r--   0 wolfgang   (501) staff       (20)        9 2020-04-18 21:25:15.000000 python-tado-0.8.0/python_tado.egg-info/requires.txt
--rw-r--r--   0 wolfgang   (501) staff       (20)        7 2020-04-18 21:25:15.000000 python-tado-0.8.0/python_tado.egg-info/top_level.txt
--rw-r--r--   0 wolfgang   (501) staff       (20)        9 2020-03-06 16:33:01.000000 python-tado-0.8.0/requirements.txt
--rw-r--r--   0 wolfgang   (501) staff       (20)       79 2020-04-18 21:25:16.000000 python-tado-0.8.0/setup.cfg
--rw-r--r--   0 wolfgang   (501) staff       (20)     1529 2020-04-18 21:25:07.000000 python-tado-0.8.0/setup.py
+drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2020-04-18 21:28:32.000000 python-tado-0.8.1/
+-rw-r--r--   0 wolfgang   (501) staff       (20)    35141 2017-05-14 20:36:03.000000 python-tado-0.8.1/LICENSE
+-rw-r--r--   0 wolfgang   (501) staff       (20)       59 2019-03-16 10:41:55.000000 python-tado-0.8.1/MANIFEST.in
+-rw-r--r--   0 wolfgang   (501) staff       (20)     2928 2020-04-18 21:28:32.000000 python-tado-0.8.1/PKG-INFO
+drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2020-04-18 21:28:32.000000 python-tado-0.8.1/PyTado/
+-rw-r--r--   0 wolfgang   (501) staff       (20)       42 2017-05-14 20:36:29.000000 python-tado-0.8.1/PyTado/__init__.py
+-rw-r--r--   0 wolfgang   (501) staff       (20)     2597 2019-03-16 10:41:55.000000 python-tado-0.8.1/PyTado/__main__.py
+-rw-r--r--   0 wolfgang   (501) staff       (20)     1901 2020-03-23 07:37:52.000000 python-tado-0.8.1/PyTado/const.py
+-rw-r--r--   0 wolfgang   (501) staff       (20)    13499 2020-04-18 21:27:52.000000 python-tado-0.8.1/PyTado/interface.py
+-rw-r--r--   0 wolfgang   (501) staff       (20)    10552 2020-04-18 21:24:16.000000 python-tado-0.8.1/PyTado/zone.py
+-rw-r--r--   0 wolfgang   (501) staff       (20)     1805 2020-03-04 09:17:26.000000 python-tado-0.8.1/README.md
+drwxr-xr-x   0 wolfgang   (501) staff       (20)        0 2020-04-18 21:28:32.000000 python-tado-0.8.1/python_tado.egg-info/
+-rw-r--r--   0 wolfgang   (501) staff       (20)     2928 2020-04-18 21:28:32.000000 python-tado-0.8.1/python_tado.egg-info/PKG-INFO
+-rw-r--r--   0 wolfgang   (501) staff       (20)      400 2020-04-18 21:28:32.000000 python-tado-0.8.1/python_tado.egg-info/SOURCES.txt
+-rw-r--r--   0 wolfgang   (501) staff       (20)        1 2020-04-18 21:28:32.000000 python-tado-0.8.1/python_tado.egg-info/dependency_links.txt
+-rw-r--r--   0 wolfgang   (501) staff       (20)       49 2020-04-18 21:28:32.000000 python-tado-0.8.1/python_tado.egg-info/entry_points.txt
+-rw-r--r--   0 wolfgang   (501) staff       (20)        1 2020-04-18 21:25:15.000000 python-tado-0.8.1/python_tado.egg-info/not-zip-safe
+-rw-r--r--   0 wolfgang   (501) staff       (20)        9 2020-04-18 21:28:32.000000 python-tado-0.8.1/python_tado.egg-info/requires.txt
+-rw-r--r--   0 wolfgang   (501) staff       (20)        7 2020-04-18 21:28:32.000000 python-tado-0.8.1/python_tado.egg-info/top_level.txt
+-rw-r--r--   0 wolfgang   (501) staff       (20)        9 2020-03-06 16:33:01.000000 python-tado-0.8.1/requirements.txt
+-rw-r--r--   0 wolfgang   (501) staff       (20)       79 2020-04-18 21:28:32.000000 python-tado-0.8.1/setup.cfg
+-rw-r--r--   0 wolfgang   (501) staff       (20)     1529 2020-04-18 21:28:29.000000 python-tado-0.8.1/setup.py
```

### Comparing `python-tado-0.8.0/LICENSE` & `python-tado-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-tado-0.8.0/PKG-INFO` & `python-tado-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-tado
-Version: 0.8.0
+Version: 0.8.1
 Summary: PyTado from chrism0dwk, modfied by w.malgadey, diplix, michaelarnauts, LenhartStephan, splifter, syssi, andersonshatch, Yippy, p0thi
 Home-page: https://github.com/wmalgadey/PyTado
 Author: chrism0dwk, w.malgadey
 Author-email: chrism0dwk@gmail.com, w.malgadey@gmail.com
 License: GPL3
 Description: PyTado -- Pythonize your central heating
         ========================================
```

### Comparing `python-tado-0.8.0/PyTado/__main__.py` & `python-tado-0.8.1/PyTado/__main__.py`

 * *Files identical despite different names*

### Comparing `python-tado-0.8.0/PyTado/const.py` & `python-tado-0.8.1/PyTado/const.py`

 * *Files identical despite different names*

### Comparing `python-tado-0.8.0/PyTado/interface.py` & `python-tado-0.8.1/PyTado/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,14 @@
         SEVEN_DAY = 2
 
     _debugCalls = False
 
     # Instance-wide constant info
     api2url = 'https://my.tado.com/api/v2/homes/'
     mobi2url = 'https://my.tado.com/mobile/1.9/'
-    refresh_token = ''
-    refresh_at = datetime.datetime.now() + datetime.timedelta(minutes=5)
     timeout = 10
 
     # 'Private' methods for use in class, Tado mobile API V1.9.
     def _mobile_apiCall(self, cmd):
         # pylint: disable=C0103
 
         self._refresh_token()
@@ -390,13 +388,16 @@
         data = self._apiCall(cmd, "DELETE", {}, True)
         return data
     
     # Ctor
     def __init__(self, username, password, timeout=10, http_session=None):
         """Performs login and save session cookie."""
         # HTTPS Interface
+        self.headers = {'Referer' : 'https://my.tado.com/'}
+        self.refresh_token = ''
+        self.refresh_at = datetime.datetime.now() + datetime.timedelta(minutes=5)
 
         # pylint: disable=C0103
         self._http_session = http_session if http_session else Session()
         self.headers = {'Referer' : 'https://my.tado.com/'}
         self._loginV2(username, password)
         self.id = self.getMe()['homes'][0]['id']
```

### Comparing `python-tado-0.8.0/PyTado/zone.py` & `python-tado-0.8.1/PyTado/zone.py`

 * *Files identical despite different names*

### Comparing `python-tado-0.8.0/README.md` & `python-tado-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `python-tado-0.8.0/python_tado.egg-info/PKG-INFO` & `python-tado-0.8.1/python_tado.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: python-tado
-Version: 0.8.0
+Version: 0.8.1
 Summary: PyTado from chrism0dwk, modfied by w.malgadey, diplix, michaelarnauts, LenhartStephan, splifter, syssi, andersonshatch, Yippy, p0thi
 Home-page: https://github.com/wmalgadey/PyTado
 Author: chrism0dwk, w.malgadey
 Author-email: chrism0dwk@gmail.com, w.malgadey@gmail.com
 License: GPL3
 Description: PyTado -- Pythonize your central heating
         ========================================
```

### Comparing `python-tado-0.8.0/setup.py` & `python-tado-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     os.system('python setup.py sdist upload')
     sys.exit()
 
 readme = open(here('README.md')).read()
 requirements = [x.strip() for x in open(here('requirements.txt')).readlines()]
 
 setup(name='python-tado',
-      version='0.8.0',
+      version='0.8.1',
       description='PyTado from chrism0dwk, modfied by w.malgadey, diplix, michaelarnauts, LenhartStephan, splifter, syssi, andersonshatch, Yippy, p0thi',
       long_description=readme,
       keywords='tado',
       author='chrism0dwk, w.malgadey',
       author_email='chrism0dwk@gmail.com, w.malgadey@gmail.com',
       url='https://github.com/wmalgadey/PyTado',
       install_requires=requirements,
```

