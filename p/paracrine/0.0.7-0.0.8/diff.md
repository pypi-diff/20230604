# Comparing `tmp/paracrine-0.0.7.tar.gz` & `tmp/paracrine-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paracrine-0.0.7.tar", last modified: Sat May 20 21:46:38 2023, max compression
+gzip compressed data, was "paracrine-0.0.8.tar", last modified: Sun Jun  4 19:48:54 2023, max compression
```

## Comparing `paracrine-0.0.7.tar` & `paracrine-0.0.8.tar`

### file list

```diff
@@ -1,64 +1,70 @@
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.135034 paracrine-0.0.7/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)    34520 2023-01-20 15:32:39.000000 paracrine-0.0.7/LICENSE
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       30 2023-01-21 23:59:01.000000 paracrine-0.0.7/MANIFEST.in
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3597 2023-05-20 21:46:38.135034 paracrine-0.0.7/PKG-INFO
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3071 2023-05-20 20:51:52.000000 paracrine-0.0.7/README.md
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4661 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/__init__.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine/commands/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/commands/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      969 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/commands/login.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      409 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/commands/reboot.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      108 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/commands/setup.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1864 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/deps.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine/helpers/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     5862 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/helpers/config.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1161 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/cron.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3492 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/debian.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)    10091 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/fs.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      896 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/network.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      412 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/python.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2382 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/systemd.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1232 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/helpers/users.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3478 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/runner.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine/runners/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/runners/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      828 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/runners/aws.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3855 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/runners/certs.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2314 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/runners/core.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine/services/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-01-25 00:04:12.000000 paracrine-0.0.7/paracrine/services/__init__.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.135034 paracrine-0.0.7/paracrine/services/cockroachdb/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1067 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/cockroachdb/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2688 2023-05-20 21:40:10.000000 paracrine-0.0.7/paracrine/services/cockroachdb/certs.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      699 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/cockroachdb/common.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      670 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/cockroachdb/init.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2441 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/cockroachdb/node.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      172 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/ntp.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4091 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/pleroma.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1242 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/postgresql.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.135034 paracrine-0.0.7/paracrine/services/wireguard/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       62 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/wireguard/__init__.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3493 2023-05-20 21:43:24.000000 paracrine-0.0.7/paracrine/services/wireguard/bootstrap.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      248 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/wireguard/common.py
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1147 2023-05-20 20:51:52.000000 paracrine-0.0.7/paracrine/services/wireguard/core.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.135034 paracrine-0.0.7/paracrine/templates/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       79 2023-01-20 15:21:51.000000 paracrine-0.0.7/paracrine/templates/certbot_requirements.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      503 2023-05-20 19:57:25.000000 paracrine-0.0.7/paracrine/templates/cockroach.service.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1774 2023-02-04 15:56:26.000000 paracrine-0.0.7/paracrine/templates/config.exs.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      121 2023-04-19 23:19:20.000000 paracrine-0.0.7/paracrine/templates/cron.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2716 2023-01-25 00:18:54.000000 paracrine-0.0.7/paracrine/templates/pleroma.nginx.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       24 2023-01-25 00:18:56.000000 paracrine-0.0.7/paracrine/templates/robots.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      300 2023-01-25 00:18:53.000000 paracrine-0.0.7/paracrine/templates/setup_db.psql.j2
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      260 2023-01-28 23:21:08.000000 paracrine-0.0.7/paracrine/templates/wg.conf.j2
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.131034 paracrine-0.0.7/paracrine.egg-info/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3597 2023-05-20 21:46:38.000000 paracrine-0.0.7/paracrine.egg-info/PKG-INFO
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1524 2023-05-20 21:46:38.000000 paracrine-0.0.7/paracrine.egg-info/SOURCES.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        1 2023-05-20 21:46:38.000000 paracrine-0.0.7/paracrine.egg-info/dependency_links.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       36 2023-05-20 21:46:38.000000 paracrine-0.0.7/paracrine.egg-info/requires.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       10 2023-05-20 21:46:38.000000 paracrine-0.0.7/paracrine.egg-info/top_level.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      871 2023-05-20 21:46:17.000000 paracrine-0.0.7/pyproject.toml
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       38 2023-05-20 21:46:38.135034 paracrine-0.0.7/setup.cfg
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 21:46:38.135034 paracrine-0.0.7/tests/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      835 2023-01-28 23:21:08.000000 paracrine-0.0.7/tests/test_ssh.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)    34520 2023-01-20 15:32:39.000000 paracrine-0.0.8/LICENSE
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       30 2023-01-21 23:59:01.000000 paracrine-0.0.8/MANIFEST.in
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3597 2023-06-04 19:48:54.506911 paracrine-0.0.8/PKG-INFO
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3071 2023-05-20 20:51:52.000000 paracrine-0.0.8/README.md
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.502911 paracrine-0.0.8/paracrine/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4661 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/__init__.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.502911 paracrine-0.0.8/paracrine/commands/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/commands/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      969 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/commands/login.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      409 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/commands/reboot.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      108 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/commands/setup.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2152 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/deps.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.502911 paracrine-0.0.8/paracrine/helpers/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/helpers/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     6180 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/helpers/config.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1282 2023-06-01 22:07:09.000000 paracrine-0.0.8/paracrine/helpers/cron.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3894 2023-06-02 18:09:42.000000 paracrine-0.0.8/paracrine/helpers/debian.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)    10423 2023-06-04 19:47:23.000000 paracrine-0.0.8/paracrine/helpers/fs.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      939 2023-06-03 22:12:18.000000 paracrine-0.0.8/paracrine/helpers/network.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      412 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/helpers/python.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2382 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/helpers/systemd.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1232 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/helpers/users.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4642 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/runner.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.502911 paracrine-0.0.8/paracrine/runners/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/runners/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      828 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/runners/aws.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3914 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/runners/certs.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2866 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/runners/core.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/paracrine/services/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        0 2023-01-25 00:04:12.000000 paracrine-0.0.8/paracrine/services/__init__.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/paracrine/services/cockroachdb/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1067 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/cockroachdb/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2712 2023-06-04 15:34:10.000000 paracrine-0.0.8/paracrine/services/cockroachdb/certs.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      699 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/cockroachdb/common.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      670 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/cockroachdb/init.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2441 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/cockroachdb/node.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      172 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/ntp.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     4091 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/pleroma.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1242 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/postgresql.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/paracrine/services/redis/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       88 2023-06-03 22:12:18.000000 paracrine-0.0.8/paracrine/services/redis/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1144 2023-06-04 19:47:23.000000 paracrine-0.0.8/paracrine/services/redis/init.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2336 2023-06-04 19:47:23.000000 paracrine-0.0.8/paracrine/services/redis/node.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/paracrine/services/wireguard/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       62 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/wireguard/__init__.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3493 2023-05-20 21:43:24.000000 paracrine-0.0.8/paracrine/services/wireguard/bootstrap.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      248 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/wireguard/common.py
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1147 2023-05-20 20:51:52.000000 paracrine-0.0.8/paracrine/services/wireguard/core.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/paracrine/templates/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       79 2023-01-20 15:21:51.000000 paracrine-0.0.8/paracrine/templates/certbot_requirements.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      503 2023-05-20 19:57:25.000000 paracrine-0.0.8/paracrine/templates/cockroach.service.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1799 2023-05-23 22:35:18.000000 paracrine-0.0.8/paracrine/templates/config.exs.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      121 2023-04-19 23:19:20.000000 paracrine-0.0.8/paracrine/templates/cron.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     2716 2023-01-25 00:18:54.000000 paracrine-0.0.8/paracrine/templates/pleroma.nginx.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      576 2023-06-04 19:47:23.000000 paracrine-0.0.8/paracrine/templates/redis-sentinel.conf.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      438 2023-06-04 19:47:23.000000 paracrine-0.0.8/paracrine/templates/redis.conf.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       24 2023-01-25 00:18:56.000000 paracrine-0.0.8/paracrine/templates/robots.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      300 2023-01-25 00:18:53.000000 paracrine-0.0.8/paracrine/templates/setup_db.psql.j2
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      260 2023-01-28 23:21:08.000000 paracrine-0.0.8/paracrine/templates/wg.conf.j2
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.502911 paracrine-0.0.8/paracrine.egg-info/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3597 2023-06-04 19:48:54.000000 paracrine-0.0.8/paracrine.egg-info/PKG-INFO
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1704 2023-06-04 19:48:54.000000 paracrine-0.0.8/paracrine.egg-info/SOURCES.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        1 2023-06-04 19:48:54.000000 paracrine-0.0.8/paracrine.egg-info/dependency_links.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       46 2023-06-04 19:48:54.000000 paracrine-0.0.8/paracrine.egg-info/requires.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       10 2023-06-04 19:48:54.000000 paracrine-0.0.8/paracrine.egg-info/top_level.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      733 2023-06-04 19:47:49.000000 paracrine-0.0.8/pyproject.toml
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       38 2023-06-04 19:48:54.506911 paracrine-0.0.8/setup.cfg
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-06-04 19:48:54.506911 paracrine-0.0.8/tests/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      835 2023-01-28 23:21:08.000000 paracrine-0.0.8/tests/test_ssh.py
```

### Comparing `paracrine-0.0.7/LICENSE` & `paracrine-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/PKG-INFO` & `paracrine-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracrine
-Version: 0.0.7
+Version: 0.0.8
 Summary: A system deployment tool
 Author-email: Tom Parker-Shemilt <palfrey@tevp.net>
 Project-URL: Homepage, https://github.com/palfrey/paracrine
 Project-URL: Bug Tracker, https://github.com/palfrey/paracrine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `paracrine-0.0.7/README.md` & `paracrine-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/__init__.py` & `paracrine-0.0.8/paracrine/__init__.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/commands/login.py` & `paracrine-0.0.8/paracrine/commands/login.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/deps.py` & `paracrine-0.0.8/paracrine/deps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import importlib
 from types import ModuleType
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from .helpers.config import set_data
+from mergedeep import merge
+
+from .helpers.config import clear_return_data, get_return_data, set_data
 
 Modules = List[Union[ModuleType, Tuple[ModuleType, Dict]]]
 """Type of modules handed to `paracrine.runner.run`"""
 
 TransmitModules = List[Union[str, Tuple[str, Dict]]]
 
 
@@ -15,23 +17,29 @@
 ) -> Dict[str, Any]:
     ret = {}
 
     def run(module: ModuleType, options: Dict):
         func: Optional[Callable] = getattr(module, name, None)
         if func is not None:
             setattr(module, "options", options)
+            clear_return_data()
             if data != {}:
                 set_data(data)
             try:
                 if module.__name__ not in ret:
                     ret[module.__name__] = []
                 if module.__name__ in arguments:
-                    ret[module.__name__].append(func(arguments[module.__name__]))
+                    info = func(arguments[module.__name__])
                 else:
-                    ret[module.__name__].append(func())
+                    info = func()
+                if isinstance(info, Dict):
+                    info = merge({}, info, get_return_data())
+                elif info is None:
+                    info = get_return_data()
+                ret[module.__name__].append(info)
             except Exception:
                 print(f"Error while running {name} for {module.__name__}")
                 raise
 
     for module in modules:
         if isinstance(module, ModuleType):
             run(module, {})
```

### Comparing `paracrine-0.0.7/paracrine/helpers/config.py` & `paracrine-0.0.8/paracrine/helpers/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import os
 import pathlib
 from typing import Any, Dict, Optional
 
 import jinja2
 import yaml
+from mergedeep import merge
 
 _jinja_env = None
 data = None
 
 CONFIG_NAME = "config.yaml"
 
 
@@ -48,14 +49,32 @@
     global _jinja_env, data
     _jinja_env = jinja2.Environment(
         loader=loader, undefined=jinja2.StrictUndefined, keep_trailing_newline=True
     )
     data = new_data
 
 
+return_data = {}
+
+
+def clear_return_data() -> None:
+    global return_data
+    return_data = {}
+
+
+def add_return_data(new_data: Dict[str, Any]) -> None:
+    global return_data
+    merge(return_data, new_data)
+
+
+def get_return_data() -> Dict:
+    global return_data
+    return return_data
+
+
 def add_folder_to_config(configs, folder, shortname=None, filter=None, prefix=""):
     if not os.path.exists(folder):
         print("Skipping %s from config as doesn't exist" % folder)
         return
     for f in os.listdir(folder):
         if filter is not None:
             if not filter(f):
```

### Comparing `paracrine-0.0.7/paracrine/helpers/cron.py` & `paracrine-0.0.8/paracrine/helpers/cron.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import pathlib
 from typing import Optional
 
 from .config import config_path, get_config_file
-from .fs import set_file_contents, set_file_contents_from_template
+from .fs import delete, set_file_contents, set_file_contents_from_template
 
 mailto: Optional[str] = None
 mailfrom: Optional[str] = None
 
 
 def local():
     global mailto, mailfrom
@@ -27,22 +27,30 @@
 
 
 def set_mailfrom(email: str) -> None:
     global mailfrom
     mailfrom = email
 
 
+def cron_path(name: str):
+    return f"/etc/cron.d/{name}"
+
+
 def create_cron(name: str, schedule: str, user: str, command: str):
     cron_info = json.loads(get_config_file("configs/cron-info"))
     envs = {}
     if cron_info["mailto"] is not None:
         envs["MAILTO"] = cron_info["mailto"]
     if cron_info["mailfrom"] is not None:
         envs["MAILFROM"] = cron_info["mailfrom"]
     set_file_contents_from_template(
-        f"/etc/cron.d/{name}",
+        cron_path(name),
         "cron.j2",
         SCHEDULE=schedule,
         USER=user,
         COMMAND=command,
         ENVS=envs,
     )
+
+
+def delete_cron(name: str):
+    delete(cron_path(name))
```

### Comparing `paracrine-0.0.7/paracrine/helpers/debian.py` & `paracrine-0.0.8/paracrine/helpers/debian.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import re
 from glob import glob
+from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 from debian.debian_support import version_compare
 
 from .fs import (
     build_with_command,
     download,
@@ -45,51 +46,60 @@
 
 # List is just "any version", Dict is a "name => min version" requirement
 def apt_install(
     packages: Union[List[str], Dict[str, Optional[str]]],
     always_install: bool = False,
     target_release: Optional[str] = None,
 ) -> bool:
-    apt_update()
     global host_arch
     if host_arch is None and packages != ["dpkg-dev"]:
         apt_install(["dpkg-dev"])
-        host_arch = run_command("dpkg-architecture -q DEB_HOST_ARCH").strip()
+        host_arch_path = Path("/opt/host-arch")
+        build_with_command(
+            host_arch_path, f"dpkg-architecture -q DEB_HOST_ARCH > {host_arch_path}"
+        )
+        host_arch = host_arch_path.open().read().strip()
     if isinstance(packages, List):
         packages = dict([(p, None) for p in packages])
     if always_install:
         to_install = list(packages.keys())
     else:
-        to_install = []
+        to_install = {}
         for package in packages.keys():
             paths = [
                 f"/var/lib/dpkg/info/{package}.list",
                 f"/var/lib/dpkg/info/{package}:{host_arch}.list",
             ]
+            wanted_version = packages[package]
             for path in paths:
                 if not os.path.exists(path):
                     continue
-                wanted_version = packages[package]
                 if wanted_version is None:  # existance is enough
                     break
                 status = run_command(f"dpkg-query --status {package}")
                 version = _version_pattern.search(status).group(1)
                 if version_compare(version, wanted_version) >= 0:
                     break
             else:
-                to_install.append(package)
+                to_install[package] = wanted_version
 
-        if to_install == []:
+        if to_install == {}:
             return False
 
+    apt_update()
     # Confdef is to fix https://unix.stackexchange.com/a/416816/73838
     os.environ["DEBIAN_FRONTEND"] = "noninteractive"
     cmd = (
         "apt-get install %s --no-install-recommends --yes -o DPkg::Options::=--force-confdef"
-        % " ".join(to_install)
+        % " ".join(
+            [
+                name if version is None else f"{name}>={version}"
+                for (name, version) in to_install.items()
+            ]
+        )
     )
     if target_release is not None:
         cmd += f" --target-release {target_release}"
     run_command(cmd)
     return True
 
 
@@ -97,16 +107,20 @@
     fname = "/etc/apt/sources.list.d/%s.list" % name
     if contents is None:
         contents = "deb http://deb.debian.org/debian %s main" % name
 
     changed = set_file_contents(fname, contents)
     if changed:
         apt_update()
+    return changed
 
 
 def set_alternative(alt_name: str, option: str):
     current_alt_path = os.path.realpath(f"/etc/alternatives/{alt_name}")
     if current_alt_path != option:
         print(
             f"current alt path for {alt_name} is {current_alt_path} not {option}, so fixing"
         )
         run_command(f"update-alternatives --set {alt_name} {option}")
+        return True
+    else:
+        return False
```

### Comparing `paracrine-0.0.7/paracrine/helpers/fs.py` & `paracrine-0.0.8/paracrine/helpers/fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,18 +60,22 @@
             open(fname, "wb").write(contents)
 
     needs_update = set_owner(fname, owner, group) or needs_update
 
     return needs_update
 
 
+def render_template(template, **kwargs):
+    return jinja_env().get_template(template).render(**kwargs)
+
+
 def set_file_contents_from_template(fname, template, ignore_changes=False, **kwargs):
     return set_file_contents(
         fname,
-        jinja_env().get_template(template).render(**kwargs),
+        render_template(template, **kwargs),
         ignore_changes=ignore_changes,
     )
 
 
 def set_file_contents_from_data(fname: str, data_path: str):
     return set_file_contents(fname, data_files()[data_path])
 
@@ -142,23 +146,25 @@
     existing = open(fname).read()
     if line not in existing:
         return set_file_contents(fname, existing + "\n" + line)
     else:
         return False
 
 
-def insert_or_replace(fname: str, matcher: re.Pattern, line: str) -> None:
+def insert_or_replace(fname: str, matcher: Union[re.Pattern, str], line: str) -> bool:
     existing = open(fname).read()
-    results = matcher.search(existing)
-    if results is not None:
-        set_file_contents(
-            fname, existing[: results.start()] + line + existing[results.end() :]
-        )
-    else:
-        set_file_contents(fname, existing + "\n" + line)
+    if isinstance(matcher, re.Pattern):
+        results = matcher.search(existing)
+        if results is not None:
+            return set_file_contents(
+                fname, existing[: results.start()] + line + existing[results.end() :]
+            )
+    elif matcher in existing:
+        return set_file_contents(fname, existing.replace(matcher, line))
+    return set_file_contents(fname, existing + "\n" + line)
 
 
 def sha_file(fname):
     from .debian import apt_install
 
     apt_install(["coreutils"])
     existing_sha = run_command("sha256sum %s" % fname).strip()
@@ -292,15 +298,21 @@
             run_command(command, directory=directory)
         return True
     else:
         return False
 
 
 def run_with_marker(
-    fname, command, deps=[], max_age=None, force_build=False, directory=None
+    fname,
+    command,
+    deps=[],
+    max_age=None,
+    force_build=False,
+    directory=None,
+    input: Optional[str] = None,
 ):
     changed = not os.path.exists(fname) or force_build
     target_modified = last_modified(fname)
     if max_age is not None:
         age = datetime.now() - datetime.fromtimestamp(target_modified)
         if age > max_age:
             changed = True
@@ -308,15 +320,15 @@
         dep_modified = last_modified(dep)
         if dep_modified > target_modified:
             logging.info("%s is younger than %s" % (dep, fname))
             changed = True
             break
 
     if changed:
-        run_command(command, directory=directory)
+        run_command(command, directory=directory, input=input)
         open(fname, "w").write(command)
 
     return changed
 
 
 def run_command(
     cmd: str,
```

### Comparing `paracrine-0.0.7/paracrine/helpers/network.py` & `paracrine-0.0.8/paracrine/helpers/network.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Dict
+
 from .config import host, network_config, other_config, servers
 
 
 def networks_by_interface(h):
     return dict([(intf["ifname"], intf) for intf in network_config(h["name"])])
 
 
@@ -17,15 +19,15 @@
     return other_config(h["name"])["external_ip"]
 
 
 def external_ips():
     return dict([(h["name"], external_ip(h)) for h in servers()])
 
 
-def wireguard_ips():
+def wireguard_ips() -> Dict[str, str]:
     return dict([(h["name"], h["wireguard_ip"]) for h in servers()])
 
 
 def wireguard_ip():
     return host()["wireguard_ip"]
```

### Comparing `paracrine-0.0.7/paracrine/helpers/systemd.py` & `paracrine-0.0.8/paracrine/helpers/systemd.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/helpers/users.py` & `paracrine-0.0.8/paracrine/helpers/users.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/runner.py` & `paracrine-0.0.8/paracrine/runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,74 @@
+import json
 import logging
 import os
 from typing import Any, Callable, Dict
 
+from mergedeep import merge
 from mitogen.core import Error, StreamError
-from mitogen.parent import Router
+from mitogen.parent import Context, Router
 from mitogen.utils import run_with_router
 
 from .deps import Modules, TransmitModules, makereal, maketransmit, runfunc
 from .helpers.config import (
     create_data,
     get_config,
+    other_config_file,
     path_to_config_file,
     set_config,
     set_data,
 )
+from .helpers.fs import set_file_contents
 from .runners import core
 
 
 def decode(info):
     for k in list(info.keys()):
         if type(k) == bytes:
             info[k.decode()] = info[k].decode()
             del info[k]
 
 
+ssh_cache: Dict[str, Context] = {}
+
+
 def main(router: Router, func: Callable[..., None], *args: Any, **kwargs: Any) -> Dict:
     config = get_config()
     calls = []
     wg = core.is_wireguard()
     data = None
     for server in config["servers"]:
         assert isinstance(server, Dict)
         hostname = server["wireguard_ip"] if wg else server["ssh_hostname"]
         port = 22 if wg else server.get("ssh_port", 22)
-        key_path = path_to_config_file(server["ssh_key"])
-        if not os.path.exists(key_path):
-            raise Exception(f"Can't find ssh key {key_path}")
-        try:
-            connect = router.ssh(
-                hostname=hostname,
-                port=port,
-                username=server["ssh_user"],
-                identity_file=key_path,
-                check_host_keys="accept",
-                python_path="python3",
-            )
-        except StreamError:
-            print(
-                "Exception while trying to login to %s@%s:%s"
-                % (server["ssh_user"], hostname, port)
-            )
-            raise
+        cache_key = f"{hostname}-{port}"
+        if cache_key not in ssh_cache:
+            key_path = path_to_config_file(server["ssh_key"])
+            if not os.path.exists(key_path):
+                raise Exception(f"Can't find ssh key {key_path}")
+            try:
+                connect = router.ssh(
+                    hostname=hostname,
+                    port=port,
+                    username=server["ssh_user"],
+                    identity_file=key_path,
+                    check_host_keys="accept",
+                    python_path="python3",
+                )
+            except StreamError:
+                print(
+                    "Exception while trying to login to %s@%s:%s"
+                    % (server["ssh_user"], hostname, port)
+                )
+                raise
 
-        sudo = router.sudo(via=connect, python_path="python3")
+            sudo = router.sudo(via=connect, python_path="python3")
+            ssh_cache[cache_key] = sudo
         data = create_data(server=server)
-        calls.append(sudo.call_async(func, data, *args, **kwargs))
+        calls.append(ssh_cache[cache_key].call_async(func, data, *args, **kwargs))
 
     infos = []
     errors = []
     for call in calls:
         try:
             info = call.get().unpickle()
             if info is not None:
@@ -84,14 +94,30 @@
     router: Router, modules: Modules, local_func: str, run_func: str, parse_func: str
 ) -> None:
     for module in modules:
         runfunc([module], local_func)
         infos = main(router, do, maketransmit([module]), run_func)
         for info in infos["infos"]:
             runfunc([module], parse_func, info, infos["data"])
+            for module_name in info:
+                for per_node in info[module_name]:
+                    if not isinstance(per_node, Dict):
+                        continue
+                    if "selector" not in per_node:
+                        continue
+                    config_path = other_config_file("selectors.json")
+                    if os.path.exists(config_path):
+                        selector_config = json.load(open(config_path))
+                    else:
+                        selector_config = {}
+                    merge(selector_config, per_node["selector"])
+                    selector_config = dict(sorted(selector_config.items()))
+                    set_file_contents(
+                        config_path, json.dumps(selector_config, indent=2)
+                    )
 
 
 def run(inventory_path: str, modules: Modules):
     logging.basicConfig()
     logging.root.setLevel(logging.INFO)
     set_config(inventory_path)
```

### Comparing `paracrine-0.0.7/paracrine/runners/aws.py` & `paracrine-0.0.8/paracrine/runners/aws.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/runners/certs.py` & `paracrine-0.0.8/paracrine/runners/certs.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,8 +112,10 @@
 
 
 def parse_return(
     infos: List[Dict],
 ) -> None:
     for info in infos:
         for key in info:
+            if key == "selector":
+                continue
             open(other_config_file(key), "w").write(info[key])
```

### Comparing `paracrine-0.0.7/paracrine/runners/core.py` & `paracrine-0.0.8/paracrine/runners/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
 import os
 import socket
 from pathlib import Path
 from typing import Dict, List
 
 from ..helpers.config import (
+    add_return_data,
     config,
     host,
     in_docker,
     network_config_file,
+    other_config,
     other_config_file,
 )
 from ..helpers.debian import apt_install
 from ..helpers.fs import run_command
 from ..helpers.users import in_vagrant, users
 
 
@@ -20,20 +22,35 @@
     return os.path.exists("/etc/wireguard")
 
 
 def hash_fn(key: str, count: int) -> int:
     return sum(bytearray(key.encode("utf-8"))) % count
 
 
+def _index_fn(name: str) -> Dict:
+    hosts = config()["servers"]
+    try:
+        existing_selectors = other_config("selectors.json")
+        return [host for host in hosts if host["name"] == existing_selectors[name]][0]
+    except KeyError:
+        index = hash_fn(name, len(hosts))
+        add_return_data({"selector": {name: hosts[index]["name"]}})
+        return hosts[index]
+
+
 # Use this host for a given service
 # Intended for "run on one machine" things
 def use_this_host(name: str) -> bool:
-    hosts = [h["name"] for h in config()["servers"]]
-    index = hash_fn(name, len(hosts))
-    return host()["name"] == hosts[index]
+    use_host = _index_fn(name)
+    return host()["name"] == use_host["name"]
+
+
+def wireguard_ip_for_machine_for(name: str) -> str:
+    use_host = _index_fn(name)
+    return use_host["wireguard_ip"]
 
 
 def run():
     apt_install(["iproute2"])
 
     data = {
         "hostname": socket.gethostname(),
@@ -44,18 +61,22 @@
     }
     ip_file = Path("/opt/ip_address")
     if ip_file.exists():
         data["external_ip"] = json.load(ip_file.open())
     else:
         if in_vagrant() or in_docker():
             networks = json.loads(data["network_devices"])
-            ext_if = [net for net in networks if net["ifname"] == "eth0"]
-            if len(ext_if) > 0 and len(ext_if[0]["addr_info"]) > 0:
+            ext_if = [
+                net
+                for net in networks
+                if net["ifname"].startswith("eth") and len(net["addr_info"]) > 0
+            ]
+            if len(ext_if) > 0:
                 data["external_ip"] = json.dumps(
-                    {"ip": ext_if[0]["addr_info"][0]["local"]}
+                    {"ip": ext_if[-1]["addr_info"][0]["local"]}
                 )
             else:
                 data["external_ip"] = "<unknown>"
         else:
             apt_install(["curl", "ca-certificates"])
             data["external_ip"] = run_command("curl https://api.ipify.org?format=json")
         json.dump(data["external_ip"], ip_file.open("w"))
```

### Comparing `paracrine-0.0.7/paracrine/services/cockroachdb/__init__.py` & `paracrine-0.0.8/paracrine/services/cockroachdb/__init__.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/services/cockroachdb/certs.py` & `paracrine-0.0.8/paracrine/services/cockroachdb/certs.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         "node_keys": node_keys,
     }
 
 
 def parse_return(infos: List[Optional[Dict]]):
     assert len(infos) == 1, infos
     info = infos[0]
-    if info is None:
+    if info is None or "ca_crt" not in info:
         return
     certs_dir = Path(config_path()).joinpath("cockroach-certs")
     make_directory(certs_dir)
     set_file_contents(certs_dir.joinpath("ca.crt"), info["ca_crt"])
     set_file_contents(certs_dir.joinpath("client.root.key"), info["root_key"])
     set_file_contents(certs_dir.joinpath("client.root.crt"), info["root_crt"])
```

### Comparing `paracrine-0.0.7/paracrine/services/cockroachdb/common.py` & `paracrine-0.0.8/paracrine/services/cockroachdb/common.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/services/cockroachdb/init.py` & `paracrine-0.0.8/paracrine/services/cockroachdb/init.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/services/cockroachdb/node.py` & `paracrine-0.0.8/paracrine/services/cockroachdb/node.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/services/pleroma.py` & `paracrine-0.0.8/paracrine/services/pleroma.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/services/postgresql.py` & `paracrine-0.0.8/paracrine/services/postgresql.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/services/wireguard/bootstrap.py` & `paracrine-0.0.8/paracrine/services/wireguard/bootstrap.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/services/wireguard/core.py` & `paracrine-0.0.8/paracrine/services/wireguard/core.py`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine/templates/config.exs.j2` & `paracrine-0.0.8/paracrine/templates/config.exs.j2`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,16 @@
    signing_salt: "{{ SIGNING_SALT }}"
 
 config :pleroma, :instance,
   name: "{{ PLEROMA_HOST }}",
   email: "{{ PLEROMA_EMAIL }}",
   notify_email: "{{ PLEROMA_EMAIL }}",
   limit: 5000,
-  registrations_open: false
+  registrations_open: false,
+  invites_enabled: true
 
 config :pleroma, :media_proxy,
   enabled: false,
   redirect_on_failure: true
   #base_url: "https://cache.pleroma.social"
 
 config :pleroma, Pleroma.Repo,
```

### Comparing `paracrine-0.0.7/paracrine/templates/pleroma.nginx.j2` & `paracrine-0.0.8/paracrine/templates/pleroma.nginx.j2`

 * *Files identical despite different names*

### Comparing `paracrine-0.0.7/paracrine.egg-info/PKG-INFO` & `paracrine-0.0.8/paracrine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracrine
-Version: 0.0.7
+Version: 0.0.8
 Summary: A system deployment tool
 Author-email: Tom Parker-Shemilt <palfrey@tevp.net>
 Project-URL: Homepage, https://github.com/palfrey/paracrine
 Project-URL: Bug Tracker, https://github.com/palfrey/paracrine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `paracrine-0.0.7/paracrine.egg-info/SOURCES.txt` & `paracrine-0.0.8/paracrine.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,20 +32,25 @@
 paracrine/services/pleroma.py
 paracrine/services/postgresql.py
 paracrine/services/cockroachdb/__init__.py
 paracrine/services/cockroachdb/certs.py
 paracrine/services/cockroachdb/common.py
 paracrine/services/cockroachdb/init.py
 paracrine/services/cockroachdb/node.py
+paracrine/services/redis/__init__.py
+paracrine/services/redis/init.py
+paracrine/services/redis/node.py
 paracrine/services/wireguard/__init__.py
 paracrine/services/wireguard/bootstrap.py
 paracrine/services/wireguard/common.py
 paracrine/services/wireguard/core.py
 paracrine/templates/certbot_requirements.txt
 paracrine/templates/cockroach.service.j2
 paracrine/templates/config.exs.j2
 paracrine/templates/cron.j2
 paracrine/templates/pleroma.nginx.j2
+paracrine/templates/redis-sentinel.conf.j2
+paracrine/templates/redis.conf.j2
 paracrine/templates/robots.txt
 paracrine/templates/setup_db.psql.j2
 paracrine/templates/wg.conf.j2
 tests/test_ssh.py
```

### Comparing `paracrine-0.0.7/pyproject.toml` & `paracrine-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [project]
 name = "paracrine"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Tom Parker-Shemilt", email="palfrey@tevp.net" },
 ]
 description = "A system deployment tool"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
-dependencies=["mitogen", "jinja2", "pyyaml", "python-debian"]
+dependencies=["mitogen", "jinja2", "pyyaml", "python-debian", "mergedeep"]
 
 [project.urls]
 "Homepage" = "https://github.com/palfrey/paracrine"
 "Bug Tracker" = "https://github.com/palfrey/paracrine/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-include = ["paracrine", "paracrine.services", "paracrine.services.wireguard", "paracrine.services.cockroachdb", "paracrine.commands", "paracrine.helpers", "paracrine.runners"]
+include = ["paracrine*"]
```

### Comparing `paracrine-0.0.7/tests/test_ssh.py` & `paracrine-0.0.8/tests/test_ssh.py`

 * *Files identical despite different names*

