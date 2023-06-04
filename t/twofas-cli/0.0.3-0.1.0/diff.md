# Comparing `tmp/twofas-cli-0.0.3.tar.gz` & `tmp/twofas-cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twofas-cli-0.0.3.tar", last modified: Sun Jun  4 04:41:36 2023, max compression
+gzip compressed data, was "twofas-cli-0.1.0.tar", last modified: Sun Jun  4 04:52:24 2023, max compression
```

## Comparing `twofas-cli-0.0.3.tar` & `twofas-cli-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/twofas_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/twofas_cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/twofas_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/twofas_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:52:24.102598 twofas-cli-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-04 04:52:14.000000 twofas-cli-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-04 04:52:24.102598 twofas-cli-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-04 04:52:14.000000 twofas-cli-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-04 04:52:14.000000 twofas-cli-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 04:52:24.102598 twofas-cli-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-04 04:52:14.000000 twofas-cli-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:52:24.098598 twofas-cli-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-04 04:52:14.000000 twofas-cli-0.1.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:52:24.102598 twofas-cli-0.1.0/twofas_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 04:52:14.000000 twofas-cli-0.1.0/twofas_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:52:24.102598 twofas-cli-0.1.0/twofas_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-04 04:52:14.000000 twofas-cli-0.1.0/twofas_cli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-04 04:52:14.000000 twofas-cli-0.1.0/twofas_cli/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-04 04:52:14.000000 twofas-cli-0.1.0/twofas_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-04 04:52:14.000000 twofas-cli-0.1.0/twofas_cli/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-04 04:52:14.000000 twofas-cli-0.1.0/twofas_cli/twofas_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:52:24.102598 twofas-cli-0.1.0/twofas_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-04 04:52:24.000000 twofas-cli-0.1.0/twofas_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-04 04:52:24.000000 twofas-cli-0.1.0/twofas_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 04:52:24.000000 twofas-cli-0.1.0/twofas_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 04:52:24.000000 twofas-cli-0.1.0/twofas_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-04 04:52:24.000000 twofas-cli-0.1.0/twofas_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 04:52:24.000000 twofas-cli-0.1.0/twofas_cli.egg-info/top_level.txt
```

### Comparing `twofas-cli-0.0.3/LICENSE` & `twofas-cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.3/PKG-INFO` & `twofas-cli-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twofas-cli
-Version: 0.0.3
+Version: 0.1.0
 Summary: Unofficial CLI tool for 2FAS using the browser extension api
 Home-page: https://packages.python.org/twofas-cli
 Author: dspd
 Author-email: inmost-chimps-0j@icloud.com
 License: BSD
 Keywords: 2fas twofas
 Classifier: Development Status :: 4 - Beta
@@ -12,16 +12,16 @@
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # An unofficial command line interface for 2FAS
 
-twofas-cli is an unofficial client for [2FAS](https://2fas.com) written in Python that can retrieve 2fa codes from your mobile device by
-registering itself as a browser extensions. You can use it for scripting automatic logins to services that require a
+twofas-cli is an unofficial client for [2FAS](https://2fas.com) written in Python that can retrieve 2fa codes stored on your mobile device by
+registering itself as a browser extension with 2FAS. Every request this tool makes for a 2FA code needs to be approved on your mobile device, just like with 2FAS' browser extensions. You can use it for scripting automatic logins to services that require a
 second factor via TOTPs.
 
 ## Installation
 
 Install via pip from PyPi:
 
 ```shell
@@ -38,8 +38,16 @@
 ```shell
 twofas-cli register
 ```
 
 After running this command successfully you should see a directory containing a QR code image called 
 `qrcode.png`. Open it and scan it using your 2FAS app.
 
-Afterward, you can type `twofas-cli get --help` to see the available options for retrieving 2fa codes.
+Afterward, you can run `twofas-cli get --help` to see the available options for retrieving 2fa codes or `twofas-cli --help` to see all possible actions.
+
+## Compatibility
+
+twofas-cli should be able to run anywhere its dependencies and Python itself runs, however, it has only been tested so far on MacOS and Linux. It requires a recentish Python 3 version (>= 3.7).
+
+## Contributing
+
+Contributions are welcome. Please use the [Github Page](https://github.com/dspitzer/twofas-cli) to report issues or submit Pull Requests.
```

### Comparing `twofas-cli-0.0.3/setup.py` & `twofas-cli-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README.md file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="twofas-cli",
-    version="0.0.3",
+    version="0.1.0",
     author="dspd",
     author_email="inmost-chimps-0j@icloud.com",
     description="Unofficial CLI tool for 2FAS using the browser extension api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="BSD",
     keywords="2fas twofas",
```

### Comparing `twofas-cli-0.0.3/tests/test_cli.py` & `twofas-cli-0.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.3/twofas_cli/api/api.py` & `twofas-cli-0.1.0/twofas_cli/api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             res.raise_for_status()
 
     @staticmethod
     def create_browser_info(name: str) -> dict:
         return {
             'name': name,
             'browser_name': '2FAS CLI',
-            'browser_version': '0.0.3',
+            'browser_version': '0.1.0',
             'public_key': get_public_key_spki()
         }
 
     def create_extension_instance(self, browser_name: str) -> dict:
         res = requests.post(f'{self.api_base_url}/browser_extensions',
                             headers=self.headers,
                             data=json.dumps(self.create_browser_info(browser_name)))
```

### Comparing `twofas-cli-0.0.3/twofas_cli/common.py` & `twofas-cli-0.1.0/twofas_cli/common.py`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.3/twofas_cli/crypt.py` & `twofas-cli-0.1.0/twofas_cli/crypt.py`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.3/twofas_cli/twofas_cli.py` & `twofas-cli-0.1.0/twofas_cli/twofas_cli.py`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.3/twofas_cli.egg-info/PKG-INFO` & `twofas-cli-0.1.0/twofas_cli.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twofas-cli
-Version: 0.0.3
+Version: 0.1.0
 Summary: Unofficial CLI tool for 2FAS using the browser extension api
 Home-page: https://packages.python.org/twofas-cli
 Author: dspd
 Author-email: inmost-chimps-0j@icloud.com
 License: BSD
 Keywords: 2fas twofas
 Classifier: Development Status :: 4 - Beta
@@ -12,16 +12,16 @@
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # An unofficial command line interface for 2FAS
 
-twofas-cli is an unofficial client for [2FAS](https://2fas.com) written in Python that can retrieve 2fa codes from your mobile device by
-registering itself as a browser extensions. You can use it for scripting automatic logins to services that require a
+twofas-cli is an unofficial client for [2FAS](https://2fas.com) written in Python that can retrieve 2fa codes stored on your mobile device by
+registering itself as a browser extension with 2FAS. Every request this tool makes for a 2FA code needs to be approved on your mobile device, just like with 2FAS' browser extensions. You can use it for scripting automatic logins to services that require a
 second factor via TOTPs.
 
 ## Installation
 
 Install via pip from PyPi:
 
 ```shell
@@ -38,8 +38,16 @@
 ```shell
 twofas-cli register
 ```
 
 After running this command successfully you should see a directory containing a QR code image called 
 `qrcode.png`. Open it and scan it using your 2FAS app.
 
-Afterward, you can type `twofas-cli get --help` to see the available options for retrieving 2fa codes.
+Afterward, you can run `twofas-cli get --help` to see the available options for retrieving 2fa codes or `twofas-cli --help` to see all possible actions.
+
+## Compatibility
+
+twofas-cli should be able to run anywhere its dependencies and Python itself runs, however, it has only been tested so far on MacOS and Linux. It requires a recentish Python 3 version (>= 3.7).
+
+## Contributing
+
+Contributions are welcome. Please use the [Github Page](https://github.com/dspitzer/twofas-cli) to report issues or submit Pull Requests.
```

