# Comparing `tmp/pykeadhcp-0.2.0.tar.gz` & `tmp/pykeadhcp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeadhcp-0.2.0.tar", max compression
+gzip compressed data, was "pykeadhcp-0.3.0.tar", max compression
```

## Comparing `pykeadhcp-0.2.0.tar` & `pykeadhcp-0.3.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0    11356 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/LICENSE
--rw-r--r--   0        0        0     7331 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/README.md
--rw-r--r--   0        0        0       30 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/__init__.py
--rw-r--r--   0        0        0      174 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/daemons/__init__.py
--rw-r--r--   0        0        0     4508 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/daemons/ctrlagent.py
--rw-r--r--   0        0        0     4526 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/daemons/ddns.py
--rw-r--r--   0        0        0    25620 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/daemons/dhcp4.py
--rw-r--r--   0        0        0    21878 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/daemons/dhcp6.py
--rw-r--r--   0        0        0     2718 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/exceptions.py
--rw-r--r--   0        0        0     7934 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/kea.py
--rw-r--r--   0        0        0        0 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/ctrlagent/__init__.py
--rw-r--r--   0        0        0      457 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/ctrlagent/config.py
--rw-r--r--   0        0        0        0 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/__init__.py
--rw-r--r--   0        0        0      331 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/client_class.py
--rw-r--r--   0        0        0      778 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/config.py
--rw-r--r--   0        0        0      207 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/lease.py
--rw-r--r--   0        0        0      303 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/reservation.py
--rw-r--r--   0        0        0      448 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/shared_network.py
--rw-r--r--   0        0        0      679 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/subnet.py
--rw-r--r--   0        0        0        0 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/__init__.py
--rw-r--r--   0        0        0      253 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/client_class.py
--rw-r--r--   0        0        0      892 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/config.py
--rw-r--r--   0        0        0      341 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/lease.py
--rw-r--r--   0        0        0      533 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/pd_pool.py
--rw-r--r--   0        0        0      202 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/reservation.py
--rw-r--r--   0        0        0      296 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/server_id.py
--rw-r--r--   0        0        0      375 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/shared_network.py
--rw-r--r--   0        0        0      491 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/subnet.py
--rw-r--r--   0        0        0     1550 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/enums.py
--rw-r--r--   0        0        0      169 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/__init__.py
--rw-r--r--   0        0        0      181 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/api_response.py
--rw-r--r--   0        0        0      472 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/authentication.py
--rw-r--r--   0        0        0      278 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/base.py
--rw-r--r--   0        0        0      403 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/client_class.py
--rw-r--r--   0        0        0     1494 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/config.py
--rw-r--r--   0        0        0      396 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/control_socket.py
--rw-r--r--   0        0        0     2433 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/daemon.py
--rw-r--r--   0        0        0      734 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/database.py
--rw-r--r--   0        0        0      394 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/dhcp_common.py
--rw-r--r--   0        0        0      873 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/dhcp_ddns.py
--rw-r--r--   0        0        0      158 2023-06-03 12:18:43.045947 pykeadhcp-0.2.0/pykeadhcp/models/generic/dhcp_queue_control.py
--rw-r--r--   0        0        0      183 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/hook.py
--rw-r--r--   0        0        0      403 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/lease.py
--rw-r--r--   0        0        0      624 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/logger.py
--rw-r--r--   0        0        0      181 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/multi_threading.py
--rw-r--r--   0        0        0      364 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/option_data.py
--rw-r--r--   0        0        0      294 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/option_def.py
--rw-r--r--   0        0        0      406 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/pool.py
--rw-r--r--   0        0        0      136 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/relay.py
--rw-r--r--   0        0        0      474 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/reservation.py
--rw-r--r--   0        0        0      112 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/sanity_check.py
--rw-r--r--   0        0        0      175 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/shared_network.py
--rw-r--r--   0        0        0      244 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/sockets.py
--rw-r--r--   0        0        0      472 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/status.py
--rw-r--r--   0        0        0      385 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/models/generic/subnet.py
--rw-r--r--   0        0        0        0 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/__init__.py
--rw-r--r--   0        0        0      508 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/ctrlagent.py
--rw-r--r--   0        0        0        0 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/ddns.py
--rw-r--r--   0        0        0     2036 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/dhcp4.py
--rw-r--r--   0        0        0      522 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/dhcp6.py
--rw-r--r--   0        0        0      825 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pykeadhcp/parsers/generic.py
--rw-r--r--   0        0        0      447 2023-06-03 12:18:43.049947 pykeadhcp-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7936 1970-01-01 00:00:00.000000 pykeadhcp-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-03 22:25:51.648940 pykeadhcp-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7331 2023-06-03 22:25:51.648940 pykeadhcp-0.3.0/README.md
+-rw-r--r--   0        0        0       30 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/daemons/__init__.py
+-rw-r--r--   0        0        0     4508 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/daemons/ctrlagent.py
+-rw-r--r--   0        0        0     4526 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/daemons/ddns.py
+-rw-r--r--   0        0        0    25840 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/daemons/dhcp4.py
+-rw-r--r--   0        0        0    22098 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/daemons/dhcp6.py
+-rw-r--r--   0        0        0     2718 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/exceptions.py
+-rw-r--r--   0        0        0     7934 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/kea.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/ctrlagent/__init__.py
+-rw-r--r--   0        0        0      457 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/ctrlagent/config.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/__init__.py
+-rw-r--r--   0        0        0      331 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/client_class.py
+-rw-r--r--   0        0        0      798 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/config.py
+-rw-r--r--   0        0        0      212 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/lease.py
+-rw-r--r--   0        0        0      303 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/reservation.py
+-rw-r--r--   0        0        0      453 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/shared_network.py
+-rw-r--r--   0        0        0      684 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/subnet.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/__init__.py
+-rw-r--r--   0        0        0      253 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/client_class.py
+-rw-r--r--   0        0        0      922 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/config.py
+-rw-r--r--   0        0        0      346 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/lease.py
+-rw-r--r--   0        0        0      543 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/pd_pool.py
+-rw-r--r--   0        0        0      212 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/reservation.py
+-rw-r--r--   0        0        0      296 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/server_id.py
+-rw-r--r--   0        0        0      380 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/shared_network.py
+-rw-r--r--   0        0        0      501 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/subnet.py
+-rw-r--r--   0        0        0     1550 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/enums.py
+-rw-r--r--   0        0        0      169 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/api_response.py
+-rw-r--r--   0        0        0      477 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/authentication.py
+-rw-r--r--   0        0        0      278 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/base.py
+-rw-r--r--   0        0        0      403 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/client_class.py
+-rw-r--r--   0        0        0     1499 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/config.py
+-rw-r--r--   0        0        0      396 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/control_socket.py
+-rw-r--r--   0        0        0     2458 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/daemon.py
+-rw-r--r--   0        0        0      734 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/database.py
+-rw-r--r--   0        0        0      399 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/dhcp_common.py
+-rw-r--r--   0        0        0      873 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/dhcp_ddns.py
+-rw-r--r--   0        0        0      158 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/dhcp_queue_control.py
+-rw-r--r--   0        0        0      183 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/hook.py
+-rw-r--r--   0        0        0      403 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/lease.py
+-rw-r--r--   0        0        0      629 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/logger.py
+-rw-r--r--   0        0        0      181 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/multi_threading.py
+-rw-r--r--   0        0        0      364 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/option_data.py
+-rw-r--r--   0        0        0      294 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/option_def.py
+-rw-r--r--   0        0        0      411 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/pool.py
+-rw-r--r--   0        0        0      141 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/relay.py
+-rw-r--r--   0        0        0      484 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/reservation.py
+-rw-r--r--   0        0        0      112 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/sanity_check.py
+-rw-r--r--   0        0        0      175 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/shared_network.py
+-rw-r--r--   0        0        0      249 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/sockets.py
+-rw-r--r--   0        0        0      477 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/status.py
+-rw-r--r--   0        0        0      390 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/subnet.py
+-rw-r--r--   0        0        0      152 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/__init__.py
+-rw-r--r--   0        0        0      508 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/ctrlagent.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/ddns.py
+-rw-r--r--   0        0        0    17838 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/dhcp4.py
+-rw-r--r--   0        0        0      522 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/dhcp6.py
+-rw-r--r--   0        0        0     2915 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/exceptions.py
+-rw-r--r--   0        0        0      825 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/generic.py
+-rw-r--r--   0        0        0      447 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7936 1970-01-01 00:00:00.000000 pykeadhcp-0.3.0/PKG-INFO
```

### Comparing `pykeadhcp-0.2.0/LICENSE` & `pykeadhcp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.2.0/README.md` & `pykeadhcp-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.2.0/pykeadhcp/daemons/ctrlagent.py` & `pykeadhcp-0.3.0/pykeadhcp/daemons/ctrlagent.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.2.0/pykeadhcp/daemons/ddns.py` & `pykeadhcp-0.3.0/pykeadhcp/daemons/ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.2.0/pykeadhcp/daemons/dhcp4.py` & `pykeadhcp-0.3.0/pykeadhcp/daemons/dhcp4.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-add
         """
         lease = Lease4(ip_address=ip_address, **kwargs)
         return self.api.send_command_with_arguments(
             command="lease4-add",
             service=self.service,
-            arguments=lease.dict(exclude_none=True, by_alias=True),
+            arguments=lease.dict(exclude_none=True, exclude_unset=True, by_alias=True),
             required_hook="lease_cmds",
         )
 
     def lease4_del(self, ip_address: str) -> KeaResponse:
         """Deletes a lease from the lease database
 
         Args:
@@ -358,15 +358,15 @@
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-update
         """
         lease = Lease4(ip_address=ip_address, **kwargs)
         return self.api.send_command_with_arguments(
             command="lease4-update",
             service=self.service,
-            arguments=lease.dict(exclude_none=True, by_alias=True),
+            arguments=lease.dict(exclude_none=True, exclude_unset=True, by_alias=True),
             required_hook="lease_cmds",
         )
 
     def lease4_wipe(self, subnet_id: int) -> KeaResponse:
         """Removes all leases assosicated to the specified subnet id
 
         Args:
@@ -425,15 +425,15 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-network4-add
         """
         return self.api.send_command_with_arguments(
             command="network4-add",
             service=self.service,
             arguments={
                 "shared-networks": [
-                    network.dict(exclude_none=True, by_alias=True)
+                    network.dict(exclude_none=True, exclude_unset=True, by_alias=True)
                     for network in shared_networks
                 ]
             },
             required_hook="subnet_cmds",
         )
 
     def network4_del(self, name: str) -> KeaResponse:
@@ -632,15 +632,16 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-subnet4-add
         """
         return self.api.send_command_with_arguments(
             command="subnet4-add",
             service=self.service,
             arguments={
                 "subnet4": [
-                    subnet.dict(exclude_none=True, by_alias=True) for subnet in subnets
+                    subnet.dict(exclude_none=True, exclude_unset=True, by_alias=True)
+                    for subnet in subnets
                 ]
             },
             required_hook="subnet_cmds",
         )
 
     def subnet4_del(self, subnet_id: int) -> KeaResponse:
         """Removes a subnet
@@ -673,15 +674,16 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet4-delta-add
         """
         return self.api.send_command_with_arguments(
             command="subnet4-delta-add",
             service=self.service,
             arguments={
                 "subnet4": [
-                    subnet.dict(exclude_none=True, by_alias=True) for subnet in subnets
+                    subnet.dict(exclude_none=True, exclude_unset=True, by_alias=True)
+                    for subnet in subnets
                 ]
             },
             required_hook="subnet_cmds",
         )
 
     def subnet4_delta_del(self, subnets: List[Subnet4]) -> KeaResponse:
         """Updates (removes) parts of a single subnet
@@ -693,15 +695,16 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet4-delta-del
         """
         return self.api.send_command_with_arguments(
             command="subnet4-delta-del",
             service=self.service,
             arguments={
                 "subnet4": [
-                    subnet.dict(exclude_none=True, by_alias=True) for subnet in subnets
+                    subnet.dict(exclude_none=True, exclude_unset=True, by_alias=True)
+                    for subnet in subnets
                 ]
             },
             required_hook="subnet_cmds",
         )
 
     def subnet4_get(self, subnet_id: int) -> Subnet4:
         """Gets detailed information about the specified subnet
@@ -753,15 +756,16 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet4-update
         """
         return self.api.send_command_with_arguments(
             command="subnet4-update",
             service=self.service,
             arguments={
                 "subnet4": [
-                    subnet.dict(exclude_none=True, by_alias=True) for subnet in subnets
+                    subnet.dict(exclude_none=True, exclude_unset=True, by_alias=True)
+                    for subnet in subnets
                 ]
             },
             required_hook="subnet_cmds",
         )
 
     def version_get(self) -> KeaResponse:
         """Returns extended information about the Kea Version that is running
```

### Comparing `pykeadhcp-0.2.0/pykeadhcp/daemons/dhcp6.py` & `pykeadhcp-0.3.0/pykeadhcp/daemons/dhcp6.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease6-add
         """
         lease = Lease6(ip_address=ip_address, duid=duid, iaid=iaid, **kwargs)
 
         return self.api.send_command_with_arguments(
             command="lease6-add",
             service=self.service,
-            arguments=lease.dict(exclude_none=True, by_alias=True),
+            arguments=lease.dict(exclude_none=True, exclude_unset=True, by_alias=True),
             required_hook="lease_cmds",
         )
 
     def lease6_del(self, ip_address: str) -> KeaResponse:
         """Deletes a lease from the lease database
 
         Args:
@@ -320,15 +320,15 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-update
         """
         lease = Lease6(ip_address=ip_address, duid=duid, iaid=iaid, **kwargs)
 
         return self.api.send_command_with_arguments(
             command="lease6-update",
             service=self.service,
-            arguments=lease.dict(exclude_none=True, by_alias=True),
+            arguments=lease.dict(exclude_none=True, exclude_unset=True, by_alias=True),
             required_hook="lease_cmds",
         )
 
     def list_commands(self) -> KeaResponse:
         """List all commands supported by the server/service
 
         Kea API Reference:
@@ -348,15 +348,15 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#ref-network6-add
         """
         return self.api.send_command_with_arguments(
             command="network6-add",
             service=self.service,
             arguments={
                 "shared-networks": [
-                    network.dict(exclude_none=True, by_alias=True)
+                    network.dict(exclude_none=True, exclude_unset=True, by_alias=True)
                     for network in shared_networks
                 ]
             },
             required_hook="subnet_cmds",
         )
 
     def network6_del(self, name: str) -> KeaResponse:
@@ -504,15 +504,16 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet6-add
         """
         return self.api.send_command_with_arguments(
             command="subnet6-add",
             service=self.service,
             arguments={
                 "subnet6": [
-                    subnet.dict(exclude_none=True, by_alias=True) for subnet in subnets
+                    subnet.dict(exclude_none=True, exclude_unset=True, by_alias=True)
+                    for subnet in subnets
                 ]
             },
             required_hook="subnet_cmds",
         )
 
     def subnet6_del(self, subnet_id: int) -> KeaResponse:
         """Removes a subnet
@@ -545,15 +546,16 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet6-delta-add
         """
         return self.api.send_command_with_arguments(
             command="subnet6-delta-add",
             service=self.service,
             arguments={
                 "subnet6": [
-                    subnet.dict(exclude_none=True, by_alias=True) for subnet in subnets
+                    subnet.dict(exclude_none=True, exclude_unset=True, by_alias=True)
+                    for subnet in subnets
                 ]
             },
             required_hook="subnet_cmds",
         )
 
     def subnet6_delta_del(self, subnets: List[Subnet6]) -> KeaResponse:
         """Updates (removes) parts of a single subnet
@@ -565,15 +567,16 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet6-delta-del
         """
         return self.api.send_command_with_arguments(
             command="subnet6-delta-del",
             service=self.service,
             arguments={
                 "subnet6": [
-                    subnet.dict(exclude_none=True, by_alias=True) for subnet in subnets
+                    subnet.dict(exclude_none=True, exclude_unset=True, by_alias=True)
+                    for subnet in subnets
                 ]
             },
             required_hook="subnet_cmds",
         )
 
     def subnet6_get(self, subnet_id: int) -> Subnet6:
         """Gets detailed information about the specified subnet
@@ -625,15 +628,16 @@
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#subnet6-update
         """
         return self.api.send_command_with_arguments(
             command="subnet6-update",
             service=self.service,
             arguments={
                 "subnet6": [
-                    subnet.dict(exclude_none=True, by_alias=True) for subnet in subnets
+                    subnet.dict(exclude_none=True, exclude_unset=True, by_alias=True)
+                    for subnet in subnets
                 ]
             },
             required_hook="subnet_cmds",
         )
 
     def version_get(self) -> KeaResponse:
         """Returns extended information about the Kea Version that is running
```

### Comparing `pykeadhcp-0.2.0/pykeadhcp/exceptions.py` & `pykeadhcp-0.3.0/pykeadhcp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.2.0/pykeadhcp/kea.py` & `pykeadhcp-0.3.0/pykeadhcp/kea.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/config.py` & `pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from pykeadhcp.models.dhcp4.client_class import ClientClass4
 from pykeadhcp.models.dhcp4.shared_network import SharedNetwork4
 from pykeadhcp.models.dhcp4.subnet import Subnet4
 from pykeadhcp.models.dhcp4.reservation import Reservation4
 
 
 class Dhcp4DaemonConfig(CommonDhcpDaemonConfig):
-    client_classes: Optional[List[ClientClass4]]
-    shared_networks: Optional[List[SharedNetwork4]]
-    reservations: Optional[List[Reservation4]]
-    subnet4: Optional[List[Subnet4]]
+    client_classes: Optional[List[ClientClass4]] = []
+    shared_networks: Optional[List[SharedNetwork4]] = []
+    reservations: Optional[List[Reservation4]] = []
+    subnet4: Optional[List[Subnet4]] = []
     echo_client_id: Optional[bool]
     match_client_id: Optional[bool]
     authoritative: Optional[bool]
     next_server: Optional[str]
     server_hostname: Optional[str]
     boot_file_name: Optional[str]
```

### Comparing `pykeadhcp-0.2.0/pykeadhcp/models/dhcp4/subnet.py` & `pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/subnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     match_client_id: Optional[bool]
     authoritative: Optional[bool]
     next_server: Optional[str]
     boot_file_name: Optional[str]
     subnet_4o6_interface: Optional[str]
     subnet_4o6_interface_id: Optional[str]
     subnet_4o6_subnet: Optional[str]
-    reservations: Optional[List[Reservation4]]
+    reservations: Optional[List[Reservation4]] = []
 
     class Config:
         fields = {
             "subnet_4o6_interface": "4o6-interface",
             "subnet_4o6_interface_id": "4o6-interface-id",
             "subnet_4o6_subnet": "4o6-subnet",
         }
```

### Comparing `pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/config.py` & `pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from pykeadhcp.models.dhcp6.shared_network import SharedNetwork6
 from pykeadhcp.models.dhcp6.subnet import Subnet6
 from pykeadhcp.models.dhcp6.reservation import Reservation6
 from pykeadhcp.models.dhcp6.server_id import ServerId
 
 
 class Dhcp6DaemonConfig(CommonDhcpDaemonConfig):
-    client_classes: Optional[List[ClientClass6]]
-    shared_networks: Optional[List[SharedNetwork6]]
-    reservations: Optional[List[Reservation6]]
+    client_classes: Optional[List[ClientClass6]] = []
+    shared_networks: Optional[List[SharedNetwork6]] = []
+    reservations: Optional[List[Reservation6]] = []
     data_directory: Optional[str]
     preferred_lifetime: Optional[int]
     min_preferred_lifetime: Optional[int]
     max_preferred_lifetime: Optional[int]
-    subnet6: Optional[List[Subnet6]]
-    mac_sources: Optional[List[str]]
-    relay_supplied_options: Optional[List[str]]
+    subnet6: Optional[List[Subnet6]] = []
+    mac_sources: Optional[List[str]] = []
+    relay_supplied_options: Optional[List[str]] = []
     server_id: ServerId
```

### Comparing `pykeadhcp-0.2.0/pykeadhcp/models/dhcp6/pd_pool.py` & `pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/pd_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pykeadhcp.models.generic.option_data import OptionData
 
 
 class PDPool(KeaBaseModel):
     prefix: str
     prefix_len: int
     delegated_len: int
-    option_data: Optional[List[OptionData]]
+    option_data: Optional[List[OptionData]] = []
     client_class: Optional[str]
-    require_client_classes: Optional[List[str]]
+    require_client_classes: Optional[List[str]] = []
     excluded_prefix: Optional[str]
     excluded_prefix_len: Optional[int]
     user_context: Optional[dict]
     comment: Optional[str]
     unknown_map_entry: Optional[str]
```

### Comparing `pykeadhcp-0.2.0/pykeadhcp/models/enums.py` & `pykeadhcp-0.3.0/pykeadhcp/models/enums.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.2.0/pykeadhcp/models/generic/config.py` & `pykeadhcp-0.3.0/pykeadhcp/models/generic/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class CommonDhcpConfig(CommonConfig):
     valid_lifetime: Optional[int]
     min_valid_lifetime: Optional[int]
     max_valid_lifetime: Optional[int]
     renew_timer: Optional[int]
     rebind_timer: Optional[int]
-    option_data: Optional[List[OptionData]]
+    option_data: Optional[List[OptionData]] = []
     reservation_mode: Optional[ReservationMode]
     reservations_global: Optional[bool]
     reservations_in_subnet: Optional[bool]
     reservations_out_of_pool: Optional[bool]
     calculate_tee_times: Optional[bool]
     t1_percent: Optional[float]
     t2_percent: Optional[float]
```

### Comparing `pykeadhcp-0.2.0/pykeadhcp/models/generic/daemon.py` & `pykeadhcp-0.3.0/pykeadhcp/models/generic/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,35 +14,35 @@
     DHCPSocketTypeEnum,
     OutboundInterfaceEnum,
     HostReservationIdentifierEnum,
 )
 
 
 class CommonDaemonConfig(CommonDhcpConfig):
-    hooks_libraries: Optional[List[Hook]]
-    loggers: Optional[List[Logger]]
+    hooks_libraries: Optional[List[Hook]] = []
+    loggers: Optional[List[Logger]] = []
 
 
 class InterfaceListConfig(KeaBaseModel):
-    interfaces: List[str]
+    interfaces: List[str] = []
     dhcp_socket_type: Optional[DHCPSocketTypeEnum]
     outbound_interface: Optional[OutboundInterfaceEnum]
     re_detect: Optional[bool]
     service_sockets_require_all: Optional[bool]
     service_sockets_retry_wait_time: Optional[int]
     service_sockets_max_retries: Optional[int]
 
 
 class CommonDhcpDaemonConfig(CommonDaemonConfig):
     interfaces_config: InterfaceListConfig
     lease_database: Optional[Database]
     hosts_database: Optional[Database]
     hosts_databases: Optional[List[Database]]
-    host_reservation_identifiers: Optional[List[HostReservationIdentifierEnum]]
-    option_def: Optional[List[OptionDef]]
+    host_reservation_identifiers: Optional[List[HostReservationIdentifierEnum]] = []
+    option_def: Optional[List[OptionDef]] = []
     expired_leases_processing: Optional[dict]
     dhcp4o6_port: Optional[int]
     control_socket: Optional[ControlSocket]
     dhcp_queue_control: Optional[DHCPQueueControl]
     dhcp_ddns: Optional[DhcpDdns]
     sanity_checks: Optional[SanityCheck]
     config_control: Optional[dict]
```

### Comparing `pykeadhcp-0.2.0/pykeadhcp/models/generic/database.py` & `pykeadhcp-0.3.0/pykeadhcp/models/generic/database.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.2.0/pykeadhcp/models/generic/dhcp_ddns.py` & `pykeadhcp-0.3.0/pykeadhcp/models/generic/dhcp_ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.2.0/pykeadhcp/models/generic/logger.py` & `pykeadhcp-0.3.0/pykeadhcp/models/generic/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     maxsize: int
     maxver: int
     pattern: Optional[str]
 
 
 class Logger(KeaBaseModel):
     name: str
-    output_options: Optional[List[Output]]
+    output_options: Optional[List[Output]] = []
     debuglevel: conint(ge=0, le=100)
     severity: Optional[LoggerLevelEnum]
     user_context: Optional[dict]
     comment: Optional[str]
     unknown_map_entry: Optional[str]
 
     class Config:
```

### Comparing `pykeadhcp-0.2.0/pykeadhcp/parsers/dhcp6.py` & `pykeadhcp-0.3.0/pykeadhcp/parsers/dhcp6.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.2.0/pykeadhcp/parsers/generic.py` & `pykeadhcp-0.3.0/pykeadhcp/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.2.0/PKG-INFO` & `pykeadhcp-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeadhcp
-Version: 0.2.0
+Version: 0.3.0
 Summary: Wrapper around requests module to query ISC Kea DHCP API Daemons (ctrlagent, dhcp4, dhcp6, ddns)
 License: Apache 2.0
 Author: Brandon Spendlove
 Author-email: brandon-spendlove@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

