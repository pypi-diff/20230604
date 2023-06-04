# Comparing `tmp/twofas-cli-0.0.2.tar.gz` & `tmp/twofas-cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twofas-cli-0.0.2.tar", last modified: Wed May 31 23:30:41 2023, max compression
+gzip compressed data, was "twofas-cli-0.0.3.tar", last modified: Sun Jun  4 04:41:36 2023, max compression
```

## Comparing `twofas-cli-0.0.2.tar` & `twofas-cli-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/twofas_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/twofas_cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/twofas_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/twofas_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/twofas_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/twofas_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-04 04:41:24.000000 twofas-cli-0.0.3/twofas_cli/twofas_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 04:41:36.617133 twofas-cli-0.0.3/twofas_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-04 04:41:36.000000 twofas-cli-0.0.3/twofas_cli.egg-info/top_level.txt
```

### Comparing `twofas-cli-0.0.2/LICENSE` & `twofas-cli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.2/PKG-INFO` & `twofas-cli-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twofas-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial CLI tool for 2FAS using the browser extension api
 Home-page: https://packages.python.org/twofas-cli
 Author: dspd
 Author-email: inmost-chimps-0j@icloud.com
 License: BSD
 Keywords: 2fas twofas
 Classifier: Development Status :: 4 - Beta
@@ -36,10 +36,10 @@
 After installing 2fas on your mobile device and PC, register twofas-cli as a browser extension by running:
 
 ```shell
 twofas-cli register
 ```
 
 After running this command successfully you should see a directory containing a QR code image called 
-`barcode.png`. Open it and scan it using your 2FAS app.
+`qrcode.png`. Open it and scan it using your 2FAS app.
 
 Afterward, you can type `twofas-cli get --help` to see the available options for retrieving 2fa codes.
```

### Comparing `twofas-cli-0.0.2/README.md` & `twofas-cli-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,10 +20,10 @@
 After installing 2fas on your mobile device and PC, register twofas-cli as a browser extension by running:
 
 ```shell
 twofas-cli register
 ```
 
 After running this command successfully you should see a directory containing a QR code image called 
-`barcode.png`. Open it and scan it using your 2FAS app.
+`qrcode.png`. Open it and scan it using your 2FAS app.
 
 Afterward, you can type `twofas-cli get --help` to see the available options for retrieving 2fa codes.
```

### Comparing `twofas-cli-0.0.2/setup.py` & `twofas-cli-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README.md file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="twofas-cli",
-    version="0.0.2",
+    version="0.0.3",
     author="dspd",
     author_email="inmost-chimps-0j@icloud.com",
     description="Unofficial CLI tool for 2FAS using the browser extension api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="BSD",
     keywords="2fas twofas",
```

### Comparing `twofas-cli-0.0.2/tests/test_cli.py` & `twofas-cli-0.0.3/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-def test_barcode_generation():
-    from twofas_cli import generate_barcode
-    from twofas_cli import BARCODE_FILE
-    generate_barcode('https://example.com')
-    assert BARCODE_FILE.exists(), "Barcode file should exist after generation"
+def test_qrcode_generation():
+    from twofas_cli import generate_qrcode
+    from twofas_cli import QRCODE_FILE
+    generate_qrcode('https://example.com')
+    assert QRCODE_FILE.exists(), "Barcode file should exist after generation"
 
 
 def test_generate_keypair():
     from twofas_cli import generate_key_pair, get_public_key, get_private_key
     generate_key_pair()
     assert get_private_key(), "Private key file should exist after generation"
     assert get_public_key(), "Public key file should exist after generation"
```

### Comparing `twofas-cli-0.0.2/twofas_cli/api/api.py` & `twofas-cli-0.0.3/twofas_cli/api/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import base64
 import json
 
 import click
 import requests
 import websockets.sync.client as ws
+from requests import Response
 
 from twofas_cli.crypt import get_public_key_spki, decrypt
 
 
 class TwoFasApi:
     API_DEFAULT_BASE_URL = 'https://api2.2fas.com'
     WS_DEFAULT_BASE_URL = 'wss://ws.2fas.com'
@@ -18,61 +19,62 @@
             'Accept': 'application/json',
             'Content-Type': 'application/json'
         }
         self.api_base_url = api_base_url
         self.ws_base_url = ws_base_url
 
     @staticmethod
-    def process_response(res):
+    def process_response(res: Response) -> dict:
         if 200 <= res.status_code < 400:
             return res.json()
         else:
             # Print body as json to stderr
             click.echo(f'Error: {res.status_code}', err=True)
             click.echo(json.dumps(res.json(), indent=2), err=True)
             res.raise_for_status()
 
     @staticmethod
     def create_browser_info(name: str) -> dict:
         return {
             'name': name,
             'browser_name': '2FAS CLI',
-            'browser_version': '0.0.2',
+            'browser_version': '0.0.3',
             'public_key': get_public_key_spki()
         }
 
-    def create_extension_instance(self, browser_name: str):
+    def create_extension_instance(self, browser_name: str) -> dict:
         res = requests.post(f'{self.api_base_url}/browser_extensions',
                             headers=self.headers,
                             data=json.dumps(self.create_browser_info(browser_name)))
         return self.process_response(res)
 
-    def update_browser_extension(self, ext_id: str, browser_name: str):
+    def update_browser_extension(self, ext_id: str, browser_name: str) -> dict:
         res = requests.put(f'{self.api_base_url}/browser_extensions/{ext_id}',
                            headers=self.headers,
                            data=json.dumps(self.create_browser_info(browser_name)))
         return self.process_response(res)
 
-    def get_all_paired_devices(self, ext_id):
+    def get_all_paired_devices(self, ext_id: str) -> dict:
         res = requests.get(f'{self.api_base_url}/browser_extensions/{ext_id}/devices',
                            headers=self.headers)
         return self.process_response(res)
 
-    def remove_paired_device(self, ext_id, device_id):
+    def remove_paired_device(self, ext_id: str, device_id: str) -> dict:
         res = requests.delete(f'{self.api_base_url}/browser_extensions/{ext_id}/devices'
                               f'/{device_id}', headers=self.headers)
         return self.process_response(res)
 
-    def request2_fa_token(self, ext_id, domain):
+    def request2_fa_token(self, ext_id: str, domain: str) -> dict:
         res = requests.post(f'{self.api_base_url}/browser_extensions/{ext_id}/commands'
                             f'/request_2fa_token',
                             headers=self.headers, data=json.dumps({"domain": domain}))
         return self.process_response(res)
 
-    def close2_fa_request(self, ext_id, request_id, status=True):
+    def close2_fa_request(self, ext_id: str, request_id: str, status: bool = True) \
+            -> dict:
         data = {"status": "completed" if status else "terminated"}
         res = requests.post(
             f'{self.api_base_url}/browser_extensions/{ext_id}/2fa_requests/{request_id}'
             f'/commands/close_2fa_request',
             headers=self.headers,
             data=json.dumps(data))
         return self.process_response(res)
@@ -87,9 +89,9 @@
                     token_encrypted_base64 = data["token"]
                     token_encrypted = base64.b64decode(token_encrypted_base64)
                     return decrypt(token_encrypted)
                 else:
                     click.echo(f'Unknown event: {data["event"]}', err=True)
 
     @staticmethod
-    def generate_qr_link(browser_ext_id):
+    def generate_qr_link(browser_ext_id: str):
         return f'twofas_c://{browser_ext_id}'
```

### Comparing `twofas-cli-0.0.2/twofas_cli/common.py` & `twofas-cli-0.0.3/twofas_cli/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,14 @@
                     Path.home().joinpath('.config'))\
         .joinpath('twofas-cli')
     settings_dir.mkdir(parents=True, exist_ok=True)
     return settings_dir
 
 
 def get_extension_id():
-    settings_dir = get_settings_dir()
-    extension_id_file = settings_dir.joinpath('extension_id')
-    return extension_id_file.read_text(encoding='utf-8')
+    return EXTENSION_ID_FILE.read_text(encoding='utf-8')
 
 
 PRIVATE_KEY_FILE = get_settings_dir().joinpath('private_key.pem')
 PUBLIC_KEY_FILE = get_settings_dir().joinpath('public_key.pem')
 EXTENSION_ID_FILE = get_settings_dir().joinpath('extension_id')
-BARCODE_FILE = get_settings_dir().joinpath('barcode.png')
+QRCODE_FILE = get_settings_dir().joinpath('qrcode.png')
```

### Comparing `twofas-cli-0.0.2/twofas_cli/crypt.py` & `twofas-cli-0.0.3/twofas_cli/crypt.py`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.2/twofas_cli/twofas_cli.py` & `twofas-cli-0.0.3/twofas_cli/twofas_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,56 @@
+import os
 import re
 import signal
 import sys
-import os
 
 import click
 
 from . import crypt
 from .api import TwoFasApi
-from .common import get_settings_dir, get_extension_id, BARCODE_FILE, \
+from .common import get_extension_id, QRCODE_FILE, \
     PRIVATE_KEY_FILE, EXTENSION_ID_FILE, PUBLIC_KEY_FILE
 
 
 @click.group(name="test")
 def cli():
     pass
 
 
 @click.command('register', help='Register with 2FAS as a new "browser extension"')
-@click.option('--name', default=f'2FAS CLI {os.uname().sysname}', 
+@click.option('--name', default=f'2FAS CLI {os.uname().sysname}',
               help='The name that you want displayed for this CLI integration on your '
                    'mobile device',
               show_default=True, prompt=True)
 @click.option('--api-base_url', default=TwoFasApi.API_DEFAULT_BASE_URL,
               help='Base URL for the 2FAS REST API', show_default=True)
 def new(api_base_url: str, name: str):
     crypt.generate_key_pair()
     api = TwoFasApi(api_base_url)
     click.echo('Registering new "browser extension"...')
-    ext = api.create_extension_instance(name)
-    extension_id = ext['id']
-    # Assert that extension_id is a valid uuid
+    response = api.create_extension_instance(name)
+    extension_id = response['id']
     click.echo(f'Extension ID: {extension_id}')
-    get_settings_dir().joinpath('extension_id').write_text(extension_id, 
-                                                           encoding='utf-8')
-    barcode_file = generate_barcode(api.generate_qr_link(extension_id))
-    click.echo(f"Please scan the QR code image found under '{barcode_file}' with your "
+    EXTENSION_ID_FILE.write_text(extension_id, encoding='utf-8')
+    qrcode_file = generate_qrcode(api.generate_qr_link(extension_id))
+    click.echo(f"Please scan the QR code image found under '{qrcode_file}' with your "
                f"2FAS mobile app (under  Settings -> 'Browser extension')")
 
 
 @click.command('get', help='Fetch a 2FA token for a website or service')
 @click.option('--domain', help='Full URL of the website you want to get the 2FA token '
                                'for', type=str)
-@click.option('--identifier', 
+@click.option('--identifier',
               help='Instead of a domain, you can also set a custom identifier that you '
                    'can associate with a 2FA code on your mobile device. Only ASCII '
                    'letters, whitespace and the following symbols are allowed: -.',
               type=str)
-@click.option('--api-base-url', default=TwoFasApi.API_DEFAULT_BASE_URL, 
+@click.option('--api-base-url', default=TwoFasApi.API_DEFAULT_BASE_URL,
               help='Base URL for the 2FAS REST API', show_default=True)
-@click.option('--ws-base-url', default=TwoFasApi.WS_DEFAULT_BASE_URL, 
+@click.option('--ws-base-url', default=TwoFasApi.WS_DEFAULT_BASE_URL,
               help='Base URL for the 2FAS Websockets API', show_default=True)
 def get(domain: str, identifier: str, api_base_url: str, ws_base_url: str):
     check_if_registered() or sys.exit(1)
     if not domain and not identifier:
         click.echo('Either --domain or --identifier must be set', err=True)
         click.echo(click.get_current_context().get_help(), err=True)
         sys.exit(1)
@@ -67,15 +65,15 @@
 
     api = TwoFasApi(api_base_url, ws_base_url)
     extension_id = get_extension_id()
     response = api.request2_fa_token(extension_id, domain)
 
     token_request_id = response['token_request_id']
     if response['status'] != 'pending':
-        click.echo(f'Invalid response status from TWOFAS: {response["status"]}', 
+        click.echo(f'Invalid response status from TWOFAS: {response["status"]}',
                    err=True)
         sys.exit(1)
 
     # noinspection PyUnusedLocal
     def signal_handler(sig, frame):
         click.echo('Aborting...', err=True)
         api.close2_fa_request(extension_id, token_request_id, status=False)
@@ -90,15 +88,15 @@
 
 @click.group(name="devices", help="Manage mobile device pairings")
 def devices():
     pass
 
 
 @click.command("list", help="List all paired mobile devices")
-@click.option('--api-base-url', default=TwoFasApi.API_DEFAULT_BASE_URL, 
+@click.option('--api-base-url', default=TwoFasApi.API_DEFAULT_BASE_URL,
               help='Base URL for the 2FAS REST API', show_default=True)
 def list_devices(api_base_url: str):
     check_if_registered() or sys.exit(1)
     api = TwoFasApi(api_base_url)
     res = api.get_all_paired_devices(get_extension_id())
     click.echo('Device ID                             Device Name', err=True)
     for device in res:
@@ -114,22 +112,22 @@
               show_default=True)
 def delete_device(device_id: str, api_base_url: str):
     check_if_registered() or sys.exit(1)
     api = TwoFasApi(api_base_url)
     api.remove_paired_device(get_extension_id(), device_id)
 
 
-def generate_barcode(barcode_link: str):
+def generate_qrcode(qrcode_link: str):
     import pyqrcode
     import click
 
-    qr = pyqrcode.create(barcode_link)
-    qr.png(BARCODE_FILE, scale=6)
-    click.launch(str(BARCODE_FILE), locate=True)
-    return str(BARCODE_FILE)
+    qr = pyqrcode.create(qrcode_link)
+    qr.png(QRCODE_FILE, scale=6)
+    click.launch(str(QRCODE_FILE), locate=True)
+    return str(QRCODE_FILE)
 
 
 def check_if_registered() -> bool:
     if not PRIVATE_KEY_FILE.exists() or not PUBLIC_KEY_FILE.exists() \
             or not EXTENSION_ID_FILE.exists():
         click.echo('Please run "twofas-cli register" first', err=True)
         return False
```

### Comparing `twofas-cli-0.0.2/twofas_cli.egg-info/PKG-INFO` & `twofas-cli-0.0.3/twofas_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twofas-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial CLI tool for 2FAS using the browser extension api
 Home-page: https://packages.python.org/twofas-cli
 Author: dspd
 Author-email: inmost-chimps-0j@icloud.com
 License: BSD
 Keywords: 2fas twofas
 Classifier: Development Status :: 4 - Beta
@@ -36,10 +36,10 @@
 After installing 2fas on your mobile device and PC, register twofas-cli as a browser extension by running:
 
 ```shell
 twofas-cli register
 ```
 
 After running this command successfully you should see a directory containing a QR code image called 
-`barcode.png`. Open it and scan it using your 2FAS app.
+`qrcode.png`. Open it and scan it using your 2FAS app.
 
 Afterward, you can type `twofas-cli get --help` to see the available options for retrieving 2fa codes.
```

