# Comparing `tmp/rosrestpy-0.7.1.tar.gz` & `tmp/rosrestpy-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosrestpy-0.7.1.tar", max compression
+gzip compressed data, was "rosrestpy-0.7.2.tar", max compression
```

## Comparing `rosrestpy-0.7.1.tar` & `rosrestpy-0.7.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0    35149 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/LICENSE
--rw-r--r--   0        0        0     2269 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/README.md
--rw-r--r--   0        0        0     1222 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      553 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/__init__.py
--rw-r--r--   0        0        0     2605 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/_base.py
--rw-r--r--   0        0        0     4631 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/_literals.py
--rw-r--r--   0        0        0     1296 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/_utils.py
--rw-r--r--   0        0        0      301 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/error.py
--rw-r--r--   0        0        0     1617 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/inteface/__init__.py
--rw-r--r--   0        0        0     1002 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/inteface/bridge/__init__.py
--rw-r--r--   0        0        0      686 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/inteface/bridge/bridge.py
--rw-r--r--   0        0        0      262 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/inteface/bridge/msti.py
--rw-r--r--   0        0        0      763 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/inteface/bridge/port.py
--rw-r--r--   0        0        0      322 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/inteface/bridge/vlan.py
--rw-r--r--   0        0        0     1931 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/inteface/ethernet.py
--rw-r--r--   0        0        0      754 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/inteface/interface.py
--rw-r--r--   0        0        0      572 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/inteface/list/__init__.py
--rw-r--r--   0        0        0      244 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/inteface/list/list.py
--rw-r--r--   0        0        0      246 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/inteface/list/member.py
--rw-r--r--   0        0        0     2477 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/__init__.py
--rw-r--r--   0        0        0      392 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/address.py
--rw-r--r--   0        0        0      544 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/arp.py
--rw-r--r--   0        0        0      278 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/cloud.py
--rw-r--r--   0        0        0     1285 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/dhcp_client.py
--rw-r--r--   0        0        0      470 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/dhcp_relay.py
--rw-r--r--   0        0        0      771 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/dhcp_server/__init__.py
--rw-r--r--   0        0        0      153 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/dhcp_server/_literals.py
--rw-r--r--   0        0        0     1100 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/dhcp_server/dhcp_server.py
--rw-r--r--   0        0        0     1050 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/dhcp_server/lease.py
--rw-r--r--   0        0        0      423 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/dhcp_server/network.py
--rw-r--r--   0        0        0     1032 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/dns/__init__.py
--rw-r--r--   0        0        0      126 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/dns/_literals.py
--rw-r--r--   0        0        0      195 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/dns/cache.py
--rw-r--r--   0        0        0      626 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/dns/static.py
--rw-r--r--   0        0        0     1472 2023-06-03 15:42:21.799545 rosrestpy-0.7.1/ros/ip/firewall/__init__.py
--rw-r--r--   0        0        0      282 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ip/firewall/_literals.py
--rw-r--r--   0        0        0      748 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ip/firewall/connection.py
--rw-r--r--   0        0        0     2703 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ip/firewall/filter.py
--rw-r--r--   0        0        0     2978 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ip/firewall/mangle.py
--rw-r--r--   0        0        0     2381 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ip/firewall/nat.py
--rw-r--r--   0        0        0     1042 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ip/route.py
--rw-r--r--   0        0        0      565 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ip/setting.py
--rw-r--r--   0        0        0      181 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/log.py
--rw-r--r--   0        0        0      744 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ppp/__init__.py
--rw-r--r--   0        0        0      220 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ppp/_literals.py
--rw-r--r--   0        0        0      160 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ppp/aaa.py
--rw-r--r--   0        0        0     1147 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ppp/profile.py
--rw-r--r--   0        0        0      640 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ppp/secret.py
--rw-r--r--   0        0        0      826 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/queue/__init__.py
--rw-r--r--   0        0        0      153 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/queue/interface.py
--rw-r--r--   0        0        0     2076 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/queue/simple.py
--rw-r--r--   0        0        0      726 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/queue/tree.py
--rw-r--r--   0        0        0     7146 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/ros.py
--rw-r--r--   0        0        0      604 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/routing/__init__.py
--rw-r--r--   0        0        0      467 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/routing/rule.py
--rw-r--r--   0        0        0      334 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/routing/table.py
--rw-r--r--   0        0        0     2407 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/__init__.py
--rw-r--r--   0        0        0      123 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/health.py
--rw-r--r--   0        0        0      214 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/history.py
--rw-r--r--   0        0        0      126 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/identity.py
--rw-r--r--   0        0        0      122 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/license.py
--rw-r--r--   0        0        0      248 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/logging.py
--rw-r--r--   0        0        0      146 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/note.py
--rw-r--r--   0        0        0      580 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/package/__init__.py
--rw-r--r--   0        0        0      101 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/package/_literals.py
--rw-r--r--   0        0        0      297 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/package/package.py
--rw-r--r--   0        0        0      774 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/package/update.py
--rw-r--r--   0        0        0      460 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/resource.py
--rw-r--r--   0        0        0      232 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/system/routerboard.py
--rw-r--r--   0        0        0     6722 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/tool/__init__.py
--rw-r--r--   0        0        0      223 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/tool/bandwith_server.py
--rw-r--r--   0        0        0      546 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/tool/bandwith_test.py
--rw-r--r--   0        0        0      158 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/tool/ip_scan.py
--rw-r--r--   0        0        0     1042 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/tool/netwatch.py
--rw-r--r--   0        0        0      236 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/tool/ping.py
--rw-r--r--   0        0        0      416 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/tool/torch.py
--rw-r--r--   0        0        0      290 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/tool/traceroute.py
--rw-r--r--   0        0        0     1746 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/user/__init__.py
--rw-r--r--   0        0        0      168 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/user/aaa.py
--rw-r--r--   0        0        0      167 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/user/active.py
--rw-r--r--   0        0        0      188 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/user/group.py
--rw-r--r--   0        0        0      129 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/user/settings.py
--rw-r--r--   0        0        0      205 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/user/ssh_keys.py
--rw-r--r--   0        0        0      249 2023-06-03 15:42:21.803545 rosrestpy-0.7.1/ros/user/user.py
--rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 rosrestpy-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/LICENSE
+-rw-r--r--   0        0        0     2269 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/README.md
+-rw-r--r--   0        0        0     1222 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      553 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/__init__.py
+-rw-r--r--   0        0        0     2675 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/_base.py
+-rw-r--r--   0        0        0     4631 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/_literals.py
+-rw-r--r--   0        0        0     1296 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/_utils.py
+-rw-r--r--   0        0        0      301 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/error.py
+-rw-r--r--   0        0        0     1617 2023-06-04 00:10:02.548545 rosrestpy-0.7.2/ros/inteface/__init__.py
+-rw-r--r--   0        0        0     1002 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/bridge/__init__.py
+-rw-r--r--   0        0        0      686 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/bridge/bridge.py
+-rw-r--r--   0        0        0      262 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/bridge/msti.py
+-rw-r--r--   0        0        0      763 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/bridge/port.py
+-rw-r--r--   0        0        0      322 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/bridge/vlan.py
+-rw-r--r--   0        0        0     1931 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/ethernet.py
+-rw-r--r--   0        0        0      754 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/interface.py
+-rw-r--r--   0        0        0      572 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/list/__init__.py
+-rw-r--r--   0        0        0      244 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/list/list.py
+-rw-r--r--   0        0        0      246 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/inteface/list/member.py
+-rw-r--r--   0        0        0     2477 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/__init__.py
+-rw-r--r--   0        0        0      392 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/address.py
+-rw-r--r--   0        0        0      544 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/arp.py
+-rw-r--r--   0        0        0      278 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/cloud.py
+-rw-r--r--   0        0        0     1285 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_client.py
+-rw-r--r--   0        0        0      470 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_relay.py
+-rw-r--r--   0        0        0      771 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_server/__init__.py
+-rw-r--r--   0        0        0      153 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_server/_literals.py
+-rw-r--r--   0        0        0     1100 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_server/dhcp_server.py
+-rw-r--r--   0        0        0     1050 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_server/lease.py
+-rw-r--r--   0        0        0      423 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dhcp_server/network.py
+-rw-r--r--   0        0        0     1032 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dns/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dns/_literals.py
+-rw-r--r--   0        0        0      195 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dns/cache.py
+-rw-r--r--   0        0        0      626 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/dns/static.py
+-rw-r--r--   0        0        0     1472 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/_literals.py
+-rw-r--r--   0        0        0      748 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/connection.py
+-rw-r--r--   0        0        0     2703 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/filter.py
+-rw-r--r--   0        0        0     2978 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/mangle.py
+-rw-r--r--   0        0        0     2381 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/firewall/nat.py
+-rw-r--r--   0        0        0     1042 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/route.py
+-rw-r--r--   0        0        0      565 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ip/setting.py
+-rw-r--r--   0        0        0      181 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/log.py
+-rw-r--r--   0        0        0      744 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ppp/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ppp/_literals.py
+-rw-r--r--   0        0        0      160 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ppp/aaa.py
+-rw-r--r--   0        0        0     1147 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ppp/profile.py
+-rw-r--r--   0        0        0      640 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ppp/secret.py
+-rw-r--r--   0        0        0      826 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/queue/__init__.py
+-rw-r--r--   0        0        0      153 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/queue/interface.py
+-rw-r--r--   0        0        0     2076 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/queue/simple.py
+-rw-r--r--   0        0        0      726 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/queue/tree.py
+-rw-r--r--   0        0        0     7146 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/ros.py
+-rw-r--r--   0        0        0      604 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/routing/__init__.py
+-rw-r--r--   0        0        0      467 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/routing/rule.py
+-rw-r--r--   0        0        0      334 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/routing/table.py
+-rw-r--r--   0        0        0     2407 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/__init__.py
+-rw-r--r--   0        0        0      123 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/health.py
+-rw-r--r--   0        0        0      214 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/history.py
+-rw-r--r--   0        0        0      126 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/identity.py
+-rw-r--r--   0        0        0      122 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/license.py
+-rw-r--r--   0        0        0      248 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/logging.py
+-rw-r--r--   0        0        0      146 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/note.py
+-rw-r--r--   0        0        0      580 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/package/__init__.py
+-rw-r--r--   0        0        0      101 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/package/_literals.py
+-rw-r--r--   0        0        0      297 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/package/package.py
+-rw-r--r--   0        0        0      774 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/package/update.py
+-rw-r--r--   0        0        0      460 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/resource.py
+-rw-r--r--   0        0        0      232 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/system/routerboard.py
+-rw-r--r--   0        0        0     6722 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/__init__.py
+-rw-r--r--   0        0        0      223 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/bandwith_server.py
+-rw-r--r--   0        0        0      546 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/bandwith_test.py
+-rw-r--r--   0        0        0      158 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/ip_scan.py
+-rw-r--r--   0        0        0     1042 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/netwatch.py
+-rw-r--r--   0        0        0      236 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/ping.py
+-rw-r--r--   0        0        0      416 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/torch.py
+-rw-r--r--   0        0        0      290 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/tool/traceroute.py
+-rw-r--r--   0        0        0     1746 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/__init__.py
+-rw-r--r--   0        0        0      168 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/aaa.py
+-rw-r--r--   0        0        0      167 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/active.py
+-rw-r--r--   0        0        0      188 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/group.py
+-rw-r--r--   0        0        0      129 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/settings.py
+-rw-r--r--   0        0        0      205 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/ssh_keys.py
+-rw-r--r--   0        0        0      249 2023-06-04 00:10:02.552545 rosrestpy-0.7.2/ros/user/user.py
+-rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 rosrestpy-0.7.2/PKG-INFO
```

### Comparing `rosrestpy-0.7.1/LICENSE` & `rosrestpy-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/README.md` & `rosrestpy-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/pyproject.toml` & `rosrestpy-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rosrestpy"
-version = "0.7.1"
+version = "0.7.2"
 description = "RouterOS v7 REST API python module"
 authors = ["hexatester <hexatester@protonmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/hexatester/rosrestpy"
 packages = [
     { include = "ros" },
```

### Comparing `rosrestpy-0.7.1/ros/__init__.py` & `rosrestpy-0.7.2/ros/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 from .inteface import InterfaceModule
 from .ip import IPModule
 from .ppp import PPPModule
 from .queue import QueueModule
 from .routing import RoutingModule
 from .system import SystemModule
 from .tool import ToolModule
```

### Comparing `rosrestpy-0.7.1/ros/_base.py` & `rosrestpy-0.7.2/ros/_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     filename: str = ""
 
     def __attrs_post_init__(self) -> None:
         if not self.filename:
             cname = self.__class__.__name__.lower()
             self.filename = "/" + cname.replace("module", "")
 
+    @property
+    def url(self) -> str:
+        return self.filename
+
 
 PR = TypeVar("PR", bound=object)
 
 
 @define
 class BaseProp(Generic[PR]):
     ros: "Ros"
```

### Comparing `rosrestpy-0.7.1/ros/_literals.py` & `rosrestpy-0.7.2/ros/_literals.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/_utils.py` & `rosrestpy-0.7.2/ros/_utils.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/inteface/__init__.py` & `rosrestpy-0.7.2/ros/inteface/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/inteface/bridge/__init__.py` & `rosrestpy-0.7.2/ros/inteface/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/inteface/bridge/bridge.py` & `rosrestpy-0.7.2/ros/inteface/bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/inteface/bridge/port.py` & `rosrestpy-0.7.2/ros/inteface/bridge/port.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/inteface/ethernet.py` & `rosrestpy-0.7.2/ros/inteface/ethernet.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/inteface/interface.py` & `rosrestpy-0.7.2/ros/inteface/interface.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/inteface/list/__init__.py` & `rosrestpy-0.7.2/ros/inteface/list/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/__init__.py` & `rosrestpy-0.7.2/ros/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/arp.py` & `rosrestpy-0.7.2/ros/ip/arp.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/dhcp_client.py` & `rosrestpy-0.7.2/ros/ip/dhcp_client.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/dhcp_server/__init__.py` & `rosrestpy-0.7.2/ros/ip/dhcp_server/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/dhcp_server/dhcp_server.py` & `rosrestpy-0.7.2/ros/ip/dhcp_server/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/dhcp_server/lease.py` & `rosrestpy-0.7.2/ros/ip/dhcp_server/lease.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/dns/__init__.py` & `rosrestpy-0.7.2/ros/ip/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/dns/static.py` & `rosrestpy-0.7.2/ros/ip/dns/static.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/firewall/__init__.py` & `rosrestpy-0.7.2/ros/ip/firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/firewall/connection.py` & `rosrestpy-0.7.2/ros/ip/firewall/connection.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/firewall/filter.py` & `rosrestpy-0.7.2/ros/ip/firewall/filter.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/firewall/mangle.py` & `rosrestpy-0.7.2/ros/ip/firewall/mangle.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/firewall/nat.py` & `rosrestpy-0.7.2/ros/ip/firewall/nat.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/route.py` & `rosrestpy-0.7.2/ros/ip/route.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ip/setting.py` & `rosrestpy-0.7.2/ros/ip/setting.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ppp/__init__.py` & `rosrestpy-0.7.2/ros/ppp/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ppp/profile.py` & `rosrestpy-0.7.2/ros/ppp/profile.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ppp/secret.py` & `rosrestpy-0.7.2/ros/ppp/secret.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/queue/__init__.py` & `rosrestpy-0.7.2/ros/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/queue/simple.py` & `rosrestpy-0.7.2/ros/queue/simple.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/queue/tree.py` & `rosrestpy-0.7.2/ros/queue/tree.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/ros.py` & `rosrestpy-0.7.2/ros/ros.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/routing/__init__.py` & `rosrestpy-0.7.2/ros/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/system/__init__.py` & `rosrestpy-0.7.2/ros/system/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/system/package/__init__.py` & `rosrestpy-0.7.2/ros/system/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/system/package/update.py` & `rosrestpy-0.7.2/ros/system/package/update.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/tool/__init__.py` & `rosrestpy-0.7.2/ros/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/tool/bandwith_test.py` & `rosrestpy-0.7.2/ros/tool/bandwith_test.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/tool/netwatch.py` & `rosrestpy-0.7.2/ros/tool/netwatch.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/ros/user/__init__.py` & `rosrestpy-0.7.2/ros/user/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.7.1/PKG-INFO` & `rosrestpy-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosrestpy
-Version: 0.7.1
+Version: 0.7.2
 Summary: RouterOS v7 REST API python module
 Home-page: https://github.com/hexatester/rosrestpy
 License: GPL-3.0-only
 Author: hexatester
 Author-email: hexatester@protonmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

