# Comparing `tmp/ipilot-1.2-py3-none-any.whl.zip` & `tmp/ipilot-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5253 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-30 19:52 app/__init__.py
--rw-r--r--  2.0 unx       78 b- defN 22-Jun-30 19:52 app/_version.py
--rw-r--r--  2.0 unx      835 b- defN 22-Jun-30 19:52 app/args.py
--rw-r--r--  2.0 unx     1247 b- defN 22-Jun-30 19:52 app/ip_info.py
--rw-r--r--  2.0 unx     2182 b- defN 22-Jun-30 19:52 app/main.py
--rw-r--r--  2.0 unx      602 b- defN 22-Jun-30 19:52 app/print_table.py
--rw-r--r--  2.0 unx      828 b- defN 22-Jun-30 19:52 app/query_normalisation.py
--rw-r--r--  2.0 unx     1489 b- defN 22-Jun-30 19:52 ipilot-1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jun-30 19:52 ipilot-1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 22-Jun-30 19:52 ipilot-1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 22-Jun-30 19:52 ipilot-1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      878 b- defN 22-Jun-30 19:52 ipilot-1.2.dist-info/RECORD
-12 files, 8277 bytes uncompressed, 3793 bytes compressed:  54.2%
+Zip file size: 5581 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-04 11:14 app/__init__.py
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-04 11:14 app/_version.py
+-rw-r--r--  2.0 unx      855 b- defN 23-Jun-04 11:14 app/args.py
+-rw-r--r--  2.0 unx     1363 b- defN 23-Jun-04 11:14 app/ip_info.py
+-rw-r--r--  2.0 unx     2183 b- defN 23-Jun-04 11:14 app/main.py
+-rw-r--r--  2.0 unx      634 b- defN 23-Jun-04 11:14 app/print_table.py
+-rw-r--r--  2.0 unx      980 b- defN 23-Jun-04 11:14 app/query_normalisation.py
+-rw-r--r--  2.0 unx     2135 b- defN 23-Jun-04 11:15 ipilot-1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 11:15 ipilot-1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-Jun-04 11:15 ipilot-1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-04 11:15 ipilot-1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Jun-04 11:15 ipilot-1.3.dist-info/RECORD
+12 files, 9263 bytes uncompressed, 4121 bytes compressed:  55.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: app/print_table.py
 Comment: 
 
 Filename: app/query_normalisation.py
 Comment: 
 
-Filename: ipilot-1.2.dist-info/METADATA
+Filename: ipilot-1.3.dist-info/METADATA
 Comment: 
 
-Filename: ipilot-1.2.dist-info/WHEEL
+Filename: ipilot-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: ipilot-1.2.dist-info/entry_points.txt
+Filename: ipilot-1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipilot-1.2.dist-info/top_level.txt
+Filename: ipilot-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ipilot-1.2.dist-info/RECORD
+Filename: ipilot-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## app/_version.py

```diff
@@ -1,5 +1,5 @@
 #!/usr/bin/env python3
 
 """MODULE: Specifies app version."""
 
-VERSION = "1.2"
+VERSION = "1.3"  # pragma: no cover
```

## app/args.py

```diff
@@ -3,15 +3,15 @@
 """MODULE: Provides CLI arguments to the application."""
 
 import argparse
 
 from app.query_normalisation import get_public_ip
 
 
-def parse_args() -> argparse.Namespace:
+def parse_args() -> argparse.Namespace:  # pragma: no cover
     """Get arguments from user via the command line."""
     parser = argparse.ArgumentParser(
         description="Query information about an IP address or domain name."
     )
     parser.add_argument(
         "-q",
         "--query",
```

## app/ip_info.py

```diff
@@ -1,37 +1,38 @@
 #!/usr/bin/env python3
 
 """MODULE: Provides functions to call various APIs to retrieve IP/prefix information."""
 
 import ipaddress
+
 import requests
 
 
-def get_ip_information(ipv4_address: ipaddress.IPv4Address) -> dict:
+def get_ip_information(ipv4_address: ipaddress.IPv4Address) -> dict | None:
     """Retrieves information about a given IPv4 address from IP-API.com."""
-    api_endpoint = f"http://ip-api.com/json/{ipv4_address}"
+    api_endpoint: str = f"http://ip-api.com/json/{ipv4_address}"
     try:
-        resp = requests.get(api_endpoint)
+        resp: requests.Response = requests.get(api_endpoint, timeout=10)
         resp.raise_for_status()
-        ret = resp.json() if resp.json().get("status") == "success" else None
+        ret: dict | None = resp.json() if resp.json().get("status") == "success" else None
     except (requests.exceptions.JSONDecodeError, requests.exceptions.HTTPError):
         ret = None
     return ret
 
 
 def get_autonomous_system_number(as_info: str) -> str:
     """Parses AS number from provided AS information."""
-    as_number = as_info.split(" ")[0]
+    as_number: str = as_info.split(" ")[0]
     return as_number
 
 
-def get_prefix_information(autonomous_system: int) -> list:
+def get_prefix_information(autonomous_system: str) -> list | None:
     """Retrieves prefix information about a given autonomous system."""
-    api_endpoint = f"https://api.hackertarget.com/aslookup/?q={str(autonomous_system)}"
+    api_endpoint: str = f"https://api.hackertarget.com/aslookup/?q={str(autonomous_system)}"
     try:
-        resp = requests.get(api_endpoint)
+        resp: requests.Response = requests.get(api_endpoint, timeout=10)
         resp.raise_for_status()
     except requests.exceptions.HTTPError:
         return None
-    prefixes = resp.text.split("\n")
+    prefixes: list[str] = resp.text.split("\n")
     prefixes.pop(0)
     return prefixes
```

## app/main.py

```diff
@@ -1,62 +1,59 @@
 #!/usr/local/bin/python3
 
 """MODULE: Main application module."""
 
 import sys
 
 from app.args import parse_args
-from app.print_table import print_table, generate_prefix_string
-from app.query_normalisation import is_ip_address, resolve_domain_name
-from app.ip_info import (  # pragma: no cover
-    get_ip_information,
+from app.ip_info import (
     get_autonomous_system_number,
+    get_ip_information,
     get_prefix_information,
 )
-
+from app.print_table import generate_prefix_string, print_table
+from app.query_normalisation import is_ip_address, resolve_domain_name
 
 HEADER = """-----------------------------------------------
 | IP Address Information Lookup Tool (iPilot) |
 |       By Luke Tainton (@luketainton)        |
 -----------------------------------------------\n"""
 
 
-def main():
+def main() -> None:
     """Main function."""
     args = parse_args()
     if not args.noheader:
         print(HEADER)
 
     # Set IP to passed IP address, or resolve passed domain name to IPv4
-    ip_address = (
-        resolve_domain_name(args.query) if not is_ip_address(args.query) else args.query
-    )
+    ip_address = resolve_domain_name(args.query) if not is_ip_address(args.query) else args.query
 
     # If not given an IPv4, and can't resolve to IPv4, then throw error and exit
     if not ip_address:
         print("ERROR: could not resolve query to IPv4 address.")
         sys.exit(1)
 
     # Get information from API
-    ip_info = get_ip_information(ip_address)
+    ip_info: dict | None = get_ip_information(ip_address)
     if not ip_info:
         print("ERROR: could not retrieve IP information from API.")
         sys.exit(1)
-    as_number = get_autonomous_system_number(ip_info.get("as"))
+    as_number: str = get_autonomous_system_number(ip_info["as"])
 
     # Assemble list for table generation
-    table_data = [
-        ["IP Address", ip_info.get("query")],
-        ["Organization", ip_info.get("org")],
-        [
-            "Location",
-            f"{ip_info.get('country')}/{ip_info.get('regionName')}/{ip_info.get('city')}",
-        ],
-        ["Timezone", ip_info.get("timezone")],
-        ["Internet Service Provider", ip_info.get("isp")],
+    country: str = ip_info["country"]
+    region: str = ip_info["regionName"]
+    city: str = ip_info["city"]
+    table_data: list = [
+        ["IP Address", ip_info["query"]],
+        ["Organization", ip_info["org"]],
+        ["Location", f"{country}/{region}/{city}"],
+        ["Timezone", ip_info["timezone"]],
+        ["Internet Service Provider", ip_info["isp"]],
         ["Autonomous System", as_number],
     ]
 
     # If wanted, get prefix information
     if args.prefixes:
         prefix_info = get_prefix_information(as_number)
         if not prefix_info:
```

## app/print_table.py

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python3
 
 """MODULE: Provides functions for preparing, then printing, retrieved data."""
 
 from tabulate import tabulate
 
 
-def generate_prefix_string(prefixes: list) -> str:
+def generate_prefix_string(prefixes: list) -> str | None:
     """Generate a string that spilts prefixes into rows of 4."""
     num_per_row = 4
     try:
-        ret = ""
+        ret: str = ""
         for i in range(0, len(prefixes), num_per_row):
             ret += ", ".join(prefixes[i : i + num_per_row]) + "\n"
         return ret
     except AttributeError:
         return None
 
 
-def print_table(table_data) -> None:
+def print_table(table_data) -> None:  # pragma: no cover
     """Print table generated by tabulate."""
     print(tabulate(table_data))
```

## app/query_normalisation.py

```diff
@@ -1,31 +1,34 @@
 #!/usr/bin/env python3
 
-"""MODULE: Provides functions that ensure an IP address is available to query the APIs for."""
+"""MODULE: Provides functions that ensure an IP address is
+available to query the APIs for."""
 
-import socket
 import ipaddress
+import socket
+
 import requests
 
 
 def is_ip_address(query: str) -> bool:
     """Verifies if a given query is a valid IPv4 address."""
     try:
         ipaddress.ip_address(query)
         return True
     except ValueError:
         return False
 
 
-def resolve_domain_name(domain_name: str) -> ipaddress.IPv4Address:
+def resolve_domain_name(domain_name: str) -> ipaddress.IPv4Address | None:
     """Resolve a domain name via DNS or return None."""
     try:
-        ip_address = socket.gethostbyname(domain_name)
-    except socket.gaierror:
-        ip_address = None
-    return ip_address
+        result: str = socket.gethostbyname(domain_name)
+        ip_address: ipaddress.IPv4Address = ipaddress.IPv4Address(result)
+        return ip_address
+    except (socket.gaierror, ipaddress.AddressValueError):
+        return None
 
 
 def get_public_ip() -> ipaddress.IPv4Address:
     """Get the user's current public IPv4 address."""
-    ip_address = requests.get("https://api.ipify.org").text
-    return ip_address
+    ip_address: str = requests.get("https://api.ipify.org", timeout=10).text
+    return ipaddress.IPv4Address(ip_address)
```

