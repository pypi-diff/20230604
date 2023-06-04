# Comparing `tmp/domain-admin-1.3.1.tar.gz` & `tmp/domain-admin-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domain-admin-1.3.1.tar", last modified: Sun Jun  4 11:01:48 2023, max compression
+gzip compressed data, was "domain-admin-1.3.2.tar", last modified: Sun Jun  4 11:20:37 2023, max compression
```

## Comparing `domain-admin-1.3.1.tar` & `domain-admin-1.3.2.tar`

### file list

```diff
@@ -1,236 +1,236 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.293270 domain-admin-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-04 11:01:38.000000 domain-admin-1.3.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-04 11:01:38.000000 domain-admin-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-06-04 11:01:48.293270 domain-admin-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-04 11:01:38.000000 domain-admin-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.277270 domain-admin-1.3.1/domain_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.277270 domain-admin-1.3.1/domain_admin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/address_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/cert_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/domain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/ip_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/log_scheduler_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/notify_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/api/whois_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.277270 domain-admin-1.3.1/domain_admin/config/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/config/default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.277270 domain-admin-1.3.1/domain_admin/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/enums/notify_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/enums/version_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.277270 domain-admin-1.3.1/domain_admin/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/migrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/migrate/migrate_102_to_103.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/migrate/migrate_106_to_110.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/migrate/migrate_110_to_1212.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/migrate/migrate_1212_to_1213.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/migrate/migrate_1213_to_131.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.277270 domain-admin-1.3.1/domain_admin/model/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/address_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/cache_domain_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/log_scheduler_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/notify_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/system_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/model/version_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.277270 domain-admin-1.3.1/domain_admin/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-06-04 11:01:46.000000 domain-admin-1.3.1/domain_admin/public/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.273270 domain-admin-1.3.1/domain_admin/public/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.273270 domain-admin-1.3.1/domain_admin/public/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.273270 domain-admin-1.3.1/domain_admin/public/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/0e/
--r--r--r--   0 runner    (1001) docker     (123)     3175 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/0e/d7eb4a521f152c1f9bd95e7eb480c1f09165ae
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/28/
--r--r--r--   0 runner    (1001) docker     (123)     4038 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/28/420029335fa4e1347a9749ff4900dcb509813d
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/35/
--r--r--r--   0 runner    (1001) docker     (123)    12130 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/35/c7d9b593caf78d8bc26ca2d5c705319df64bce
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/39/
--r--r--r--   0 runner    (1001) docker     (123)      585 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/39/8a6e00e326b167bbbbafeae3fbfdac6bc16179
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/40/
--r--r--r--   0 runner    (1001) docker     (123)      229 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/40/60293e2ea143c10233675d3b2a12c7df256566
--r--r--r--   0 runner    (1001) docker     (123)      437 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/40/74e54058b5de2fe8e8f0f64fafa41851da289e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/46/
--r--r--r--   0 runner    (1001) docker     (123)     1441 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/46/02beb67fcbd0847be12eac9564f6cc074b586b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/52/
--r--r--r--   0 runner    (1001) docker     (123)    62564 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/54/
--r--r--r--   0 runner    (1001) docker     (123)   279771 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/54/c186d682acad66785d7fc148ceeef6b4ad0946
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/57/
--r--r--r--   0 runner    (1001) docker     (123)     1429 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/57/e5db996081ddbd7008afae5c24b23e9f2417a9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/6a/
--r--r--r--   0 runner    (1001) docker     (123)      989 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/6a/88267aadd02ec9f25862b364fa6bf5c090ea6a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/6c/
--r--r--r--   0 runner    (1001) docker     (123)      223 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/6c/9dc4623cf1fb08b71b8478bb3531d5b2e29ea6
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/6f/
--r--r--r--   0 runner    (1001) docker     (123)    73032 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/6f/cd2c55887a9ccc2f613a9a60b501ebfd38c893
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/78/
--r--r--r--   0 runner    (1001) docker     (123)      150 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/78/89b97dbf667fed699345ebc14e30c012cfc0e8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/92/
--r--r--r--   0 runner    (1001) docker     (123)      141 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/92/10349e182e675aa2021dd2aabc15f539796480
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/ad/
--r--r--r--   0 runner    (1001) docker     (123)      464 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/ad/77a2a7ab2da9fec1ce861f5d70071d8367f4f4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/b2/
--r--r--r--   0 runner    (1001) docker     (123)      462 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/b2/066831e02035414ce060599a69c4b61ca7826a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/b3/
--r--r--r--   0 runner    (1001) docker     (123)    41902 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
--r--r--r--   0 runner    (1001) docker     (123)      130 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/b3/9249471f41dc154ccbabd607bb322c92b292fd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/d2/
--r--r--r--   0 runner    (1001) docker     (123)     3194 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/d2/bb330b9eb09960c48b9881a9a5a911f2610909
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/da/
--r--r--r--   0 runner    (1001) docker     (123)      586 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/da/906831a48153c2aab0584132a4c640237894c5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.281270 domain-admin-1.3.1/domain_admin/public/.git/objects/e0/
--r--r--r--   0 runner    (1001) docker     (123)     4443 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/e0/070199d593788b787f27da1f0d67ec7b94b277
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.285270 domain-admin-1.3.1/domain_admin/public/.git/objects/e4/
--r--r--r--   0 runner    (1001) docker     (123)    62418 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/e4/22b4250d248909013befbeac5f70b8b651c014
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.285270 domain-admin-1.3.1/domain_admin/public/.git/objects/e6/
--r--r--r--   0 runner    (1001) docker     (123)    10076 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/objects/e6/ad2c129e0ca20fc7903657a4555a64062df9a3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.273270 domain-admin-1.3.1/domain_admin/public/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.285270 domain-admin-1.3.1/domain_admin/public/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.273270 domain-admin-1.3.1/domain_admin/public/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.285270 domain-admin-1.3.1/domain_admin/public/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.285270 domain-admin-1.3.1/domain_admin/public/css/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/css/index.3c8142bf.css
--rw-r--r--   0 runner    (1001) docker     (123)   324879 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/css/index.56f1f605.css
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/css/index.6730720e.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.285270 domain-admin-1.3.1/domain_admin/public/js/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/ConnectStatus.1b8b9c89.js
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/SelectGroup.bb54ab1b.js
--rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/element-icon.1ce1c350.js
--rw-r--r--   0 runner    (1001) docker     (123)   749550 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/element-plus.d9ab67b4.js
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/index.1918b941.js
--rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/index.353f6c08.js
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/index.7e1bfc76.js
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/index.87f37741.js
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/index.8ca50aef.js
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/index.94134290.js
--rw-r--r--   0 runner    (1001) docker     (123)   219500 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/index.9da88c42.js
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/index.c00b6c6b.js
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/validator.0c34c3e7.js
--rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/vendor-lib.65d1e499.js
--rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-06-04 11:01:47.000000 domain-admin-1.3.1/domain_admin/public/js/vendor-vue.9e61e0af.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.285270 domain-admin-1.3.1/domain_admin/router/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/router/api_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/router/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.289270 domain-admin-1.3.1/domain_admin/service/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/async_task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/cache_domain_info_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/email_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/global_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/group_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/notify_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/render_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/scheduler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/system_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/token_service.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/version_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/service/work_weixin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.289270 domain-admin-1.3.1/domain_admin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/templates/domain-cert-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/templates/domain-export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.289270 domain-admin-1.3.1/domain_admin/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/bcrypt_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.289270 domain-admin-1.3.1/domain_admin/utils/cert_util/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/cert_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/cert_util/cert_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/cert_util/cert_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/cert_util/cert_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/cert_util/cert_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/cert_util/cert_socket_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/datetime_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/domain_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.289270 domain-admin-1.3.1/domain_admin/utils/flask_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/api_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/app_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/flask_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/http_code_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.289270 domain-admin-1.3.1/domain_admin/utils/flask_ext/json/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/json/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/json/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/json/json_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/flask_ext/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/json_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.289270 domain-admin-1.3.1/domain_admin/utils/peewee_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/peewee_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/peewee_ext/model_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/secret_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/text_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.293270 domain-admin-1.3.1/domain_admin/utils/whois_util/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/whois_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/whois_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/whois_util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/whois_util/whois-servers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/whois_util/whois_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/utils/work_weixin_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-06-04 11:01:38.000000 domain-admin-1.3.1/domain_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.277270 domain-admin-1.3.1/domain_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-06-04 11:01:48.000000 domain-admin-1.3.1/domain_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-06-04 11:01:48.000000 domain-admin-1.3.1/domain_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 11:01:48.000000 domain-admin-1.3.1/domain_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-04 11:01:48.000000 domain-admin-1.3.1/domain_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-04 11:01:48.000000 domain-admin-1.3.1/domain_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 11:01:48.000000 domain-admin-1.3.1/domain_admin.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:01:48.293270 domain-admin-1.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-04 11:01:38.000000 domain-admin-1.3.1/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 11:01:48.293270 domain-admin-1.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1928 2023-06-04 11:01:38.000000 domain-admin-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.415659 domain-admin-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-04 11:20:27.000000 domain-admin-1.3.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-04 11:20:27.000000 domain-admin-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-06-04 11:20:37.415659 domain-admin-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-04 11:20:27.000000 domain-admin-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.383659 domain-admin-1.3.2/domain_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.387659 domain-admin-1.3.2/domain_admin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/address_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/cert_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/domain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/ip_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/log_scheduler_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/notify_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/api/whois_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.387659 domain-admin-1.3.2/domain_admin/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/config/default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.387659 domain-admin-1.3.2/domain_admin/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/enums/notify_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/enums/version_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.387659 domain-admin-1.3.2/domain_admin/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/migrate/migrate_102_to_103.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/migrate/migrate_106_to_110.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/migrate/migrate_110_to_1212.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/migrate/migrate_1212_to_1213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/migrate/migrate_1213_to_131.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.391659 domain-admin-1.3.2/domain_admin/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/address_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/cache_domain_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/log_scheduler_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/notify_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/system_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/model/version_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.391659 domain-admin-1.3.2/domain_admin/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.391659 domain-admin-1.3.2/domain_admin/public/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.375659 domain-admin-1.3.2/domain_admin/public/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.375659 domain-admin-1.3.2/domain_admin/public/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.379659 domain-admin-1.3.2/domain_admin/public/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/0e/
+-r--r--r--   0 runner    (1001) docker     (123)     3175 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/0e/d7eb4a521f152c1f9bd95e7eb480c1f09165ae
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/28/
+-r--r--r--   0 runner    (1001) docker     (123)     4038 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/28/420029335fa4e1347a9749ff4900dcb509813d
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/35/
+-r--r--r--   0 runner    (1001) docker     (123)    12130 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/35/c7d9b593caf78d8bc26ca2d5c705319df64bce
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/39/
+-r--r--r--   0 runner    (1001) docker     (123)      585 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/39/8a6e00e326b167bbbbafeae3fbfdac6bc16179
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/40/
+-r--r--r--   0 runner    (1001) docker     (123)      229 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/40/60293e2ea143c10233675d3b2a12c7df256566
+-r--r--r--   0 runner    (1001) docker     (123)      437 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/40/74e54058b5de2fe8e8f0f64fafa41851da289e
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/46/
+-r--r--r--   0 runner    (1001) docker     (123)     1441 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/46/02beb67fcbd0847be12eac9564f6cc074b586b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/52/
+-r--r--r--   0 runner    (1001) docker     (123)    62564 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/54/
+-r--r--r--   0 runner    (1001) docker     (123)   279771 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/54/c186d682acad66785d7fc148ceeef6b4ad0946
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/57/
+-r--r--r--   0 runner    (1001) docker     (123)     1429 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/57/e5db996081ddbd7008afae5c24b23e9f2417a9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/6a/
+-r--r--r--   0 runner    (1001) docker     (123)      989 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/6a/88267aadd02ec9f25862b364fa6bf5c090ea6a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/6c/
+-r--r--r--   0 runner    (1001) docker     (123)      223 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/6c/9dc4623cf1fb08b71b8478bb3531d5b2e29ea6
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/6f/
+-r--r--r--   0 runner    (1001) docker     (123)    73032 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/6f/cd2c55887a9ccc2f613a9a60b501ebfd38c893
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.395659 domain-admin-1.3.2/domain_admin/public/.git/objects/78/
+-r--r--r--   0 runner    (1001) docker     (123)      150 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/78/89b97dbf667fed699345ebc14e30c012cfc0e8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/.git/objects/92/
+-r--r--r--   0 runner    (1001) docker     (123)      141 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/92/10349e182e675aa2021dd2aabc15f539796480
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/.git/objects/ad/
+-r--r--r--   0 runner    (1001) docker     (123)      464 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/ad/77a2a7ab2da9fec1ce861f5d70071d8367f4f4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/.git/objects/b2/
+-r--r--r--   0 runner    (1001) docker     (123)      462 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/b2/066831e02035414ce060599a69c4b61ca7826a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/.git/objects/b3/
+-r--r--r--   0 runner    (1001) docker     (123)    41902 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
+-r--r--r--   0 runner    (1001) docker     (123)      130 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/b3/9249471f41dc154ccbabd607bb322c92b292fd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/.git/objects/d2/
+-r--r--r--   0 runner    (1001) docker     (123)     3194 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/d2/bb330b9eb09960c48b9881a9a5a911f2610909
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/.git/objects/da/
+-r--r--r--   0 runner    (1001) docker     (123)      586 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/da/906831a48153c2aab0584132a4c640237894c5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/.git/objects/e0/
+-r--r--r--   0 runner    (1001) docker     (123)     4443 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/e0/070199d593788b787f27da1f0d67ec7b94b277
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/.git/objects/e4/
+-r--r--r--   0 runner    (1001) docker     (123)    62418 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/e4/22b4250d248909013befbeac5f70b8b651c014
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/.git/objects/e6/
+-r--r--r--   0 runner    (1001) docker     (123)    10076 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/objects/e6/ad2c129e0ca20fc7903657a4555a64062df9a3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.379659 domain-admin-1.3.2/domain_admin/public/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.379659 domain-admin-1.3.2/domain_admin/public/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 11:20:35.000000 domain-admin-1.3.2/domain_admin/public/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.399659 domain-admin-1.3.2/domain_admin/public/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/css/index.3c8142bf.css
+-rw-r--r--   0 runner    (1001) docker     (123)   324879 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/css/index.56f1f605.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/css/index.6730720e.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.403659 domain-admin-1.3.2/domain_admin/public/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/ConnectStatus.1b8b9c89.js
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/SelectGroup.bb54ab1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/element-icon.1ce1c350.js
+-rw-r--r--   0 runner    (1001) docker     (123)   749550 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/element-plus.d9ab67b4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/index.1918b941.js
+-rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/index.353f6c08.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/index.7e1bfc76.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/index.87f37741.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/index.8ca50aef.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/index.94134290.js
+-rw-r--r--   0 runner    (1001) docker     (123)   219500 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/index.9da88c42.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/index.c00b6c6b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/validator.0c34c3e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/vendor-lib.65d1e499.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-06-04 11:20:36.000000 domain-admin-1.3.2/domain_admin/public/js/vendor-vue.9e61e0af.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.403659 domain-admin-1.3.2/domain_admin/router/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/router/api_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/router/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.407659 domain-admin-1.3.2/domain_admin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/async_task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/cache_domain_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/email_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/global_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/group_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/notify_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/render_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/scheduler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/system_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/version_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/service/work_weixin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.407659 domain-admin-1.3.2/domain_admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/templates/domain-cert-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/templates/domain-export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.411659 domain-admin-1.3.2/domain_admin/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/bcrypt_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.411659 domain-admin-1.3.2/domain_admin/utils/cert_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/cert_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/cert_util/cert_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/cert_util/cert_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/cert_util/cert_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/cert_util/cert_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/cert_util/cert_socket_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/datetime_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/domain_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.411659 domain-admin-1.3.2/domain_admin/utils/flask_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/api_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/app_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/http_code_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.415659 domain-admin-1.3.2/domain_admin/utils/flask_ext/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/json/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/json/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/json/json_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/flask_ext/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/json_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.415659 domain-admin-1.3.2/domain_admin/utils/peewee_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/peewee_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/peewee_ext/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/secret_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/text_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.415659 domain-admin-1.3.2/domain_admin/utils/whois_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/whois_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/whois_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/whois_util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/whois_util/whois-servers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/whois_util/whois_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/utils/work_weixin_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-06-04 11:20:27.000000 domain-admin-1.3.2/domain_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.383659 domain-admin-1.3.2/domain_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-06-04 11:20:37.000000 domain-admin-1.3.2/domain_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-06-04 11:20:37.000000 domain-admin-1.3.2/domain_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 11:20:37.000000 domain-admin-1.3.2/domain_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-04 11:20:37.000000 domain-admin-1.3.2/domain_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-04 11:20:37.000000 domain-admin-1.3.2/domain_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 11:20:37.000000 domain-admin-1.3.2/domain_admin.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:20:37.415659 domain-admin-1.3.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-04 11:20:27.000000 domain-admin-1.3.2/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 11:20:37.415659 domain-admin-1.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1928 2023-06-04 11:20:27.000000 domain-admin-1.3.2/setup.py
```

### Comparing `domain-admin-1.3.1/LICENSE` & `domain-admin-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/PKG-INFO` & `domain-admin-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.3.1
+Version: 1.3.2
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain ssl cert
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `domain-admin-1.3.1/README.md` & `domain-admin-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/api/address_api.py` & `domain-admin-1.3.2/domain_admin/api/address_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/api/auth_api.py` & `domain-admin-1.3.2/domain_admin/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/api/domain_api.py` & `domain-admin-1.3.2/domain_admin/api/domain_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/api/group_api.py` & `domain-admin-1.3.2/domain_admin/api/group_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/api/log_scheduler_api.py` & `domain-admin-1.3.2/domain_admin/api/log_scheduler_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/api/notify_api.py` & `domain-admin-1.3.2/domain_admin/api/notify_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/api/system_api.py` & `domain-admin-1.3.2/domain_admin/api/system_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/api/user_api.py` & `domain-admin-1.3.2/domain_admin/api/user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/config/default_config.py` & `domain-admin-1.3.2/domain_admin/config/default_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/enums/version_enum.py` & `domain-admin-1.3.2/domain_admin/enums/version_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/log.py` & `domain-admin-1.3.2/domain_admin/log.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/main.py` & `domain-admin-1.3.2/domain_admin/main.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/migrate/migrate_102_to_103.py` & `domain-admin-1.3.2/domain_admin/migrate/migrate_102_to_103.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/migrate/migrate_106_to_110.py` & `domain-admin-1.3.2/domain_admin/migrate/migrate_106_to_110.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/migrate/migrate_110_to_1212.py` & `domain-admin-1.3.2/domain_admin/migrate/migrate_110_to_1212.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/migrate/migrate_1212_to_1213.py` & `domain-admin-1.3.2/domain_admin/migrate/migrate_1212_to_1213.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/migrate/migrate_1213_to_131.py` & `domain-admin-1.3.2/domain_admin/migrate/migrate_1213_to_131.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/model/address_model.py` & `domain-admin-1.3.2/domain_admin/model/address_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/model/base_model.py` & `domain-admin-1.3.2/domain_admin/model/base_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/model/cache_domain_info_model.py` & `domain-admin-1.3.2/domain_admin/model/cache_domain_info_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/model/database.py` & `domain-admin-1.3.2/domain_admin/model/database.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/model/domain_model.py` & `domain-admin-1.3.2/domain_admin/model/domain_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     # 用户id
     user_id = IntegerField(default=0)
 
     # 域名
     domain = CharField()
 
     # 端口 @since v1.2.24
-    port = IntegerField(default=0)
+    port = IntegerField(default=443)
 
     # 别名/备注
     alias = CharField(default="")
 
     # ip
     # @Deprecated
     ip = CharField(default="")
```

### Comparing `domain-admin-1.3.1/domain_admin/model/group_model.py` & `domain-admin-1.3.2/domain_admin/model/group_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/model/log_scheduler_model.py` & `domain-admin-1.3.2/domain_admin/model/log_scheduler_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/model/notify_model.py` & `domain-admin-1.3.2/domain_admin/model/notify_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/model/system_model.py` & `domain-admin-1.3.2/domain_admin/model/system_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/model/user_model.py` & `domain-admin-1.3.2/domain_admin/model/user_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/model/version_model.py` & `domain-admin-1.3.2/domain_admin/model/version_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/hooks/commit-msg.sample` & `domain-admin-1.3.2/domain_admin/public/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.3.2/domain_admin/public/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/hooks/pre-commit.sample` & `domain-admin-1.3.2/domain_admin/public/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/hooks/pre-push.sample` & `domain-admin-1.3.2/domain_admin/public/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/hooks/pre-rebase.sample` & `domain-admin-1.3.2/domain_admin/public/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/hooks/pre-receive.sample` & `domain-admin-1.3.2/domain_admin/public/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.3.2/domain_admin/public/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/hooks/push-to-checkout.sample` & `domain-admin-1.3.2/domain_admin/public/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/hooks/update.sample` & `domain-admin-1.3.2/domain_admin/public/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/0e/d7eb4a521f152c1f9bd95e7eb480c1f09165ae` & `domain-admin-1.3.2/domain_admin/public/.git/objects/0e/d7eb4a521f152c1f9bd95e7eb480c1f09165ae`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/28/420029335fa4e1347a9749ff4900dcb509813d` & `domain-admin-1.3.2/domain_admin/public/.git/objects/28/420029335fa4e1347a9749ff4900dcb509813d`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/35/c7d9b593caf78d8bc26ca2d5c705319df64bce` & `domain-admin-1.3.2/domain_admin/public/.git/objects/35/c7d9b593caf78d8bc26ca2d5c705319df64bce`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/39/8a6e00e326b167bbbbafeae3fbfdac6bc16179` & `domain-admin-1.3.2/domain_admin/public/.git/objects/39/8a6e00e326b167bbbbafeae3fbfdac6bc16179`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/46/02beb67fcbd0847be12eac9564f6cc074b586b` & `domain-admin-1.3.2/domain_admin/public/.git/objects/46/02beb67fcbd0847be12eac9564f6cc074b586b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462` & `domain-admin-1.3.2/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/54/c186d682acad66785d7fc148ceeef6b4ad0946` & `domain-admin-1.3.2/domain_admin/public/.git/objects/54/c186d682acad66785d7fc148ceeef6b4ad0946`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/57/e5db996081ddbd7008afae5c24b23e9f2417a9` & `domain-admin-1.3.2/domain_admin/public/.git/objects/57/e5db996081ddbd7008afae5c24b23e9f2417a9`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/6a/88267aadd02ec9f25862b364fa6bf5c090ea6a` & `domain-admin-1.3.2/domain_admin/public/.git/objects/6a/88267aadd02ec9f25862b364fa6bf5c090ea6a`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/6f/cd2c55887a9ccc2f613a9a60b501ebfd38c893` & `domain-admin-1.3.2/domain_admin/public/.git/objects/6f/cd2c55887a9ccc2f613a9a60b501ebfd38c893`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad` & `domain-admin-1.3.2/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/d2/bb330b9eb09960c48b9881a9a5a911f2610909` & `domain-admin-1.3.2/domain_admin/public/.git/objects/d2/bb330b9eb09960c48b9881a9a5a911f2610909`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/da/906831a48153c2aab0584132a4c640237894c5` & `domain-admin-1.3.2/domain_admin/public/.git/objects/da/906831a48153c2aab0584132a4c640237894c5`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/e0/070199d593788b787f27da1f0d67ec7b94b277` & `domain-admin-1.3.2/domain_admin/public/.git/objects/e0/070199d593788b787f27da1f0d67ec7b94b277`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/e4/22b4250d248909013befbeac5f70b8b651c014` & `domain-admin-1.3.2/domain_admin/public/.git/objects/e4/22b4250d248909013befbeac5f70b8b651c014`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/.git/objects/e6/ad2c129e0ca20fc7903657a4555a64062df9a3` & `domain-admin-1.3.2/domain_admin/public/.git/objects/e6/ad2c129e0ca20fc7903657a4555a64062df9a3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/css/index.56f1f605.css` & `domain-admin-1.3.2/domain_admin/public/css/index.56f1f605.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/css/index.6730720e.css` & `domain-admin-1.3.2/domain_admin/public/css/index.6730720e.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/favicon.ico` & `domain-admin-1.3.2/domain_admin/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/index.html` & `domain-admin-1.3.2/domain_admin/public/index.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/ConnectStatus.1b8b9c89.js` & `domain-admin-1.3.2/domain_admin/public/js/ConnectStatus.1b8b9c89.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/SelectGroup.bb54ab1b.js` & `domain-admin-1.3.2/domain_admin/public/js/SelectGroup.bb54ab1b.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/element-icon.1ce1c350.js` & `domain-admin-1.3.2/domain_admin/public/js/element-icon.1ce1c350.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/element-plus.d9ab67b4.js` & `domain-admin-1.3.2/domain_admin/public/js/element-plus.d9ab67b4.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/index.1918b941.js` & `domain-admin-1.3.2/domain_admin/public/js/index.1918b941.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/index.353f6c08.js` & `domain-admin-1.3.2/domain_admin/public/js/index.353f6c08.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/index.7e1bfc76.js` & `domain-admin-1.3.2/domain_admin/public/js/index.7e1bfc76.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/index.87f37741.js` & `domain-admin-1.3.2/domain_admin/public/js/index.87f37741.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/index.8ca50aef.js` & `domain-admin-1.3.2/domain_admin/public/js/index.8ca50aef.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/index.94134290.js` & `domain-admin-1.3.2/domain_admin/public/js/index.94134290.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/index.9da88c42.js` & `domain-admin-1.3.2/domain_admin/public/js/index.9da88c42.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/index.c00b6c6b.js` & `domain-admin-1.3.2/domain_admin/public/js/index.c00b6c6b.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/vendor-lib.65d1e499.js` & `domain-admin-1.3.2/domain_admin/public/js/vendor-lib.65d1e499.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/public/js/vendor-vue.9e61e0af.js` & `domain-admin-1.3.2/domain_admin/public/js/vendor-vue.9e61e0af.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/router/api_map.py` & `domain-admin-1.3.2/domain_admin/router/api_map.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/router/permission.py` & `domain-admin-1.3.2/domain_admin/router/permission.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/service/auth_service.py` & `domain-admin-1.3.2/domain_admin/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/service/cache_domain_info_service.py` & `domain-admin-1.3.2/domain_admin/service/cache_domain_info_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/service/domain_service.py` & `domain-admin-1.3.2/domain_admin/service/domain_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/service/email_service.py` & `domain-admin-1.3.2/domain_admin/service/email_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/service/file_service.py` & `domain-admin-1.3.2/domain_admin/service/file_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/service/notify_service.py` & `domain-admin-1.3.2/domain_admin/service/notify_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/service/scheduler_service.py` & `domain-admin-1.3.2/domain_admin/service/scheduler_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/service/system_service.py` & `domain-admin-1.3.2/domain_admin/service/system_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/service/token_service.py` & `domain-admin-1.3.2/domain_admin/service/token_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/service/version_service.py` & `domain-admin-1.3.2/domain_admin/service/version_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/service/work_weixin_service.py` & `domain-admin-1.3.2/domain_admin/service/work_weixin_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/templates/domain-cert-email.html` & `domain-admin-1.3.2/domain_admin/templates/domain-cert-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/bcrypt_util.py` & `domain-admin-1.3.2/domain_admin/utils/bcrypt_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/cert_util/__init__.py` & `domain-admin-1.3.2/domain_admin/utils/cert_util/__init__.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/cert_util/cert_common.py` & `domain-admin-1.3.2/domain_admin/utils/cert_util/cert_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/cert_util/cert_openssl.py` & `domain-admin-1.3.2/domain_admin/utils/cert_util/cert_openssl.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/cert_util/cert_socket.py` & `domain-admin-1.3.2/domain_admin/utils/cert_util/cert_socket.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/cert_util/cert_socket_v2.py` & `domain-admin-1.3.2/domain_admin/utils/cert_util/cert_socket_v2.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/datetime_util.py` & `domain-admin-1.3.2/domain_admin/utils/datetime_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/domain_util.py` & `domain-admin-1.3.2/domain_admin/utils/domain_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/email_util.py` & `domain-admin-1.3.2/domain_admin/utils/email_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/flask_ext/api_result.py` & `domain-admin-1.3.2/domain_admin/utils/flask_ext/api_result.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/flask_ext/app_exception.py` & `domain-admin-1.3.2/domain_admin/utils/flask_ext/app_exception.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/flask_ext/flask_app.py` & `domain-admin-1.3.2/domain_admin/utils/flask_ext/flask_app.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/flask_ext/handler.py` & `domain-admin-1.3.2/domain_admin/utils/flask_ext/handler.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/ip_util.py` & `domain-admin-1.3.2/domain_admin/utils/ip_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/json_util.py` & `domain-admin-1.3.2/domain_admin/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/peewee_ext/model_util.py` & `domain-admin-1.3.2/domain_admin/utils/peewee_ext/model_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/text_util.py` & `domain-admin-1.3.2/domain_admin/utils/text_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/time_util.py` & `domain-admin-1.3.2/domain_admin/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/whois_util/config.py` & `domain-admin-1.3.2/domain_admin/utils/whois_util/config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/whois_util/util.py` & `domain-admin-1.3.2/domain_admin/utils/whois_util/util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/whois_util/whois-servers.txt` & `domain-admin-1.3.2/domain_admin/utils/whois_util/whois-servers.txt`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/whois_util/whois_util.py` & `domain-admin-1.3.2/domain_admin/utils/whois_util/whois_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin/utils/work_weixin_api.py` & `domain-admin-1.3.2/domain_admin/utils/work_weixin_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/domain_admin.egg-info/PKG-INFO` & `domain-admin-1.3.2/domain_admin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.3.1
+Version: 1.3.2
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain ssl cert
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `domain-admin-1.3.1/domain_admin.egg-info/SOURCES.txt` & `domain-admin-1.3.2/domain_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domain-admin-1.3.1/setup.py` & `domain-admin-1.3.2/setup.py`

 * *Files identical despite different names*

