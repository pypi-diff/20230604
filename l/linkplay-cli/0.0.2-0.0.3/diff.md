# Comparing `tmp/linkplay-cli-0.0.2.tar.gz` & `tmp/linkplay-cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkplay-cli-0.0.2.tar", last modified: Mon May 29 19:51:08 2023, max compression
+gzip compressed data, was "linkplay-cli-0.0.3.tar", last modified: Sun Jun  4 17:53:54 2023, max compression
```

## Comparing `linkplay-cli-0.0.2.tar` & `linkplay-cli-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxr-x   0 rami      (1000) rami      (1000)        0 2023-05-29 19:51:08.216573 linkplay-cli-0.0.2/
--rw-rw-r--   0 rami      (1000) rami      (1000)     1211 2023-05-29 19:42:12.000000 linkplay-cli-0.0.2/LICENSE
--rw-rw-r--   0 rami      (1000) rami      (1000)     1086 2023-05-29 19:51:08.216573 linkplay-cli-0.0.2/PKG-INFO
--rw-rw-r--   0 rami      (1000) rami      (1000)      804 2023-05-29 19:42:12.000000 linkplay-cli-0.0.2/README.md
-drwxrwxr-x   0 rami      (1000) rami      (1000)        0 2023-05-29 19:51:08.216573 linkplay-cli-0.0.2/linkplay_cli/
--rw-rw-r--   0 rami      (1000) rami      (1000)        1 2023-05-29 19:42:12.000000 linkplay-cli-0.0.2/linkplay_cli/__init__.py
--rw-rw-r--   0 rami      (1000) rami      (1000)    10556 2023-05-29 19:49:07.000000 linkplay-cli-0.0.2/linkplay_cli/cli.py
-drwxrwxr-x   0 rami      (1000) rami      (1000)        0 2023-05-29 19:51:08.216573 linkplay-cli-0.0.2/linkplay_cli.egg-info/
--rw-rw-r--   0 rami      (1000) rami      (1000)     1086 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/PKG-INFO
--rw-rw-r--   0 rami      (1000) rami      (1000)      289 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 rami      (1000) rami      (1000)        1 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 rami      (1000) rami      (1000)       55 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/entry_points.txt
--rw-rw-r--   0 rami      (1000) rami      (1000)       27 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/requires.txt
--rw-rw-r--   0 rami      (1000) rami      (1000)       13 2023-05-29 19:51:08.000000 linkplay-cli-0.0.2/linkplay_cli.egg-info/top_level.txt
--rw-rw-r--   0 rami      (1000) rami      (1000)       38 2023-05-29 19:51:08.216573 linkplay-cli-0.0.2/setup.cfg
--rw-rw-r--   0 rami      (1000) rami      (1000)      787 2023-05-29 19:50:51.000000 linkplay-cli-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:53:54.468422 linkplay-cli-0.0.3/
+-rw-rw-rw-   0        0        0     1211 2023-05-26 14:29:31.000000 linkplay-cli-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1161 2023-06-04 17:53:54.467421 linkplay-cli-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      804 2023-05-28 21:18:52.000000 linkplay-cli-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 17:53:54.417421 linkplay-cli-0.0.3/linkplay_cli/
+-rw-rw-rw-   0        0        0        1 2023-05-29 21:05:26.000000 linkplay-cli-0.0.3/linkplay_cli/__init__.py
+-rw-rw-rw-   0        0        0    10334 2023-06-04 17:51:21.000000 linkplay-cli-0.0.3/linkplay_cli/cli.py
+-rw-rw-rw-   0        0        0      217 2023-06-04 17:51:21.000000 linkplay-cli-0.0.3/linkplay_cli/config.py
+-rw-rw-rw-   0        0        0     2423 2023-06-04 17:51:21.000000 linkplay-cli-0.0.3/linkplay_cli/discovery.py
+-rw-rw-rw-   0        0        0     2300 2023-06-04 17:51:21.000000 linkplay-cli-0.0.3/linkplay_cli/firmware_update.py
+-rw-rw-rw-   0        0        0      739 2023-06-04 17:51:21.000000 linkplay-cli-0.0.3/linkplay_cli/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:53:54.464419 linkplay-cli-0.0.3/linkplay_cli.egg-info/
+-rw-rw-rw-   0        0        0     1161 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-04 17:53:54.000000 linkplay-cli-0.0.3/linkplay_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 17:53:54.469422 linkplay-cli-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-06-04 17:53:06.000000 linkplay-cli-0.0.3/setup.py
```

### Comparing `linkplay-cli-0.0.2/LICENSE` & `linkplay-cli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `linkplay-cli-0.0.2/PKG-INFO` & `linkplay-cli-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-Metadata-Version: 2.1
-Name: linkplay-cli
-Version: 0.0.2
-Summary: Control Linkplay devices from the comfort of your shell
-Home-page: https://github.com/ramikg/linkplay-cli
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Linkplay CLI
-
-Control audio devices supporting the Linkplay API, from the comfort of your shell.  
-Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
-
-![Screenshot](resources/screenshot.png)
-
-# Installation
-```bash
-pip install linkplay-cli
-```
-
-After installing, run `linkplay-cli -h` to get started.
-
-## FAQ
-
-### I'm getting the error `command not found: linkplay-cli` 
-
-The installed script is probably not in your `PATH`.  
-Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
-
-### Some commands have no effect
-
-This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
-For example, most commands won't work when the audio source is YouTube playing from your browser.
+Metadata-Version: 2.1
+Name: linkplay-cli
+Version: 0.0.3
+Summary: Control Linkplay devices from the comfort of your shell
+Home-page: https://github.com/ramikg/linkplay-cli
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Linkplay CLI
+
+Control audio devices supporting the Linkplay API, from the comfort of your shell.  
+Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
+
+![Screenshot](resources/screenshot.png)
+
+# Installation
+```bash
+pip install linkplay-cli
+```
+
+After installing, run `linkplay-cli -h` to get started.
+
+## FAQ
+
+### I'm getting the error `command not found: linkplay-cli` 
+
+The installed script is probably not in your `PATH`.  
+Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
+
+### Some commands have no effect
+
+This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
+For example, most commands won't work when the audio source is YouTube playing from your browser.
+
+
```

### Comparing `linkplay-cli-0.0.2/README.md` & `linkplay-cli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `linkplay-cli-0.0.2/linkplay_cli/cli.py` & `linkplay-cli-0.0.3/linkplay_cli/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,123 +1,49 @@
 import argparse
-import asyncio
-from http import HTTPStatus
 import ipaddress
 import re
 import sys
+import time
 from pathlib import Path
 
-from async_upnp_client.search import async_search
-import requests
+from bs4 import BeautifulSoup
+from Crypto.Cipher import ARC4
 
-
-class LinkplayCliCommandFailedException(Exception):
-    pass
+from linkplay_cli import config
+from linkplay_cli.discovery import discover_linkplay_address
+from linkplay_cli.firmware_update import print_latest_version_and_release_date
+from linkplay_cli.utils import perform_get_request
 
 
-class LinkplayCliGetRequestFailedException(Exception):
+class LinkplayCliCommandFailedException(Exception):
     pass
 
 
 class LinkplayCliInvalidVolumeArgumentException(Exception):
     pass
 
 
-class LinkplayCliDeviceNotFoundException(Exception):
-    pass
-
-
 class LinkplayCli:
-    OK_MESSAGE = 'OK'
-    GET_REQUEST_TIMEOUT_SECONDS = 5
-    UPNP_DISCOVER_TIMEOUT_SECONDS = 5
-    UPNP_DEVICE_TYPE = 'urn:schemas-upnp-org:device:MediaRenderer:1'
-    CACHE_FILE = Path.home() / '.linkplay_cached_device_address'
-
     def __init__(self, verbose, address=None) -> None:
         self._verbose = verbose
-        self._ip_address = address or self._discover_address()
-
-    @staticmethod
-    def _is_speaker_ip_address(ip_address):
-        if ip_address is None:
-            return False
-
-        response = requests.get(f'http://{ip_address}/httpapi.asp?command=setPlayerCmd',
-                                timeout=LinkplayCli.GET_REQUEST_TIMEOUT_SECONDS)
-
-        return response.status_code == HTTPStatus.OK
-
-    def _discover_address(self):
-        try:
-            if LinkplayCli.CACHE_FILE.exists():
-                cached_ip_address = ipaddress.IPv4Address(LinkplayCli.CACHE_FILE.read_text())
-                if LinkplayCli._is_speaker_ip_address(cached_ip_address):
-                    if self._verbose:
-                        print(f'Using cached IP address {cached_ip_address}')
-                    return cached_ip_address
-        except ipaddress.AddressValueError:
-            print('Cached IP address is corrupted. Rediscovering.')
-        except requests.exceptions.RequestException:
-            print('Connection failed. Rediscovering.')
-
-        print('Starting device discovery...')
-        linkplay_ip_addresses = []
-
-        async def add_speaker_to_list(upnp_device):
-            device_ip_address = upnp_device.get('_host')
-            if not LinkplayCli._is_speaker_ip_address(device_ip_address):
-                return
-
-            linkplay_ip_addresses.append(device_ip_address)
-
-        # Run synchronously, as our code is not async
-        asyncio.new_event_loop().run_until_complete(async_search(
-            search_target=LinkplayCli.UPNP_DEVICE_TYPE,
-            timeout=LinkplayCli.UPNP_DISCOVER_TIMEOUT_SECONDS,
-            async_callback=add_speaker_to_list
-        ))
-
-        if len(linkplay_ip_addresses) != 1:
-            if self._verbose and linkplay_ip_addresses:
-                print(f'Linkplay devices found: {linkplay_ip_addresses}')
-            raise LinkplayCliDeviceNotFoundException(f'Found {len(linkplay_ip_addresses)} devices. '
-                                                     'Please specify IP address manually.')
-
-        ip_address = linkplay_ip_addresses[0]
-        LinkplayCli.CACHE_FILE.write_text(ip_address)
-        print(f'Discovered device at IP address {ip_address}. Caching for future use.')
-
-        return ipaddress.IPv4Address(ip_address)
+        self._ip_address = address or discover_linkplay_address(verbose)
 
     @staticmethod
     def verify_volume_argument(arg):
         match_result = re.match(r'^[-+]?(\d+)$', arg)
         if match_result is None:
             raise LinkplayCliInvalidVolumeArgumentException(f'Invalid argument "{arg}". See the command\'s help.')
 
         return arg
 
     def _run_command(self, command, expect_json=False):
-        params = {'command': command}
-        response = requests.get(f'http://{self._ip_address}/httpapi.asp',
-                                params=params,
-                                timeout=LinkplayCli.GET_REQUEST_TIMEOUT_SECONDS)
-
-        verbose_message = f'GET {response.request.url} returned {response.status_code}: {response.text}'
-
-        if response.status_code != HTTPStatus.OK:
-            raise LinkplayCliGetRequestFailedException(verbose_message)
-        if self._verbose:
-            print(verbose_message)
-
-        if expect_json:
-            return response.json()
-        else:
-            return response.text
+        return perform_get_request(f'http://{self._ip_address}/httpapi.asp',
+                                   verbose=self._verbose,
+                                   params={'command': command},
+                                   expect_json=expect_json)
 
     @staticmethod
     def _convert_ms_to_duration_string(ms):
         ms = int(ms)
 
         seconds, _ = divmod(ms, 1000)
         minutes, seconds = divmod(seconds, 60)
@@ -144,56 +70,58 @@
             status_string = '▶️'
         elif status == 'pause':
             status_string = '⏸'
         else:
             status_string = '⏹️'
 
         output_string = f'{status_string}  {artist} - {title}'
-        if args.no_time:
+        if not args.no_time:
             if int(player_status['curpos']) > int(player_status['totlen']):
                 # There's a bug where the current position is some constant garbage value
                 current_position_in_ms = '?:??'
             else:
                 current_position_in_ms = self._convert_ms_to_duration_string(player_status['curpos'])
             total_length_in_ms = self._convert_ms_to_duration_string(player_status['totlen'])
 
             output_string += f' {UNICODE_LTR_MARK}[{current_position_in_ms}/{total_length_in_ms}]'
 
         print(output_string)
 
-    def _run_player_command_expecting_ok_response(self, command):
-        response = self._run_command(command)
-        if response != LinkplayCli.OK_MESSAGE:
-            raise LinkplayCliCommandFailedException(f'Command {command} failed with response {response}.')
+    def _run_player_command_expecting_ok_output(self, command):
+        OK_MESSAGE = 'OK'
+
+        output = self._run_command(command)
+        if output != OK_MESSAGE:
+            raise LinkplayCliCommandFailedException(f'Command {command} failed with output {output}.')
 
     def _get_player_status(self):
         return self._run_command('getPlayerStatus', expect_json=True)
 
     def pause(self, _):
-        self._run_player_command_expecting_ok_response('setPlayerCmd:pause')
+        self._run_player_command_expecting_ok_output('setPlayerCmd:pause')
         print('Playback paused')
 
     def play(self, _):
-        self._run_player_command_expecting_ok_response('setPlayerCmd:resume')
+        self._run_player_command_expecting_ok_output('setPlayerCmd:resume')
         print('Playback resumed')
 
     def next(self, _):
-        self._run_player_command_expecting_ok_response('setPlayerCmd:next')
+        self._run_player_command_expecting_ok_output('setPlayerCmd:next')
         print('Switched to next track')
 
     def previous(self, _):
-        self._run_player_command_expecting_ok_response('setPlayerCmd:prev')
+        self._run_player_command_expecting_ok_output('setPlayerCmd:prev')
         print('Switched to previous track')
 
     def mute(self, _):
-        self._run_player_command_expecting_ok_response('setPlayerCmd:mute:1')
+        self._run_player_command_expecting_ok_output('setPlayerCmd:mute:1')
         print('Muted')
 
     def unmute(self, _):
-        self._run_player_command_expecting_ok_response('setPlayerCmd:mute:0')
+        self._run_player_command_expecting_ok_output('setPlayerCmd:mute:0')
         print('Unmuted')
 
     def volume(self, volume_args):
         player_status = self._get_player_status()
         orig_volume = int(player_status['vol'])
         muted = player_status['mute'] == '1'
 
@@ -208,20 +136,64 @@
             new_volume = min(100, orig_volume + int(volume_arg[1:]))
         elif volume_arg.startswith('-'):
             new_volume = max(0, orig_volume - int(volume_arg[1:]))
         else:
             # Negative input is interpreted as "decrease volume"
             new_volume = min(100, int(volume_arg))
 
-        self._run_player_command_expecting_ok_response(f'setPlayerCmd:vol:{new_volume}')
+        self._run_player_command_expecting_ok_output(f'setPlayerCmd:vol:{new_volume}')
         print(f'Volume: {orig_volume} -> {new_volume}{muted_string}')
 
     def raw(self, raw_args):
         print(self._run_command(raw_args.command))
 
+    @staticmethod
+    def _print_info_if_not_empty(info_name, value):
+        if value not in ['', '0']:
+            print(f'{info_name}: {value}')
+
+    def _print_latest_version_and_release_date(self, model, hardware):
+        update_server = self._run_command('GetUpdateServer')
+
+        print_latest_version_and_release_date(update_server, model, hardware, self._verbose)
+
+    def info(self, _):
+        status = self._run_command('getStatus', expect_json=True)
+
+        model = status["project"]
+        hardware = status["hardware"]
+
+        print(f'Device name: {status["DeviceName"]}')
+        print(f'Model: {model}')
+        self._print_info_if_not_empty('Wi-Fi IP address', status["apcli0"])
+        self._print_info_if_not_empty('Wi-Fi SSID', self._decode_string(status["essid"]))
+        self._print_info_if_not_empty('Ethernet IP address', status["eth2"])
+        print(f'UUID: {status["uuid"]}')
+        print(f'Hardware: {hardware}')
+        self._print_info_if_not_empty('MCU version', status["mcu_ver"])
+        self._print_info_if_not_empty('DSP version', status["dsp_ver"])
+        print(f'Firmware version: {status["firmware"]} (released {status["Release"]})')
+
+        self._print_latest_version_and_release_date(model, hardware)
+
+    def getsyslog(self, args):
+        download_page = self._run_command('getsyslog')  # The download URL is always the same, but needs to be refreshed
+        download_url = f'http://{self._ip_address}/' + BeautifulSoup(download_page, 'lxml').find('a')['href']
+        encrypted_log = perform_get_request(download_url, verbose=False, expect_bytes=True)
+
+        output_file_path = args.output_file or Path.cwd() / ('sys.log-' + time.strftime('%Y%m%d%H%M%S'))
+
+        with open(output_file_path, 'wb') as output_file:
+            for chunk_start in range(0, len(encrypted_log), config.log_chunk_size):
+                chunk = encrypted_log[chunk_start:chunk_start + config.log_chunk_size]
+                cipher = ARC4.new(config.log_key)
+                output_file.write(cipher.decrypt(chunk))
+
+        print(f'Log file downloaded to {output_file_path}')
+
 
 def _parse_args():
     main_parser = argparse.ArgumentParser(epilog='For more information about a given command, use "<command> -h"')
 
     common_parser = argparse.ArgumentParser(add_help=False)
     common_parser.add_argument('--ip-address', type=ipaddress.IPv4Address, help='The IP address of the device')
     common_parser.add_argument('--verbose', '-v', action='store_true', help='Verbose mode')
@@ -259,14 +231,21 @@
     previous_parser = subparsers.add_parser('unmute', parents=[common_parser], help='Unmute')
     previous_parser.set_defaults(func=LinkplayCli.unmute)
 
     raw_parser = subparsers.add_parser('raw', parents=[common_parser], help='Execute a raw Linkplay command')
     raw_parser.set_defaults(func=LinkplayCli.raw)
     raw_parser.add_argument('command', help='The LinkPlay API command to execute')
 
+    info_parser = subparsers.add_parser('info', parents=[common_parser], help='Get basic device information')
+    info_parser.set_defaults(func=LinkplayCli.info)
+
+    getsyslog_parser = subparsers.add_parser('getsyslog', parents=[common_parser], help='Download device log file')
+    getsyslog_parser.set_defaults(func=LinkplayCli.getsyslog)
+    getsyslog_parser.add_argument('--output-file', '-o', help='Output path. Defaults to "./sys.log-<timestamp>"')
+
     if len(sys.argv) < 2:
         main_parser.print_help()
         sys.exit(0)
 
     return main_parser.parse_args()
```

### Comparing `linkplay-cli-0.0.2/linkplay_cli.egg-info/PKG-INFO` & `linkplay-cli-0.0.3/linkplay_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-Metadata-Version: 2.1
-Name: linkplay-cli
-Version: 0.0.2
-Summary: Control Linkplay devices from the comfort of your shell
-Home-page: https://github.com/ramikg/linkplay-cli
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Linkplay CLI
-
-Control audio devices supporting the Linkplay API, from the comfort of your shell.  
-Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
-
-![Screenshot](resources/screenshot.png)
-
-# Installation
-```bash
-pip install linkplay-cli
-```
-
-After installing, run `linkplay-cli -h` to get started.
-
-## FAQ
-
-### I'm getting the error `command not found: linkplay-cli` 
-
-The installed script is probably not in your `PATH`.  
-Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
-
-### Some commands have no effect
-
-This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
-For example, most commands won't work when the audio source is YouTube playing from your browser.
+Metadata-Version: 2.1
+Name: linkplay-cli
+Version: 0.0.3
+Summary: Control Linkplay devices from the comfort of your shell
+Home-page: https://github.com/ramikg/linkplay-cli
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Linkplay CLI
+
+Control audio devices supporting the Linkplay API, from the comfort of your shell.  
+Supports UPnP auto-discovery, so you don't even have to know your device's IP address.
+
+![Screenshot](resources/screenshot.png)
+
+# Installation
+```bash
+pip install linkplay-cli
+```
+
+After installing, run `linkplay-cli -h` to get started.
+
+## FAQ
+
+### I'm getting the error `command not found: linkplay-cli` 
+
+The installed script is probably not in your `PATH`.  
+Run `pip install` with the `-v` flag to find out the script's directory, and make sure that it's in your path.
+
+### Some commands have no effect
+
+This CLI utility is a wrapper around the Linkplay API, which may not work in all situations.  
+For example, most commands won't work when the audio source is YouTube playing from your browser.
+
+
```

### Comparing `linkplay-cli-0.0.2/setup.py` & `linkplay-cli-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,21 @@
     long_description = readme.read()
 
 setup(name='linkplay-cli',
       description='Control Linkplay devices from the comfort of your shell',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/ramikg/linkplay-cli',
-      version='0.0.2',
+      version='0.0.3',
       packages=find_packages(),
       install_requires=[
           'async_upnp_client',
+          'beautifulsoup4',
+          'lxml',
+          'pycryptodome',
           'requests'
       ],
       entry_points={
           'console_scripts': [
               'linkplay-cli = linkplay_cli.cli:main',
           ]
       },
```

