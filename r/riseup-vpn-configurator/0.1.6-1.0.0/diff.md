# Comparing `tmp/riseup_vpn_configurator-0.1.6.tar.gz` & `tmp/riseup_vpn_configurator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riseup_vpn_configurator-0.1.6.tar", max compression
+gzip compressed data, was "riseup_vpn_configurator-1.0.0.tar", max compression
```

## Comparing `riseup_vpn_configurator-0.1.6.tar` & `riseup_vpn_configurator-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-02-13 13:46:29.483007 riseup_vpn_configurator-0.1.6/LICENSE
--rw-r--r--   0        0        0     5378 2023-02-27 16:31:36.044888 riseup_vpn_configurator-0.1.6/README.md
--rw-r--r--   0        0        0     1137 2023-04-06 08:54:30.236880 riseup_vpn_configurator-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    16336 2023-04-06 08:52:54.261541 riseup_vpn_configurator-0.1.6/riseup_vpn_configurator/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 16:23:10.812807 riseup_vpn_configurator-0.1.6/riseup_vpn_configurator/latency.py
--rw-r--r--   0        0        0      305 2023-02-27 16:08:48.769650 riseup_vpn_configurator-0.1.6/riseup_vpn_configurator/riseup-vpn.yaml
--rw-r--r--   0        0        0     6300 1970-01-01 00:00:00.000000 riseup_vpn_configurator-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-13 13:46:29.483007 riseup_vpn_configurator-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5520 2023-06-04 19:44:35.142687 riseup_vpn_configurator-1.0.0/README.md
+-rw-r--r--   0        0        0     1137 2023-06-04 19:45:13.419493 riseup_vpn_configurator-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    16767 2023-06-04 19:41:37.418707 riseup_vpn_configurator-1.0.0/riseup_vpn_configurator/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-27 16:23:10.812807 riseup_vpn_configurator-1.0.0/riseup_vpn_configurator/latency.py
+-rw-r--r--   0        0        0      305 2023-02-27 16:08:48.769650 riseup_vpn_configurator-1.0.0/riseup_vpn_configurator/riseup-vpn.yaml
+-rw-r--r--   0        0        0     6442 1970-01-01 00:00:00.000000 riseup_vpn_configurator-1.0.0/PKG-INFO
```

### Comparing `riseup_vpn_configurator-0.1.6/LICENSE` & `riseup_vpn_configurator-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `riseup_vpn_configurator-0.1.6/README.md` & `riseup_vpn_configurator-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,23 +22,24 @@
 The riseup-vpn-configurator is a simple command line tool that tries to solve these problems. It generates an OpenVPN configuration file that can be used by `systemctl`.
 
 # Installation
 
 Please don't install it as user and run it as root, as this makes it very easy for an attacker to escalate privileges. You can install the [Arch Linux AUR package](https://aur.archlinux.org/packages/riseup-vpn-configurator) or use it with `pip install --user riseup-vpn-configurator` as root. Check out the `How to use it` below to get the VPN up and running. You can start RiseupVPN with `systemctl start openvpn-client@riseup` and autostart it with `systemctl enable openvpn-client@riseup`. Please keep in mind that the client certificate is only valid for 90 and you have to update it manually.
 
 ```bash
-kmille@linbox:~ riseup-vpn-configurator --help
-usage: riseup-vpn-configurator [-h] [-v] [-d] [-u] [--uninstall] [-l] [-b] [-c] [-g] [-s] [--version]
+usage: riseup-vpn-configurator [-h] [-v] [--no-check-certificate] [-d] [-u] [--uninstall] [-l] [-b] [-c] [-g] [-s] [--version]
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         show verbose output
+  --no-check-certificate
+                        skip ssl certificate check (used by --update to get the config/client private key from the API)
   -d, --default-config  print default config file risup-vpn.yaml
   -u, --update          update gateway list and client certificate/key
-  --uninstall           remove all files
+  --uninstall           remove all files in /opt/riseup-vpn
   -l, --list-gateways   show available VPN server
   -b, --benchmark       use with --list - pings the gateway and shows the latency
   -c, --check-config    check syntax of /etc/riseup-vpn.yaml. Generates default config
   -g, --generate-config
                         Generate openvpn config (/etc/openvpn/client/riseup.conf)
   -s, --status          show current state of riseup-vpn
   --version             show version
```

### Comparing `riseup_vpn_configurator-0.1.6/pyproject.toml` & `riseup_vpn_configurator-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "riseup-vpn-configurator"
-version = "0.1.6"
+version = "1.0.0"
 description = "a simple command line tool to get RiseupVPN up and running"
 authors = ["kmille <github@androidloves.me>"]
 readme = "README.md"
 packages = [{include = "riseup_vpn_configurator"}]
 license = "GPL-3.0-only"
 repository = "https://github.com/kmille/riseup-vpn-configurator"
 homepage = "https://github.com/kmille/riseup-vpn-configurator"
```

### Comparing `riseup_vpn_configurator-0.1.6/riseup_vpn_configurator/__init__.py` & `riseup_vpn_configurator-1.0.0/riseup_vpn_configurator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing import Optional, NoReturn
 
 import ping3
 ping3.EXCEPTIONS = True
 
 FORMAT = "%(levelname)s: %(message)s"
 logging.basicConfig(format=FORMAT, level=logging.INFO)
-logging.getLogger("urllib3").setLevel(logging.WARNING)
+# logging.getLogger("urllib3").setLevel(logging.WARNING)
 
 working_dir = Path("/opt/riseup-vpn")
 api_ca_cert_file = working_dir / Path("api-ca.pem")
 gateway_json = working_dir / Path("gateways.json")
 
 ca_cert_file = working_dir / Path("vpn-ca.pem")
 cert_file = working_dir / Path("cert.pem")
@@ -38,14 +38,15 @@
 
 GATEWAYS_API_URL = "https://api.black.riseup.net/1/configs/eip-service.json"
 PROVIDER_API_URL = "https://riseup.net/provider.json"
 VPN_CA_CERT_URL = "https://black.riseup.net/ca.crt"
 VPN_CLIENT_CREDENTIALS_URL = "https://api.black.riseup.net/1/cert"
 
 VPN_USER = "openvpn"
+VERIFY_SSL_CERTIFICATE = True
 
 
 def calc_latency(ip: str) -> float:
     latency = 0.0
     iterations = 4
     for i in range(iterations):
         try:
@@ -57,19 +58,19 @@
     return latency_avg
 
 
 def cache_api_ca_cert() -> None:
     logging.debug("Updating riseup.net API API CA certificate")
     logging.debug(f"Fetching riseup.net VPN metadata from {PROVIDER_API_URL}")
     try:
-        resp = requests.get(PROVIDER_API_URL)
+        resp = requests.get(PROVIDER_API_URL, verify=VERIFY_SSL_CERTIFICATE)
         j = resp.json()
         assert "ca_cert_uri" in j.keys()
         logging.debug(f"Fetching API CA certificate from {j['ca_cert_uri']}")
-        resp = requests.get(j['ca_cert_uri'])
+        resp = requests.get(j['ca_cert_uri'], verify=VERIFY_SSL_CERTIFICATE)
         api_ca_cert_file.write_text(resp.text)
     except Exception as e:
         logging.error(e)
         sys.exit(1)
     fix_file_permissions(api_ca_cert_file)
     logging.info(f"Sucessfully cached API CA certificate to {api_ca_cert_file}")
 
@@ -93,15 +94,15 @@
 
 def update_vpn_ca_certificate() -> None:
     """
     curl https://black.riseup.net/ca.crt
     """
     logging.info("Updating VPN CA certificate")
     try:
-        resp = requests.get(VPN_CA_CERT_URL)
+        resp = requests.get(VPN_CA_CERT_URL, verify=VERIFY_SSL_CERTIFICATE)
         assert "-----BEGIN CERTIFICATE-----" in resp.text
         assert "-----END CERTIFICATE-----" in resp.text
         ca_cert_file.write_text(resp.text)
     except Exception as e:
         logging.error(e)
         sys.exit(1)
     fix_file_permissions(ca_cert_file)
@@ -414,31 +415,35 @@
     sys.exit()
 
 
 def main() -> None:
 
     parser = argparse.ArgumentParser()
     parser.add_argument("-v", "--verbose", action="store_true", help="show verbose output")
+    parser.add_argument("--no-check-certificate", action="store_true", help="skip ssl certificate check (used by --update to get the config/client private key from the API)")
     parser.add_argument("-d", "--default-config", action="store_true", help="print default config file risup-vpn.yaml")
     parser.add_argument("-u", "--update", action="store_true", help="update gateway list and client certificate/key")
-    parser.add_argument("--uninstall", action="store_true", help="remove all files")
+    parser.add_argument("--uninstall", action="store_true", help=f"remove all files in {working_dir}")
     parser.add_argument("-l", "--list-gateways", action="store_true", help="show available VPN server")
     parser.add_argument("-b", "--benchmark", action="store_true", help="use with --list - pings the gateway and shows the latency")
     parser.add_argument("-c", "--check-config", action="store_true", help=f"check syntax of {config_file}. Generates default config")
     parser.add_argument("-g", "--generate-config", action="store_true", help=f"Generate openvpn config ({ovpn_file})")
     parser.add_argument("-s", "--status", action="store_true", help="show current state of riseup-vpn")
     parser.add_argument("--version", action="store_true", help="show version")
 
     args = parser.parse_args()
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(1)
 
     if args.verbose:
         logging.getLogger().setLevel(logging.DEBUG)
+    elif args.no_check_certificate:
+        global VERIFY_SSL_CERTIFICATE
+        VERIFY_SSL_CERTIFICATE = False
     elif args.version:
         show_version()
     elif args.default_config:
         print_default_config(0)
 
     check_root_permissions()
```

### Comparing `riseup_vpn_configurator-0.1.6/PKG-INFO` & `riseup_vpn_configurator-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riseup-vpn-configurator
-Version: 0.1.6
+Version: 1.0.0
 Summary: a simple command line tool to get RiseupVPN up and running
 Home-page: https://github.com/kmille/riseup-vpn-configurator
 License: GPL-3.0-only
 Author: kmille
 Author-email: github@androidloves.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -45,23 +45,24 @@
 The riseup-vpn-configurator is a simple command line tool that tries to solve these problems. It generates an OpenVPN configuration file that can be used by `systemctl`.
 
 # Installation
 
 Please don't install it as user and run it as root, as this makes it very easy for an attacker to escalate privileges. You can install the [Arch Linux AUR package](https://aur.archlinux.org/packages/riseup-vpn-configurator) or use it with `pip install --user riseup-vpn-configurator` as root. Check out the `How to use it` below to get the VPN up and running. You can start RiseupVPN with `systemctl start openvpn-client@riseup` and autostart it with `systemctl enable openvpn-client@riseup`. Please keep in mind that the client certificate is only valid for 90 and you have to update it manually.
 
 ```bash
-kmille@linbox:~ riseup-vpn-configurator --help
-usage: riseup-vpn-configurator [-h] [-v] [-d] [-u] [--uninstall] [-l] [-b] [-c] [-g] [-s] [--version]
+usage: riseup-vpn-configurator [-h] [-v] [--no-check-certificate] [-d] [-u] [--uninstall] [-l] [-b] [-c] [-g] [-s] [--version]
 
 options:
   -h, --help            show this help message and exit
   -v, --verbose         show verbose output
+  --no-check-certificate
+                        skip ssl certificate check (used by --update to get the config/client private key from the API)
   -d, --default-config  print default config file risup-vpn.yaml
   -u, --update          update gateway list and client certificate/key
-  --uninstall           remove all files
+  --uninstall           remove all files in /opt/riseup-vpn
   -l, --list-gateways   show available VPN server
   -b, --benchmark       use with --list - pings the gateway and shows the latency
   -c, --check-config    check syntax of /etc/riseup-vpn.yaml. Generates default config
   -g, --generate-config
                         Generate openvpn config (/etc/openvpn/client/riseup.conf)
   -s, --status          show current state of riseup-vpn
   --version             show version
```

