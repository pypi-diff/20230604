# Comparing `tmp/bovine-0.2.5.tar.gz` & `tmp/bovine-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine-0.2.5.tar", max compression
+gzip compressed data, was "bovine-0.2.6.tar", max compression
```

## Comparing `bovine-0.2.5.tar` & `bovine-0.2.6.tar`

### file list

```diff
@@ -1,111 +1,106 @@
--rw-r--r--   0        0        0     1363 2023-05-28 14:16:21.774046 bovine-0.2.5/README.md
--rw-r--r--   0        0        0     9485 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 14:16:21.898047 bovine-0.2.5/bovine/activitypub/__init__.py
--rw-r--r--   0        0        0      173 2023-05-28 14:17:29.786760 bovine-0.2.5/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3741 2023-05-28 14:17:29.786760 bovine-0.2.5/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
--rw-r--r--   0        0        0     2173 2023-05-28 14:17:30.310766 bovine-0.2.5/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
--rw-r--r--   0        0        0      922 2023-05-28 14:17:30.314766 bovine-0.2.5/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
--rw-r--r--   0        0        0     3638 2023-05-28 14:17:30.654770 bovine-0.2.5/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1212 2023-05-28 14:17:30.710770 bovine-0.2.5/bovine/activitypub/__pycache__/test_collection_helper.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3505 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitypub/authorization_wrapper.py
--rw-r--r--   0        0        0     2267 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitypub/collection_helper.py
--rw-r--r--   0        0        0      434 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitypub/collection_iterator.py
--rw-r--r--   0        0        0     2757 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitypub/test_actor.py
--rw-r--r--   0        0        0      498 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitypub/test_collection_helper.py
--rw-r--r--   0        0        0     4957 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitystreams/__init__.py
--rw-r--r--   0        0        0     4645 2023-05-28 14:17:30.314766 bovine-0.2.5/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4269 2023-05-28 14:17:30.314766 bovine-0.2.5/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4028 2023-05-28 14:17:30.318766 bovine-0.2.5/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4584 2023-05-28 14:17:30.722770 bovine-0.2.5/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3327 2023-05-28 14:17:30.730770 bovine-0.2.5/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3113 2023-05-28 14:17:30.734770 bovine-0.2.5/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1951 2023-05-28 14:17:30.738770 bovine-0.2.5/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1386 2023-05-28 14:17:30.742771 bovine-0.2.5/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     4203 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitystreams/activity_factory.py
--rw-r--r--   0        0        0     4178 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitystreams/object_factory.py
--rw-r--r--   0        0        0     2195 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitystreams/test_activity_factory.py
--rw-r--r--   0        0        0     1442 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitystreams/test_actor.py
--rw-r--r--   0        0        0     1257 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitystreams/test_object_factory.py
--rw-r--r--   0        0        0     1034 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitystreams/test_ordered_collection_builder.py
--rw-r--r--   0        0        0      817 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitystreams/test_ordered_collection_page.py
--rw-r--r--   0        0        0     2354 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitystreams/utils/__init__.py
--rw-r--r--   0        0        0     2836 2023-05-28 14:17:30.318766 bovine-0.2.5/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4763 2023-05-28 14:17:30.750771 bovine-0.2.5/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      865 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitystreams/utils/print.py
--rw-r--r--   0        0        0     2266 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/activitystreams/utils/test_utils.py
--rw-r--r--   0        0        0     3968 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/__init__.py
--rw-r--r--   0        0        0     4002 2023-05-28 14:17:30.090764 bovine-0.2.5/bovine/clients/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1916 2023-05-28 14:17:30.094764 bovine-0.2.5/bovine/clients/__pycache__/bearer.cpython-310.pyc
--rw-r--r--   0        0        0      268 2023-05-28 14:17:30.090764 bovine-0.2.5/bovine/clients/__pycache__/consts.cpython-310.pyc
--rw-r--r--   0        0        0     1719 2023-05-28 14:17:30.146764 bovine-0.2.5/bovine/clients/__pycache__/event_source.cpython-310.pyc
--rw-r--r--   0        0        0     1084 2023-05-28 14:17:30.090764 bovine-0.2.5/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
--rw-r--r--   0        0        0     2534 2023-05-28 14:17:30.150764 bovine-0.2.5/bovine/clients/__pycache__/moo_auth.cpython-310.pyc
--rw-r--r--   0        0        0     1237 2023-05-28 14:17:30.090764 bovine-0.2.5/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
--rw-r--r--   0        0        0     1529 2023-05-28 14:17:30.310766 bovine-0.2.5/bovine/clients/__pycache__/signed_http.cpython-310.pyc
--rw-r--r--   0        0        0     2479 2023-05-28 14:17:30.310766 bovine-0.2.5/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc
--rw-r--r--   0        0        0     1507 2023-05-28 14:17:30.758771 bovine-0.2.5/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2844 2023-05-28 14:17:30.762771 bovine-0.2.5/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1217 2023-05-28 14:17:30.766771 bovine-0.2.5/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2102 2023-05-28 14:17:30.770771 bovine-0.2.5/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      814 2023-05-28 14:17:30.774771 bovine-0.2.5/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1794 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/bearer.py
--rw-r--r--   0        0        0       91 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/consts.py
--rw-r--r--   0        0        0     1520 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/event_source.py
--rw-r--r--   0        0        0      868 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/lookup_account.py
--rw-r--r--   0        0        0     3001 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/moo_auth.py
--rw-r--r--   0        0        0      948 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/nodeinfo.py
--rw-r--r--   0        0        0     1150 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/signed_http.py
--rw-r--r--   0        0        0     3278 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/signed_http_methods.py
--rw-r--r--   0        0        0      651 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/test_event_source.py
--rw-r--r--   0        0        0     1505 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/test_lookup_account.py
--rw-r--r--   0        0        0      319 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/test_nodeinfo.py
--rw-r--r--   0        0        0     1153 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/test_signed_http.py
--rw-r--r--   0        0        0      522 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/clients/test_signed_http_client.py
--rw-r--r--   0        0        0     4141 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/crypto/__init__.py
--rw-r--r--   0        0        0     3749 2023-05-28 14:17:30.150764 bovine-0.2.5/bovine/crypto/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2863 2023-05-28 14:17:30.306766 bovine-0.2.5/bovine/crypto/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     2909 2023-05-28 14:17:30.310766 bovine-0.2.5/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
--rw-r--r--   0        0        0     2257 2023-05-28 14:17:30.310766 bovine-0.2.5/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
--rw-r--r--   0        0        0     1784 2023-05-28 14:17:30.310766 bovine-0.2.5/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
--rw-r--r--   0        0        0     2363 2023-05-28 14:17:30.706770 bovine-0.2.5/bovine/crypto/__pycache__/test.cpython-310.pyc
--rw-r--r--   0        0        0     5821 2023-05-28 14:17:30.782771 bovine-0.2.5/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2742 2023-05-28 14:17:30.786771 bovine-0.2.5/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     7454 2023-05-28 14:17:30.798771 bovine-0.2.5/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2674 2023-05-28 14:17:30.806771 bovine-0.2.5/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2664 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/crypto/helper.py
--rw-r--r--   0        0        0     2112 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/crypto/http_signature.py
--rw-r--r--   0        0        0     2942 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/crypto/signature_checker.py
--rw-r--r--   0        0        0     1266 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/crypto/signature_parser.py
--rw-r--r--   0        0        0     2199 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/crypto/test.py
--rw-r--r--   0        0        0     4995 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/crypto/test_crypto.py
--rw-r--r--   0        0        0      896 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/crypto/test_helper.py
--rw-r--r--   0        0        0     5081 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/crypto/test_http_signature.py
--rw-r--r--   0        0        0     1207 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/crypto/test_signature_parser.py
--rw-r--r--   0        0        0      302 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/ed25519_key.py
--rw-r--r--   0        0        0     3342 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/jsonld.py
--rw-r--r--   0        0        0      826 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/msg.py
--rw-r--r--   0        0        0     3256 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/repl.py
--rw-r--r--   0        0        0      178 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/test_bovine_client.py
--rw-r--r--   0        0        0     5250 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/test_jsonld.py
--rw-r--r--   0        0        0      282 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/test_types.py
--rw-r--r--   0        0        0     2397 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/types.py
--rw-r--r--   0        0        0      856 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/utils/__init__.py
--rw-r--r--   0        0        0     1120 2023-05-28 14:17:30.090764 bovine-0.2.5/bovine/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      877 2023-05-28 14:17:30.094764 bovine-0.2.5/bovine/utils/__pycache__/date.cpython-310.pyc
--rw-r--r--   0        0        0     3240 2023-05-28 14:17:30.642769 bovine-0.2.5/bovine/utils/__pycache__/pyld_requests.cpython-310.pyc
--rw-r--r--   0        0        0     3465 2023-05-28 14:17:30.814771 bovine-0.2.5/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1662 2023-05-28 14:17:30.818771 bovine-0.2.5/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1625 2023-05-28 14:17:30.818771 bovine-0.2.5/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      519 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/utils/date.py
--rw-r--r--   0        0        0     1432 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/utils/msg/__init__.py
--rw-r--r--   0        0        0     1934 2023-05-28 14:17:30.822771 bovine-0.2.5/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1967 2023-05-28 14:17:30.826771 bovine-0.2.5/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      659 2023-05-28 14:17:30.822771 bovine-0.2.5/bovine/utils/msg/__pycache__/validation.cpython-310.pyc
--rw-r--r--   0        0        0      599 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/utils/msg/test_validation.py
--rw-r--r--   0        0        0      261 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/utils/msg/validation.py
--rw-r--r--   0        0        0     4736 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/utils/pyld_requests.py
--rw-r--r--   0        0        0      761 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/utils/test_date.py
--rw-r--r--   0        0        0      452 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/utils/test_parse.py
--rw-r--r--   0        0        0      368 2023-05-28 14:16:21.774046 bovine-0.2.5/bovine/utils/test_webfinger.py
--rw-r--r--   0        0        0     1405 2023-05-28 14:16:21.778046 bovine-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 bovine-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1363 2023-06-04 18:31:36.354114 bovine-0.2.6/README.md
+-rw-r--r--   0        0        0     9472 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/__init__.py
+-rw-r--r--   0        0        0     4957 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/__init__.py
+-rw-r--r--   0        0        0     4645 2023-06-04 18:32:41.834765 bovine-0.2.6/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4483 2023-06-04 18:32:41.834765 bovine-0.2.6/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     2145 2023-06-04 18:32:41.842765 bovine-0.2.6/bovine/activitystreams/__pycache__/collection_helper.cpython-310.pyc
+-rw-r--r--   0        0        0     4369 2023-06-04 18:32:41.838765 bovine-0.2.6/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4584 2023-06-04 18:32:42.814775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3327 2023-06-04 18:32:42.822775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      795 2023-06-04 18:32:42.826775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_collection_helper.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3113 2023-06-04 18:32:42.834775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1951 2023-06-04 18:32:42.838775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1386 2023-06-04 18:32:42.842775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     4386 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/activity_factory.py
+-rw-r--r--   0        0        0     2151 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/collection_helper.py
+-rw-r--r--   0        0        0     4515 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/object_factory.py
+-rw-r--r--   0        0        0     2195 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_activity_factory.py
+-rw-r--r--   0        0        0     1442 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_actor.py
+-rw-r--r--   0        0        0      471 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_collection_helper.py
+-rw-r--r--   0        0        0     1257 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_object_factory.py
+-rw-r--r--   0        0        0     1034 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_ordered_collection_builder.py
+-rw-r--r--   0        0        0      817 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_ordered_collection_page.py
+-rw-r--r--   0        0        0     2354 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/utils/__init__.py
+-rw-r--r--   0        0        0     2836 2023-06-04 18:32:41.838765 bovine-0.2.6/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4763 2023-06-04 18:32:42.854776 bovine-0.2.6/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      865 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/utils/print.py
+-rw-r--r--   0        0        0     2266 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/utils/test_utils.py
+-rw-r--r--   0        0        0     3968 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/__init__.py
+-rw-r--r--   0        0        0     4002 2023-06-04 18:32:41.842765 bovine-0.2.6/bovine/clients/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3683 2023-06-04 18:32:42.154769 bovine-0.2.6/bovine/clients/__pycache__/authorization_wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     1916 2023-06-04 18:32:42.402771 bovine-0.2.6/bovine/clients/__pycache__/bearer.cpython-310.pyc
+-rw-r--r--   0        0        0      268 2023-06-04 18:32:42.154769 bovine-0.2.6/bovine/clients/__pycache__/consts.cpython-310.pyc
+-rw-r--r--   0        0        0     1719 2023-06-04 18:32:42.406771 bovine-0.2.6/bovine/clients/__pycache__/event_source.cpython-310.pyc
+-rw-r--r--   0        0        0     1084 2023-06-04 18:32:42.154769 bovine-0.2.6/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
+-rw-r--r--   0        0        0     2534 2023-06-04 18:32:42.406771 bovine-0.2.6/bovine/clients/__pycache__/moo_auth.cpython-310.pyc
+-rw-r--r--   0        0        0     1237 2023-06-04 18:32:42.154769 bovine-0.2.6/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
+-rw-r--r--   0        0        0     1529 2023-06-04 18:32:42.406771 bovine-0.2.6/bovine/clients/__pycache__/signed_http.cpython-310.pyc
+-rw-r--r--   0        0        0     2479 2023-06-04 18:32:42.406771 bovine-0.2.6/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc
+-rw-r--r--   0        0        0     1507 2023-06-04 18:32:42.858775 bovine-0.2.6/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2844 2023-06-04 18:32:42.862776 bovine-0.2.6/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1217 2023-06-04 18:32:42.866776 bovine-0.2.6/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2102 2023-06-04 18:32:42.870776 bovine-0.2.6/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      814 2023-06-04 18:32:42.870776 bovine-0.2.6/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3451 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/authorization_wrapper.py
+-rw-r--r--   0        0        0     1794 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/bearer.py
+-rw-r--r--   0        0        0       91 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/consts.py
+-rw-r--r--   0        0        0     1520 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/event_source.py
+-rw-r--r--   0        0        0      868 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/lookup_account.py
+-rw-r--r--   0        0        0     3001 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/moo_auth.py
+-rw-r--r--   0        0        0      948 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/nodeinfo.py
+-rw-r--r--   0        0        0     1150 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/signed_http.py
+-rw-r--r--   0        0        0     3278 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/signed_http_methods.py
+-rw-r--r--   0        0        0      651 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/test_event_source.py
+-rw-r--r--   0        0        0     1505 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/clients/test_lookup_account.py
+-rw-r--r--   0        0        0      319 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/clients/test_nodeinfo.py
+-rw-r--r--   0        0        0     1153 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/clients/test_signed_http.py
+-rw-r--r--   0        0        0      522 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/clients/test_signed_http_client.py
+-rw-r--r--   0        0        0     4141 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/__init__.py
+-rw-r--r--   0        0        0     3749 2023-06-04 18:32:42.154769 bovine-0.2.6/bovine/crypto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2863 2023-06-04 18:32:42.354771 bovine-0.2.6/bovine/crypto/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     2909 2023-06-04 18:32:42.354771 bovine-0.2.6/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
+-rw-r--r--   0        0        0     2257 2023-06-04 18:32:42.354771 bovine-0.2.6/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2023-06-04 18:32:42.402771 bovine-0.2.6/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2363 2023-06-04 18:32:42.430771 bovine-0.2.6/bovine/crypto/__pycache__/test.cpython-310.pyc
+-rw-r--r--   0        0        0     5821 2023-06-04 18:32:42.878776 bovine-0.2.6/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2742 2023-06-04 18:32:42.886776 bovine-0.2.6/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     7454 2023-06-04 18:32:42.898776 bovine-0.2.6/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2674 2023-06-04 18:32:42.910776 bovine-0.2.6/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2664 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/helper.py
+-rw-r--r--   0        0        0     2112 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/http_signature.py
+-rw-r--r--   0        0        0     2942 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/signature_checker.py
+-rw-r--r--   0        0        0     1266 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/signature_parser.py
+-rw-r--r--   0        0        0     2199 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/test.py
+-rw-r--r--   0        0        0     4995 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/test_crypto.py
+-rw-r--r--   0        0        0      896 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/test_helper.py
+-rw-r--r--   0        0        0     5081 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/test_http_signature.py
+-rw-r--r--   0        0        0     1207 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/test_signature_parser.py
+-rw-r--r--   0        0        0      302 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/ed25519_key.py
+-rw-r--r--   0        0        0     3342 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/jsonld.py
+-rw-r--r--   0        0        0      826 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/msg.py
+-rw-r--r--   0        0        0     3286 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/repl.py
+-rw-r--r--   0        0        0     2757 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/test_bovine_actor.py
+-rw-r--r--   0        0        0      178 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/test_bovine_client.py
+-rw-r--r--   0        0        0     5250 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/test_jsonld.py
+-rw-r--r--   0        0        0      282 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/test_types.py
+-rw-r--r--   0        0        0     2397 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/types.py
+-rw-r--r--   0        0        0      936 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/__init__.py
+-rw-r--r--   0        0        0     1170 2023-06-04 18:32:42.150769 bovine-0.2.6/bovine/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      877 2023-06-04 18:32:42.358770 bovine-0.2.6/bovine/utils/__pycache__/date.cpython-310.pyc
+-rw-r--r--   0        0        0     3240 2023-06-04 18:32:42.798775 bovine-0.2.6/bovine/utils/__pycache__/pyld_requests.cpython-310.pyc
+-rw-r--r--   0        0        0     3465 2023-06-04 18:32:42.918776 bovine-0.2.6/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1662 2023-06-04 18:32:42.922776 bovine-0.2.6/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1627 2023-06-04 18:32:42.926776 bovine-0.2.6/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      519 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/date.py
+-rw-r--r--   0        0        0     1432 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/msg/__init__.py
+-rw-r--r--   0        0        0     1934 2023-06-04 18:32:42.930776 bovine-0.2.6/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1967 2023-06-04 18:32:42.930776 bovine-0.2.6/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      659 2023-06-04 18:32:42.930776 bovine-0.2.6/bovine/utils/msg/__pycache__/validation.cpython-310.pyc
+-rw-r--r--   0        0        0      599 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/msg/test_validation.py
+-rw-r--r--   0        0        0      261 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/msg/validation.py
+-rw-r--r--   0        0        0     4736 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/pyld_requests.py
+-rw-r--r--   0        0        0      761 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/test_date.py
+-rw-r--r--   0        0        0      452 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/test_parse.py
+-rw-r--r--   0        0        0      370 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/test_webfinger.py
+-rw-r--r--   0        0        0     1479 2023-06-04 18:31:36.362115 bovine-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2608 1970-01-01 00:00:00.000000 bovine-0.2.6/PKG-INFO
```

### Comparing `bovine-0.2.5/README.md` & `bovine-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/__init__.py` & `bovine-0.2.6/bovine/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import logging
 from typing import Optional
 from urllib.parse import urlparse
 
 import tomli
 
-from .activitypub.authorization_wrapper import AuthorizationWrapper
-from .activitypub.collection_helper import CollectionHelper, all_collection_elements
 from .activitystreams import Collection
 from .activitystreams.activity_factory import ActivityFactory
+from .activitystreams.collection_helper import CollectionHelper
 from .activitystreams.object_factory import ObjectFactory
+from .clients.authorization_wrapper import AuthorizationWrapper
 
 logger = logging.getLogger(__name__)
 
 
 class BovineClient(AuthorizationWrapper):
     """BovineClient is meant to serve as the basis of building ActivityPub Clients.
     It defines methods for interacting with the endpoints defined by the corresponding
@@ -126,15 +126,17 @@
 
         event_source_url = self.information["endpoints"]["eventSource"]
         return self.client.event_source(event_source_url)
 
     async def simplify_collection(self, collection):
         """Returns a Collection containing all items from the passed collection
         or collection id"""
-        items = await all_collection_elements(self, collection)
+        # items = await all_collection_elements(self, collection)
+
+        items = []
 
         if isinstance(collection, str):
             collection_id = collection
         else:
             collection_id = collection.get("id")
         return Collection(id=collection_id, items=items).build()
 
@@ -164,22 +166,24 @@
     @property
     def followers(self) -> str:
         """The id of the follows collection"""
         return self.information["followers"]
 
     async def inbox(self):
         """Provides a CollectionHelper for the Actors inbox"""
-        inbox_collection = CollectionHelper(self.information["inbox"], self)
-        await inbox_collection.refresh()
+        inbox_collection = CollectionHelper(
+            self.information["inbox"], self, resolve=True
+        )
         return inbox_collection
 
     async def outbox(self):
         """Provides a CollectionHelper for the Actors outbox"""
-        inbox_collection = CollectionHelper(self.information["outbox"], self)
-        await inbox_collection.refresh()
+        inbox_collection = CollectionHelper(
+            self.information["outbox"], self, resolve=True
+        )
         return inbox_collection
 
     @staticmethod
     def from_file(config_file: str):
         """Initializes the BovineClient from a toml config file"""
         with open(config_file, "rb") as fp:
             config = tomli.load(fp)
```

### Comparing `bovine-0.2.5/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/authorization_wrapper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 3505 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,234 +1,231 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 b10d 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 7b0d 0000  o.........|d{...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
-00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
+00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
+00000060: 0100 6404 6406 6c08 6d09 5a09 0100 6404  ..d.d.l.m.Z...d.
+00000070: 6407 6c0a 6d0b 5a0b 0100 6404 6408 6c0c  d.l.m.Z...d.d.l.
 00000080: 6d0d 5a0d 0100 6500 a00e 650f a101 5a10  m.Z...e...e...Z.
-00000090: 4700 6408 6409 8400 6409 8302 5a11 6401  G.d.d...d...Z.d.
-000000a0: 5300 290a e900 0000 004e 2901 da08 4f70  S.)......N)...Op
-000000b0: 7469 6f6e 616c 2901 da19 6c6f 6f6b 7570  tional)...lookup
-000000c0: 5f64 6964 5f77 6974 685f 7765 6266 696e  _did_with_webfin
-000000d0: 6765 7229 01da 1042 6561 7265 7241 7574  ger)...BearerAut
-000000e0: 6843 6c69 656e 7429 01da 0d4d 6f6f 4175  hClient)...MooAu
-000000f0: 7468 436c 6965 6e74 2901 da10 5369 676e  thClient)...Sign
-00000100: 6564 4874 7470 436c 6965 6e74 2901 da16  edHttpClient)...
-00000110: 7072 6976 6174 655f 6b65 795f 746f 5f64  private_key_to_d
-00000120: 6964 5f6b 6579 6300 0000 0000 0000 0000  id_keyc.........
-00000130: 0000 0000 0000 0008 0000 0040 0000 0073  ...........@...s
-00000140: ca00 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
-00000150: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
-00000160: 8400 5a05 6421 6408 6506 6507 6a08 1900  ..Z.d!d.e.e.j...
-00000170: 6602 6409 640a 8405 5a09 0907 6421 640b  f.d.d...Z...d!d.
-00000180: 650a 640c 650a 6408 6506 6507 6a08 1900  e.d.e.d.e.e.j...
-00000190: 6606 640d 640e 8405 5a0b 640f 650a 6602  f.d.d...Z.d.e.f.
-000001a0: 6410 6411 8404 5a0c 0907 6421 6412 650a  d.d...Z...d!d.e.
-000001b0: 640c 650a 6408 6506 6507 6a08 1900 6606  d.e.d.e.e.j...f.
-000001c0: 6413 6414 8405 5a0d 0907 6421 6415 650a  d.d...Z...d!d.e.
-000001d0: 6408 6506 6507 6a08 1900 6604 6416 6417  d.e.e.j...f.d.d.
-000001e0: 8405 5a0e 6418 6419 8400 5a0f 641a 641b  ..Z.d.d...Z.d.d.
-000001f0: 8400 5a10 641c 641d 8400 5a11 641e 6512  ..Z.d.d...Z.d.e.
-00000200: 6602 641f 6420 8404 5a13 6407 5300 2922  f.d.d ..Z.d.S.)"
-00000210: da14 4175 7468 6f72 697a 6174 696f 6e57  ..AuthorizationW
-00000220: 7261 7070 6572 6301 0000 0000 0000 0000  rapperc.........
-00000230: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-00000240: 1c00 0000 6400 7c00 5f00 6400 7c00 5f01  ....d.|._.d.|._.
-00000250: 6400 7c00 5f02 6400 7c00 5f03 6400 5300  d.|._.d.|._.d.S.
-00000260: a901 4e29 04da 0663 6f6e 6669 67da 0861  ..N)...config..a
-00000270: 6374 6f72 5f69 64da 0663 6c69 656e 74da  ctor_id..client.
-00000280: 0773 6573 7369 6f6e a901 da04 7365 6c66  .session....self
-00000290: a900 7210 0000 00fa 5d2f 776f 6f64 7065  ..r.....]/woodpe
-000002a0: 636b 6572 2f73 7263 2f63 6f64 6562 6572  cker/src/codeber
-000002b0: 672e 6f72 672f 626f 7669 6e65 2f62 6f76  g.org/bovine/bov
-000002c0: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
-000002d0: 652f 6163 7469 7669 7479 7075 622f 6175  e/activitypub/au
-000002e0: 7468 6f72 697a 6174 696f 6e5f 7772 6170  thorization_wrap
-000002f0: 7065 722e 7079 da08 5f5f 696e 6974 5f5f  per.py..__init__
-00000300: 1000 0000 7308 0000 0006 0106 0106 010a  ....s...........
-00000310: 017a 1d41 7574 686f 7269 7a61 7469 6f6e  .z.Authorization
-00000320: 5772 6170 7065 722e 5f5f 696e 6974 5f5f  Wrapper.__init__
-00000330: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000340: 0002 0000 00c3 0000 0073 1400 0000 8101  .........s......
-00000350: 7c00 a000 a100 4900 6400 4800 0100 7c00  |.....I.d.H...|.
-00000360: 5300 7209 0000 0029 01da 0469 6e69 7472  S.r....)...initr
-00000370: 0e00 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
-00000380: 0000 00da 0a5f 5f61 656e 7465 725f 5f16  .....__aenter__.
-00000390: 0000 0073 0600 0000 0280 0e01 0401 7a1f  ...s..........z.
-000003a0: 4175 7468 6f72 697a 6174 696f 6e57 7261  AuthorizationWra
-000003b0: 7070 6572 2e5f 5f61 656e 7465 725f 5f63  pper.__aenter__c
-000003c0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000003d0: 0200 0000 c700 0000 7316 0000 0081 017c  ........s......|
-000003e0: 006a 00a0 01a1 0049 0064 0048 0001 0064  .j.....I.d.H...d
-000003f0: 0053 0072 0900 0000 2902 720d 0000 00da  .S.r....).r.....
-00000400: 0563 6c6f 7365 2902 720f 0000 00da 0461  .close).r......a
-00000410: 7267 7372 1000 0000 7210 0000 0072 1100  rgsr....r....r..
-00000420: 0000 da09 5f5f 6165 7869 745f 5f1a 0000  ....__aexit__...
-00000430: 0073 0400 0000 0280 1401 7a1e 4175 7468  .s........z.Auth
-00000440: 6f72 697a 6174 696f 6e57 7261 7070 6572  orizationWrapper
-00000450: 2e5f 5f61 6578 6974 5f5f 4e72 0d00 0000  .__aexit__Nr....
-00000460: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000470: 0005 0000 00c3 0000 0073 c000 0000 8101  .........s......
-00000480: 7c01 7c00 5f00 7c01 6400 7500 720d 7401  |.|._.|.d.u.r.t.
-00000490: a002 a100 7c00 5f00 7c00 6a03 7312 4a00  ....|._.|.j.s.J.
-000004a0: 8201 7c00 a004 a100 722a 7c00 6a05 7c00  ..|.....r*|.j.|.
-000004b0: 6a03 6401 1900 7c00 6a03 6402 1900 7c00  j.d...|.j.d...|.
-000004c0: 6a00 6403 8d03 4900 6400 4800 0100 6400  j.d...I.d.H...d.
-000004d0: 5300 7c00 a006 a100 7245 7c00 6a03 6404  S.|.....rE|.j.d.
-000004e0: 1900 7c00 5f07 7c00 6a08 7c00 6a03 6405  ..|._.|.j.|.j.d.
-000004f0: 1900 7c00 6a03 6402 1900 7c00 6a00 6403  ..|.j.d...|.j.d.
-00000500: 8d03 0100 6400 5300 7c00 a009 a100 725c  ....d.S.|.....r\
-00000510: 7c00 6a03 6404 1900 7c00 5f07 7c00 6a0a  |.j.d...|._.|.j.
-00000520: 7c00 6a03 6406 1900 7c00 6a00 6403 8d02  |.j.d...|.j.d...
-00000530: 0100 6400 5300 740b 6407 8301 8201 2908  ..d.S.t.d.....).
-00000540: 4eda 0468 6f73 74da 0b70 7269 7661 7465  N..host..private
-00000550: 5f6b 6579 2901 720d 0000 00da 0b61 6363  _key).r......acc
-00000560: 6f75 6e74 5f75 726c da0e 7075 626c 6963  ount_url..public
-00000570: 5f6b 6579 5f75 726c da0c 6163 6365 7373  _key_url..access
-00000580: 5f74 6f6b 656e 7a27 4e6f 206b 6e6f 776e  _tokenz'No known
-00000590: 2061 7574 686f 7269 7a61 7469 6f6e 206d   authorization m
-000005a0: 6574 686f 6420 6176 6169 6c61 626c 6529  ethod available)
-000005b0: 0c72 0d00 0000 da07 6169 6f68 7474 70da  .r......aiohttp.
-000005c0: 0d43 6c69 656e 7453 6573 7369 6f6e 720a  .ClientSessionr.
-000005d0: 0000 00da 0d5f 6861 735f 6d6f 6f5f 6175  ....._has_moo_au
-000005e0: 7468 da21 7769 7468 5f68 6f73 745f 616e  th.!with_host_an
-000005f0: 645f 6564 3235 3531 395f 7072 6976 6174  d_ed25519_privat
-00000600: 655f 6b65 79da 135f 6861 735f 6874 7470  e_key.._has_http
-00000610: 5f73 6967 6e61 7475 7265 720b 0000 00da  _signaturer.....
-00000620: 1377 6974 685f 6874 7470 5f73 6967 6e61  .with_http_signa
-00000630: 7475 7265 da10 5f68 6173 5f62 6561 7265  ture.._has_beare
-00000640: 725f 6175 7468 da11 7769 7468 5f62 6561  r_auth..with_bea
-00000650: 7265 725f 746f 6b65 6eda 0945 7863 6570  rer_token..Excep
-00000660: 7469 6f6e 2902 720f 0000 0072 0d00 0000  tion).r....r....
-00000670: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-00000680: 1300 0000 1d00 0000 7328 0000 0002 8006  ........s(......
-00000690: 0108 010a 010a 0208 0204 0114 0110 ff08  ................
-000006a0: 030c 0104 0108 0108 0104 010a fd08 050c  ................
-000006b0: 011a 0108 027a 1941 7574 686f 7269 7a61  .....z.Authoriza
-000006c0: 7469 6f6e 5772 6170 7065 722e 696e 6974  tionWrapper.init
-000006d0: 7218 0000 0072 1900 0000 6304 0000 0000  r....r....c.....
-000006e0: 0000 0000 0000 0005 0000 0004 0000 00c3  ................
-000006f0: 0000 0073 5e00 0000 8101 7c03 6400 7500  ...s^.....|.d.u.
-00000700: 7209 7400 a001 a100 7d03 7402 7c02 8301  r.t.....}.t.|...
-00000710: 7d04 7403 7c03 7c01 7c04 8303 4900 6400  }.t.|.|.|...I.d.
-00000720: 4800 7c00 5f04 7405 7c00 6a04 7406 8302  H.|._.t.|.j.t...
-00000730: 7326 7407 a008 6401 a101 0100 7409 6402  s&t...d.....t.d.
-00000740: 8301 8201 740a 7c03 7c04 7c02 8303 7c00  ....t.|.|.|...|.
-00000750: 5f0b 7c00 5300 2903 4e7a 1946 6169 6c65  _.|.S.).Nz.Faile
-00000760: 6420 746f 206c 6f6f 6b75 7020 6163 746f  d to lookup acto
-00000770: 7220 6964 7a20 4661 696c 6564 2074 6f20  r idz Failed to 
-00000780: 6372 6561 7465 204d 6f6f 2041 7574 6820  create Moo Auth 
-00000790: 436c 6965 6e74 290c 721d 0000 0072 1e00  Client).r....r..
-000007a0: 0000 7207 0000 0072 0300 0000 720b 0000  ..r....r....r...
-000007b0: 00da 0a69 7369 6e73 7461 6e63 65da 0373  ...isinstance..s
-000007c0: 7472 da06 6c6f 6767 6572 da05 6572 726f  tr..logger..erro
-000007d0: 7272 2500 0000 7205 0000 0072 0c00 0000  rr%...r....r....
-000007e0: 2905 720f 0000 0072 1800 0000 7219 0000  ).r....r....r...
-000007f0: 0072 0d00 0000 5a07 6469 645f 6b65 7972  .r....Z.did_keyr
-00000800: 1000 0000 7210 0000 0072 1100 0000 7220  ....r....r....r 
-00000810: 0000 0035 0000 0073 1400 0000 0280 0806  ...5...s........
-00000820: 0801 0801 1402 0c02 0a01 0801 0e02 0402  ................
-00000830: 7a36 4175 7468 6f72 697a 6174 696f 6e57  z6AuthorizationW
-00000840: 7261 7070 6572 2e77 6974 685f 686f 7374  rapper.with_host
-00000850: 5f61 6e64 5f65 6432 3535 3139 5f70 7269  _and_ed25519_pri
-00000860: 7661 7465 5f6b 6579 720b 0000 0063 0200  vate_keyr....c..
-00000870: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000880: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
-00000890: 007c 0053 0072 0900 0000 2901 720b 0000  .|.S.r....).r...
-000008a0: 0029 0272 0f00 0000 720b 0000 0072 1000  .).r....r....r..
-000008b0: 0000 7210 0000 0072 1100 0000 da0d 7769  ..r....r......wi
-000008c0: 7468 5f61 6374 6f72 5f69 6449 0000 0073  th_actor_idI...s
-000008d0: 0400 0000 0601 0401 7a22 4175 7468 6f72  ........z"Author
-000008e0: 697a 6174 696f 6e57 7261 7070 6572 2e77  izationWrapper.w
-000008f0: 6974 685f 6163 746f 725f 6964 721b 0000  ith_actor_idr...
-00000900: 0063 0400 0000 0000 0000 0000 0000 0400  .c..............
-00000910: 0000 0400 0000 4300 0000 7322 0000 007c  ......C...s"...|
-00000920: 0364 0075 0072 0874 00a0 01a1 007d 0374  .d.u.r.t.....}.t
-00000930: 027c 037c 017c 0283 037c 005f 037c 0053  .|.|.|...|._.|.S
-00000940: 0072 0900 0000 2904 721d 0000 0072 1e00  .r....).r....r..
-00000950: 0000 7206 0000 0072 0c00 0000 2904 720f  ..r....r....).r.
-00000960: 0000 0072 1b00 0000 7219 0000 0072 0d00  ...r....r....r..
-00000970: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00000980: 0072 2200 0000 4d00 0000 7308 0000 0008  .r"...M...s.....
-00000990: 0608 010e 0204 027a 2841 7574 686f 7269  .......z(Authori
-000009a0: 7a61 7469 6f6e 5772 6170 7065 722e 7769  zationWrapper.wi
-000009b0: 7468 5f68 7474 705f 7369 676e 6174 7572  th_http_signatur
-000009c0: 6572 1c00 0000 6303 0000 0000 0000 0000  er....c.........
-000009d0: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
-000009e0: 2000 0000 7c02 6400 7500 7208 7400 a001   ...|.d.u.r.t...
-000009f0: a100 7d02 7402 7c02 7c01 8302 7c00 5f03  ..}.t.|.|...|._.
-00000a00: 7c00 5300 7209 0000 0029 0472 1d00 0000  |.S.r....).r....
-00000a10: 721e 0000 0072 0400 0000 720c 0000 0029  r....r....r....)
-00000a20: 0372 0f00 0000 721c 0000 0072 0d00 0000  .r....r....r....
-00000a30: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-00000a40: 2400 0000 5a00 0000 7308 0000 0008 0508  $...Z...s.......
-00000a50: 010c 0204 027a 2641 7574 686f 7269 7a61  .....z&Authoriza
-00000a60: 7469 6f6e 5772 6170 7065 722e 7769 7468  tionWrapper.with
-00000a70: 5f62 6561 7265 725f 746f 6b65 6e63 0100  _bearer_tokenc..
-00000a80: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00000a90: 0000 4300 0000 730e 0000 007c 00a0 0067  ..C...s....|...g
-00000aa0: 0064 01a2 01a1 0153 0029 024e 2903 721a  .d.....S.).N).r.
-00000ab0: 0000 0072 1b00 0000 7219 0000 00a9 01da  ...r....r.......
-00000ac0: 095f 6861 735f 6b65 7973 720e 0000 0072  ._has_keysr....r
-00000ad0: 1000 0000 7210 0000 0072 1100 0000 7221  ....r....r....r!
-00000ae0: 0000 0066 0000 00f3 0200 0000 0e01 7a28  ...f..........z(
-00000af0: 4175 7468 6f72 697a 6174 696f 6e57 7261  AuthorizationWra
-00000b00: 7070 6572 2e5f 6861 735f 6874 7470 5f73  pper._has_http_s
-00000b10: 6967 6e61 7475 7265 6301 0000 0000 0000  ignaturec.......
-00000b20: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00000b30: 00f3 0e00 0000 7c00 a000 6401 6402 6702  ......|...d.d.g.
-00000b40: a101 5300 2903 4e72 1800 0000 7219 0000  ..S.).Nr....r...
-00000b50: 0072 2b00 0000 720e 0000 0072 1000 0000  .r+...r....r....
-00000b60: 7210 0000 0072 1100 0000 721f 0000 0069  r....r....r....i
-00000b70: 0000 0072 2d00 0000 7a22 4175 7468 6f72  ...r-...z"Author
-00000b80: 697a 6174 696f 6e57 7261 7070 6572 2e5f  izationWrapper._
-00000b90: 6861 735f 6d6f 6f5f 6175 7468 6301 0000  has_moo_authc...
-00000ba0: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00000bb0: 0043 0000 0072 2e00 0000 2903 4e72 1a00  .C...r....).Nr..
-00000bc0: 0000 721c 0000 0072 2b00 0000 720e 0000  ..r....r+...r...
-00000bd0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000be0: 7223 0000 006c 0000 0072 2d00 0000 7a25  r#...l...r-...z%
-00000bf0: 4175 7468 6f72 697a 6174 696f 6e57 7261  AuthorizationWra
-00000c00: 7070 6572 2e5f 6861 735f 6265 6172 6572  pper._has_bearer
-00000c10: 5f61 7574 68da 086b 6579 5f6c 6973 7463  _auth..key_listc
-00000c20: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00000c30: 0300 0000 4300 0000 731e 0000 007c 0144  ....C...s....|.D
-00000c40: 005d 0a7d 027c 027c 006a 0076 0172 0c01  .].}.|.|.j.v.r..
-00000c50: 0064 0153 0071 0264 0253 0029 034e 4654  .d.S.q.d.S.).NFT
-00000c60: 2901 720a 0000 0029 0372 0f00 0000 722f  ).r....).r....r/
-00000c70: 0000 00da 036b 6579 7210 0000 0072 1000  .....keyr....r..
-00000c80: 0000 7211 0000 0072 2c00 0000 6f00 0000  ..r....r,...o...
-00000c90: 730a 0000 0008 010a 0106 0102 ff04 037a  s..............z
-00000ca0: 1e41 7574 686f 7269 7a61 7469 6f6e 5772  .AuthorizationWr
-00000cb0: 6170 7065 722e 5f68 6173 5f6b 6579 7372  apper._has_keysr
-00000cc0: 0900 0000 2914 da08 5f5f 6e61 6d65 5f5f  ....)...__name__
-00000cd0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000ce0: 7175 616c 6e61 6d65 5f5f 7212 0000 0072  qualname__r....r
-00000cf0: 1400 0000 7217 0000 0072 0200 0000 721d  ....r....r....r.
-00000d00: 0000 0072 1e00 0000 7213 0000 0072 2700  ...r....r....r'.
-00000d10: 0000 7220 0000 0072 2a00 0000 7222 0000  ..r ...r*...r"..
-00000d20: 0072 2400 0000 7221 0000 0072 1f00 0000  .r$...r!...r....
-00000d30: 7223 0000 00da 046c 6973 7472 2c00 0000  r#.....listr,...
-00000d40: 7210 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-00000d50: 1100 0000 7208 0000 000f 0000 0073 4000  ....r........s@.
-00000d60: 0000 0800 0801 0806 0804 1603 021c 04fc  ................
-00000d70: 0202 02fe 0203 02fd 0804 0afc 0e14 0208  ................
-00000d80: 04fc 0202 02fe 0203 02fd 0804 0afc 0210  ................
-00000d90: 04fd 0202 02fe 0803 0afd 080c 0803 0803  ................
-00000da0: 1203 7208 0000 0029 12da 076c 6f67 6769  ..r....)...loggi
-00000db0: 6e67 da06 7479 7069 6e67 7202 0000 0072  ng..typingr....r
-00000dc0: 1d00 0000 5a0e 626f 7669 6e65 2e63 6c69  ....Z.bovine.cli
-00000dd0: 656e 7473 7203 0000 005a 1562 6f76 696e  entsr....Z.bovin
-00000de0: 652e 636c 6965 6e74 732e 6265 6172 6572  e.clients.bearer
-00000df0: 7204 0000 005a 1762 6f76 696e 652e 636c  r....Z.bovine.cl
-00000e00: 6965 6e74 732e 6d6f 6f5f 6175 7468 7205  ients.moo_authr.
-00000e10: 0000 005a 1a62 6f76 696e 652e 636c 6965  ...Z.bovine.clie
-00000e20: 6e74 732e 7369 676e 6564 5f68 7474 7072  nts.signed_httpr
-00000e30: 0600 0000 5a0d 626f 7669 6e65 2e63 7279  ....Z.bovine.cry
-00000e40: 7074 6f72 0700 0000 da09 6765 744c 6f67  ptor......getLog
-00000e50: 6765 7272 3100 0000 7228 0000 0072 0800  gerr1...r(...r..
-00000e60: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
-00000e70: 0072 1100 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000e80: 0100 0000 7314 0000 0008 000c 0108 020c  ....s...........
-00000e90: 020c 010c 010c 010c 010a 0212 03         .............
+00000090: 4700 6409 640a 8400 640a 8302 5a11 6401  G.d.d...d...Z.d.
+000000a0: 5300 290b e900 0000 004e 2901 da08 4f70  S.)......N)...Op
+000000b0: 7469 6f6e 616c 2901 da16 7072 6976 6174  tional)...privat
+000000c0: 655f 6b65 795f 746f 5f64 6964 5f6b 6579  e_key_to_did_key
+000000d0: e901 0000 0029 01da 196c 6f6f 6b75 705f  .....)...lookup_
+000000e0: 6469 645f 7769 7468 5f77 6562 6669 6e67  did_with_webfing
+000000f0: 6572 2901 da10 4265 6172 6572 4175 7468  er)...BearerAuth
+00000100: 436c 6965 6e74 2901 da0d 4d6f 6f41 7574  Client)...MooAut
+00000110: 6843 6c69 656e 7429 01da 1053 6967 6e65  hClient)...Signe
+00000120: 6448 7474 7043 6c69 656e 7463 0000 0000  dHttpClientc....
+00000130: 0000 0000 0000 0000 0000 0000 0800 0000  ................
+00000140: 4000 0000 73ca 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00000150: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
+00000160: 0464 0564 0684 005a 0564 2164 0865 0665  .d.d...Z.d!d.e.e
+00000170: 076a 0819 0066 0264 0964 0a84 055a 0909  .j...f.d.d...Z..
+00000180: 0764 2164 0b65 0a64 0c65 0a64 0865 0665  .d!d.e.d.e.d.e.e
+00000190: 076a 0819 0066 0664 0d64 0e84 055a 0b64  .j...f.d.d...Z.d
+000001a0: 0f65 0a66 0264 1064 1184 045a 0c09 0764  .e.f.d.d...Z...d
+000001b0: 2164 1265 0a64 0c65 0a64 0865 0665 076a  !d.e.d.e.d.e.e.j
+000001c0: 0819 0066 0664 1364 1484 055a 0d09 0764  ...f.d.d...Z...d
+000001d0: 2164 1565 0a64 0865 0665 076a 0819 0066  !d.e.d.e.e.j...f
+000001e0: 0464 1664 1784 055a 0e64 1864 1984 005a  .d.d...Z.d.d...Z
+000001f0: 0f64 1a64 1b84 005a 1064 1c64 1d84 005a  .d.d...Z.d.d...Z
+00000200: 1164 1e65 1266 0264 1f64 2084 045a 1364  .d.e.f.d.d ..Z.d
+00000210: 0753 0029 22da 1441 7574 686f 7269 7a61  .S.)"..Authoriza
+00000220: 7469 6f6e 5772 6170 7065 7263 0100 0000  tionWrapperc....
+00000230: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00000240: 4300 0000 731c 0000 0064 007c 005f 0064  C...s....d.|._.d
+00000250: 007c 005f 0164 007c 005f 0264 007c 005f  .|._.d.|._.d.|._
+00000260: 0364 0053 00a9 014e 2904 da06 636f 6e66  .d.S...N)...conf
+00000270: 6967 da08 6163 746f 725f 6964 da06 636c  ig..actor_id..cl
+00000280: 6965 6e74 da07 7365 7373 696f 6ea9 01da  ient..session...
+00000290: 0473 656c 66a9 0072 1100 0000 fa59 2f77  .self..r.....Y/w
+000002a0: 6f6f 6470 6563 6b65 722f 7372 632f 636f  oodpecker/src/co
+000002b0: 6465 6265 7267 2e6f 7267 2f62 6f76 696e  deberg.org/bovin
+000002c0: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
+000002d0: 626f 7669 6e65 2f63 6c69 656e 7473 2f61  bovine/clients/a
+000002e0: 7574 686f 7269 7a61 7469 6f6e 5f77 7261  uthorization_wra
+000002f0: 7070 6572 2e70 79da 085f 5f69 6e69 745f  pper.py..__init_
+00000300: 5f11 0000 0073 0800 0000 0601 0601 0601  _....s..........
+00000310: 0a01 7a1d 4175 7468 6f72 697a 6174 696f  ..z.Authorizatio
+00000320: 6e57 7261 7070 6572 2e5f 5f69 6e69 745f  nWrapper.__init_
+00000330: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00000340: 0000 0200 0000 c300 0000 7314 0000 0081  ..........s.....
+00000350: 017c 00a0 00a1 0049 0064 0048 0001 007c  .|.....I.d.H...|
+00000360: 0053 0072 0a00 0000 2901 da04 696e 6974  .S.r....)...init
+00000370: 720f 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00000380: 1200 0000 da0a 5f5f 6165 6e74 6572 5f5f  ......__aenter__
+00000390: 1700 0000 7306 0000 0002 800e 0104 017a  ....s..........z
+000003a0: 1f41 7574 686f 7269 7a61 7469 6f6e 5772  .AuthorizationWr
+000003b0: 6170 7065 722e 5f5f 6165 6e74 6572 5f5f  apper.__aenter__
+000003c0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000003d0: 0002 0000 00c7 0000 0073 1600 0000 8101  .........s......
+000003e0: 7c00 6a00 a001 a100 4900 6400 4800 0100  |.j.....I.d.H...
+000003f0: 6400 5300 720a 0000 0029 0272 0e00 0000  d.S.r....).r....
+00000400: da05 636c 6f73 6529 0272 1000 0000 da04  ..close).r......
+00000410: 6172 6773 7211 0000 0072 1100 0000 7212  argsr....r....r.
+00000420: 0000 00da 095f 5f61 6578 6974 5f5f 1b00  .....__aexit__..
+00000430: 0000 7304 0000 0002 8014 017a 1e41 7574  ..s........z.Aut
+00000440: 686f 7269 7a61 7469 6f6e 5772 6170 7065  horizationWrappe
+00000450: 722e 5f5f 6165 7869 745f 5f4e 720e 0000  r.__aexit__Nr...
+00000460: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00000470: 0000 0500 0000 c300 0000 73c0 0000 0081  ..........s.....
+00000480: 017c 017c 005f 007c 0164 0075 0072 0d74  .|.|._.|.d.u.r.t
+00000490: 01a0 02a1 007c 005f 007c 006a 0373 124a  .....|._.|.j.s.J
+000004a0: 0082 017c 00a0 04a1 0072 2a7c 006a 057c  ...|.....r*|.j.|
+000004b0: 006a 0364 0119 007c 006a 0364 0219 007c  .j.d...|.j.d...|
+000004c0: 006a 0064 038d 0349 0064 0048 0001 0064  .j.d...I.d.H...d
+000004d0: 0053 007c 00a0 06a1 0072 457c 006a 0364  .S.|.....rE|.j.d
+000004e0: 0419 007c 005f 077c 006a 087c 006a 0364  ...|._.|.j.|.j.d
+000004f0: 0519 007c 006a 0364 0219 007c 006a 0064  ...|.j.d...|.j.d
+00000500: 038d 0301 0064 0053 007c 00a0 09a1 0072  .....d.S.|.....r
+00000510: 5c7c 006a 0364 0419 007c 005f 077c 006a  \|.j.d...|._.|.j
+00000520: 0a7c 006a 0364 0619 007c 006a 0064 038d  .|.j.d...|.j.d..
+00000530: 0201 0064 0053 0074 0b64 0783 0182 0129  ...d.S.t.d.....)
+00000540: 084e da04 686f 7374 da0b 7072 6976 6174  .N..host..privat
+00000550: 655f 6b65 7929 0172 0e00 0000 da0b 6163  e_key).r......ac
+00000560: 636f 756e 745f 7572 6cda 0e70 7562 6c69  count_url..publi
+00000570: 635f 6b65 795f 7572 6cda 0c61 6363 6573  c_key_url..acces
+00000580: 735f 746f 6b65 6e7a 274e 6f20 6b6e 6f77  s_tokenz'No know
+00000590: 6e20 6175 7468 6f72 697a 6174 696f 6e20  n authorization 
+000005a0: 6d65 7468 6f64 2061 7661 696c 6162 6c65  method available
+000005b0: 290c 720e 0000 00da 0761 696f 6874 7470  ).r......aiohttp
+000005c0: da0d 436c 6965 6e74 5365 7373 696f 6e72  ..ClientSessionr
+000005d0: 0b00 0000 da0d 5f68 6173 5f6d 6f6f 5f61  ......_has_moo_a
+000005e0: 7574 68da 2177 6974 685f 686f 7374 5f61  uth.!with_host_a
+000005f0: 6e64 5f65 6432 3535 3139 5f70 7269 7661  nd_ed25519_priva
+00000600: 7465 5f6b 6579 da13 5f68 6173 5f68 7474  te_key.._has_htt
+00000610: 705f 7369 676e 6174 7572 6572 0c00 0000  p_signaturer....
+00000620: da13 7769 7468 5f68 7474 705f 7369 676e  ..with_http_sign
+00000630: 6174 7572 65da 105f 6861 735f 6265 6172  ature.._has_bear
+00000640: 6572 5f61 7574 68da 1177 6974 685f 6265  er_auth..with_be
+00000650: 6172 6572 5f74 6f6b 656e da09 4578 6365  arer_token..Exce
+00000660: 7074 696f 6e29 0272 1000 0000 720e 0000  ption).r....r...
+00000670: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000680: 7214 0000 001e 0000 0073 2800 0000 0280  r........s(.....
+00000690: 0601 0801 0a01 0a02 0802 0401 1401 10ff  ................
+000006a0: 0803 0c01 0401 0801 0801 0401 0afd 0805  ................
+000006b0: 0c01 1a01 0802 7a19 4175 7468 6f72 697a  ......z.Authoriz
+000006c0: 6174 696f 6e57 7261 7070 6572 2e69 6e69  ationWrapper.ini
+000006d0: 7472 1900 0000 721a 0000 0063 0400 0000  tr....r....c....
+000006e0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
+000006f0: c300 0000 735e 0000 0081 017c 0364 0075  ....s^.....|.d.u
+00000700: 0072 0974 00a0 01a1 007d 0374 027c 0283  .r.t.....}.t.|..
+00000710: 017d 0474 037c 037c 017c 0483 0349 0064  .}.t.|.|.|...I.d
+00000720: 0048 007c 005f 0474 057c 006a 0474 0683  .H.|._.t.|.j.t..
+00000730: 0273 2674 07a0 0864 01a1 0101 0074 0964  .s&t...d.....t.d
+00000740: 0283 0182 0174 0a7c 037c 047c 0283 037c  .....t.|.|.|...|
+00000750: 005f 0b7c 0053 0029 034e 7a19 4661 696c  ._.|.S.).Nz.Fail
+00000760: 6564 2074 6f20 6c6f 6f6b 7570 2061 6374  ed to lookup act
+00000770: 6f72 2069 647a 2046 6169 6c65 6420 746f  or idz Failed to
+00000780: 2063 7265 6174 6520 4d6f 6f20 4175 7468   create Moo Auth
+00000790: 2043 6c69 656e 7429 0c72 1e00 0000 721f   Client).r....r.
+000007a0: 0000 0072 0300 0000 7205 0000 0072 0c00  ...r....r....r..
+000007b0: 0000 da0a 6973 696e 7374 616e 6365 da03  ....isinstance..
+000007c0: 7374 72da 066c 6f67 6765 72da 0565 7272  str..logger..err
+000007d0: 6f72 7226 0000 0072 0700 0000 720d 0000  orr&...r....r...
+000007e0: 0029 0572 1000 0000 7219 0000 0072 1a00  .).r....r....r..
+000007f0: 0000 720e 0000 005a 0764 6964 5f6b 6579  ..r....Z.did_key
+00000800: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00000810: 2100 0000 3600 0000 7314 0000 0002 8008  !...6...s.......
+00000820: 0608 0108 0114 020c 020a 0108 010e 0204  ................
+00000830: 027a 3641 7574 686f 7269 7a61 7469 6f6e  .z6Authorization
+00000840: 5772 6170 7065 722e 7769 7468 5f68 6f73  Wrapper.with_hos
+00000850: 745f 616e 645f 6564 3235 3531 395f 7072  t_and_ed25519_pr
+00000860: 6976 6174 655f 6b65 7972 0c00 0000 6302  ivate_keyr....c.
+00000870: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00000880: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
+00000890: 5f00 7c00 5300 720a 0000 0029 0172 0c00  _.|.S.r....).r..
+000008a0: 0000 2902 7210 0000 0072 0c00 0000 7211  ..).r....r....r.
+000008b0: 0000 0072 1100 0000 7212 0000 00da 0d77  ...r....r......w
+000008c0: 6974 685f 6163 746f 725f 6964 4a00 0000  ith_actor_idJ...
+000008d0: 7304 0000 0006 0104 017a 2241 7574 686f  s........z"Autho
+000008e0: 7269 7a61 7469 6f6e 5772 6170 7065 722e  rizationWrapper.
+000008f0: 7769 7468 5f61 6374 6f72 5f69 6472 1c00  with_actor_idr..
+00000900: 0000 6304 0000 0000 0000 0000 0000 0004  ..c.............
+00000910: 0000 0004 0000 0043 0000 0073 2200 0000  .......C...s"...
+00000920: 7c03 6400 7500 7208 7400 a001 a100 7d03  |.d.u.r.t.....}.
+00000930: 7402 7c03 7c01 7c02 8303 7c00 5f03 7c00  t.|.|.|...|._.|.
+00000940: 5300 720a 0000 0029 0472 1e00 0000 721f  S.r....).r....r.
+00000950: 0000 0072 0800 0000 720d 0000 0029 0472  ...r....r....).r
+00000960: 1000 0000 721c 0000 0072 1a00 0000 720e  ....r....r....r.
+00000970: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
+00000980: 0000 7223 0000 004e 0000 0073 0800 0000  ..r#...N...s....
+00000990: 0806 0801 0e02 0402 7a28 4175 7468 6f72  ........z(Author
+000009a0: 697a 6174 696f 6e57 7261 7070 6572 2e77  izationWrapper.w
+000009b0: 6974 685f 6874 7470 5f73 6967 6e61 7475  ith_http_signatu
+000009c0: 7265 721d 0000 0063 0300 0000 0000 0000  rer....c........
+000009d0: 0000 0000 0300 0000 0300 0000 4300 0000  ............C...
+000009e0: 7320 0000 007c 0264 0075 0072 0874 00a0  s ...|.d.u.r.t..
+000009f0: 01a1 007d 0274 027c 027c 0183 027c 005f  ...}.t.|.|...|._
+00000a00: 037c 0053 0072 0a00 0000 2904 721e 0000  .|.S.r....).r...
+00000a10: 0072 1f00 0000 7206 0000 0072 0d00 0000  .r....r....r....
+00000a20: 2903 7210 0000 0072 1d00 0000 720e 0000  ).r....r....r...
+00000a30: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000a40: 7225 0000 005b 0000 0073 0800 0000 0805  r%...[...s......
+00000a50: 0801 0c02 0402 7a26 4175 7468 6f72 697a  ......z&Authoriz
+00000a60: 6174 696f 6e57 7261 7070 6572 2e77 6974  ationWrapper.wit
+00000a70: 685f 6265 6172 6572 5f74 6f6b 656e 6301  h_bearer_tokenc.
+00000a80: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000a90: 0000 0043 0000 0073 0e00 0000 7c00 a000  ...C...s....|...
+00000aa0: 6700 6401 a201 a101 5300 2902 4e29 0372  g.d.....S.).N).r
+00000ab0: 1b00 0000 721c 0000 0072 1a00 0000 a901  ....r....r......
+00000ac0: da09 5f68 6173 5f6b 6579 7372 0f00 0000  .._has_keysr....
+00000ad0: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00000ae0: 2200 0000 6700 0000 f302 0000 000e 017a  "...g..........z
+00000af0: 2841 7574 686f 7269 7a61 7469 6f6e 5772  (AuthorizationWr
+00000b00: 6170 7065 722e 5f68 6173 5f68 7474 705f  apper._has_http_
+00000b10: 7369 676e 6174 7572 6563 0100 0000 0000  signaturec......
+00000b20: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00000b30: 0000 f30e 0000 007c 00a0 0064 0164 0267  .......|...d.d.g
+00000b40: 02a1 0153 0029 034e 7219 0000 0072 1a00  ...S.).Nr....r..
+00000b50: 0000 722c 0000 0072 0f00 0000 7211 0000  ..r,...r....r...
+00000b60: 0072 1100 0000 7212 0000 0072 2000 0000  .r....r....r ...
+00000b70: 6a00 0000 722e 0000 007a 2241 7574 686f  j...r....z"Autho
+00000b80: 7269 7a61 7469 6f6e 5772 6170 7065 722e  rizationWrapper.
+00000b90: 5f68 6173 5f6d 6f6f 5f61 7574 6863 0100  _has_moo_authc..
+00000ba0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00000bb0: 0000 4300 0000 722f 0000 0029 034e 721b  ..C...r/...).Nr.
+00000bc0: 0000 0072 1d00 0000 722c 0000 0072 0f00  ...r....r,...r..
+00000bd0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
+00000be0: 0072 2400 0000 6d00 0000 722e 0000 007a  .r$...m...r....z
+00000bf0: 2541 7574 686f 7269 7a61 7469 6f6e 5772  %AuthorizationWr
+00000c00: 6170 7065 722e 5f68 6173 5f62 6561 7265  apper._has_beare
+00000c10: 725f 6175 7468 da08 6b65 795f 6c69 7374  r_auth..key_list
+00000c20: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00000c30: 0003 0000 0043 0000 0073 1e00 0000 7c01  .....C...s....|.
+00000c40: 4400 5d0a 7d02 7c02 7c00 6a00 7601 720c  D.].}.|.|.j.v.r.
+00000c50: 0100 6401 5300 7102 6402 5300 2903 4e46  ..d.S.q.d.S.).NF
+00000c60: 5429 0172 0b00 0000 2903 7210 0000 0072  T).r....).r....r
+00000c70: 3000 0000 da03 6b65 7972 1100 0000 7211  0.....keyr....r.
+00000c80: 0000 0072 1200 0000 722d 0000 0070 0000  ...r....r-...p..
+00000c90: 0073 0a00 0000 0801 0a01 0601 02ff 0403  .s..............
+00000ca0: 7a1e 4175 7468 6f72 697a 6174 696f 6e57  z.AuthorizationW
+00000cb0: 7261 7070 6572 2e5f 6861 735f 6b65 7973  rapper._has_keys
+00000cc0: 720a 0000 0029 14da 085f 5f6e 616d 655f  r....)...__name_
+00000cd0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000ce0: 5f71 7561 6c6e 616d 655f 5f72 1300 0000  _qualname__r....
+00000cf0: 7215 0000 0072 1800 0000 7202 0000 0072  r....r....r....r
+00000d00: 1e00 0000 721f 0000 0072 1400 0000 7228  ....r....r....r(
+00000d10: 0000 0072 2100 0000 722b 0000 0072 2300  ...r!...r+...r#.
+00000d20: 0000 7225 0000 0072 2200 0000 7220 0000  ..r%...r"...r ..
+00000d30: 0072 2400 0000 da04 6c69 7374 722d 0000  .r$.....listr-..
+00000d40: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
+00000d50: 7212 0000 0072 0900 0000 1000 0000 7340  r....r........s@
+00000d60: 0000 0008 0008 0108 0608 0416 0302 1c04  ................
+00000d70: fc02 0202 fe02 0302 fd08 040a fc0e 1402  ................
+00000d80: 0804 fc02 0202 fe02 0302 fd08 040a fc02  ................
+00000d90: 1004 fd02 0202 fe08 030a fd08 0c08 0308  ................
+00000da0: 0312 0372 0900 0000 2912 da07 6c6f 6767  ...r....)...logg
+00000db0: 696e 67da 0674 7970 696e 6772 0200 0000  ing..typingr....
+00000dc0: 721e 0000 005a 0d62 6f76 696e 652e 6372  r....Z.bovine.cr
+00000dd0: 7970 746f 7203 0000 00da 0072 0500 0000  yptor......r....
+00000de0: 5a06 6265 6172 6572 7206 0000 005a 086d  Z.bearerr....Z.m
+00000df0: 6f6f 5f61 7574 6872 0700 0000 5a0b 7369  oo_authr....Z.si
+00000e00: 676e 6564 5f68 7474 7072 0800 0000 da09  gned_httpr......
+00000e10: 6765 744c 6f67 6765 7272 3200 0000 7229  getLoggerr2...r)
+00000e20: 0000 0072 0900 0000 7211 0000 0072 1100  ...r....r....r..
+00000e30: 0000 7211 0000 0072 1200 0000 da08 3c6d  ..r....r......<m
+00000e40: 6f64 756c 653e 0100 0000 7314 0000 0008  odule>....s.....
+00000e50: 000c 0108 020c 020c 020c 010c 010c 010a  ................
+00000e60: 0212 03                                  ...
```

### Comparing `bovine-0.2.5/bovine/activitypub/authorization_wrapper.py` & `bovine-0.2.6/bovine/clients/authorization_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from typing import Optional
 
 import aiohttp
 
-from bovine.clients import lookup_did_with_webfinger
-from bovine.clients.bearer import BearerAuthClient
-from bovine.clients.moo_auth import MooAuthClient
-from bovine.clients.signed_http import SignedHttpClient
 from bovine.crypto import private_key_to_did_key
 
+from . import lookup_did_with_webfinger
+from .bearer import BearerAuthClient
+from .moo_auth import MooAuthClient
+from .signed_http import SignedHttpClient
+
 logger = logging.getLogger(__name__)
 
 
 class AuthorizationWrapper:
     def __init__(self):
         self.config: Optional[dict] = None
         self.actor_id: Optional[str] = None
```

### Comparing `bovine-0.2.5/bovine/activitypub/test_actor.py` & `bovine-0.2.6/bovine/test_bovine_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/activitystreams/__init__.py` & `bovine-0.2.6/bovine/activitystreams/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.6/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 4957 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 5d13 0000  o.......5bsd]...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 5d13 0000  o.........|d]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6406 6c09 6d0a 5a0a 0100 6407  ..d.d.l.m.Z...d.
 00000070: 650b 6408 6504 6508 650a 6602 1900 6604  e.d.e.e.e.f...f.
@@ -140,15 +140,15 @@
 000008b0: 0372 2c7c 0253 007c 00a0 06a1 007d 037c  .r,|.S.|.....}.|
 000008c0: 0372 367c 037c 0264 033c 007c 006a 0772  .r6|.|.d.<.|.j.r
 000008d0: 3e7c 006a 077c 0264 043c 007c 006a 0872  >|.j.|.d.<.|.j.r
 000008e0: 467c 006a 087c 0264 053c 007c 0253 0029  F|.j.|.d.<.|.S.)
 000008f0: 064e 7213 0000 0072 1400 0000 da09 656e  .Nr....r......en
 00000900: 6470 6f69 6e74 7372 1500 0000 7216 0000  dpointsr....r...
 00000910: 0029 0972 0500 0000 7223 0000 0072 1300  .).r....r#...r..
-00000920: 0000 720f 0000 0072 1400 0000 da05 4f57  ..r....r......OW
+00000920: 0000 720f 0000 0072 1400 0000 5a05 4f57  ..r....r....Z.OW
 00000930: 4e45 52da 155f 6275 696c 645f 7573 6572  NER.._build_user
 00000940: 5f65 6e64 706f 696e 7473 7215 0000 0072  _endpointsr....r
 00000950: 1600 0000 2904 7225 0000 0072 1f00 0000  ....).r%...r....
 00000960: 7226 0000 0072 2e00 0000 720b 0000 0072  r&...r....r....r
 00000970: 0b00 0000 720c 0000 0072 2200 0000 5900  ....r....r"...Y.
 00000980: 0000 7326 0000 0004 010a 0204 0106 020c  ..s&............
 00000990: 010a 0206 020c 010a 020a 0204 0108 0204  ................
@@ -158,30 +158,30 @@
 000009d0: 0000 0200 0000 0300 0000 4300 0000 7328  ..........C...s(
 000009e0: 0000 0069 007d 017c 006a 0072 0a7c 006a  ...i.}.|.j.r.|.j
 000009f0: 007c 0164 013c 007c 006a 0172 127c 006a  .|.d.<.|.j.r.|.j
 00000a00: 017c 0164 023c 007c 0153 0029 034e da0b  .|.d.<.|.S.).N..
 00000a10: 6576 656e 7453 6f75 7263 65da 0870 726f  eventSource..pro
 00000a20: 7879 5572 6c29 0272 1900 0000 721a 0000  xyUrl).r....r...
 00000a30: 0029 0272 2500 0000 722e 0000 0072 0b00  .).r%...r....r..
-00000a40: 0000 720b 0000 0072 0c00 0000 7230 0000  ..r....r....r0..
+00000a40: 0000 720b 0000 0072 0c00 0000 722f 0000  ..r....r....r/..
 00000a50: 0077 0000 0073 0c00 0000 0401 0601 0a01  .w...s..........
 00000a60: 0601 0a01 0401 7a1b 4163 746f 722e 5f62  ......z.Actor._b
 00000a70: 7569 6c64 5f75 7365 725f 656e 6470 6f69  uild_user_endpoi
 00000a80: 6e74 7329 1dda 085f 5f6e 616d 655f 5fda  nts)...__name__.
 00000a90: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
 00000aa0: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
 00000ab0: 5f5f da03 7374 72da 0f5f 5f61 6e6e 6f74  __..str..__annot
 00000ac0: 6174 696f 6e73 5f5f 7210 0000 0072 1100  ations__r....r..
 00000ad0: 0000 7203 0000 0072 1200 0000 7213 0000  ..r....r....r...
 00000ae0: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
 00000af0: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
 00000b00: 1a00 0000 721b 0000 0072 1c00 0000 da04  ....r....r......
-00000b10: 6469 6374 721d 0000 0072 0500 0000 da06  dictr....r......
+00000b10: 6469 6374 721d 0000 0072 0500 0000 5a06  dictr....r....Z.
 00000b20: 5055 424c 4943 7229 0000 0072 2000 0000  PUBLICr)...r ...
-00000b30: 7221 0000 0072 2200 0000 7230 0000 0072  r!...r"...r0...r
+00000b30: 7221 0000 0072 2200 0000 722f 0000 0072  r!...r"...r/...r
 00000b40: 0b00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
 00000b50: 0000 0072 0e00 0000 1100 0000 732c 0000  ...r........s,..
 00000b60: 000a 0004 0208 020c 0110 0110 0110 0110  ................
 00000b70: 0110 0110 0110 0110 0110 0110 0110 0210  ................
 00000b80: 0110 010e 0208 1f08 0908 0b0c 1e72 0e00  .............r..
 00000b90: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
 00000ba0: 0000 0003 0000 0040 0000 0073 2c00 0000  .......@...s,...
@@ -189,26 +189,26 @@
 00000bc0: 3c00 6505 6504 6402 3c00 6403 6506 6602  <.e.e.d.<.d.e.f.
 00000bd0: 6404 6405 8404 5a07 6406 5300 2907 da0a  d.d...Z.d.S.)...
 00000be0: 436f 6c6c 6563 7469 6f6e 720f 0000 0072  Collectionr....r
 00000bf0: 2400 0000 720a 0000 0063 0100 0000 0000  $...r....c......
 00000c00: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
 00000c10: 0000 7312 0000 0064 017c 006a 007c 006a  ..s....d.|.j.|.j
 00000c20: 0164 0264 039c 0453 0029 044e 722a 0000  .d.d...S.).Nr*..
-00000c30: 0072 3b00 0000 2904 721e 0000 0072 0f00  .r;...).r....r..
+00000c30: 0072 3900 0000 2904 721e 0000 0072 0f00  .r9...).r....r..
 00000c40: 0000 7224 0000 0072 1000 0000 2902 720f  ..r$...r....).r.
 00000c50: 0000 0072 2400 0000 722b 0000 0072 0b00  ...r$...r+...r..
 00000c60: 0000 720b 0000 0072 0c00 0000 7229 0000  ..r....r....r)..
 00000c70: 0085 0000 0073 0a00 0000 0202 0401 0401  .....s..........
 00000c80: 0201 06fc 7a10 436f 6c6c 6563 7469 6f6e  ....z.Collection
-00000c90: 2e62 7569 6c64 4e29 0872 3300 0000 7234  .buildN).r3...r4
-00000ca0: 0000 0072 3500 0000 7237 0000 0072 3800  ...r5...r7...r8.
-00000cb0: 0000 da04 6c69 7374 7239 0000 0072 2900  ....listr9...r).
+00000c90: 2e62 7569 6c64 4e29 0872 3200 0000 7233  .buildN).r2...r3
+00000ca0: 0000 0072 3400 0000 7236 0000 0072 3700  ...r4...r6...r7.
+00000cb0: 0000 da04 6c69 7374 7238 0000 0072 2900  ....listr8...r).
 00000cc0: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-00000cd0: 0072 0c00 0000 723b 0000 0080 0000 0073  .r....r;.......s
-00000ce0: 0800 0000 0a00 0802 0801 1202 723b 0000  ............r;..
+00000cd0: 0072 0c00 0000 7239 0000 0080 0000 0073  .r....r9.......s
+00000ce0: 0800 0000 0a00 0802 0801 1202 7239 0000  ............r9..
 00000cf0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
 00000d00: 0000 0300 0000 4000 0000 7360 0000 0065  ......@...s`...e
 00000d10: 005a 0164 005a 0255 0065 0365 0464 013c  .Z.d.Z.U.e.e.d.<
 00000d20: 0064 025a 0565 0664 0242 0065 0464 033c  .d.Z.e.d.B.e.d.<
 00000d30: 0064 045a 0765 0865 0464 053c 0064 025a  .d.Z.e.e.d.<.d.Z
 00000d40: 0965 0364 0242 0065 0464 063c 0064 025a  .e.d.B.e.d.<.d.Z
 00000d50: 0a65 0364 0242 0065 0464 073c 0064 0865  .e.d.B.e.d.<.d.e
@@ -219,33 +219,33 @@
 00000da0: 7374 da04 6c61 7374 720a 0000 0063 0100  st..lastr....c..
 00000db0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
 00000dc0: 0000 4300 0000 7346 0000 0064 017c 006a  ..C...sF...d.|.j
 00000dd0: 007c 006a 0164 0264 039c 047d 017c 006a  .|.j.d.d...}.|.j
 00000de0: 0272 117c 006a 027c 0164 043c 007c 006a  .r.|.j.|.d.<.|.j
 00000df0: 0372 197c 006a 037c 0164 053c 007c 006a  .r.|.j.|.d.<.|.j
 00000e00: 0472 217c 006a 047c 0164 063c 007c 0153  .r!|.j.|.d.<.|.S
-00000e10: 0029 074e 722a 0000 0072 3d00 0000 2904  .).Nr*...r=...).
+00000e10: 0029 074e 722a 0000 0072 3b00 0000 2904  .).Nr*...r;...).
 00000e20: 721e 0000 0072 0f00 0000 da0a 746f 7461  r....r......tota
 00000e30: 6c49 7465 6d73 7210 0000 00da 0c6f 7264  lItemsr......ord
-00000e40: 6572 6564 4974 656d 7372 3f00 0000 7240  eredItemsr?...r@
-00000e50: 0000 0029 0572 0f00 0000 723e 0000 0072  ...).r....r>...r
-00000e60: 2400 0000 723f 0000 0072 4000 0000 a902  $...r?...r@.....
+00000e40: 6572 6564 4974 656d 7372 3d00 0000 723e  eredItemsr=...r>
+00000e50: 0000 0029 0572 0f00 0000 723c 0000 0072  ...).r....r<...r
+00000e60: 2400 0000 723d 0000 0072 3e00 0000 a902  $...r=...r>.....
 00000e70: 7225 0000 0072 2600 0000 720b 0000 0072  r%...r&...r....r
 00000e80: 0b00 0000 720c 0000 0072 2900 0000 9600  ....r....r).....
 00000e90: 0000 7318 0000 0002 0204 0104 0102 0106  ..s.............
 00000ea0: fc06 070a 0106 020a 0106 020a 0104 027a  ...............z
 00000eb0: 174f 7264 6572 6564 436f 6c6c 6563 7469  .OrderedCollecti
-00000ec0: 6f6e 2e62 7569 6c64 290d 7233 0000 0072  on.build).r3...r
-00000ed0: 3400 0000 7235 0000 0072 3700 0000 7238  4...r5...r7...r8
-00000ee0: 0000 0072 2400 0000 723c 0000 0072 3e00  ...r$...r<...r>.
-00000ef0: 0000 da03 696e 7472 3f00 0000 7240 0000  ....intr?...r@..
-00000f00: 0072 3900 0000 7229 0000 0072 0b00 0000  .r9...r)...r....
+00000ec0: 6f6e 2e62 7569 6c64 290d 7232 0000 0072  on.build).r2...r
+00000ed0: 3300 0000 7234 0000 0072 3600 0000 7237  3...r4...r6...r7
+00000ee0: 0000 0072 2400 0000 723a 0000 0072 3c00  ...r$...r:...r<.
+00000ef0: 0000 da03 696e 7472 3d00 0000 723e 0000  ....intr=...r>..
+00000f00: 0072 3800 0000 7229 0000 0072 0b00 0000  .r8...r)...r....
 00000f10: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000f20: 3d00 0000 8e00 0000 730e 0000 000a 0008  =.......s.......
-00000f30: 0210 010c 0110 0110 0112 0272 3d00 0000  ...........r=...
+00000f20: 3b00 0000 8e00 0000 730e 0000 000a 0008  ;.......s.......
+00000f30: 0210 010c 0110 0110 0112 0272 3b00 0000  ...........r;...
 00000f40: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000f50: 0003 0000 0040 0000 0073 5400 0000 6500  .....@...sT...e.
 00000f60: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
 00000f70: 6505 6504 6402 3c00 6503 6504 6403 3c00  e.e.d.<.e.e.d.<.
 00000f80: 6404 5a06 6503 6404 4200 6504 6405 3c00  d.Z.e.d.B.e.d.<.
 00000f90: 6404 5a07 6503 6404 4200 6504 6406 3c00  d.Z.e.d.B.e.d.<.
 00000fa0: 6407 6508 6602 6408 6409 8404 5a09 6404  d.e.f.d.d...Z.d.
@@ -255,37 +255,37 @@
 00000fe0: 046e 6578 74da 0470 7265 7672 0a00 0000  .next..prevr....
 00000ff0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
 00001000: 0006 0000 0043 0000 0073 3a00 0000 6401  .....C...s:...d.
 00001010: 7c00 6a00 7c00 6a01 7c00 6a02 6402 6403  |.j.|.j.|.j.d.d.
 00001020: 9c05 7d01 7c00 6a03 7213 7c00 6a03 7c01  ..}.|.j.r.|.j.|.
 00001030: 6404 3c00 7c00 6a04 721b 7c00 6a04 7c01  d.<.|.j.r.|.j.|.
 00001040: 6405 3c00 7c01 5300 2906 4e72 2a00 0000  d.<.|.S.).Nr*...
-00001050: 7245 0000 0029 0572 1e00 0000 720f 0000  rE...).r....r...
-00001060: 005a 0670 6172 744f 6672 4200 0000 7210  .Z.partOfrB...r.
-00001070: 0000 0072 4700 0000 7248 0000 0029 0572  ...rG...rH...).r
-00001080: 0f00 0000 7246 0000 0072 2400 0000 7247  ....rF...r$...rG
-00001090: 0000 0072 4800 0000 7243 0000 0072 0b00  ...rH...rC...r..
+00001050: 7243 0000 0029 0572 1e00 0000 720f 0000  rC...).r....r...
+00001060: 005a 0670 6172 744f 6672 4000 0000 7210  .Z.partOfr@...r.
+00001070: 0000 0072 4500 0000 7246 0000 0029 0572  ...rE...rF...).r
+00001080: 0f00 0000 7244 0000 0072 2400 0000 7245  ....rD...r$...rE
+00001090: 0000 0072 4600 0000 7241 0000 0072 0b00  ...rF...rA...r..
 000010a0: 0000 720b 0000 0072 0c00 0000 7229 0000  ..r....r....r)..
 000010b0: 00b2 0000 0073 1600 0000 0202 0401 0401  .....s..........
 000010c0: 0401 0201 06fb 0608 0a01 0602 0a01 0402  ................
 000010d0: 7a1b 4f72 6465 7265 6443 6f6c 6c65 6374  z.OrderedCollect
 000010e0: 696f 6e50 6167 652e 6275 696c 6429 0a72  ionPage.build).r
-000010f0: 3300 0000 7234 0000 0072 3500 0000 7237  3...r4...r5...r7
-00001100: 0000 0072 3800 0000 723c 0000 0072 4700  ...r8...r<...rG.
-00001110: 0000 7248 0000 0072 3900 0000 7229 0000  ..rH...r9...r)..
+000010f0: 3200 0000 7233 0000 0072 3400 0000 7236  2...r3...r4...r6
+00001100: 0000 0072 3700 0000 723a 0000 0072 4500  ...r7...r:...rE.
+00001110: 0000 7246 0000 0072 3800 0000 7229 0000  ..rF...r8...r)..
 00001120: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00001130: 720c 0000 0072 4500 0000 aa00 0000 730e  r....rE.......s.
+00001130: 720c 0000 0072 4300 0000 aa00 0000 730e  r....rC.......s.
 00001140: 0000 000a 0008 0208 0108 0110 0110 0112  ................
-00001150: 0272 4500 0000 4e29 11da 0b64 6174 6163  .rE...N)...datac
+00001150: 0272 4300 0000 4e29 11da 0b64 6174 6163  .rC...N)...datac
 00001160: 6c61 7373 6573 7202 0000 00da 0674 7970  lassesr......typ
-00001170: 696e 6772 0300 0000 7204 0000 00da 0c62  ingr....r......b
+00001170: 696e 6772 0300 0000 7204 0000 005a 0c62  ingr....r....Z.b
 00001180: 6f76 696e 652e 7479 7065 7372 0500 0000  ovine.typesr....
 00001190: da10 6163 7469 7669 7479 5f66 6163 746f  ..activity_facto
 000011a0: 7279 7207 0000 00da 0e6f 626a 6563 745f  ryr......object_
-000011b0: 6661 6374 6f72 7972 0800 0000 7239 0000  factoryr....r9..
-000011c0: 0072 0d00 0000 720e 0000 0072 3b00 0000  .r....r....r;...
-000011d0: 723d 0000 0072 4500 0000 720b 0000 0072  r=...rE...r....r
+000011b0: 6661 6374 6f72 7972 0800 0000 7238 0000  factoryr....r8..
+000011c0: 0072 0d00 0000 720e 0000 0072 3900 0000  .r....r....r9...
+000011d0: 723b 0000 0072 4300 0000 720b 0000 0072  r;...rC...r....r
 000011e0: 0b00 0000 720b 0000 0072 0c00 0000 da08  ....r....r......
 000011f0: 3c6d 6f64 756c 653e 0100 0000 7324 0000  <module>....s$..
 00001200: 000c 0010 010c 020c 020c 0102 0302 0102  ................
 00001210: ff0a 020a fe02 0710 0102 6e10 0102 0d10  ..........n.....
 00001220: 0102 1b14 01                             .....
```

### Comparing `bovine-0.2.5/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc` & `bovine-0.2.6/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 4203 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,267 +1,281 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 6b10 0000  o.......5bsdk...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 2211 0000  o.........|d"...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6501  d.l.m.Z.m.Z...e.
 00000050: 4700 6403 6404 8400 6404 8302 8301 5a06  G.d.d...d.....Z.
 00000060: 4700 6405 6406 8400 6406 8302 5a07 6407  G.d.d...d...Z.d.
 00000070: 5300 2908 e900 0000 0029 02da 0964 6174  S.)......)...dat
 00000080: 6163 6c61 7373 da05 6669 656c 6429 02da  aclass..field)..
 00000090: 084f 7074 696f 6e61 6cda 0353 6574 6300  .Optional..Setc.
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-000000b0: 0000 0040 0000 0073 f400 0000 6500 5a01  ...@...s....e.Z.
+000000b0: 0000 0040 0000 0073 fc00 0000 6500 5a01  ...@...s....e.Z.
 000000c0: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
 000000d0: 3c00 6403 5a06 6507 6504 1900 6505 6404  <.d.Z.e.e...e.d.
 000000e0: 3c00 6403 5a08 6507 6504 1900 6505 6405  <.d.Z.e.e...e.d.
 000000f0: 3c00 6403 5a09 6507 6504 1900 6505 6406  <.d.Z.e.e...e.d.
 00000100: 3c00 6403 5a0a 6507 6504 1900 6505 6407  <.d.Z.e.e...e.d.
 00000110: 3c00 650b 650c 6408 8d01 5a0d 650e 6504  <.e.e.d...Z.e.e.
 00000120: 1900 6505 6409 3c00 650b 650c 6408 8d01  ..e.d.<.e.e.d...
 00000130: 5a0f 650e 6504 1900 6505 640a 3c00 6403  Z.e.e...e.d.<.d.
 00000140: 5a10 6507 6504 1900 6505 640b 3c00 6403  Z.e.e...e.d.<.d.
 00000150: 5a11 6507 6504 1900 6505 640c 3c00 6403  Z.e.e...e.d.<.d.
 00000160: 5a12 6507 6504 1900 6505 640d 3c00 6403  Z.e.e...e.d.<.d.
 00000170: 5a13 6507 6504 1900 6505 640e 3c00 6403  Z.e.e...e.d.<.d.
 00000180: 5a14 6507 6504 1900 6505 640f 3c00 6410  Z.e.e...e.d.<.d.
 00000190: 6411 8400 5a15 6412 6413 8400 5a16 6414  d...Z.d.d...Z.d.
-000001a0: 6517 6602 6415 6416 8404 5a18 6403 5300  e.f.d.d...Z.d.S.
-000001b0: 2917 da08 4163 7469 7669 7479 7a7e 4120  )...Activityz~A 
-000001c0: 6461 7461 636c 6173 7320 7265 7072 6573  dataclass repres
-000001d0: 656e 7469 6e67 2061 6e20 6041 6374 6976  enting an `Activ
-000001e0: 6974 7953 7472 6561 6d73 2041 6374 6976  ityStreams Activ
-000001f0: 6974 790a 2020 2020 3c68 7474 7073 3a2f  ity.    <https:/
-00000200: 2f77 7777 2e77 332e 6f72 672f 5452 2f61  /www.w3.org/TR/a
-00000210: 6374 6976 6974 7973 7472 6561 6d73 2d76  ctivitystreams-v
-00000220: 6f63 6162 756c 6172 792f 2361 6374 6976  ocabulary/#activ
-00000230: 6974 792d 7479 7065 733e 605f da04 7479  ity-types>`_..ty
-00000240: 7065 4eda 0561 6374 6f72 da09 666f 6c6c  peN..actor..foll
-00000250: 6f77 6572 73da 0269 64da 0970 7562 6c69  owers..id..publi
-00000260: 7368 6564 2901 da0f 6465 6661 756c 745f  shed)...default_
-00000270: 6661 6374 6f72 79da 0274 6fda 0263 63da  factory..to..cc.
-00000280: 046e 616d 65da 0773 756d 6d61 7279 da07  .name..summary..
-00000290: 636f 6e74 656e 74da 0674 6172 6765 74da  content..target.
-000002a0: 066f 626a 6563 7463 0100 0000 0000 0000  .objectc........
-000002b0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-000002c0: 7324 0000 007c 006a 00a0 0164 01a1 0101  s$...|.j...d....
-000002d0: 007c 006a 0272 107c 006a 03a0 017c 006a  .|.j.r.|.j...|.j
-000002e0: 02a1 0101 007c 0053 0029 027a 406d 616b  .....|.S.).z@mak
-000002f0: 6573 2074 6865 2061 6374 6976 6974 7920  es the activity 
-00000300: 7075 626c 6963 2c20 692e 652e 2070 7562  public, i.e. pub
-00000310: 6c69 6320 696e 2074 6f20 616e 6420 666f  lic in to and fo
-00000320: 6c6c 6f77 6572 7320 696e 2063 63fa 2c68  llowers in cc.,h
-00000330: 7474 7073 3a2f 2f77 7777 2e77 332e 6f72  ttps://www.w3.or
-00000340: 672f 6e73 2f61 6374 6976 6974 7973 7472  g/ns/activitystr
-00000350: 6561 6d73 2350 7562 6c69 6329 0472 0d00  eams#Public).r..
-00000360: 0000 da03 6164 6472 0900 0000 720e 0000  ....addr....r...
-00000370: 00a9 01da 0473 656c 66a9 0072 1800 0000  .....self..r....
-00000380: fa5c 2f77 6f6f 6470 6563 6b65 722f 7372  .\/woodpecker/sr
-00000390: 632f 636f 6465 6265 7267 2e6f 7267 2f62  c/codeberg.org/b
-000003a0: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
-000003b0: 696e 652f 626f 7669 6e65 2f61 6374 6976  ine/bovine/activ
-000003c0: 6974 7973 7472 6561 6d73 2f61 6374 6976  itystreams/activ
-000003d0: 6974 795f 6661 6374 6f72 792e 7079 da09  ity_factory.py..
-000003e0: 6173 5f70 7562 6c69 6319 0000 0073 0800  as_public....s..
-000003f0: 0000 0c02 0601 0e01 0401 7a12 4163 7469  ..........z.Acti
-00000400: 7669 7479 2e61 735f 7075 626c 6963 6301  vity.as_publicc.
-00000410: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000420: 0000 0043 0000 0073 2400 0000 7c00 6a00  ...C...s$...|.j.
-00000430: 720a 7c00 6a01 a002 7c00 6a00 a101 0100  r.|.j...|.j.....
-00000440: 7c00 6a03 a002 6401 a101 0100 7c00 5300  |.j...d.....|.S.
-00000450: 2902 7a42 6d61 6b65 7320 7468 6520 6163  ).zBmakes the ac
-00000460: 7469 7669 7479 2075 6e6c 6973 7465 642c  tivity unlisted,
-00000470: 2069 2e65 2e20 7075 626c 6963 2069 6e20   i.e. public in 
-00000480: 6363 2061 6e64 2066 6f6c 6c6f 7765 7273  cc and followers
-00000490: 2069 6e20 746f 7214 0000 0029 0472 0900   in tor....).r..
-000004a0: 0000 720d 0000 0072 1500 0000 720e 0000  ..r....r....r...
-000004b0: 0072 1600 0000 7218 0000 0072 1800 0000  .r....r....r....
-000004c0: 7219 0000 00da 0b61 735f 756e 6c69 7374  r......as_unlist
-000004d0: 6564 2000 0000 7308 0000 0006 020e 010c  ed ...s.........
-000004e0: 0104 017a 1441 6374 6976 6974 792e 6173  ...z.Activity.as
-000004f0: 5f75 6e6c 6973 7465 64da 0672 6574 7572  _unlisted..retur
-00000500: 6e63 0100 0000 0000 0000 0000 0000 0500  nc..............
-00000510: 0000 0800 0000 4300 0000 73ae 0000 0064  ......C...s....d
-00000520: 017c 006a 007c 006a 0174 027c 006a 0383  .|.j.|.j.t.|.j..
-00000530: 0174 027c 006a 047c 006a 0318 0083 0164  .t.|.j.|.j.....d
-00000540: 029c 057d 017c 006a 057c 006a 067c 006a  ...}.|.j.|.j.|.j
-00000550: 077c 006a 087c 006a 097c 006a 0a7c 006a  .|.j.|.j.|.j.|.j
-00000560: 0b64 039c 077d 027c 0164 0419 0064 0575  .d...}.|.d...d.u
-00000570: 0172 3574 0c7c 0164 0419 0083 0164 066b  .r5t.|.d.....d.k
-00000580: 0272 357c 0164 043d 007c 0164 0719 0064  .r5|.d.=.|.d...d
-00000590: 0575 0172 4674 0c7c 0164 0719 0083 0164  .u.rFt.|.d.....d
-000005a0: 066b 0272 467c 0164 073d 007c 02a0 0da1  .k.rF|.d.=.|....
-000005b0: 0044 005d 0a5c 027d 037d 047c 0472 547c  .D.].\.}.}.|.rT|
-000005c0: 047c 017c 033c 0071 4a7c 0153 0029 087a  .|.|.<.qJ|.S.).z
-000005d0: 4163 6f6e 7665 7274 7320 7468 6520 6163  Aconverts the ac
-000005e0: 7469 7669 7479 2069 6e74 6f20 6120 6469  tivity into a di
-000005f0: 6374 2c20 7468 6174 2063 616e 2062 6520  ct, that can be 
-00000600: 7365 7269 616c 697a 6564 2074 6f20 4a53  serialized to JS
-00000610: 4f4e 7a25 6874 7470 733a 2f2f 7777 772e  ONz%https://www.
-00000620: 7733 2e6f 7267 2f6e 732f 6163 7469 7669  w3.org/ns/activi
-00000630: 7479 7374 7265 616d 7329 057a 0840 636f  tystreams).z.@co
-00000640: 6e74 6578 7472 0700 0000 7208 0000 0072  ntextr....r....r
-00000650: 0d00 0000 720e 0000 0029 0772 0a00 0000  ....r....).r....
-00000660: 720b 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00000670: 1100 0000 7212 0000 0072 1300 0000 720d  ....r....r....r.
-00000680: 0000 004e 7201 0000 0072 0e00 0000 290e  ...Nr....r....).
-00000690: 7207 0000 0072 0800 0000 da04 6c69 7374  r....r......list
-000006a0: 720d 0000 0072 0e00 0000 720a 0000 0072  r....r....r....r
-000006b0: 0b00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
-000006c0: 0000 0072 1200 0000 7213 0000 00da 036c  ...r....r......l
-000006d0: 656e da05 6974 656d 7329 0572 1700 0000  en..items).r....
-000006e0: da06 7265 7375 6c74 5a0c 6578 7472 615f  ..resultZ.extra_
-000006f0: 6669 656c 6473 da03 6b65 79da 0576 616c  fields..key..val
-00000700: 7565 7218 0000 0072 1800 0000 7219 0000  uer....r....r...
-00000710: 00da 0562 7569 6c64 2700 0000 732e 0000  ...build'...s...
-00000720: 0002 0304 0104 0108 010e 0106 fb04 0904  ................
-00000730: 0104 0104 0104 0104 0104 0106 f91c 0a06  ................
-00000740: 011c 0106 0110 0204 0108 0102 8004 027a  ...............z
-00000750: 0e41 6374 6976 6974 792e 6275 696c 6429  .Activity.build)
-00000760: 19da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000770: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000780: 616d 655f 5fda 075f 5f64 6f63 5f5f da03  ame__..__doc__..
-00000790: 7374 72da 0f5f 5f61 6e6e 6f74 6174 696f  str..__annotatio
-000007a0: 6e73 5f5f 7208 0000 0072 0400 0000 7209  ns__r....r....r.
-000007b0: 0000 0072 0a00 0000 720b 0000 0072 0300  ...r....r....r..
-000007c0: 0000 da03 7365 7472 0d00 0000 7205 0000  ....setr....r...
-000007d0: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
-000007e0: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000007f0: 1a00 0000 721b 0000 00da 0464 6963 7472  ....r......dictr
-00000800: 2300 0000 7218 0000 0072 1800 0000 7218  #...r....r....r.
-00000810: 0000 0072 1900 0000 7206 0000 0005 0000  ...r....r.......
-00000820: 0073 2200 0000 0a00 0402 0803 1001 1001  .s".............
-00000830: 1001 1001 1601 1601 1002 1001 1001 1002  ................
-00000840: 1001 0802 0807 1207 7206 0000 0063 0000  ........r....c..
-00000850: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00000860: 0000 4000 0000 7358 0000 0065 005a 0164  ..@...sX...e.Z.d
-00000870: 005a 0264 015a 0364 0264 0384 005a 0464  .Z.d.Z.d.d...Z.d
-00000880: 0464 0584 005a 0564 0664 0784 005a 0664  .d...Z.d.d...Z.d
-00000890: 0864 0984 005a 0764 0a64 0b84 005a 0864  .d...Z.d.d...Z.d
-000008a0: 0c64 0d84 005a 0964 0e64 0f84 005a 0a64  .d...Z.d.d...Z.d
-000008b0: 1064 1184 005a 0b64 1264 1384 005a 0c64  .d...Z.d.d...Z.d
-000008c0: 1453 0029 15da 0f41 6374 6976 6974 7946  .S.)...ActivityF
-000008d0: 6163 746f 7279 7a49 4261 7369 6320 6661  actoryzIBasic fa
-000008e0: 6374 6f72 7920 666f 7220 4163 7469 7669  ctory for Activi
-000008f0: 7479 206f 626a 6563 7473 2e0a 0a20 2020  ty objects...   
-00000900: 2055 7361 6c6c 7920 6372 6561 7465 6420   Usally created 
-00000910: 6279 2061 2042 6f76 696e 6543 6c69 656e  by a BovineClien
-00000920: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
-00000930: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00000940: 017c 005f 0064 0053 0029 014e 2901 da0b  .|._.d.S.).N)...
-00000950: 696e 666f 726d 6174 696f 6e29 0272 1700  information).r..
-00000960: 0000 da11 6163 746f 725f 696e 666f 726d  ....actor_inform
-00000970: 6174 696f 6e72 1800 0000 7218 0000 0072  ationr....r....r
-00000980: 1900 0000 da08 5f5f 696e 6974 5f5f 4c00  ......__init__L.
-00000990: 0000 7302 0000 000a 017a 1841 6374 6976  ..s......z.Activ
-000009a0: 6974 7946 6163 746f 7279 2e5f 5f69 6e69  ityFactory.__ini
-000009b0: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
-000009c0: 0300 0000 0a00 0000 4b00 0000 f336 0000  ........K....6..
-000009d0: 0074 0064 0764 017c 0164 0219 0074 017c  .t.d.d.|.d...t.|
-000009e0: 01a0 0264 0367 00a1 0283 0174 017c 01a0  ...d.g.....t.|..
-000009f0: 0264 0467 00a1 0283 017c 0164 059c 057c  .d.g.....|.d...|
-00000a00: 02a4 018e 0153 0029 087a 2341 6374 6976  .....S.).z#Activ
-00000a10: 6974 7920 6f66 2074 7970 6520 4372 6561  ity of type Crea
-00000a20: 7465 2066 726f 6d20 4f62 6a65 6374 5a06  te from ObjectZ.
-00000a30: 4372 6561 7465 da0c 6174 7472 6962 7574  Create..attribut
-00000a40: 6564 546f 720e 0000 0072 0d00 0000 a905  edTor....r......
-00000a50: 7207 0000 0072 0800 0000 720e 0000 0072  r....r....r....r
-00000a60: 0d00 0000 7213 0000 004e 7218 0000 00a9  ....r....Nr.....
-00000a70: 0372 0600 0000 722a 0000 00da 0367 6574  .r....r*.....get
-00000a80: a903 7217 0000 00da 036f 626a da06 6b77  ..r......obj..kw
-00000a90: 6172 6773 7218 0000 0072 1800 0000 7219  argsr....r....r.
-00000aa0: 0000 00da 0663 7265 6174 654f 0000 00f3  .....createO....
-00000ab0: 1200 0000 0402 0201 0601 0e01 0e01 0201  ................
-00000ac0: 04fb 0206 06fa 7a16 4163 7469 7669 7479  ......z.Activity
-00000ad0: 4661 6374 6f72 792e 6372 6561 7465 6302  Factory.createc.
-00000ae0: 0000 0000 0000 0000 0000 0003 0000 000a  ................
-00000af0: 0000 004b 0000 0072 3000 0000 2908 7a23  ...K...r0...).z#
-00000b00: 4163 7469 7669 7479 206f 6620 7479 7065  Activity of type
-00000b10: 2055 7064 6174 6520 6672 6f6d 204f 626a   Update from Obj
-00000b20: 6563 745a 0655 7064 6174 6572 3100 0000  ectZ.Updater1...
-00000b30: 720e 0000 0072 0d00 0000 7232 0000 004e  r....r....r2...N
-00000b40: 7218 0000 0072 3300 0000 7235 0000 0072  r....r3...r5...r
-00000b50: 1800 0000 7218 0000 0072 1900 0000 da06  ....r....r......
-00000b60: 7570 6461 7465 5a00 0000 7239 0000 007a  updateZ...r9...z
-00000b70: 1641 6374 6976 6974 7946 6163 746f 7279  .ActivityFactory
-00000b80: 2e75 7064 6174 6563 0200 0000 0000 0000  .updatec........
-00000b90: 0000 0000 0300 0000 0600 0000 4b00 0000  ............K...
-00000ba0: f31c 0000 0074 0064 0564 017c 006a 0164  .....t.d.d.|.j.d
-00000bb0: 0219 007c 0164 039c 037c 02a4 018e 0153  ...|.d...|.....S
-00000bc0: 0029 067a 0f4c 696b 6520 666f 7220 7461  .).z.Like for ta
-00000bd0: 7267 6574 5a04 4c69 6b65 720a 0000 00a9  rgetZ.Liker.....
-00000be0: 0372 0700 0000 7208 0000 0072 1300 0000  .r....r....r....
-00000bf0: 4e72 1800 0000 a902 7206 0000 0072 2d00  Nr......r....r-.
-00000c00: 0000 a903 7217 0000 0072 1200 0000 7237  ....r....r....r7
-00000c10: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000c20: 0000 da04 6c69 6b65 6500 0000 f30a 0000  ....likee.......
-00000c30: 0004 020c 0104 ff02 0106 ff7a 1441 6374  ...........z.Act
-00000c40: 6976 6974 7946 6163 746f 7279 2e6c 696b  ivityFactory.lik
-00000c50: 6563 0200 0000 0000 0000 0000 0000 0300  ec..............
-00000c60: 0000 0600 0000 4b00 0000 723b 0000 0029  ......K...r;...)
-00000c70: 067a 1144 656c 6574 6520 666f 7220 7461  .z.Delete for ta
-00000c80: 7267 6574 da06 4465 6c65 7465 720a 0000  rget..Deleter...
-00000c90: 0072 3c00 0000 4e72 1800 0000 723d 0000  .r<...Nr....r=..
-00000ca0: 0072 3e00 0000 7218 0000 0072 1800 0000  .r>...r....r....
-00000cb0: 7219 0000 00da 0664 656c 6574 656b 0000  r......deletek..
-00000cc0: 0072 4000 0000 7a16 4163 7469 7669 7479  .r@...z.Activity
-00000cd0: 4661 6374 6f72 792e 6465 6c65 7465 6302  Factory.deletec.
-00000ce0: 0000 0000 0000 0000 0000 0003 0000 0006  ................
-00000cf0: 0000 004b 0000 0072 3b00 0000 2906 7a11  ...K...r;...).z.
-00000d00: 4163 6365 7074 2066 6f72 206f 626a 6563  Accept for objec
-00000d10: 74da 0641 6363 6570 7472 0a00 0000 723c  t..Acceptr....r<
-00000d20: 0000 004e 7218 0000 0072 3d00 0000 7235  ...Nr....r=...r5
-00000d30: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000d40: 0000 da06 6163 6365 7074 7100 0000 7240  ....acceptq...r@
-00000d50: 0000 007a 1641 6374 6976 6974 7946 6163  ...z.ActivityFac
-00000d60: 746f 7279 2e61 6363 6570 7463 0200 0000  tory.acceptc....
-00000d70: 0000 0000 0000 0000 0300 0000 0600 0000  ................
-00000d80: 4b00 0000 723b 0000 0029 067a 1152 656a  K...r;...).z.Rej
-00000d90: 6563 7420 666f 7220 6f62 6a65 6374 5a06  ect for objectZ.
-00000da0: 5265 6a65 6374 720a 0000 0072 3c00 0000  Rejectr....r<...
-00000db0: 4e72 1800 0000 723d 0000 0072 3500 0000  Nr....r=...r5...
-00000dc0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00000dd0: 0672 656a 6563 7477 0000 0072 4000 0000  .rejectw...r@...
-00000de0: 7a16 4163 7469 7669 7479 4661 6374 6f72  z.ActivityFactor
-00000df0: 792e 7265 6a65 6374 6302 0000 0000 0000  y.rejectc.......
-00000e00: 0000 0000 0003 0000 0009 0000 004b 0000  .............K..
-00000e10: 0073 2800 0000 7400 6406 6401 7c00 6a01  .s(...t.d.d.|.j.
-00000e20: 6402 1900 7c01 7c00 6a01 a002 6403 6700  d...|.|.j...d.g.
-00000e30: a102 6404 9c04 7c02 a401 8e01 5300 2907  ..d...|.....S.).
-00000e40: 7a13 416e 6e6f 756e 6365 2066 6f72 206f  z.Announce for o
-00000e50: 626a 6563 745a 0841 6e6e 6f75 6e63 6572  bjectZ.Announcer
-00000e60: 0a00 0000 7209 0000 0029 0472 0700 0000  ....r....).r....
-00000e70: 7208 0000 0072 1300 0000 7209 0000 004e  r....r....r....N
-00000e80: 7218 0000 0029 0372 0600 0000 722d 0000  r....).r....r-..
-00000e90: 0072 3400 0000 7235 0000 0072 1800 0000  .r4...r5...r....
-00000ea0: 7218 0000 0072 1900 0000 da08 616e 6e6f  r....r......anno
-00000eb0: 756e 6365 7d00 0000 7310 0000 0004 0202  unce}...s.......
-00000ec0: 0108 0102 010c 0104 fc02 0506 fb7a 1841  .............z.A
-00000ed0: 6374 6976 6974 7946 6163 746f 7279 2e61  ctivityFactory.a
-00000ee0: 6e6e 6f75 6e63 6563 0200 0000 0000 0000  nnouncec........
-00000ef0: 0000 0000 0300 0000 0700 0000 4b00 0000  ............K...
-00000f00: 7324 0000 0074 0064 0564 017c 006a 0164  s$...t.d.d.|.j.d
-00000f10: 0219 007c 0174 027c 0167 0183 0164 039c  ...|.t.|.g...d..
-00000f20: 047c 02a4 018e 0153 0029 067a 1146 6f6c  .|.....S.).z.Fol
-00000f30: 6c6f 7720 666f 7220 6f62 6a65 6374 5a06  low for objectZ.
-00000f40: 466f 6c6c 6f77 720a 0000 0029 0472 0700  Followr....).r..
-00000f50: 0000 7208 0000 0072 1300 0000 720d 0000  ..r....r....r...
-00000f60: 004e 7218 0000 0029 0372 0600 0000 722d  .Nr....).r....r-
-00000f70: 0000 0072 2a00 0000 7235 0000 0072 1800  ...r*...r5...r..
-00000f80: 0000 7218 0000 0072 1900 0000 da06 666f  ..r....r......fo
-00000f90: 6c6c 6f77 8700 0000 7310 0000 0004 0202  llow....s.......
-00000fa0: 0108 0102 0108 0104 fc02 0506 fb7a 1641  .............z.A
-00000fb0: 6374 6976 6974 7946 6163 746f 7279 2e66  ctivityFactory.f
-00000fc0: 6f6c 6c6f 774e 290d 7224 0000 0072 2500  ollowN).r$...r%.
-00000fd0: 0000 7226 0000 0072 2700 0000 722f 0000  ..r&...r'...r/..
-00000fe0: 0072 3800 0000 723a 0000 0072 3f00 0000  .r8...r:...r?...
-00000ff0: 7242 0000 0072 4400 0000 7245 0000 0072  rB...rD...rE...r
-00001000: 4600 0000 7247 0000 0072 1800 0000 7218  F...rG...r....r.
-00001010: 0000 0072 1800 0000 7219 0000 0072 2c00  ...r....r....r,.
-00001020: 0000 4700 0000 7316 0000 0008 0004 0108  ..G...s.........
-00001030: 0408 0308 0b08 0b08 0608 0608 0608 060c  ................
-00001040: 0a72 2c00 0000 4e29 08da 0b64 6174 6163  .r,...N)...datac
-00001050: 6c61 7373 6573 7202 0000 0072 0300 0000  lassesr....r....
-00001060: da06 7479 7069 6e67 7204 0000 0072 0500  ..typingr....r..
-00001070: 0000 7206 0000 0072 2c00 0000 7218 0000  ..r....r,...r...
-00001080: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00001090: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
-000010a0: 0000 0010 0010 0102 0310 0112 41         ............A
+000001a0: 6415 8400 5a17 6416 6518 6602 6417 6418  d...Z.d.e.f.d.d.
+000001b0: 8404 5a19 6403 5300 2919 da08 4163 7469  ..Z.d.S.)...Acti
+000001c0: 7669 7479 7a7e 4120 6461 7461 636c 6173  vityz~A dataclas
+000001d0: 7320 7265 7072 6573 656e 7469 6e67 2061  s representing a
+000001e0: 6e20 6041 6374 6976 6974 7953 7472 6561  n `ActivityStrea
+000001f0: 6d73 2041 6374 6976 6974 790a 2020 2020  ms Activity.    
+00000200: 3c68 7474 7073 3a2f 2f77 7777 2e77 332e  <https://www.w3.
+00000210: 6f72 672f 5452 2f61 6374 6976 6974 7973  org/TR/activitys
+00000220: 7472 6561 6d73 2d76 6f63 6162 756c 6172  treams-vocabular
+00000230: 792f 2361 6374 6976 6974 792d 7479 7065  y/#activity-type
+00000240: 733e 605f da04 7479 7065 4eda 0561 6374  s>`_..typeN..act
+00000250: 6f72 da09 666f 6c6c 6f77 6572 73da 0269  or..followers..i
+00000260: 64da 0970 7562 6c69 7368 6564 2901 da0f  d..published)...
+00000270: 6465 6661 756c 745f 6661 6374 6f72 79da  default_factory.
+00000280: 0274 6fda 0263 63da 046e 616d 65da 0773  .to..cc..name..s
+00000290: 756d 6d61 7279 da07 636f 6e74 656e 74da  ummary..content.
+000002a0: 0674 6172 6765 74da 066f 626a 6563 7463  .target..objectc
+000002b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000002c0: 0300 0000 4300 0000 7324 0000 007c 006a  ....C...s$...|.j
+000002d0: 00a0 0164 01a1 0101 007c 006a 0272 107c  ...d.....|.j.r.|
+000002e0: 006a 03a0 017c 006a 02a1 0101 007c 0053  .j...|.j.....|.S
+000002f0: 0029 027a 406d 616b 6573 2074 6865 2061  .).z@makes the a
+00000300: 6374 6976 6974 7920 7075 626c 6963 2c20  ctivity public, 
+00000310: 692e 652e 2070 7562 6c69 6320 696e 2074  i.e. public in t
+00000320: 6f20 616e 6420 666f 6c6c 6f77 6572 7320  o and followers 
+00000330: 696e 2063 63fa 2c68 7474 7073 3a2f 2f77  in cc.,https://w
+00000340: 7777 2e77 332e 6f72 672f 6e73 2f61 6374  ww.w3.org/ns/act
+00000350: 6976 6974 7973 7472 6561 6d73 2350 7562  ivitystreams#Pub
+00000360: 6c69 6329 0472 0d00 0000 da03 6164 6472  lic).r......addr
+00000370: 0900 0000 720e 0000 00a9 01da 0473 656c  ....r........sel
+00000380: 66a9 0072 1800 0000 fa5c 2f77 6f6f 6470  f..r.....\/woodp
+00000390: 6563 6b65 722f 7372 632f 636f 6465 6265  ecker/src/codebe
+000003a0: 7267 2e6f 7267 2f62 6f76 696e 652f 626f  rg.org/bovine/bo
+000003b0: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
+000003c0: 6e65 2f61 6374 6976 6974 7973 7472 6561  ne/activitystrea
+000003d0: 6d73 2f61 6374 6976 6974 795f 6661 6374  ms/activity_fact
+000003e0: 6f72 792e 7079 da09 6173 5f70 7562 6c69  ory.py..as_publi
+000003f0: 6319 0000 0073 0800 0000 0c02 0601 0e01  c....s..........
+00000400: 0401 7a12 4163 7469 7669 7479 2e61 735f  ..z.Activity.as_
+00000410: 7075 626c 6963 6301 0000 0000 0000 0000  publicc.........
+00000420: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00000430: 1800 0000 7c00 6a00 720a 7c00 6a01 a002  ....|.j.r.|.j...
+00000440: 7c00 6a00 a101 0100 7c00 5300 2901 7a34  |.j.....|.S.).z4
+00000450: 6164 6472 6573 7365 7320 7468 6520 6163  addresses the ac
+00000460: 7469 7669 7479 2074 6f20 666f 6c6c 6f77  tivity to follow
+00000470: 6572 732c 2069 6620 7468 6579 2061 7265  ers, if they are
+00000480: 2073 6574 2903 7209 0000 0072 0d00 0000   set).r....r....
+00000490: 7215 0000 0072 1600 0000 7218 0000 0072  r....r....r....r
+000004a0: 1800 0000 7219 0000 00da 0c61 735f 666f  ....r......as_fo
+000004b0: 6c6c 6f77 6572 7320 0000 0073 0600 0000  llowers ...s....
+000004c0: 0602 0e01 0401 7a15 4163 7469 7669 7479  ......z.Activity
+000004d0: 2e61 735f 666f 6c6c 6f77 6572 7363 0100  .as_followersc..
+000004e0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000004f0: 0000 4300 0000 7324 0000 007c 006a 0072  ..C...s$...|.j.r
+00000500: 0a7c 006a 01a0 027c 006a 00a1 0101 007c  .|.j...|.j.....|
+00000510: 006a 03a0 0264 01a1 0101 007c 0053 0029  .j...d.....|.S.)
+00000520: 027a 426d 616b 6573 2074 6865 2061 6374  .zBmakes the act
+00000530: 6976 6974 7920 756e 6c69 7374 6564 2c20  ivity unlisted, 
+00000540: 692e 652e 2070 7562 6c69 6320 696e 2063  i.e. public in c
+00000550: 6320 616e 6420 666f 6c6c 6f77 6572 7320  c and followers 
+00000560: 696e 2074 6f72 1400 0000 2904 7209 0000  in tor....).r...
+00000570: 0072 0d00 0000 7215 0000 0072 0e00 0000  .r....r....r....
+00000580: 7216 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
+00000590: 1900 0000 da0b 6173 5f75 6e6c 6973 7465  ......as_unliste
+000005a0: 6426 0000 0073 0800 0000 0602 0e01 0c01  d&...s..........
+000005b0: 0401 7a14 4163 7469 7669 7479 2e61 735f  ..z.Activity.as_
+000005c0: 756e 6c69 7374 6564 da06 7265 7475 726e  unlisted..return
+000005d0: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
+000005e0: 0008 0000 0043 0000 0073 ae00 0000 6401  .....C...s....d.
+000005f0: 7c00 6a00 7c00 6a01 7402 7c00 6a03 8301  |.j.|.j.t.|.j...
+00000600: 7402 7c00 6a04 7c00 6a03 1800 8301 6402  t.|.j.|.j.....d.
+00000610: 9c05 7d01 7c00 6a05 7c00 6a06 7c00 6a07  ..}.|.j.|.j.|.j.
+00000620: 7c00 6a08 7c00 6a09 7c00 6a0a 7c00 6a0b  |.j.|.j.|.j.|.j.
+00000630: 6403 9c07 7d02 7c01 6404 1900 6405 7501  d...}.|.d...d.u.
+00000640: 7235 740c 7c01 6404 1900 8301 6406 6b02  r5t.|.d.....d.k.
+00000650: 7235 7c01 6404 3d00 7c01 6407 1900 6405  r5|.d.=.|.d...d.
+00000660: 7501 7246 740c 7c01 6407 1900 8301 6406  u.rFt.|.d.....d.
+00000670: 6b02 7246 7c01 6407 3d00 7c02 a00d a100  k.rF|.d.=.|.....
+00000680: 4400 5d0a 5c02 7d03 7d04 7c04 7254 7c04  D.].\.}.}.|.rT|.
+00000690: 7c01 7c03 3c00 714a 7c01 5300 2908 7a41  |.|.<.qJ|.S.).zA
+000006a0: 636f 6e76 6572 7473 2074 6865 2061 6374  converts the act
+000006b0: 6976 6974 7920 696e 746f 2061 2064 6963  ivity into a dic
+000006c0: 742c 2074 6861 7420 6361 6e20 6265 2073  t, that can be s
+000006d0: 6572 6961 6c69 7a65 6420 746f 204a 534f  erialized to JSO
+000006e0: 4e7a 2568 7474 7073 3a2f 2f77 7777 2e77  Nz%https://www.w
+000006f0: 332e 6f72 672f 6e73 2f61 6374 6976 6974  3.org/ns/activit
+00000700: 7973 7472 6561 6d73 2905 7a08 4063 6f6e  ystreams).z.@con
+00000710: 7465 7874 7207 0000 0072 0800 0000 720d  textr....r....r.
+00000720: 0000 0072 0e00 0000 2907 720a 0000 0072  ...r....).r....r
+00000730: 0b00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+00000740: 0000 0072 1200 0000 7213 0000 0072 0d00  ...r....r....r..
+00000750: 0000 4e72 0100 0000 720e 0000 0029 0e72  ..Nr....r....).r
+00000760: 0700 0000 7208 0000 00da 046c 6973 7472  ....r......listr
+00000770: 0d00 0000 720e 0000 0072 0a00 0000 720b  ....r....r....r.
+00000780: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
+00000790: 0000 7212 0000 0072 1300 0000 da03 6c65  ..r....r......le
+000007a0: 6eda 0569 7465 6d73 2905 7217 0000 00da  n..items).r.....
+000007b0: 0672 6573 756c 745a 0c65 7874 7261 5f66  .resultZ.extra_f
+000007c0: 6965 6c64 73da 036b 6579 da05 7661 6c75  ields..key..valu
+000007d0: 6572 1800 0000 7218 0000 0072 1900 0000  er....r....r....
+000007e0: da05 6275 696c 642d 0000 0073 2e00 0000  ..build-...s....
+000007f0: 0203 0401 0401 0801 0e01 06fb 0409 0401  ................
+00000800: 0401 0401 0401 0401 0401 06f9 1c0a 0601  ................
+00000810: 1c01 0601 1002 0401 0801 0280 0402 7a0e  ..............z.
+00000820: 4163 7469 7669 7479 2e62 7569 6c64 291a  Activity.build).
+00000830: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000840: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000850: 6d65 5f5f da07 5f5f 646f 635f 5fda 0373  me__..__doc__..s
+00000860: 7472 da0f 5f5f 616e 6e6f 7461 7469 6f6e  tr..__annotation
+00000870: 735f 5f72 0800 0000 7204 0000 0072 0900  s__r....r....r..
+00000880: 0000 720a 0000 0072 0b00 0000 7203 0000  ..r....r....r...
+00000890: 00da 0373 6574 720d 0000 0072 0500 0000  ...setr....r....
+000008a0: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+000008b0: 1100 0000 7212 0000 0072 1300 0000 721a  ....r....r....r.
+000008c0: 0000 0072 1b00 0000 721c 0000 00da 0464  ...r....r......d
+000008d0: 6963 7472 2400 0000 7218 0000 0072 1800  ictr$...r....r..
+000008e0: 0000 7218 0000 0072 1900 0000 7206 0000  ..r....r....r...
+000008f0: 0005 0000 0073 2400 0000 0a00 0402 0803  .....s$.........
+00000900: 1001 1001 1001 1001 1601 1601 1002 1001  ................
+00000910: 1001 1002 1001 0802 0807 0806 1207 7206  ..............r.
+00000920: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000930: 0000 0000 0200 0000 4000 0000 7358 0000  ........@...sX..
+00000940: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
+00000950: 0384 005a 0464 0464 0584 005a 0564 0664  ...Z.d.d...Z.d.d
+00000960: 0784 005a 0664 0864 0984 005a 0764 0a64  ...Z.d.d...Z.d.d
+00000970: 0b84 005a 0864 0c64 0d84 005a 0964 0e64  ...Z.d.d...Z.d.d
+00000980: 0f84 005a 0a64 1064 1184 005a 0b64 1264  ...Z.d.d...Z.d.d
+00000990: 1384 005a 0c64 1453 0029 15da 0f41 6374  ...Z.d.S.)...Act
+000009a0: 6976 6974 7946 6163 746f 7279 7a49 4261  ivityFactoryzIBa
+000009b0: 7369 6320 6661 6374 6f72 7920 666f 7220  sic factory for 
+000009c0: 4163 7469 7669 7479 206f 626a 6563 7473  Activity objects
+000009d0: 2e0a 0a20 2020 2055 7361 6c6c 7920 6372  ...    Usally cr
+000009e0: 6561 7465 6420 6279 2061 2042 6f76 696e  eated by a Bovin
+000009f0: 6543 6c69 656e 7463 0200 0000 0000 0000  eClientc........
+00000a00: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00000a10: 730a 0000 007c 017c 005f 0064 0053 0029  s....|.|._.d.S.)
+00000a20: 014e 2901 da0b 696e 666f 726d 6174 696f  .N)...informatio
+00000a30: 6e29 0272 1700 0000 da11 6163 746f 725f  n).r......actor_
+00000a40: 696e 666f 726d 6174 696f 6e72 1800 0000  informationr....
+00000a50: 7218 0000 0072 1900 0000 da08 5f5f 696e  r....r......__in
+00000a60: 6974 5f5f 5200 0000 7302 0000 000a 017a  it__R...s......z
+00000a70: 1841 6374 6976 6974 7946 6163 746f 7279  .ActivityFactory
+00000a80: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
+00000a90: 0000 0000 0000 0300 0000 0a00 0000 4b00  ..............K.
+00000aa0: 0000 f336 0000 0074 0064 0764 017c 0164  ...6...t.d.d.|.d
+00000ab0: 0219 0074 017c 01a0 0264 0367 00a1 0283  ...t.|...d.g....
+00000ac0: 0174 017c 01a0 0264 0467 00a1 0283 017c  .t.|...d.g.....|
+00000ad0: 0164 059c 057c 02a4 018e 0153 0029 087a  .d...|.....S.).z
+00000ae0: 2341 6374 6976 6974 7920 6f66 2074 7970  #Activity of typ
+00000af0: 6520 4372 6561 7465 2066 726f 6d20 4f62  e Create from Ob
+00000b00: 6a65 6374 5a06 4372 6561 7465 da0c 6174  jectZ.Create..at
+00000b10: 7472 6962 7574 6564 546f 720e 0000 0072  tributedTor....r
+00000b20: 0d00 0000 a905 7207 0000 0072 0800 0000  ......r....r....
+00000b30: 720e 0000 0072 0d00 0000 7213 0000 004e  r....r....r....N
+00000b40: 7218 0000 00a9 0372 0600 0000 722b 0000  r......r....r+..
+00000b50: 00da 0367 6574 a903 7217 0000 00da 036f  ...get..r......o
+00000b60: 626a da06 6b77 6172 6773 7218 0000 0072  bj..kwargsr....r
+00000b70: 1800 0000 7219 0000 00da 0663 7265 6174  ....r......creat
+00000b80: 6555 0000 00f3 1200 0000 0402 0201 0601  eU..............
+00000b90: 0e01 0e01 0201 04fb 0206 06fa 7a16 4163  ............z.Ac
+00000ba0: 7469 7669 7479 4661 6374 6f72 792e 6372  tivityFactory.cr
+00000bb0: 6561 7465 6302 0000 0000 0000 0000 0000  eatec...........
+00000bc0: 0003 0000 000a 0000 004b 0000 0072 3100  .........K...r1.
+00000bd0: 0000 2908 7a23 4163 7469 7669 7479 206f  ..).z#Activity o
+00000be0: 6620 7479 7065 2055 7064 6174 6520 6672  f type Update fr
+00000bf0: 6f6d 204f 626a 6563 745a 0655 7064 6174  om ObjectZ.Updat
+00000c00: 6572 3200 0000 720e 0000 0072 0d00 0000  er2...r....r....
+00000c10: 7233 0000 004e 7218 0000 0072 3400 0000  r3...Nr....r4...
+00000c20: 7236 0000 0072 1800 0000 7218 0000 0072  r6...r....r....r
+00000c30: 1900 0000 da06 7570 6461 7465 6000 0000  ......update`...
+00000c40: 723a 0000 007a 1641 6374 6976 6974 7946  r:...z.ActivityF
+00000c50: 6163 746f 7279 2e75 7064 6174 6563 0200  actory.updatec..
+00000c60: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+00000c70: 0000 4b00 0000 f31c 0000 0074 0064 0564  ..K........t.d.d
+00000c80: 017c 006a 0164 0219 007c 0164 039c 037c  .|.j.d...|.d...|
+00000c90: 02a4 018e 0153 0029 067a 0f4c 696b 6520  .....S.).z.Like 
+00000ca0: 666f 7220 7461 7267 6574 5a04 4c69 6b65  for targetZ.Like
+00000cb0: 720a 0000 00a9 0372 0700 0000 7208 0000  r......r....r...
+00000cc0: 0072 1300 0000 4e72 1800 0000 a902 7206  .r....Nr......r.
+00000cd0: 0000 0072 2e00 0000 a903 7217 0000 0072  ...r......r....r
+00000ce0: 1200 0000 7238 0000 0072 1800 0000 7218  ....r8...r....r.
+00000cf0: 0000 0072 1900 0000 da04 6c69 6b65 6b00  ...r......likek.
+00000d00: 0000 f30a 0000 0004 020c 0104 ff02 0106  ................
+00000d10: ff7a 1441 6374 6976 6974 7946 6163 746f  .z.ActivityFacto
+00000d20: 7279 2e6c 696b 6563 0200 0000 0000 0000  ry.likec........
+00000d30: 0000 0000 0300 0000 0600 0000 4b00 0000  ............K...
+00000d40: 723c 0000 0029 067a 1144 656c 6574 6520  r<...).z.Delete 
+00000d50: 666f 7220 7461 7267 6574 da06 4465 6c65  for target..Dele
+00000d60: 7465 720a 0000 0072 3d00 0000 4e72 1800  ter....r=...Nr..
+00000d70: 0000 723e 0000 0072 3f00 0000 7218 0000  ..r>...r?...r...
+00000d80: 0072 1800 0000 7219 0000 00da 0664 656c  .r....r......del
+00000d90: 6574 6571 0000 0072 4100 0000 7a16 4163  eteq...rA...z.Ac
+00000da0: 7469 7669 7479 4661 6374 6f72 792e 6465  tivityFactory.de
+00000db0: 6c65 7465 6302 0000 0000 0000 0000 0000  letec...........
+00000dc0: 0003 0000 0006 0000 004b 0000 0072 3c00  .........K...r<.
+00000dd0: 0000 2906 7a11 4163 6365 7074 2066 6f72  ..).z.Accept for
+00000de0: 206f 626a 6563 745a 0641 6363 6570 7472   objectZ.Acceptr
+00000df0: 0a00 0000 723d 0000 004e 7218 0000 0072  ....r=...Nr....r
+00000e00: 3e00 0000 7236 0000 0072 1800 0000 7218  >...r6...r....r.
+00000e10: 0000 0072 1900 0000 da06 6163 6365 7074  ...r......accept
+00000e20: 7700 0000 7241 0000 007a 1641 6374 6976  w...rA...z.Activ
+00000e30: 6974 7946 6163 746f 7279 2e61 6363 6570  ityFactory.accep
+00000e40: 7463 0200 0000 0000 0000 0000 0000 0300  tc..............
+00000e50: 0000 0600 0000 4b00 0000 723c 0000 0029  ......K...r<...)
+00000e60: 067a 1152 656a 6563 7420 666f 7220 6f62  .z.Reject for ob
+00000e70: 6a65 6374 5a06 5265 6a65 6374 720a 0000  jectZ.Rejectr...
+00000e80: 0072 3d00 0000 4e72 1800 0000 723e 0000  .r=...Nr....r>..
+00000e90: 0072 3600 0000 7218 0000 0072 1800 0000  .r6...r....r....
+00000ea0: 7219 0000 00da 0672 656a 6563 747d 0000  r......reject}..
+00000eb0: 0072 4100 0000 7a16 4163 7469 7669 7479  .rA...z.Activity
+00000ec0: 4661 6374 6f72 792e 7265 6a65 6374 6302  Factory.rejectc.
+00000ed0: 0000 0000 0000 0000 0000 0003 0000 0009  ................
+00000ee0: 0000 004b 0000 0073 2800 0000 7400 6406  ...K...s(...t.d.
+00000ef0: 6401 7c00 6a01 6402 1900 7c01 7c00 6a01  d.|.j.d...|.|.j.
+00000f00: a002 6403 6700 a102 6404 9c04 7c02 a401  ..d.g...d...|...
+00000f10: 8e01 5300 2907 7a13 416e 6e6f 756e 6365  ..S.).z.Announce
+00000f20: 2066 6f72 206f 626a 6563 745a 0841 6e6e   for objectZ.Ann
+00000f30: 6f75 6e63 6572 0a00 0000 7209 0000 0029  ouncer....r....)
+00000f40: 0472 0700 0000 7208 0000 0072 1300 0000  .r....r....r....
+00000f50: 7209 0000 004e 7218 0000 0029 0372 0600  r....Nr....).r..
+00000f60: 0000 722e 0000 0072 3500 0000 7236 0000  ..r....r5...r6..
+00000f70: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000f80: da08 616e 6e6f 756e 6365 8300 0000 7310  ..announce....s.
+00000f90: 0000 0004 0202 0108 0102 010c 0104 fc02  ................
+00000fa0: 0506 fb7a 1841 6374 6976 6974 7946 6163  ...z.ActivityFac
+00000fb0: 746f 7279 2e61 6e6e 6f75 6e63 6563 0200  tory.announcec..
+00000fc0: 0000 0000 0000 0000 0000 0300 0000 0700  ................
+00000fd0: 0000 4b00 0000 7324 0000 0074 0064 0564  ..K...s$...t.d.d
+00000fe0: 017c 006a 0164 0219 007c 0174 027c 0167  .|.j.d...|.t.|.g
+00000ff0: 0183 0164 039c 047c 02a4 018e 0153 0029  ...d...|.....S.)
+00001000: 067a 1146 6f6c 6c6f 7720 666f 7220 6f62  .z.Follow for ob
+00001010: 6a65 6374 5a06 466f 6c6c 6f77 720a 0000  jectZ.Followr...
+00001020: 0029 0472 0700 0000 7208 0000 0072 1300  .).r....r....r..
+00001030: 0000 720d 0000 004e 7218 0000 0029 0372  ..r....Nr....).r
+00001040: 0600 0000 722e 0000 0072 2b00 0000 7236  ....r....r+...r6
+00001050: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00001060: 0000 da06 666f 6c6c 6f77 8d00 0000 7310  ....follow....s.
+00001070: 0000 0004 0202 0108 0102 0108 0104 fc02  ................
+00001080: 0506 fb7a 1641 6374 6976 6974 7946 6163  ...z.ActivityFac
+00001090: 746f 7279 2e66 6f6c 6c6f 774e 290d 7225  tory.followN).r%
+000010a0: 0000 0072 2600 0000 7227 0000 0072 2800  ...r&...r'...r(.
+000010b0: 0000 7230 0000 0072 3900 0000 723b 0000  ..r0...r9...r;..
+000010c0: 0072 4000 0000 7243 0000 0072 4400 0000  .r@...rC...rD...
+000010d0: 7245 0000 0072 4600 0000 7247 0000 0072  rE...rF...rG...r
+000010e0: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
+000010f0: 0000 0072 2d00 0000 4d00 0000 7316 0000  ...r-...M...s...
+00001100: 0008 0004 0108 0408 0308 0b08 0b08 0608  ................
+00001110: 0608 0608 060c 0a72 2d00 0000 4e29 08da  .......r-...N)..
+00001120: 0b64 6174 6163 6c61 7373 6573 7202 0000  .dataclassesr...
+00001130: 0072 0300 0000 da06 7479 7069 6e67 7204  .r......typingr.
+00001140: 0000 0072 0500 0000 7206 0000 0072 2d00  ...r....r....r-.
+00001150: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
+00001160: 0072 1900 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001170: 0100 0000 730a 0000 0010 0010 0102 0310  ....s...........
+00001180: 0112 47                                  ..G
```

### Comparing `bovine-0.2.5/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc` & `bovine-0.2.6/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 4178 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 5210 0000  o.......5bsdR...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 a311 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
 00000050: 0100 6403 6404 6c07 6d08 5a08 0100 6501  ..d.d.l.m.Z...e.
 00000060: 4700 6405 6406 8400 6406 8302 8301 5a09  G.d.d...d.....Z.
 00000070: 4700 6407 6408 8400 6408 8302 5a0a 6409  G.d.d...d...Z.d.
 00000080: 5300 290a e900 0000 0029 02da 0964 6174  S.)......)...dat
 00000090: 6163 6c61 7373 da05 6669 656c 6429 03da  aclass..field)..
 000000a0: 044c 6973 74da 084f 7074 696f 6e61 6cda  .List..Optional.
 000000b0: 0353 6574 e901 0000 0029 01da 1b66 6564  .Set.....)...fed
 000000c0: 6976 6572 7365 5f68 616e 646c 655f 6672  iverse_handle_fr
 000000d0: 6f6d 5f61 6374 6f72 6300 0000 0000 0000  om_actorc.......
 000000e0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-000000f0: 0073 5a01 0000 6500 5a01 6400 5a02 5500  .sZ...e.Z.d.Z.U.
+000000f0: 0073 6201 0000 6500 5a01 6400 5a02 5500  .sb...e.Z.d.Z.U.
 00000100: 6401 5a03 6504 6505 6402 3c00 6403 5a06  d.Z.e.e.d.<.d.Z.
 00000110: 6507 6504 1900 6505 6404 3c00 6403 5a08  e.e...e.d.<.d.Z.
 00000120: 6507 6504 1900 6505 6405 3c00 6403 5a09  e.e...e.d.<.d.Z.
 00000130: 6507 6504 1900 6505 6406 3c00 6403 5a0a  e.e...e.d.<.d.Z.
 00000140: 6507 6504 1900 6505 6407 3c00 650b 650c  e.e...e.d.<.e.e.
 00000150: 6408 8d01 5a0d 650e 6504 1900 6505 6409  d...Z.e.e...e.d.
 00000160: 3c00 650b 650c 6408 8d01 5a0f 650e 6504  <.e.e.d...Z.e.e.
@@ -30,223 +30,245 @@
 000001d0: 1900 6505 6410 3c00 6403 5a18 6507 6504  ..e.d.<.d.Z.e.e.
 000001e0: 1900 6505 6411 3c00 6403 5a19 6507 6504  ..e.d.<.d.Z.e.e.
 000001f0: 1900 6505 6412 3c00 650b 651a 6408 8d01  ..e.d.<.e.e.d...
 00000200: 5a1b 651c 6514 1900 6505 6413 3c00 650b  Z.e.e...e.d.<.e.
 00000210: 651a 6408 8d01 5a1d 651c 6514 1900 6505  e.d...Z.e.e...e.
 00000220: 6414 3c00 6403 5a1e 6507 6504 1900 6505  d.<.d.Z.e.e...e.
 00000230: 6415 3c00 6416 6417 8400 5a1f 6418 6419  d.<.d.d...Z.d.d.
-00000240: 8400 5a20 641a 641b 8400 5a21 6403 5300  ..Z d.d...Z!d.S.
-00000250: 291c da06 4f62 6a65 6374 7a7a 4120 6461  )...ObjectzzA da
-00000260: 7461 636c 6173 7320 7265 7072 6573 656e  taclass represen
-00000270: 7469 6e67 2061 6e20 6041 6374 6976 6974  ting an `Activit
-00000280: 7953 7472 6561 6d73 204f 626a 6563 740a  yStreams Object.
-00000290: 2020 2020 3c68 7474 7073 3a2f 2f77 7777      <https://www
-000002a0: 2e77 332e 6f72 672f 5452 2f61 6374 6976  .w3.org/TR/activ
-000002b0: 6974 7973 7472 6561 6d73 2d76 6f63 6162  itystreams-vocab
-000002c0: 756c 6172 792f 236f 626a 6563 742d 7479  ulary/#object-ty
-000002d0: 7065 733e 605f da04 7479 7065 4eda 0d61  pes>`_..typeN..a
-000002e0: 7474 7269 6275 7465 645f 746f da09 666f  ttributed_to..fo
-000002f0: 6c6c 6f77 6572 73da 0269 64da 0970 7562  llowers..id..pub
-00000300: 6c69 7368 6564 2901 da0f 6465 6661 756c  lished)...defaul
-00000310: 745f 6661 6374 6f72 79da 0274 6fda 0263  t_factory..to..c
-00000320: 63da 046e 616d 65da 0773 756d 6d61 7279  c..name..summary
-00000330: da07 636f 6e74 656e 74da 0673 6f75 7263  ..content..sourc
-00000340: 65da 0577 6964 7468 da06 6865 6967 6874  e..width..height
-00000350: da0b 696e 5f72 6570 6c79 5f74 6fda 0375  ..in_reply_to..u
-00000360: 726c da03 7461 67da 0a61 7474 6163 686d  rl..tag..attachm
-00000370: 656e 74da 0468 7265 6663 0100 0000 0000  ent..hrefc......
-00000380: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00000390: 0000 7324 0000 007c 006a 00a0 0164 01a1  ..s$...|.j...d..
-000003a0: 0101 007c 006a 0272 107c 006a 03a0 017c  ...|.j.r.|.j...|
-000003b0: 006a 02a1 0101 007c 0053 00a9 024e 7a2c  .j.....|.S...Nz,
-000003c0: 6874 7470 733a 2f2f 7777 772e 7733 2e6f  https://www.w3.o
-000003d0: 7267 2f6e 732f 6163 7469 7669 7479 7374  rg/ns/activityst
-000003e0: 7265 616d 7323 5075 626c 6963 2904 7210  reams#Public).r.
-000003f0: 0000 00da 0361 6464 720c 0000 0072 1100  .....addr....r..
-00000400: 0000 a901 da04 7365 6c66 a900 7221 0000  ......self..r!..
-00000410: 00fa 5a2f 776f 6f64 7065 636b 6572 2f73  ..Z/woodpecker/s
-00000420: 7263 2f63 6f64 6562 6572 672e 6f72 672f  rc/codeberg.org/
-00000430: 626f 7669 6e65 2f62 6f76 696e 652f 626f  bovine/bovine/bo
-00000440: 7669 6e65 2f62 6f76 696e 652f 6163 7469  vine/bovine/acti
-00000450: 7669 7479 7374 7265 616d 732f 6f62 6a65  vitystreams/obje
-00000460: 6374 5f66 6163 746f 7279 2e70 79da 0961  ct_factory.py..a
-00000470: 735f 7075 626c 6963 2200 0000 7308 0000  s_public"...s...
-00000480: 000c 0106 010e 0104 017a 104f 626a 6563  .........z.Objec
-00000490: 742e 6173 5f70 7562 6c69 6363 0100 0000  t.as_publicc....
-000004a0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000004b0: 4300 0000 7324 0000 007c 006a 0072 0a7c  C...s$...|.j.r.|
-000004c0: 006a 01a0 027c 006a 00a1 0101 007c 006a  .j...|.j.....|.j
-000004d0: 03a0 0264 01a1 0101 007c 0053 0072 1d00  ...d.....|.S.r..
-000004e0: 0000 2904 720c 0000 0072 1000 0000 721e  ..).r....r....r.
-000004f0: 0000 0072 1100 0000 721f 0000 0072 2100  ...r....r....r!.
-00000500: 0000 7221 0000 0072 2200 0000 da0b 6173  ..r!...r".....as
-00000510: 5f75 6e6c 6973 7465 6428 0000 0073 0800  _unlisted(...s..
-00000520: 0000 0601 0e01 0c01 0401 7a12 4f62 6a65  ..........z.Obje
-00000530: 6374 2e61 735f 756e 6c69 7374 6564 6301  ct.as_unlistedc.
-00000540: 0000 0000 0000 0000 0000 0005 0000 0005  ................
-00000550: 0000 0043 0000 0073 fc00 0000 6401 7c00  ...C...s....d.|.
-00000560: 6a00 6402 9c02 7d01 6900 6403 7c00 6a01  j.d...}.i.d.|.j.
-00000570: 9301 6404 7402 7c00 6a03 8301 9301 6405  ..d.t.|.j.....d.
-00000580: 7402 7c00 6a04 7c00 6a03 1800 8301 9301  t.|.j.|.j.......
-00000590: 6406 7c00 6a05 9301 6407 7c00 6a06 9301  d.|.j...d.|.j...
-000005a0: 6408 7c00 6a07 9301 6409 7c00 6a08 9301  d.|.j...d.|.j...
-000005b0: 640a 7c00 6a09 9301 640b 7c00 6a0a 9301  d.|.j...d.|.j...
-000005c0: 640c 7c00 6a0b 9301 640d 7c00 6a0c 9301  d.|.j...d.|.j...
-000005d0: 640e 7c00 6a0d 9301 640f 7c00 6a0e 9301  d.|.j...d.|.j...
-000005e0: 6410 7c00 6a0f 9301 6411 7c00 6a10 9301  d.|.j...d.|.j...
-000005f0: 6412 7c00 6a11 9301 7d02 7c02 a012 a100  d.|.j...}.|.....
-00000600: 4400 5d0a 5c02 7d03 7d04 7c04 725d 7c04  D.].\.}.}.|.r]|.
-00000610: 7c01 7c03 3c00 7153 6404 7c01 7600 726d  |.|.<.qSd.|.v.rm
-00000620: 7413 7c01 6404 1900 8301 6413 6b02 726d  t.|.d.....d.k.rm
-00000630: 7c01 6404 3d00 6405 7c01 7600 727c 7413  |.d.=.d.|.v.r|t.
-00000640: 7c01 6405 1900 8301 6413 6b02 727c 7c01  |.d.....d.k.r||.
-00000650: 6405 3d00 7c01 5300 2914 4e7a 2568 7474  d.=.|.S.).Nz%htt
-00000660: 7073 3a2f 2f77 7777 2e77 332e 6f72 672f  ps://www.w3.org/
-00000670: 6e73 2f61 6374 6976 6974 7973 7472 6561  ns/activitystrea
-00000680: 6d73 2902 7a08 4063 6f6e 7465 7874 720a  ms).z.@contextr.
-00000690: 0000 00da 0c61 7474 7269 6275 7465 6454  .....attributedT
-000006a0: 6f72 1000 0000 7211 0000 0072 0d00 0000  or....r....r....
-000006b0: 5a09 696e 5265 706c 7954 6f72 0e00 0000  Z.inReplyTor....
-000006c0: 7215 0000 0072 1200 0000 7219 0000 0072  r....r....r....r
-000006d0: 1300 0000 7214 0000 0072 1a00 0000 721b  ....r....r....r.
-000006e0: 0000 0072 1c00 0000 7216 0000 0072 1700  ...r....r....r..
-000006f0: 0000 7201 0000 0029 1472 0a00 0000 720b  ..r....).r....r.
-00000700: 0000 00da 046c 6973 7472 1000 0000 7211  .....listr....r.
-00000710: 0000 0072 0d00 0000 7218 0000 0072 0e00  ...r....r....r..
-00000720: 0000 7215 0000 0072 1200 0000 7219 0000  ..r....r....r...
-00000730: 0072 1300 0000 7214 0000 0072 1a00 0000  .r....r....r....
-00000740: 721b 0000 0072 1c00 0000 7216 0000 0072  r....r....r....r
-00000750: 1700 0000 da05 6974 656d 73da 036c 656e  ......items..len
-00000760: 2905 7220 0000 00da 0672 6573 756c 74da  ).r .....result.
-00000770: 0c65 7874 7261 5f66 6965 6c64 73da 036b  .extra_fields..k
-00000780: 6579 da05 7661 6c75 6572 2100 0000 7221  ey..valuer!...r!
-00000790: 0000 0072 2200 0000 da05 6275 696c 642e  ...r".....build.
-000007a0: 0000 0073 5a00 0000 0202 0401 06fe 0205  ...sZ...........
-000007b0: 0601 02ff 0a02 02fe 1003 02fd 0604 02fc  ................
-000007c0: 0605 02fb 0606 02fa 0607 02f9 0608 02f8  ................
-000007d0: 0609 02f7 060a 02f6 060b 02f5 060c 02f4  ................
-000007e0: 060d 02f3 060e 02f2 060f 02f1 0610 04f0  ................
-000007f0: 1013 0401 0801 0280 1802 0601 1801 0601  ................
-00000800: 0402 7a0c 4f62 6a65 6374 2e62 7569 6c64  ..z.Object.build
-00000810: 2922 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )"..__name__..__
-00000820: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000830: 6e61 6d65 5f5f da07 5f5f 646f 635f 5fda  name__..__doc__.
-00000840: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
-00000850: 6f6e 735f 5f72 0b00 0000 7205 0000 0072  ons__r....r....r
-00000860: 0c00 0000 720d 0000 0072 0e00 0000 7203  ....r....r....r.
-00000870: 0000 00da 0373 6574 7210 0000 0072 0600  .....setr....r..
-00000880: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00000890: 0072 1400 0000 7215 0000 00da 0464 6963  .r....r......dic
-000008a0: 7472 1600 0000 da03 696e 7472 1700 0000  tr......intr....
-000008b0: 7218 0000 0072 1900 0000 7226 0000 0072  r....r....r&...r
-000008c0: 1a00 0000 7204 0000 0072 1b00 0000 721c  ....r....r....r.
-000008d0: 0000 0072 2300 0000 7224 0000 0072 2d00  ...r#...r$...r-.
-000008e0: 0000 7221 0000 0072 2100 0000 7221 0000  ..r!...r!...r!..
-000008f0: 0072 2200 0000 7209 0000 0007 0000 0073  .r"...r........s
-00000900: 2e00 0000 0a00 0402 0803 1001 1001 1001  ................
-00000910: 1001 1601 1601 1002 1001 1001 1001 1002  ................
-00000920: 1001 1002 1001 1601 1601 1001 0802 0806  ................
-00000930: 0c06 7209 0000 0063 0000 0000 0000 0000  ..r....c........
-00000940: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000950: 733a 0000 0065 005a 0164 005a 0264 015a  s:...e.Z.d.Z.d.Z
-00000960: 0364 0d64 0364 0484 015a 0464 0564 0684  .d.d.d...Z.d.d..
-00000970: 005a 0564 0764 0884 005a 0664 0964 0a84  .Z.d.d...Z.d.d..
-00000980: 005a 0764 0b64 0c84 005a 0864 0253 0029  .Z.d.d...Z.d.S.)
-00000990: 0eda 0d4f 626a 6563 7446 6163 746f 7279  ...ObjectFactory
-000009a0: 7a34 4f62 6a65 6374 4661 6374 6f72 7920  z4ObjectFactory 
-000009b0: 7573 7561 6c6c 7920 6372 6561 7465 6420  usually created 
-000009c0: 7468 726f 7567 6820 6120 426f 7669 6e65  through a Bovine
-000009d0: 436c 6965 6e74 4e63 0300 0000 0000 0000  ClientNc........
-000009e0: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
-000009f0: 7332 0000 007c 0272 0b7c 027c 005f 007c  s2...|.r.|.|._.|
-00000a00: 026a 017c 005f 0164 0053 007c 0172 1564  .j.|._.d.S.|.r.d
-00000a10: 007c 005f 007c 017c 005f 0164 0053 0074  .|._.|.|._.d.S.t
-00000a20: 0264 0183 0182 0129 024e 7a3e 596f 7520  .d.....).Nz>You 
-00000a30: 6e65 6564 2074 6f20 6569 7468 6572 2073  need to either s
-00000a40: 7065 6369 6679 2061 6374 6f72 5f69 6e66  pecify actor_inf
-00000a50: 6f72 6d61 7469 6f6e 206f 7220 6120 426f  ormation or a Bo
-00000a60: 7669 6e65 436c 6965 6e74 2903 da06 636c  vineClient)...cl
-00000a70: 6965 6e74 da0b 696e 666f 726d 6174 696f  ient..informatio
-00000a80: 6eda 0954 7970 6545 7272 6f72 2903 7220  n..TypeError).r 
-00000a90: 0000 00da 1161 6374 6f72 5f69 6e66 6f72  .....actor_infor
-00000aa0: 6d61 7469 6f6e 7238 0000 0072 2100 0000  mationr8...r!...
-00000ab0: 7221 0000 0072 2200 0000 da08 5f5f 696e  r!...r".....__in
-00000ac0: 6974 5f5f 5600 0000 7312 0000 0004 0106  it__V...s.......
-00000ad0: 010c 0104 0106 010a 0102 0202 0104 ff7a  ...............z
-00000ae0: 164f 626a 6563 7446 6163 746f 7279 2e5f  .ObjectFactory._
-00000af0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00000b00: 0000 0000 0200 0000 0700 0000 4b00 0000  ............K...
-00000b10: f324 0000 0074 0064 067c 006a 0164 0119  .$...t.d.|.j.d..
-00000b20: 0064 027c 006a 01a0 0264 03a1 0164 049c  .d.|.j...d...d..
-00000b30: 037c 01a4 018e 0153 0029 077a 1543 7265  .|.....S.).z.Cre
-00000b40: 6174 6573 2061 204e 6f74 6520 4f62 6a65  ates a Note Obje
-00000b50: 6374 720d 0000 005a 044e 6f74 6572 0c00  ctr....Z.Noter..
-00000b60: 0000 a903 720b 0000 0072 0a00 0000 720c  ....r....r....r.
-00000b70: 0000 004e 7221 0000 00a9 0372 0900 0000  ...Nr!.....r....
-00000b80: 7239 0000 00da 0367 6574 a902 7220 0000  r9.....get..r ..
-00000b90: 00da 066b 7761 7267 7372 2100 0000 7221  ...kwargsr!...r!
-00000ba0: 0000 0072 2200 0000 da04 6e6f 7465 6200  ...r".....noteb.
-00000bb0: 0000 f30e 0000 0004 0208 0102 010a 0104  ................
-00000bc0: fd02 0406 fc7a 124f 626a 6563 7446 6163  .....z.ObjectFac
-00000bd0: 746f 7279 2e6e 6f74 6563 0100 0000 0000  tory.notec......
-00000be0: 0000 0000 0000 0200 0000 0700 0000 4b00  ..............K.
-00000bf0: 0000 723d 0000 0029 077a 1943 7265 6174  ..r=...).z.Creat
-00000c00: 6573 2061 6e20 4172 7469 636c 6520 4f62  es an Article Ob
-00000c10: 6a65 6374 720d 0000 005a 0741 7274 6963  jectr....Z.Artic
-00000c20: 6c65 720c 0000 0072 3e00 0000 4e72 2100  ler....r>...Nr!.
-00000c30: 0000 723f 0000 0072 4100 0000 7221 0000  ..r?...rA...r!..
-00000c40: 0072 2100 0000 7222 0000 00da 0761 7274  .r!...r".....art
-00000c50: 6963 6c65 6b00 0000 7244 0000 007a 154f  iclek...rD...z.O
-00000c60: 626a 6563 7446 6163 746f 7279 2e61 7274  bjectFactory.art
-00000c70: 6963 6c65 6301 0000 0000 0000 0000 0000  iclec...........
-00000c80: 0002 0000 0007 0000 004b 0000 0072 3d00  .........K...r=.
-00000c90: 0000 2907 7a17 4372 6561 7465 7320 616e  ..).z.Creates an
-00000ca0: 2045 7665 6e74 204f 626a 6563 7472 0d00   Event Objectr..
-00000cb0: 0000 da05 4576 656e 7472 0c00 0000 723e  ....Eventr....r>
-00000cc0: 0000 004e 7221 0000 0072 3f00 0000 7241  ...Nr!...r?...rA
-00000cd0: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00000ce0: 0000 da05 6576 656e 7474 0000 0072 4400  ....eventt...rD.
-00000cf0: 0000 7a13 4f62 6a65 6374 4661 6374 6f72  ..z.ObjectFactor
-00000d00: 792e 6576 656e 7463 0200 0000 0000 0000  y.eventc........
-00000d10: 0000 0000 0300 0000 0500 0000 c300 0000  ................
-00000d20: 7334 0000 0081 017c 006a 0073 0874 0164  s4.....|.j.s.t.d
-00000d30: 0183 0182 017c 006a 00a0 027c 01a1 0149  .....|.j...|...I
-00000d40: 0064 0248 007d 0274 0364 037c 0174 047c  .d.H.}.t.d.|.t.|
-00000d50: 0283 0164 048d 0353 0029 057a 8843 7265  ...d...S.).z.Cre
-00000d60: 6174 6573 2061 206d 656e 7469 6f6e 206f  ates a mention o
-00000d70: 626a 6563 7420 666f 7220 616e 6f74 6865  bject for anothe
-00000d80: 7220 6163 746f 722e 2052 6571 7569 7265  r actor. Require
-00000d90: 7320 636c 6965 6e74 2074 6f20 6265 2073  s client to be s
-00000da0: 6574 2e0a 0a20 2020 2020 2020 203a 7061  et...        :pa
-00000db0: 7261 6d20 6163 746f 725f 746f 5f6d 656e  ram actor_to_men
-00000dc0: 7469 6f6e 3a20 5468 6520 5552 4920 6f66  tion: The URI of
-00000dd0: 2074 6865 2061 6374 6f72 2074 6f20 6d65   the actor to me
-00000de0: 6e74 696f 6e7a 2663 6c69 656e 7420 6e65  ntionz&client ne
-00000df0: 6564 7320 746f 2062 6520 7365 7420 6174  eds to be set at
-00000e00: 2063 6f6e 7374 7275 6374 696f 6e4e 5a07   constructionNZ.
-00000e10: 4d65 6e74 696f 6e29 0372 0a00 0000 721c  Mention).r....r.
-00000e20: 0000 0072 1200 0000 2905 7238 0000 0072  ...r....).r8...r
-00000e30: 3a00 0000 da0d 7072 6f78 795f 656c 656d  :.....proxy_elem
-00000e40: 656e 7472 0900 0000 7208 0000 0029 0372  entr....r....).r
-00000e50: 2000 0000 5a10 6163 746f 725f 746f 5f6d   ...Z.actor_to_m
-00000e60: 656e 7469 6f6e 5a0c 7265 6d6f 7465 5f61  entionZ.remote_a
-00000e70: 6374 6f72 7221 0000 0072 2100 0000 7222  ctorr!...r!...r"
-00000e80: 0000 00da 156d 656e 7469 6f6e 5f66 6f72  .....mention_for
-00000e90: 5f61 6374 6f72 5f75 7269 7d00 0000 7312  _actor_uri}...s.
-00000ea0: 0000 0002 8006 0508 0112 0202 0202 0102  ................
-00000eb0: 0106 0106 fd7a 234f 626a 6563 7446 6163  .....z#ObjectFac
-00000ec0: 746f 7279 2e6d 656e 7469 6f6e 5f66 6f72  tory.mention_for
-00000ed0: 5f61 6374 6f72 5f75 7269 2902 4e4e 2909  _actor_uri).NN).
-00000ee0: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
-00000ef0: 3100 0000 723c 0000 0072 4300 0000 7245  1...r<...rC...rE
-00000f00: 0000 0072 4700 0000 7249 0000 0072 2100  ...rG...rI...r!.
-00000f10: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-00000f20: 0072 3700 0000 5300 0000 730e 0000 0008  .r7...S...s.....
-00000f30: 0004 010a 0208 0c08 0908 090c 0972 3700  .............r7.
-00000f40: 0000 4e29 0bda 0b64 6174 6163 6c61 7373  ..N)...dataclass
-00000f50: 6573 7202 0000 0072 0300 0000 da06 7479  esr....r......ty
-00000f60: 7069 6e67 7204 0000 0072 0500 0000 7206  pingr....r....r.
-00000f70: 0000 00da 0575 7469 6c73 7208 0000 0072  .....utilsr....r
-00000f80: 0900 0000 7237 0000 0072 2100 0000 7221  ....r7...r!...r!
-00000f90: 0000 0072 2100 0000 7222 0000 00da 083c  ...r!...r".....<
-00000fa0: 6d6f 6475 6c65 3e01 0000 0073 0c00 0000  module>....s....
-00000fb0: 1000 1401 0c02 0203 1001 124b            ...........K
+00000240: 8400 5a20 641a 641b 8400 5a21 641c 641d  ..Z d.d...Z!d.d.
+00000250: 8400 5a22 6403 5300 291e da06 4f62 6a65  ..Z"d.S.)...Obje
+00000260: 6374 7a7a 4120 6461 7461 636c 6173 7320  ctzzA dataclass 
+00000270: 7265 7072 6573 656e 7469 6e67 2061 6e20  representing an 
+00000280: 6041 6374 6976 6974 7953 7472 6561 6d73  `ActivityStreams
+00000290: 204f 626a 6563 740a 2020 2020 3c68 7474   Object.    <htt
+000002a0: 7073 3a2f 2f77 7777 2e77 332e 6f72 672f  ps://www.w3.org/
+000002b0: 5452 2f61 6374 6976 6974 7973 7472 6561  TR/activitystrea
+000002c0: 6d73 2d76 6f63 6162 756c 6172 792f 236f  ms-vocabulary/#o
+000002d0: 626a 6563 742d 7479 7065 733e 605f da04  bject-types>`_..
+000002e0: 7479 7065 4eda 0d61 7474 7269 6275 7465  typeN..attribute
+000002f0: 645f 746f da09 666f 6c6c 6f77 6572 73da  d_to..followers.
+00000300: 0269 64da 0970 7562 6c69 7368 6564 2901  .id..published).
+00000310: da0f 6465 6661 756c 745f 6661 6374 6f72  ..default_factor
+00000320: 79da 0274 6fda 0263 63da 046e 616d 65da  y..to..cc..name.
+00000330: 0773 756d 6d61 7279 da07 636f 6e74 656e  .summary..conten
+00000340: 74da 0673 6f75 7263 65da 0577 6964 7468  t..source..width
+00000350: da06 6865 6967 6874 da0b 696e 5f72 6570  ..height..in_rep
+00000360: 6c79 5f74 6fda 0375 726c da03 7461 67da  ly_to..url..tag.
+00000370: 0a61 7474 6163 686d 656e 74da 0468 7265  .attachment..hre
+00000380: 6663 0100 0000 0000 0000 0000 0000 0100  fc..............
+00000390: 0000 0300 0000 4300 0000 7324 0000 007c  ......C...s$...|
+000003a0: 006a 00a0 0164 01a1 0101 007c 006a 0272  .j...d.....|.j.r
+000003b0: 107c 006a 03a0 017c 006a 02a1 0101 007c  .|.j...|.j.....|
+000003c0: 0053 0029 027a 3e6d 616b 6573 2074 6865  .S.).z>makes the
+000003d0: 206f 626a 6563 7420 7075 626c 6963 2c20   object public, 
+000003e0: 692e 652e 2070 7562 6c69 6320 696e 2074  i.e. public in t
+000003f0: 6f20 616e 6420 666f 6c6c 6f77 6572 7320  o and followers 
+00000400: 696e 2063 63fa 2c68 7474 7073 3a2f 2f77  in cc.,https://w
+00000410: 7777 2e77 332e 6f72 672f 6e73 2f61 6374  ww.w3.org/ns/act
+00000420: 6976 6974 7973 7472 6561 6d73 2350 7562  ivitystreams#Pub
+00000430: 6c69 6329 0472 1000 0000 da03 6164 6472  lic).r......addr
+00000440: 0c00 0000 7211 0000 00a9 01da 0473 656c  ....r........sel
+00000450: 66a9 0072 2100 0000 fa5a 2f77 6f6f 6470  f..r!....Z/woodp
+00000460: 6563 6b65 722f 7372 632f 636f 6465 6265  ecker/src/codebe
+00000470: 7267 2e6f 7267 2f62 6f76 696e 652f 626f  rg.org/bovine/bo
+00000480: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
+00000490: 6e65 2f61 6374 6976 6974 7973 7472 6561  ne/activitystrea
+000004a0: 6d73 2f6f 626a 6563 745f 6661 6374 6f72  ms/object_factor
+000004b0: 792e 7079 da09 6173 5f70 7562 6c69 6322  y.py..as_public"
+000004c0: 0000 0073 0800 0000 0c02 0601 0e01 0401  ...s............
+000004d0: 7a10 4f62 6a65 6374 2e61 735f 7075 626c  z.Object.as_publ
+000004e0: 6963 6301 0000 0000 0000 0000 0000 0001  icc.............
+000004f0: 0000 0003 0000 0043 0000 0073 1800 0000  .......C...s....
+00000500: 7c00 6a00 720a 7c00 6a01 a002 7c00 6a00  |.j.r.|.j...|.j.
+00000510: a101 0100 7c00 5300 2901 7a32 6164 6472  ....|.S.).z2addr
+00000520: 6573 7365 7320 7468 6520 6f62 6a65 6374  esses the object
+00000530: 2074 6f20 666f 6c6c 6f77 6572 732c 2069   to followers, i
+00000540: 6620 7468 6579 2061 7265 2073 6574 2903  f they are set).
+00000550: 720c 0000 0072 1000 0000 721e 0000 0072  r....r....r....r
+00000560: 1f00 0000 7221 0000 0072 2100 0000 7222  ....r!...r!...r"
+00000570: 0000 00da 0c61 735f 666f 6c6c 6f77 6572  .....as_follower
+00000580: 7329 0000 0073 0600 0000 0602 0e01 0401  s)...s..........
+00000590: 7a13 4f62 6a65 6374 2e61 735f 666f 6c6c  z.Object.as_foll
+000005a0: 6f77 6572 7363 0100 0000 0000 0000 0000  owersc..........
+000005b0: 0000 0100 0000 0300 0000 4300 0000 7324  ..........C...s$
+000005c0: 0000 007c 006a 0072 0a7c 006a 01a0 027c  ...|.j.r.|.j...|
+000005d0: 006a 00a1 0101 007c 006a 03a0 0264 01a1  .j.....|.j...d..
+000005e0: 0101 007c 0053 0029 027a 406d 616b 6573  ...|.S.).z@makes
+000005f0: 2074 6865 206f 626a 6563 7420 756e 6c69   the object unli
+00000600: 7374 6564 2c20 692e 652e 2070 7562 6c69  sted, i.e. publi
+00000610: 6320 696e 2063 6320 616e 6420 666f 6c6c  c in cc and foll
+00000620: 6f77 6572 7320 696e 2074 6f72 1d00 0000  owers in tor....
+00000630: 2904 720c 0000 0072 1000 0000 721e 0000  ).r....r....r...
+00000640: 0072 1100 0000 721f 0000 0072 2100 0000  .r....r....r!...
+00000650: 7221 0000 0072 2200 0000 da0b 6173 5f75  r!...r".....as_u
+00000660: 6e6c 6973 7465 642f 0000 0073 0800 0000  nlisted/...s....
+00000670: 0602 0e01 0c01 0401 7a12 4f62 6a65 6374  ........z.Object
+00000680: 2e61 735f 756e 6c69 7374 6564 6301 0000  .as_unlistedc...
+00000690: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+000006a0: 0043 0000 0073 fc00 0000 6401 7c00 6a00  .C...s....d.|.j.
+000006b0: 6402 9c02 7d01 6900 6403 7c00 6a01 9301  d...}.i.d.|.j...
+000006c0: 6404 7402 7c00 6a03 8301 9301 6405 7402  d.t.|.j.....d.t.
+000006d0: 7c00 6a04 7c00 6a03 1800 8301 9301 6406  |.j.|.j.......d.
+000006e0: 7c00 6a05 9301 6407 7c00 6a06 9301 6408  |.j...d.|.j...d.
+000006f0: 7c00 6a07 9301 6409 7c00 6a08 9301 640a  |.j...d.|.j...d.
+00000700: 7c00 6a09 9301 640b 7c00 6a0a 9301 640c  |.j...d.|.j...d.
+00000710: 7c00 6a0b 9301 640d 7c00 6a0c 9301 640e  |.j...d.|.j...d.
+00000720: 7c00 6a0d 9301 640f 7c00 6a0e 9301 6410  |.j...d.|.j...d.
+00000730: 7c00 6a0f 9301 6411 7c00 6a10 9301 6412  |.j...d.|.j...d.
+00000740: 7c00 6a11 9301 7d02 7c02 a012 a100 4400  |.j...}.|.....D.
+00000750: 5d0a 5c02 7d03 7d04 7c04 725d 7c04 7c01  ].\.}.}.|.r]|.|.
+00000760: 7c03 3c00 7153 6404 7c01 7600 726d 7413  |.<.qSd.|.v.rmt.
+00000770: 7c01 6404 1900 8301 6413 6b02 726d 7c01  |.d.....d.k.rm|.
+00000780: 6404 3d00 6405 7c01 7600 727c 7413 7c01  d.=.d.|.v.r|t.|.
+00000790: 6405 1900 8301 6413 6b02 727c 7c01 6405  d.....d.k.r||.d.
+000007a0: 3d00 7c01 5300 2914 4e7a 2568 7474 7073  =.|.S.).Nz%https
+000007b0: 3a2f 2f77 7777 2e77 332e 6f72 672f 6e73  ://www.w3.org/ns
+000007c0: 2f61 6374 6976 6974 7973 7472 6561 6d73  /activitystreams
+000007d0: 2902 7a08 4063 6f6e 7465 7874 720a 0000  ).z.@contextr...
+000007e0: 00da 0c61 7474 7269 6275 7465 6454 6f72  ...attributedTor
+000007f0: 1000 0000 7211 0000 0072 0d00 0000 5a09  ....r....r....Z.
+00000800: 696e 5265 706c 7954 6f72 0e00 0000 7215  inReplyTor....r.
+00000810: 0000 0072 1200 0000 7219 0000 0072 1300  ...r....r....r..
+00000820: 0000 7214 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000830: 0072 1c00 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000840: 7201 0000 0029 1472 0a00 0000 720b 0000  r....).r....r...
+00000850: 00da 046c 6973 7472 1000 0000 7211 0000  ...listr....r...
+00000860: 0072 0d00 0000 7218 0000 0072 0e00 0000  .r....r....r....
+00000870: 7215 0000 0072 1200 0000 7219 0000 0072  r....r....r....r
+00000880: 1300 0000 7214 0000 0072 1a00 0000 721b  ....r....r....r.
+00000890: 0000 0072 1c00 0000 7216 0000 0072 1700  ...r....r....r..
+000008a0: 0000 da05 6974 656d 73da 036c 656e 2905  ....items..len).
+000008b0: 7220 0000 00da 0672 6573 756c 74da 0c65  r .....result..e
+000008c0: 7874 7261 5f66 6965 6c64 73da 036b 6579  xtra_fields..key
+000008d0: da05 7661 6c75 6572 2100 0000 7221 0000  ..valuer!...r!..
+000008e0: 0072 2200 0000 da05 6275 696c 6436 0000  .r".....build6..
+000008f0: 0073 5a00 0000 0202 0401 06fe 0205 0601  .sZ.............
+00000900: 02ff 0a02 02fe 1003 02fd 0604 02fc 0605  ................
+00000910: 02fb 0606 02fa 0607 02f9 0608 02f8 0609  ................
+00000920: 02f7 060a 02f6 060b 02f5 060c 02f4 060d  ................
+00000930: 02f3 060e 02f2 060f 02f1 0610 04f0 1013  ................
+00000940: 0401 0801 0280 1802 0601 1801 0601 0402  ................
+00000950: 7a0c 4f62 6a65 6374 2e62 7569 6c64 2923  z.Object.build)#
+00000960: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000970: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000980: 6d65 5f5f da07 5f5f 646f 635f 5fda 0373  me__..__doc__..s
+00000990: 7472 da0f 5f5f 616e 6e6f 7461 7469 6f6e  tr..__annotation
+000009a0: 735f 5f72 0b00 0000 7205 0000 0072 0c00  s__r....r....r..
+000009b0: 0000 720d 0000 0072 0e00 0000 7203 0000  ..r....r....r...
+000009c0: 00da 0373 6574 7210 0000 0072 0600 0000  ...setr....r....
+000009d0: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+000009e0: 1400 0000 7215 0000 00da 0464 6963 7472  ....r......dictr
+000009f0: 1600 0000 da03 696e 7472 1700 0000 7218  ......intr....r.
+00000a00: 0000 0072 1900 0000 7227 0000 0072 1a00  ...r....r'...r..
+00000a10: 0000 7204 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00000a20: 0072 2300 0000 7224 0000 0072 2500 0000  .r#...r$...r%...
+00000a30: 722e 0000 0072 2100 0000 7221 0000 0072  r....r!...r!...r
+00000a40: 2100 0000 7222 0000 0072 0900 0000 0700  !...r"...r......
+00000a50: 0000 7330 0000 000a 0004 0208 0310 0110  ..s0............
+00000a60: 0110 0110 0116 0116 0110 0210 0110 0110  ................
+00000a70: 0110 0210 0110 0210 0116 0116 0110 0108  ................
+00000a80: 0208 0708 060c 0772 0900 0000 6300 0000  .......r....c...
+00000a90: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000aa0: 0040 0000 0073 3a00 0000 6500 5a01 6400  .@...s:...e.Z.d.
+00000ab0: 5a02 6401 5a03 640d 6403 6404 8401 5a04  Z.d.Z.d.d.d...Z.
+00000ac0: 6405 6406 8400 5a05 6407 6408 8400 5a06  d.d...Z.d.d...Z.
+00000ad0: 6409 640a 8400 5a07 640b 640c 8400 5a08  d.d...Z.d.d...Z.
+00000ae0: 6402 5300 290e da0d 4f62 6a65 6374 4661  d.S.)...ObjectFa
+00000af0: 6374 6f72 797a 344f 626a 6563 7446 6163  ctoryz4ObjectFac
+00000b00: 746f 7279 2075 7375 616c 6c79 2063 7265  tory usually cre
+00000b10: 6174 6564 2074 6872 6f75 6768 2061 2042  ated through a B
+00000b20: 6f76 696e 6543 6c69 656e 744e 6303 0000  ovineClientNc...
+00000b30: 0000 0000 0000 0000 0003 0000 0002 0000  ................
+00000b40: 0043 0000 0073 3200 0000 7c02 720b 7c02  .C...s2...|.r.|.
+00000b50: 7c00 5f00 7c02 6a01 7c00 5f01 6400 5300  |._.|.j.|._.d.S.
+00000b60: 7c01 7215 6400 7c00 5f00 7c01 7c00 5f01  |.r.d.|._.|.|._.
+00000b70: 6400 5300 7402 6401 8301 8201 2902 4e7a  d.S.t.d.....).Nz
+00000b80: 3e59 6f75 206e 6565 6420 746f 2065 6974  >You need to eit
+00000b90: 6865 7220 7370 6563 6966 7920 6163 746f  her specify acto
+00000ba0: 725f 696e 666f 726d 6174 696f 6e20 6f72  r_information or
+00000bb0: 2061 2042 6f76 696e 6543 6c69 656e 7429   a BovineClient)
+00000bc0: 03da 0663 6c69 656e 74da 0b69 6e66 6f72  ...client..infor
+00000bd0: 6d61 7469 6f6e da09 5479 7065 4572 726f  mation..TypeErro
+00000be0: 7229 0372 2000 0000 da11 6163 746f 725f  r).r .....actor_
+00000bf0: 696e 666f 726d 6174 696f 6e72 3900 0000  informationr9...
+00000c00: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
+00000c10: 085f 5f69 6e69 745f 5f5e 0000 0073 1200  .__init__^...s..
+00000c20: 0000 0401 0601 0c01 0401 0601 0a01 0202  ................
+00000c30: 0201 04ff 7a16 4f62 6a65 6374 4661 6374  ....z.ObjectFact
+00000c40: 6f72 792e 5f5f 696e 6974 5f5f 6301 0000  ory.__init__c...
+00000c50: 0000 0000 0000 0000 0002 0000 0007 0000  ................
+00000c60: 004b 0000 00f3 2400 0000 7400 6406 7c00  .K....$...t.d.|.
+00000c70: 6a01 6401 1900 6402 7c00 6a01 a002 6403  j.d...d.|.j...d.
+00000c80: a101 6404 9c03 7c01 a401 8e01 5300 2907  ..d...|.....S.).
+00000c90: 7a15 4372 6561 7465 7320 6120 4e6f 7465  z.Creates a Note
+00000ca0: 204f 626a 6563 7472 0d00 0000 5a04 4e6f   Objectr....Z.No
+00000cb0: 7465 720c 0000 00a9 0372 0b00 0000 720a  ter......r....r.
+00000cc0: 0000 0072 0c00 0000 4e72 2100 0000 a903  ...r....Nr!.....
+00000cd0: 7209 0000 0072 3a00 0000 da03 6765 74a9  r....r:.....get.
+00000ce0: 0272 2000 0000 da06 6b77 6172 6773 7221  .r .....kwargsr!
+00000cf0: 0000 0072 2100 0000 7222 0000 00da 046e  ...r!...r".....n
+00000d00: 6f74 656a 0000 00f3 0e00 0000 0402 0801  otej............
+00000d10: 0201 0a01 04fd 0204 06fc 7a12 4f62 6a65  ..........z.Obje
+00000d20: 6374 4661 6374 6f72 792e 6e6f 7465 6301  ctFactory.notec.
+00000d30: 0000 0000 0000 0000 0000 0002 0000 0007  ................
+00000d40: 0000 004b 0000 0072 3e00 0000 2907 7a19  ...K...r>...).z.
+00000d50: 4372 6561 7465 7320 616e 2041 7274 6963  Creates an Artic
+00000d60: 6c65 204f 626a 6563 7472 0d00 0000 5a07  le Objectr....Z.
+00000d70: 4172 7469 636c 6572 0c00 0000 723f 0000  Articler....r?..
+00000d80: 004e 7221 0000 0072 4000 0000 7242 0000  .Nr!...r@...rB..
+00000d90: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+00000da0: da07 6172 7469 636c 6573 0000 0072 4500  ..articles...rE.
+00000db0: 0000 7a15 4f62 6a65 6374 4661 6374 6f72  ..z.ObjectFactor
+00000dc0: 792e 6172 7469 636c 6563 0100 0000 0000  y.articlec......
+00000dd0: 0000 0000 0000 0200 0000 0700 0000 4b00  ..............K.
+00000de0: 0000 723e 0000 0029 077a 1743 7265 6174  ..r>...).z.Creat
+00000df0: 6573 2061 6e20 4576 656e 7420 4f62 6a65  es an Event Obje
+00000e00: 6374 720d 0000 00da 0545 7665 6e74 720c  ctr......Eventr.
+00000e10: 0000 0072 3f00 0000 4e72 2100 0000 7240  ...r?...Nr!...r@
+00000e20: 0000 0072 4200 0000 7221 0000 0072 2100  ...rB...r!...r!.
+00000e30: 0000 7222 0000 00da 0565 7665 6e74 7c00  ..r".....event|.
+00000e40: 0000 7245 0000 007a 134f 626a 6563 7446  ..rE...z.ObjectF
+00000e50: 6163 746f 7279 2e65 7665 6e74 6302 0000  actory.eventc...
+00000e60: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+00000e70: 00c3 0000 0073 3400 0000 8101 7c00 6a00  .....s4.....|.j.
+00000e80: 7308 7401 6401 8301 8201 7c00 6a00 a002  s.t.d.....|.j...
+00000e90: 7c01 a101 4900 6402 4800 7d02 7403 6403  |...I.d.H.}.t.d.
+00000ea0: 7c01 7404 7c02 8301 6404 8d03 5300 2905  |.t.|...d...S.).
+00000eb0: 7a88 4372 6561 7465 7320 6120 6d65 6e74  z.Creates a ment
+00000ec0: 696f 6e20 6f62 6a65 6374 2066 6f72 2061  ion object for a
+00000ed0: 6e6f 7468 6572 2061 6374 6f72 2e20 5265  nother actor. Re
+00000ee0: 7175 6972 6573 2063 6c69 656e 7420 746f  quires client to
+00000ef0: 2062 6520 7365 742e 0a0a 2020 2020 2020   be set...      
+00000f00: 2020 3a70 6172 616d 2061 6374 6f72 5f74    :param actor_t
+00000f10: 6f5f 6d65 6e74 696f 6e3a 2054 6865 2055  o_mention: The U
+00000f20: 5249 206f 6620 7468 6520 6163 746f 7220  RI of the actor 
+00000f30: 746f 206d 656e 7469 6f6e 7a26 636c 6965  to mentionz&clie
+00000f40: 6e74 206e 6565 6473 2074 6f20 6265 2073  nt needs to be s
+00000f50: 6574 2061 7420 636f 6e73 7472 7563 7469  et at constructi
+00000f60: 6f6e 4e5a 074d 656e 7469 6f6e 2903 720a  onNZ.Mention).r.
+00000f70: 0000 0072 1c00 0000 7212 0000 0029 0572  ...r....r....).r
+00000f80: 3900 0000 723b 0000 00da 0d70 726f 7879  9...r;.....proxy
+00000f90: 5f65 6c65 6d65 6e74 7209 0000 0072 0800  _elementr....r..
+00000fa0: 0000 2903 7220 0000 005a 1061 6374 6f72  ..).r ...Z.actor
+00000fb0: 5f74 6f5f 6d65 6e74 696f 6e5a 0c72 656d  _to_mentionZ.rem
+00000fc0: 6f74 655f 6163 746f 7272 2100 0000 7221  ote_actorr!...r!
+00000fd0: 0000 0072 2200 0000 da15 6d65 6e74 696f  ...r".....mentio
+00000fe0: 6e5f 666f 725f 6163 746f 725f 7572 6985  n_for_actor_uri.
+00000ff0: 0000 0073 1200 0000 0280 0605 0801 1202  ...s............
+00001000: 0202 0201 0201 0601 06fd 7a23 4f62 6a65  ..........z#Obje
+00001010: 6374 4661 6374 6f72 792e 6d65 6e74 696f  ctFactory.mentio
+00001020: 6e5f 666f 725f 6163 746f 725f 7572 6929  n_for_actor_uri)
+00001030: 024e 4e29 0972 2f00 0000 7230 0000 0072  .NN).r/...r0...r
+00001040: 3100 0000 7232 0000 0072 3d00 0000 7244  1...r2...r=...rD
+00001050: 0000 0072 4600 0000 7248 0000 0072 4a00  ...rF...rH...rJ.
+00001060: 0000 7221 0000 0072 2100 0000 7221 0000  ..r!...r!...r!..
+00001070: 0072 2200 0000 7238 0000 005b 0000 0073  .r"...r8...[...s
+00001080: 0e00 0000 0800 0401 0a02 080c 0809 0809  ................
+00001090: 0c09 7238 0000 004e 290b da0b 6461 7461  ..r8...N)...data
+000010a0: 636c 6173 7365 7372 0200 0000 7203 0000  classesr....r...
+000010b0: 00da 0674 7970 696e 6772 0400 0000 7205  ...typingr....r.
+000010c0: 0000 0072 0600 0000 da05 7574 696c 7372  ...r......utilsr
+000010d0: 0800 0000 7209 0000 0072 3800 0000 7221  ....r....r8...r!
+000010e0: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+000010f0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001100: 730c 0000 0010 0014 010c 0202 0310 0112  s...............
+00001110: 53                                       S
```

### Comparing `bovine-0.2.5/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 2195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 9308 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 9308 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6402 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6410 6406 6407 8404 5a0a 6410 6408 6409  d.d.d...Z.d.d.d.
 00000070: 8404 5a0b 640a 640b 8400 5a0c 6410 640c  ..Z.d.d...Z.d.d.
@@ -242,16 +242,16 @@
 00000f10: a00a 7c02 a101 7405 a00a 7c03 a101 7405  ..|...t...|...t.
 00000f20: a00a 7c04 a101 7405 a00a 7c05 a101 640a  ..|...t...|...d.
 00000f30: 9c06 1600 7d07 640b 640c 7c07 6901 1600  ....}.d.d.|.i...
 00000f40: 7d08 740b 7405 a00c 7c08 a101 8301 8201  }.t.t...|.......
 00000f50: 6400 0400 7d02 0400 7d03 0400 7d04 0400  d...}...}...}...
 00000f60: 7d06 7d05 6400 5300 290d 4e72 0600 0000  }.}.d.S.).Nr....
 00000f70: 7207 0000 0072 0800 0000 720a 0000 003e  r....r....r....>
-00000f80: 0400 0000 720c 0000 0072 3000 0000 7218  ....r....r0...r.
-00000f90: 0000 0072 2f00 0000 720e 0000 0029 017a  ...r/...r....).z
+00000f80: 0400 0000 7218 0000 0072 2f00 0000 7230  ....r....r/...r0
+00000f90: 0000 0072 0c00 0000 720e 0000 0029 017a  ...r....r....).z
 00000fa0: 6225 2870 7937 2973 0a7b 2528 7079 3729  b%(py7)s.{%(py7)
 00000fb0: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
 00000fc0: 3529 730a 7b25 2870 7935 2973 203d 2025  5)s.{%(py5)s = %
 00000fd0: 2870 7933 2973 0a7b 2528 7079 3329 7320  (py3)s.{%(py3)s 
 00000fe0: 3d20 2528 7079 3129 732e 6b65 7973 0a7d  = %(py1)s.keys.}
 00000ff0: 2829 0a7d 290a 7d20 3d3d 2025 2870 7931  ().}).} == %(py1
 00001000: 3029 73da 0373 6574 7224 0000 0029 06da  0)s..setr$...)..
```

### Comparing `bovine-0.2.5/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 1442 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 a205 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 a205 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 640c 6406 6407 8404 5a0a 640c 6408 6409  d.d.d...Z.d.d.d.
 00000070: 8404 5a0b 640c 640a 640b 8404 5a0c 6401  ..Z.d.d.d...Z.d.
@@ -61,35 +61,35 @@
 000003c0: 6601 6413 7c09 7c0a 6602 a104 7404 a009  f.d.|.|.f...t...
 000003d0: 7c09 a101 7404 a009 7c0a a101 6414 9c02  |...t...|...d...
 000003e0: 1600 7d0b 6415 6416 7c0b 6901 1600 7d0c  ..}.d.d.|.i...}.
 000003f0: 740a 7404 a00b 7c0c a101 8301 8201 6400  t.t...|.......d.
 00000400: 0400 7d09 0400 7d02 7d0a 6400 5300 2917  ..}...}.}.d.S.).
 00000410: 4efa 1c68 7474 703a 2f2f 6578 616d 706c  N..http://exampl
 00000420: 652e 636f 6d2f 6163 746f 722f 3132 3329  e.com/actor/123)
-00000430: 01da 0269 643e 0500 0000 fa08 4063 6f6e  ...id>......@con
-00000440: 7465 7874 da05 696e 626f 78da 066f 7574  text..inbox..out
-00000450: 626f 7872 0700 0000 da04 7479 7065 a901  boxr......type..
+00000430: 01da 0269 643e 0500 0000 7207 0000 00da  ...id>....r.....
+00000440: 0569 6e62 6f78 da04 7479 7065 da06 6f75  .inbox..type..ou
+00000450: 7462 6f78 fa08 4063 6f6e 7465 7874 a901  tbox..@context..
 00000460: fa02 3d3d 2901 7a62 2528 7079 3729 730a  ..==).zb%(py7)s.
 00000470: 7b25 2870 7937 2973 203d 2025 2870 7930  {%(py7)s = %(py0
 00000480: 2973 2825 2870 7935 2973 0a7b 2528 7079  )s(%(py5)s.{%(py
 00000490: 3529 7320 3d20 2528 7079 3329 730a 7b25  5)s = %(py3)s.{%
 000004a0: 2870 7933 2973 203d 2025 2870 7931 2973  (py3)s = %(py1)s
 000004b0: 2e6b 6579 730a 7d28 290a 7d29 0a7d 203d  .keys.}().}).} =
 000004c0: 3d20 2528 7079 3130 2973 da03 7365 74da  = %(py10)s..set.
 000004d0: 0672 6573 756c 7429 06da 0370 7930 da03  .result)...py0..
 000004e0: 7079 31da 0370 7933 da03 7079 35da 0370  py1..py3..py5..p
 000004f0: 7937 da04 7079 3130 7a0f 6173 7365 7274  y7..py10z.assert
 00000500: 2025 2870 7931 3229 73da 0470 7931 327a   %(py12)s..py12z
-00000510: 084a 6f68 6e20 446f 653e 0600 0000 7208  .John Doe>....r.
-00000520: 0000 0072 0900 0000 720a 0000 0072 0700  ...r....r....r..
+00000510: 084a 6f68 6e20 446f 653e 0600 0000 7207  .John Doe>....r.
+00000520: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
 00000530: 0000 da04 6e61 6d65 720b 0000 005a 1130  ....namer....Z.0
 00000540: 3132 3334 3536 3738 3930 3132 3334 3536  1234567890123456
-00000550: da03 6b65 793e 0700 0000 7208 0000 0072  ..key>....r....r
-00000560: 0900 0000 720a 0000 0072 0700 0000 7217  ....r....r....r.
-00000570: 0000 00da 0970 7562 6c69 634b 6579 720b  .....publicKeyr.
+00000550: da03 6b65 793e 0700 0000 7207 0000 0072  ..key>....r....r
+00000560: 0800 0000 7209 0000 0072 0a00 0000 da09  ....r....r......
+00000570: 7075 626c 6963 4b65 7972 1700 0000 720b  publicKeyr....r.
 00000580: 0000 0072 1900 0000 7a04 236b 6579 2903  ...r....z.#key).
 00000590: 7207 0000 00da 056f 776e 6572 da0c 7075  r......owner..pu
 000005a0: 626c 6963 4b65 7950 656d a901 7a12 2528  blicKeyPem..z.%(
 000005b0: 7079 3129 7320 3d3d 2025 2870 7934 2973  py1)s == %(py4)s
 000005c0: a902 7211 0000 00da 0370 7934 fa0e 6173  ..r......py4..as
 000005d0: 7365 7274 2025 2870 7936 2973 da03 7079  sert %(py6)s..py
 000005e0: 3629 1072 0400 0000 da05 6275 696c 64da  6).r......build.
@@ -152,16 +152,16 @@
 00000970: 7d01 7c01 640c 1900 640d 1900 7d02 640a  }.|.d...d...}.d.
 00000980: 7d03 7c02 7c03 6b02 7d04 7c04 73b0 7402  }.|.|.k.}.|.s.t.
 00000990: a003 6405 7c04 6601 6406 7c02 7c03 6602  ..d.|.f.d.|.|.f.
 000009a0: a104 7402 a004 7c02 a101 7402 a004 7c03  ..t...|...t...|.
 000009b0: a101 6407 9c02 1600 7d05 6408 6409 7c05  ..d.....}.d.d.|.
 000009c0: 6901 1600 7d06 7405 7402 a006 7c06 a101  i...}.t.t...|...
 000009d0: 8301 8201 6400 0400 7d02 0400 7d04 7d03  ....d...}...}.}.
-000009e0: 6400 5300 290e 4e72 0600 0000 7209 0000  d.S.).Nr....r...
-000009f0: 0072 0a00 0000 a903 7207 0000 0072 0900  .r......r....r..
+000009e0: 6400 5300 290e 4e72 0600 0000 7208 0000  d.S.).Nr....r...
+000009f0: 0072 0a00 0000 a903 7207 0000 0072 0800  .r......r....r..
 00000a00: 0000 720a 0000 0072 0c00 0000 721c 0000  ..r....r....r...
 00000a10: 0072 1d00 0000 721f 0000 0072 2000 0000  .r....r....r ...
 00000a20: 7a18 6874 7470 3a2f 2f65 7861 6d70 6c65  z.http://example
 00000a30: 2e63 6f6d 2f70 726f 7879 2901 da0a 7669  .com/proxy)...vi
 00000a40: 7369 6269 6c69 7479 da09 656e 6470 6f69  sibility..endpoi
 00000a50: 6e74 73da 0870 726f 7879 5572 6c29 0a72  nts..proxyUrl).r
 00000a60: 0400 0000 7221 0000 0072 2300 0000 7224  ....r!...r#...r$
@@ -181,16 +181,16 @@
 00000b40: 7d02 6405 6406 6901 7d03 7c02 7c03 6b02  }.d.d.i.}.|.|.k.
 00000b50: 7d04 7c04 7341 7403 a004 6408 7c04 6601  }.|.sAt...d.|.f.
 00000b60: 6409 7c02 7c03 6602 a104 7403 a005 7c02  d.|.|.f...t...|.
 00000b70: a101 7403 a005 7c03 a101 640a 9c02 1600  ..t...|...d.....
 00000b80: 7d05 640b 640c 7c05 6901 1600 7d06 7406  }.d.d.|.i...}.t.
 00000b90: 7403 a007 7c06 a101 8301 8201 6400 0400  t...|.......d...
 00000ba0: 7d02 0400 7d04 7d03 6400 5300 290d 4e72  }...}.}.d.S.).Nr
-00000bb0: 0600 0000 7209 0000 0072 0a00 0000 723c  ....r....r....r<
-00000bc0: 0000 0072 0b00 0000 5a05 496d 6167 65da  ...r....Z.Image.
+00000bb0: 0600 0000 7208 0000 0072 0a00 0000 723c  ....r....r....r<
+00000bc0: 0000 0072 0900 0000 5a05 496d 6167 65da  ...r....Z.Image.
 00000bd0: 0469 636f 6e72 0c00 0000 721c 0000 0072  .iconr....r....r
 00000be0: 1d00 0000 721f 0000 0072 2000 0000 2908  ....r....r ...).
 00000bf0: 7204 0000 0072 4400 0000 7221 0000 0072  r....rD...r!...r
 00000c00: 2300 0000 7224 0000 0072 2800 0000 7229  #...r$...r(...r)
 00000c10: 0000 0072 2a00 0000 7242 0000 0072 3900  ...r*...rB...r9.
 00000c20: 0000 7239 0000 0072 3a00 0000 da14 7465  ..r9...r:.....te
 00000c30: 7374 5f61 6374 6f72 5f77 6974 685f 6963  st_actor_with_ic
```

### Comparing `bovine-0.2.5/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 1257 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 e904 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 e904 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 640a 6406 6407 8404 5a0a 640a 6408 6409  d.d.d...Z.d.d.d.
 00000070: 8404 5a0b 6401 5300 290b e900 0000 004e  ..Z.d.S.)......N
@@ -39,17 +39,17 @@
 00000260: 0474 07a0 0c7c 0aa1 0174 07a0 0c7c 0ba1  .t...|...t...|..
 00000270: 0164 109c 0216 007d 0c64 1164 127c 0c69  .d.....}.d.d.|.i
 00000280: 0116 007d 0d74 0d74 07a0 0e7c 0da1 0183  ...}.t.t...|....
 00000290: 0182 0164 0004 007d 0a04 007d 037d 0b64  ...d...}...}.}.d
 000002a0: 0053 0029 144e da08 6163 746f 725f 6964  .S.).N..actor_id
 000002b0: da09 666f 6c6c 6f77 6572 7329 02da 0269  ..followers)...i
 000002c0: 6472 0700 0000 da04 7465 7874 3e06 0000  dr......text>...
-000002d0: 00fa 0840 636f 6e74 6578 74da 0263 63da  ...@context..cc.
-000002e0: 0c61 7474 7269 6275 7465 6454 6fda 0763  .attributedTo..c
-000002f0: 6f6e 7465 6e74 da02 746f da04 7479 7065  ontent..to..type
+000002d0: 00da 0263 63da 0763 6f6e 7465 6e74 da04  ...cc..content..
+000002e0: 7479 7065 da0c 6174 7472 6962 7574 6564  type..attributed
+000002f0: 546f da02 746f fa08 4063 6f6e 7465 7874  To..to..@context
 00000300: a901 fa02 3d3d a901 7a62 2528 7079 3729  ....==..zb%(py7)
 00000310: 730a 7b25 2870 7937 2973 203d 2025 2870  s.{%(py7)s = %(p
 00000320: 7930 2973 2825 2870 7935 2973 0a7b 2528  y0)s(%(py5)s.{%(
 00000330: 7079 3529 7320 3d20 2528 7079 3329 730a  py5)s = %(py3)s.
 00000340: 7b25 2870 7933 2973 203d 2025 2870 7931  {%(py3)s = %(py1
 00000350: 2973 2e6b 6579 730a 7d28 290a 7d29 0a7d  )s.keys.}().}).}
 00000360: 203d 3d20 2528 7079 3130 2973 da03 7365   == %(py10)s..se
@@ -59,17 +59,17 @@
 000003a0: 7274 2025 2870 7931 3229 73da 0470 7931  rt %(py12)s..py1
 000003b0: 3272 0e00 0000 7a2c 6874 7470 733a 2f2f  2r....z,https://
 000003c0: 7777 772e 7733 2e6f 7267 2f6e 732f 6163  www.w3.org/ns/ac
 000003d0: 7469 7669 7479 7374 7265 616d 7323 5075  tivitystreams#Pu
 000003e0: 626c 6963 a901 7a12 2528 7079 3129 7320  blic..z.%(py1)s 
 000003f0: 3d3d 2025 2870 7934 2973 a902 7217 0000  == %(py4)s..r...
 00000400: 00da 0370 7934 fa0e 6173 7365 7274 2025  ...py4..assert %
-00000410: 2870 7936 2973 da03 7079 3672 0b00 0000  (py6)s..py6r....
+00000410: 2870 7936 2973 da03 7079 3672 0a00 0000  (py6)s..py6r....
 00000420: 290f 7204 0000 00da 046e 6f74 65da 0961  ).r......note..a
-00000430: 735f 7075 626c 6963 720d 0000 00da 0562  s_publicr......b
+00000430: 735f 7075 626c 6963 720b 0000 00da 0562  s_publicr......b
 00000440: 7569 6c64 da04 6b65 7973 7213 0000 00da  uild..keysr.....
 00000450: 0a40 7079 7465 7374 5f61 72da 115f 6361  .@pytest_ar.._ca
 00000460: 6c6c 5f72 6570 7263 6f6d 7061 7265 da0c  ll_reprcompare..
 00000470: 4070 795f 6275 696c 7469 6e73 da06 6c6f  @py_builtins..lo
 00000480: 6361 6c73 da18 5f73 686f 756c 645f 7265  cals.._should_re
 00000490: 7072 5f67 6c6f 6261 6c5f 6e61 6d65 da09  pr_global_name..
 000004a0: 5f73 6166 6572 6570 72da 0e41 7373 6572  _saferepr..Asser
@@ -142,29 +142,29 @@
 000008d0: 6413 6414 7c0e 6901 1600 7d0f 740e 7408  d.d.|.i...}.t.t.
 000008e0: a00f 7c0f a101 8301 8201 6400 0400 7d0c  ..|.......d...}.
 000008f0: 0400 7d05 7d0d 6400 5300 291d 4e7a 1468  ..}.}.d.S.).Nz.h
 00000900: 7474 7073 3a2f 2f72 656d 6f74 652f 616c  ttps://remote/al
 00000910: 6963 657a 2568 7474 7073 3a2f 2f77 7777  icez%https://www
 00000920: 2e77 332e 6f72 672f 6e73 2f61 6374 6976  .w3.org/ns/activ
 00000930: 6974 7973 7472 6561 6d73 da06 5065 7273  itystreams..Pers
-00000940: 6f6e 5a06 616c 7973 7361 2904 720a 0000  onZ.alyssa).r...
-00000950: 0072 0800 0000 720f 0000 00da 1170 7265  .r....r......pre
+00000940: 6f6e 5a06 616c 7973 7361 2904 720f 0000  onZ.alyssa).r...
+00000950: 0072 0800 0000 720c 0000 00da 1170 7265  .r....r......pre
 00000960: 6665 7272 6564 5573 6572 6e61 6d65 2901  ferredUsername).
-00000970: da06 636c 6965 6e74 3e04 0000 0072 0a00  ..client>....r..
-00000980: 0000 da04 6e61 6d65 720f 0000 00da 0468  ....namer......h
-00000990: 7265 6672 1000 0000 7212 0000 0072 1300  refr....r....r..
+00000970: da06 636c 6965 6e74 3e04 0000 00da 0468  ..client>......h
+00000980: 7265 6672 0c00 0000 da04 6e61 6d65 720f  refr......namer.
+00000990: 0000 0072 1000 0000 7212 0000 0072 1300  ...r....r....r..
 000009a0: 0000 da07 6d65 6e74 696f 6e72 1500 0000  ....mentionr....
-000009b0: 721c 0000 0072 1d00 0000 720f 0000 00da  r....r....r.....
+000009b0: 721c 0000 0072 1d00 0000 720c 0000 00da  r....r....r.....
 000009c0: 074d 656e 7469 6f6e 721e 0000 0072 1f00  .Mentionr....r..
-000009d0: 0000 7221 0000 0072 2200 0000 7242 0000  ..r!...r"...rB..
+000009d0: 0000 7221 0000 0072 2200 0000 7241 0000  ..r!...r"...rA..
 000009e0: 0029 017a 1225 2870 7931 2973 203d 3d20  .).z.%(py1)s == 
 000009f0: 2528 7079 3329 73da 0a72 656d 6f74 655f  %(py3)s..remote_
 00000a00: 7572 6929 0272 1700 0000 7218 0000 007a  uri).r....r....z
 00000a10: 0e61 7373 6572 7420 2528 7079 3529 7372  .assert %(py5)sr
-00000a20: 1900 0000 7241 0000 007a 0d61 6c79 7373  ....rA...z.alyss
+00000a20: 1900 0000 7242 0000 007a 0d61 6c79 7373  ....rB...z.alyss
 00000a30: 6140 7265 6d6f 7465 2910 7202 0000 00da  a@remote).r.....
 00000a40: 0d70 726f 7879 5f65 6c65 6d65 6e74 da0c  .proxy_element..
 00000a50: 7265 7475 726e 5f76 616c 7565 7204 0000  return_valuer...
 00000a60: 00da 156d 656e 7469 6f6e 5f66 6f72 5f61  ...mention_for_a
 00000a70: 6374 6f72 5f75 7269 7225 0000 0072 2600  ctor_urir%...r&.
 00000a80: 0000 7213 0000 0072 2700 0000 7228 0000  ..r....r'...r(..
 00000a90: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
```

### Comparing `bovine-0.2.5/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 1034 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 0a04 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 0a04 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 640b 6405 6406 8404 5a08 640b  Z...d.d.d...Z.d.
 00000060: 6407 6408 8404 5a09 640b 6409 640a 8404  d.d...Z.d.d.d...
 00000070: 5a0a 6401 5300 290c e900 0000 004e e901  Z.d.S.)......N..
```

### Comparing `bovine-0.2.5/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 817 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 3103 0000  o.......5bsd1...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 3103 0000  o.........|d1...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6407 6405 6406 8404 5a08 6401  Z...d.d.d...Z.d.
 00000060: 5300 2908 e900 0000 004e e901 0000 0029  S.)......N.....)
 00000070: 01da 154f 7264 6572 6564 436f 6c6c 6563  ...OrderedCollec
```

### Comparing `bovine-0.2.5/bovine/activitystreams/activity_factory.py` & `bovine-0.2.6/bovine/activitystreams/activity_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,20 @@
     def as_public(self):
         """makes the activity public, i.e. public in to and followers in cc"""
         self.to.add("https://www.w3.org/ns/activitystreams#Public")
         if self.followers:
             self.cc.add(self.followers)
         return self
 
+    def as_followers(self):
+        """addresses the activity to followers, if they are set"""
+        if self.followers:
+            self.to.add(self.followers)
+        return self
+
     def as_unlisted(self):
         """makes the activity unlisted, i.e. public in cc and followers in to"""
         if self.followers:
             self.to.add(self.followers)
         self.cc.add("https://www.w3.org/ns/activitystreams#Public")
         return self
```

### Comparing `bovine-0.2.5/bovine/activitystreams/object_factory.py` & `bovine-0.2.6/bovine/activitystreams/object_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,20 +28,28 @@
     in_reply_to: Optional[str] = None
     url: Optional[str] = None
     tag: List[dict] = field(default_factory=list)
     attachment: List[dict] = field(default_factory=list)
     href: Optional[str] = None
 
     def as_public(self):
+        """makes the object public, i.e. public in to and followers in cc"""
         self.to.add("https://www.w3.org/ns/activitystreams#Public")
         if self.followers:
             self.cc.add(self.followers)
         return self
 
+    def as_followers(self):
+        """addresses the object to followers, if they are set"""
+        if self.followers:
+            self.to.add(self.followers)
+        return self
+
     def as_unlisted(self):
+        """makes the object unlisted, i.e. public in cc and followers in to"""
         if self.followers:
             self.to.add(self.followers)
         self.cc.add("https://www.w3.org/ns/activitystreams#Public")
         return self
 
     def build(self):
         result = {
```

### Comparing `bovine-0.2.5/bovine/activitystreams/test_activity_factory.py` & `bovine-0.2.6/bovine/activitystreams/test_activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/activitystreams/test_actor.py` & `bovine-0.2.6/bovine/activitystreams/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/activitystreams/test_object_factory.py` & `bovine-0.2.6/bovine/activitystreams/test_object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/activitystreams/test_ordered_collection_builder.py` & `bovine-0.2.6/bovine/activitystreams/test_ordered_collection_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/activitystreams/test_ordered_collection_page.py` & `bovine-0.2.6/bovine/activitystreams/test_ordered_collection_page.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/activitystreams/utils/__init__.py` & `bovine-0.2.6/bovine/activitystreams/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.6/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 2354 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 3209 0000  o.......5bsd2...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 3209 0000  o.........|d2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6504 6404 6505 6604  m.Z...d.e.d.e.f.
 00000050: 6405 6406 8404 5a06 6403 6501 6504 6505  d.d...Z.d.e.e.e.
 00000060: 4200 1900 6404 6501 6505 1900 6604 6407  B...d.e.e...f.d.
 00000070: 6408 8404 5a07 6409 640a 8400 5a08 6403  d...Z.d.d...Z.d.
```

### Comparing `bovine-0.2.5/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 2266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 da08 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 da08 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6405 6406  Z.m.Z.m.Z...d.d.
 00000070: 8400 5a0d 6407 6408 8400 5a0e 6409 640a  ..Z.d.d...Z.d.d.
@@ -33,16 +33,16 @@
 00000200: 636f 756e 742f 666f 6c6c 6f77 6572 73a9  count/followers.
 00000210: 03da 0474 7970 65da 0d61 7474 7269 6275  ...type..attribu
 00000220: 7465 645f 746f da09 666f 6c6c 6f77 6572  ted_to..follower
 00000230: 73da 0263 63da 0274 6fda 0473 616d 653e  s..cc..to..same>
 00000240: 0500 0000 720f 0000 0072 1100 0000 7a2c  ....r....r....z,
 00000250: 6874 7470 733a 2f2f 7777 772e 7733 2e6f  https://www.w3.o
 00000260: 7267 2f6e 732f 6163 7469 7669 7479 7374  rg/ns/activityst
-00000270: 7265 616d 7323 5075 626c 6963 720a 0000  reams#Publicr...
-00000280: 0072 1000 0000 a901 fa02 3d3d 2901 7a12  .r........==).z.
+00000270: 7265 616d 7323 5075 626c 6963 7210 0000  reams#Publicr...
+00000280: 0072 0a00 0000 a901 fa02 3d3d 2901 7a12  .r........==).z.
 00000290: 2528 7079 3029 7320 3d3d 2025 2870 7933  %(py0)s == %(py3
 000002a0: 2973 da0a 7265 6369 7069 656e 7473 2902  )s..recipients).
 000002b0: da03 7079 30da 0370 7933 7a0e 6173 7365  ..py0..py3z.asse
 000002c0: 7274 2025 2870 7935 2973 da03 7079 3529  rt %(py5)s..py5)
 000002d0: 0f72 0200 0000 da09 6173 5f70 7562 6c69  .r......as_publi
 000002e0: 6372 0f00 0000 da03 6164 6472 1000 0000  cr......addr....
 000002f0: da05 6275 696c 6472 0700 0000 da0a 4070  ..buildr......@p
```

### Comparing `bovine-0.2.5/bovine/activitystreams/utils/print.py` & `bovine-0.2.6/bovine/activitystreams/utils/print.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/activitystreams/utils/test_utils.py` & `bovine-0.2.6/bovine/activitystreams/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/__init__.py` & `bovine-0.2.6/bovine/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 3968 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 800f 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 800f 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 0601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6403 6c07 6d08 5a08 0100 6404 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6404 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -183,23 +183,23 @@
 00000b60: 6573 7369 6f6e 3a20 7468 6520 6169 6f68  ession: the aioh
 00000b70: 7474 702e 436c 6965 6e74 5365 7373 696f  ttp.ClientSessio
 00000b80: 6e20 746f 2075 7365 0a20 2020 203a 7061  n to use.    :pa
 00000b90: 7261 6d20 646f 6d61 696e 3a20 7468 6520  ram domain: the 
 00000ba0: 646f 6d61 696e 2074 6f20 7065 7266 6f72  domain to perfor
 00000bb0: 6d20 7468 6520 6c6f 6f6b 7570 2066 726f  m the lookup fro
 00000bc0: 6d0a 2020 2020 7a09 5f61 706f 626a 6964  m.    z._apobjid
-00000bd0: 2eda 0354 5854 4e29 05da 0661 696f 646e  ...TXTN)...aiodn
-00000be0: 73da 0b44 4e53 5265 736f 6c76 6572 da05  s..DNSResolver..
+00000bd0: 2e5a 0354 5854 4e29 05da 0661 696f 646e  .Z.TXTN)...aiodn
+00000be0: 735a 0b44 4e53 5265 736f 6c76 6572 da05  sZ.DNSResolver..
 00000bf0: 7175 6572 79da 0474 6578 74da 0945 7863  query..text..Exc
 00000c00: 6570 7469 6f6e 2904 7209 0000 0072 1500  eption).r....r..
 00000c10: 0000 da08 7265 736f 6c76 6572 720f 0000  ....resolverr...
 00000c20: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
 00000c30: da0f 6c6f 6f6b 7570 5f77 6974 685f 646e  ..lookup_with_dn
 00000c40: 7350 0000 0073 1000 0000 0280 080a 0201  sP...s..........
-00000c50: 1a01 0802 0c01 0601 02ff 7225 0000 0063  ..........r%...c
+00000c50: 1a01 0802 0c01 0601 02ff 7223 0000 0063  ..........r#...c
 00000c60: 0200 0000 0000 0000 0000 0000 0600 0000  ................
 00000c70: 0a00 0000 c300 0000 739e 0000 0081 017a  ........s......z
 00000c80: 2574 007c 007c 0183 0249 0064 0148 007d  %t.|.|...I.d.H.}
 00000c90: 027c 0264 0219 0044 005d 157d 037c 0364  .|.d...D.].}.|.d
 00000ca0: 0319 0064 046b 0272 2374 017c 007c 0364  ...d.k.r#t.|.|.d
 00000cb0: 0519 0083 0249 0064 0148 0002 0001 0057  .....I.d.H.....W
 00000cc0: 0053 0071 0e57 0064 0153 0004 0074 0279  .S.q.W.d.S...t.y
@@ -209,43 +209,43 @@
 00000d00: 0071 3b57 0059 0064 017d 047e 0464 0153  .q;W.Y.d.}.~.d.S
 00000d10: 0064 017d 047e 0477 0177 0029 067a 5846  .d.}.~.w.w.).zXF
 00000d20: 6574 6368 6573 2074 6865 206e 6f64 6569  etches the nodei
 00000d30: 6e66 6f20 322e 3020 6f62 6a65 6374 2066  nfo 2.0 object f
 00000d40: 726f 6d20 646f 6d61 696e 2075 7369 6e67  rom domain using
 00000d50: 2074 6865 202f 2e77 656c 6c2d 6b6e 6f77   the /.well-know
 00000d60: 6e2f 6e6f 6465 696e 666f 0a20 2020 2065  n/nodeinfo.    e
-00000d70: 6e64 706f 696e 744e da05 6c69 6e6b 73da  ndpointN..links.
+00000d70: 6e64 706f 696e 744e 5a05 6c69 6e6b 73da  ndpointNZ.links.
 00000d80: 0372 656c 7a2f 6874 7470 3a2f 2f6e 6f64  .relz/http://nod
 00000d90: 6569 6e66 6f2e 6469 6173 706f 7261 2e73  einfo.diaspora.s
 00000da0: 6f66 7477 6172 652f 6e73 2f73 6368 656d  oftware/ns/schem
-00000db0: 612f 322e 305a 0468 7265 6629 0972 0800  a/2.0Z.href).r..
-00000dc0: 0000 7207 0000 0072 2300 0000 da06 6c6f  ..r....r#.....lo
+00000db0: 612f 322e 30da 0468 7265 6629 0972 0800  a/2.0..href).r..
+00000dc0: 0000 7207 0000 0072 2100 0000 da06 6c6f  ..r....r!.....lo
 00000dd0: 6767 6572 da05 6572 726f 72da 0373 7472  gger..error..str
 00000de0: da09 7472 6163 6562 6163 6bda 0a66 6f72  ..traceback..for
 00000df0: 6d61 745f 6578 63da 0a73 706c 6974 6c69  mat_exc..splitli
 00000e00: 6e65 7329 0672 0900 0000 7215 0000 00da  nes).r....r.....
 00000e10: 0464 6174 61da 046c 696e 6bda 0165 5a08  .data..link..eZ.
 00000e20: 6c6f 675f 6c69 6e65 7211 0000 0072 1100  log_liner....r..
 00000e30: 0000 7212 0000 00da 0e66 6574 6368 5f6e  ..r......fetch_n
 00000e40: 6f64 6569 6e66 6f63 0000 0073 1e00 0000  odeinfoc...s....
 00000e50: 0280 0204 1001 0c02 0c01 1a01 02ff 0603  ................
-00000e60: 0e02 0e01 1001 0c01 0e01 0880 02fc 7231  ..............r1
+00000e60: 0e02 0e01 1001 0c01 0e01 0880 02fc 722f  ..............r/
 00000e70: 0000 0029 014e 291a da07 6c6f 6767 696e  ...).N)...loggin
-00000e80: 6772 2b00 0000 da06 7479 7069 6e67 7202  gr+.....typingr.
-00000e90: 0000 0072 0300 0000 721f 0000 00da 0761  ...r....r......a
+00000e80: 6772 2900 0000 da06 7479 7069 6e67 7202  gr).....typingr.
+00000e90: 0000 0072 0300 0000 721e 0000 005a 0761  ...r....r....Z.a
 00000ea0: 696f 6874 7470 5a0c 626f 7669 6e65 2e75  iohttpZ.bovine.u
 00000eb0: 7469 6c73 7204 0000 005a 0e6c 6f6f 6b75  tilsr....Z.looku
 00000ec0: 705f 6163 636f 756e 7472 0600 0000 5a08  p_accountr....Z.
 00000ed0: 6e6f 6465 696e 666f 7207 0000 0072 0800  nodeinfor....r..
 00000ee0: 0000 da09 6765 744c 6f67 6765 72da 085f  ....getLogger.._
-00000ef0: 5f6e 616d 655f 5f72 2800 0000 da0d 436c  _name__r(.....Cl
-00000f00: 6965 6e74 5365 7373 696f 6e72 2a00 0000  ientSessionr*...
+00000ef0: 5f6e 616d 655f 5f72 2600 0000 5a0d 436c  _name__r&...Z.Cl
+00000f00: 6965 6e74 5365 7373 696f 6e72 2800 0000  ientSessionr(...
 00000f10: 7213 0000 0072 1700 0000 da04 626f 6f6c  r....r......bool
-00000f20: 720e 0000 0072 2500 0000 da04 6469 6374  r....r%.....dict
-00000f30: 7231 0000 0072 1100 0000 7211 0000 0072  r1...r....r....r
+00000f20: 720e 0000 0072 2300 0000 da04 6469 6374  r....r#.....dict
+00000f30: 722f 0000 0072 1100 0000 7211 0000 0072  r/...r....r....r
 00000f40: 1100 0000 7212 0000 00da 083c 6d6f 6475  ....r......<modu
 00000f50: 6c65 3e01 0000 0073 4600 0000 0800 0801  le>....sF.......
 00000f60: 1001 0802 0801 0c02 0c02 1001 0a02 0203  ................
 00000f70: 0401 02ff 0201 02ff 0602 0afe 0210 0401  ................
 00000f80: 02ff 0201 02ff 0201 0aff 0211 04ff 0401  ................
 00000f90: 02ff 0201 02ff 0601 02ff 1202 0afe 1c20  ............... 
 00000fa0: 2013                                      .
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/bearer.cpython-310.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/bearer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 1794 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 0207 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 0207 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 0100 4700 6406 6407  d.l.m.Z...G.d.d.
 00000060: 8400 6407 8302 5a07 6401 5300 2908 e900  ..d...Z.d.S.)...
 00000070: 0000 004e 2901 da0b 6765 745f 676d 745f  ...N)...get_gmt_
@@ -107,14 +107,14 @@
 000006a0: 5365 7373 696f 6eda 0373 7472 720c 0000  Session..strr...
 000006b0: 00da 0464 6963 7472 1600 0000 721b 0000  ...dictr....r...
 000006c0: 0072 0500 0000 721d 0000 0072 0a00 0000  .r....r....r....
 000006d0: 720a 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
 000006e0: 0600 0000 0900 0000 731e 0000 0008 0004  ........s.......
 000006f0: 0114 0216 0404 0c04 ff02 0102 ff02 0102  ................
 00000700: ff02 0102 ff06 010a ff1e 1072 0600 0000  ...........r....
-00000710: 2908 7222 0000 005a 1162 6f76 696e 652e  ).r"...Z.bovine.
+00000710: 2908 7222 0000 00da 1162 6f76 696e 652e  ).r".....bovine.
 00000720: 7574 696c 732e 6461 7465 7202 0000 00da  utils.dater.....
 00000730: 0663 6f6e 7374 7372 0400 0000 721d 0000  .constsr....r...
 00000740: 0072 0500 0000 7206 0000 0072 0a00 0000  .r....r....r....
 00000750: 720a 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
 00000760: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
 00000770: 0000 0800 0c02 0c02 0c01 1203            ............
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/event_source.cpython-310.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/event_source.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 1520 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 f005 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 f005 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 4700  Z.d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 8302 5a05 6402 5300  d.d...d...Z.d.S.
 00000060: 2906 e900 0000 0029 01da 0444 6963 744e  )......)...DictN
 00000070: 2901 da0f 5365 7276 6572 5365 6e74 4576  )...ServerSentEv
@@ -75,15 +75,15 @@
 000004a0: 7c03 6403 1900 6404 6b02 722a 7118 7c03  |.d...d.k.r*q.|.
 000004b0: 6405 6b02 723b 7404 a005 7c01 a101 7d04  d.k.r;t...|...}.
 000004c0: 7c04 6a06 723a 7c04 0200 0100 5300 7118  |.j.r:|.....S.q.
 000004d0: 7c01 9b00 7c03 9b00 9d02 7d01 7118 3600  |...|.....}.q.6.
 000004e0: 6400 5300 2906 4eda 007a 0575 7466 2d38  d.S.).N..z.utf-8
 000004f0: 7201 0000 00fa 013a da01 0a29 0772 0900  r......:...).r..
 00000500: 0000 7219 0000 00da 0763 6f6e 7465 6e74  ..r......content
-00000510: da06 6465 636f 6465 7203 0000 005a 0a70  ..decoder....Z.p
+00000510: da06 6465 636f 6465 7203 0000 00da 0a70  ..decoder......p
 00000520: 6172 7365 5f75 7466 38da 0464 6174 6129  arse_utf8..data)
 00000530: 0572 0a00 0000 5a08 746f 5f70 6172 7365  .r....Z.to_parse
 00000540: 5a0d 6c69 6e65 5f69 6e5f 6279 7465 73da  Z.line_in_bytes.
 00000550: 046c 696e 65da 0565 7665 6e74 720b 0000  .line..eventr...
 00000560: 0072 0b00 0000 720c 0000 00da 095f 5f61  .r....r......__a
 00000570: 6e65 7874 5f5f 2400 0000 7322 0000 0002  next__$...s"....
 00000580: 800a 010e 0104 020a 0214 020a 010c 0102  ................
@@ -91,18 +91,18 @@
 000005a0: 0b7a 1545 7665 6e74 536f 7572 6365 2e5f  .z.EventSource._
 000005b0: 5f61 6e65 7874 5f5f 2902 720e 0000 004e  _anext__).r....N
 000005c0: 290c da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000005d0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 000005e0: 6e61 6d65 5f5f 7214 0000 00da 0d43 6c69  name__r......Cli
 000005f0: 656e 7453 6573 7369 6f6e da03 7374 7272  entSession..strr
 00000600: 0200 0000 720d 0000 0072 1900 0000 721a  ....r....r....r.
-00000610: 0000 0072 0300 0000 7223 0000 0072 0b00  ...r....r#...r..
+00000610: 0000 0072 0300 0000 7224 0000 0072 0b00  ...r....r$...r..
 00000620: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
 00000630: 0072 0400 0000 0800 0000 7318 0000 0008  .r........s.....
 00000640: 0002 0204 ff04 0102 ff02 0102 ff0a 010a  ................
 00000650: ff0a 0808 1016 0372 0400 0000 2906 da06  .......r....)...
 00000660: 7479 7069 6e67 7202 0000 0072 1400 0000  typingr....r....
-00000670: 5a0c 626f 7669 6e65 2e74 7970 6573 7203  Z.bovine.typesr.
+00000670: da0c 626f 7669 6e65 2e74 7970 6573 7203  ..bovine.typesr.
 00000680: 0000 0072 0400 0000 720b 0000 0072 0b00  ...r....r....r..
 00000690: 0000 720b 0000 0072 0c00 0000 da08 3c6d  ..r....r......<m
 000006a0: 6f64 756c 653e 0100 0000 7308 0000 000c  odule>....s.....
 000006b0: 0008 020c 0212 03                        .......
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/lookup_account.cpython-310.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/lookup_account.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 868 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 6403 0000  o.......5bsdd...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 6403 0000  o.........|dd...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c04 6d05 5a05 0100 6501 a006 6507  d.l.m.Z...e...e.
 00000060: a101 5a08 6404 6503 6a09 6405 650a 6406  ..Z.d.e.j.d.e.d.
 00000070: 650b 6606 6407 6408 8404 5a0c 6401 5300  e.f.d.d...Z.d.S.
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/moo_auth.cpython-310.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/moo_auth.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 3001 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 b90b 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 b90b 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6405 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6408 6409 8400 5a0c 4700  m.Z...d.d...Z.G.
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 948 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 b403 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 b403 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c04 6d05 5a05 0100 6501 a006 6507  d.l.m.Z...e...e.
 00000060: a101 5a08 6404 6503 6a09 6405 650a 6406  ..Z.d.e.j.d.e.d.
 00000070: 650b 6606 6407 6408 8404 5a0c 6404 6503  e.f.d.d...Z.d.e.
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/signed_http.cpython-310.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/signed_http.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 1150 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 7e04 0000  o.......5bsd~...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 7e04 0000  o.........|d~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a02 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0003 0000 0040 0000 0073 4400 0000 6500  .....@...sD...e.
 00000070: 5a01 6400 5a02 6401 5a03 640d 6403 6404  Z.d.Z.d.Z.d.d.d.
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 3278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 ce0c 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 ce0c 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6406 6408 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 651 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 8b02 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 8b02 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6408 6406 6407 8404 5a0a 6401 5300 2909  d.d.d...Z.d.S.).
 00000070: e900 0000 004e 2901 da09 4173 796e 634d  .....N)...AsyncM
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 1505 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 e105 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 e105 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 6d09 5a09 6d0a  d.d.l.m.Z.m.Z.m.
 00000060: 5a0a 0100 6404 6405 8400 5a0b 6406 6407  Z...d.d...Z.d.d.
 00000070: 8400 5a0c 6408 6409 8400 5a0d 640a 640b  ..Z.d.d...Z.d.d.
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 319 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 3f01 0000  o.......5bsd?...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 3f01 0000  o.........|d?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 8400 5a09 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0e66 6574 6368 5f6e  .....)...fetch_n
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 1153 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 8104 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 8104 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a09  Z.m.Z...d.d.l.Z.
 00000060: 6400 6403 6c0a 6d0b 5a0b 0100 6400 6404  d.d.l.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6405 6406  l.m.Z.m.Z...d.d.
```

### Comparing `bovine-0.2.5/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 522 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 0a02 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 0a02 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6401 6c08 5a08 6400 6403  Z...d.d.l.Z.d.d.
 00000060: 6c09 6d0a 5a0a 0100 6404 6405 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6406 6407 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
```

### Comparing `bovine-0.2.5/bovine/clients/bearer.py` & `bovine-0.2.6/bovine/clients/bearer.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/event_source.py` & `bovine-0.2.6/bovine/clients/event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/lookup_account.py` & `bovine-0.2.6/bovine/clients/lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/moo_auth.py` & `bovine-0.2.6/bovine/clients/moo_auth.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/nodeinfo.py` & `bovine-0.2.6/bovine/clients/nodeinfo.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/signed_http.py` & `bovine-0.2.6/bovine/clients/signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/signed_http_methods.py` & `bovine-0.2.6/bovine/clients/signed_http_methods.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/test_event_source.py` & `bovine-0.2.6/bovine/clients/test_event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/test_lookup_account.py` & `bovine-0.2.6/bovine/clients/test_lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/test_signed_http.py` & `bovine-0.2.6/bovine/clients/test_signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/clients/test_signed_http_client.py` & `bovine-0.2.6/bovine/clients/test_signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/crypto/__init__.py` & `bovine-0.2.6/bovine/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/crypto/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.6/bovine/crypto/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 4141 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 2d10 0000  o.......5bsd-...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 2d10 0000  o.........|d-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0b 6406 6407 6c0c 6d0d 5a0d 6d0e 5a0e  Z.d.d.l.m.Z.m.Z.
@@ -193,43 +193,43 @@
 00000c00: 0b00 0000 4e7a 0f78 2d6d 6f6f 2d73 6967  ....Nz.x-moo-sig
 00000c10: 6e61 7475 7265 da04 6461 7465 da04 686f  nature..date..ho
 00000c20: 7374 da03 6765 747a 1028 7265 7175 6573  st..getz.(reques
 00000c30: 742d 7461 7267 6574 297a 0467 6574 20da  t-target)z.get .
 00000c40: 0664 6967 6573 7429 024e 4e7a 0570 6f73  .digest).NNz.pos
 00000c50: 7420 290e da07 6865 6164 6572 73da 0662  t )...headers..b
 00000c60: 6f76 696e 65da 0575 7469 6c73 7228 0000  ovine..utilsr(..
-00000c70: 00da 0970 6172 7365 5f67 6d74 da14 6368  ...parse_gmt..ch
+00000c70: 005a 0970 6172 7365 5f67 6d74 5a14 6368  .Z.parse_gmtZ.ch
 00000c80: 6563 6b5f 6d61 785f 6f66 6673 6574 5f6e  eck_max_offset_n
 00000c90: 6f77 da06 6d65 7468 6f64 da05 6c6f 7765  ow..method..lowe
-00000ca0: 7272 0d00 0000 da0a 7769 7468 5f66 6965  rr......with_fie
+00000ca0: 7272 0d00 0000 5a0a 7769 7468 5f66 6965  rr....Z.with_fie
 00000cb0: 6c64 da04 7061 7468 da08 6765 745f 6461  ld..path..get_da
 00000cc0: 7461 720a 0000 005a 0e65 6432 3535 3139  tar....Z.ed25519
 00000cd0: 5f76 6572 6966 7929 08da 0772 6571 7565  _verify)...reque
 00000ce0: 7374 da06 646f 6d61 696e 5a06 6469 646b  st..domainZ.didk
 00000cf0: 6579 da09 7369 676e 6174 7572 65da 0264  ey..signature..d
 00000d00: 74da 0e68 7474 705f 7369 676e 6174 7572  t..http_signatur
 00000d10: 65da 0872 6177 5f64 6174 6172 2b00 0000  e..raw_datar+...
 00000d20: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
 00000d30: 1b76 616c 6964 6174 655f 6d6f 6f5f 6175  .validate_moo_au
 00000d40: 7468 5f73 6967 6e61 7475 7265 4a00 0000  th_signatureJ...
 00000d50: 7332 0000 0002 8012 0f0a 0114 0212 0112  s2..............
 00000d60: 010e 0204 020e 010e 010e 0104 fc0e 0708  ................
 00000d70: 010e 0104 0104 020e 010e 010e 010e 0102  ................
-00000d80: fb0c 0808 0104 0172 3c00 0000 291a da06  .......r<...)...
+00000d80: fb0c 0808 0104 0172 3900 0000 291a da06  .......r9...)...
 00000d90: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
 00000da0: 5a1e 6372 7970 746f 6772 6170 6879 2e68  Z.cryptography.h
 00000db0: 617a 6d61 742e 7072 696d 6974 6976 6573  azmat.primitives
 00000dc0: 7204 0000 005a 2963 7279 7074 6f67 7261  r....Z)cryptogra
 00000dd0: 7068 792e 6861 7a6d 6174 2e70 7269 6d69  phy.hazmat.primi
 00000de0: 7469 7665 732e 6173 796d 6d65 7472 6963  tives.asymmetric
 00000df0: 7205 0000 0072 0600 0000 5a0c 6d75 6c74  r....r....Z.mult
 00000e00: 6966 6f72 6d61 7473 7207 0000 0072 0800  iformatsr....r..
 00000e10: 0000 722d 0000 00da 0668 656c 7065 7272  ..r-.....helperr
-00000e20: 0a00 0000 720b 0000 0072 0c00 0000 723a  ....r....r....r:
+00000e20: 0a00 0000 720b 0000 0072 0c00 0000 7237  ....r....r....r7
 00000e30: 0000 0072 0d00 0000 7224 0000 0072 0e00  ...r....r$...r..
 00000e40: 0000 da03 7374 7272 1d00 0000 7220 0000  ....strr....r ..
-00000e50: 0072 2300 0000 7225 0000 0072 3c00 0000  .r#...r%...r<...
+00000e50: 0072 2300 0000 7225 0000 0072 3900 0000  .r#...r%...r9...
 00000e60: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
 00000e70: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
 00000e80: 0000 731e 0000 0010 000c 0210 0110 0108  ..s.............
 00000e90: 0214 020c 010c 010e 0312 0f16 0c08 1602  ................
 00000ea0: 0b12 020e fe                             .....
```

### Comparing `bovine-0.2.5/bovine/crypto/__pycache__/helper.cpython-310.pyc` & `bovine-0.2.6/bovine/crypto/__pycache__/helper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 2664 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 680a 0000  o.......5bsdh...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 680a 0000  o.........|dh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `bovine-0.2.5/bovine/crypto/__pycache__/http_signature.cpython-310.pyc` & `bovine-0.2.6/bovine/crypto/__pycache__/http_signature.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 2112 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 4008 0000  o.......5bsd@...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 4008 0000  o.........|d@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6405  d.l.m.Z.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6500 a00c 650d a101 5a0e 6407 6408  ..e...e...Z.d.d.
```

### Comparing `bovine-0.2.5/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc` & `bovine-0.2.6/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 2942 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 7e0b 0000  o.......5bsd~...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 7e0b 0000  o.........|d~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6403 6c04 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 0100 6404 6406 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6404 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -125,15 +125,15 @@
 000007c0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
 000007d0: 6c6e 616d 655f 5f72 0d00 0000 7233 0000  lname__r....r3..
 000007e0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
 000007f0: 720c 0000 0072 0800 0000 0f00 0000 7306  r....r........s.
 00000800: 0000 0008 0008 010c 0372 0800 0000 2911  .........r....).
 00000810: da07 6c6f 6767 696e 6772 2700 0000 da0c  ..loggingr'.....
 00000820: 7572 6c6c 6962 2e70 6172 7365 7202 0000  urllib.parser...
-00000830: 00da 1162 6f76 696e 652e 7574 696c 732e  ...bovine.utils.
+00000830: 005a 1162 6f76 696e 652e 7574 696c 732e  .Z.bovine.utils.
 00000840: 6461 7465 721c 0000 0072 0300 0000 da06  dater....r......
 00000850: 6865 6c70 6572 7205 0000 0072 2c00 0000  helperr....r,...
 00000860: 7206 0000 005a 1073 6967 6e61 7475 7265  r....Z.signature
 00000870: 5f70 6172 7365 7272 0700 0000 da09 6765  _parserr......ge
 00000880: 744c 6f67 6765 7272 3400 0000 7215 0000  tLoggerr4...r...
 00000890: 0072 0800 0000 720b 0000 0072 0b00 0000  .r....r....r....
 000008a0: 720b 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
```

### Comparing `bovine-0.2.5/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc` & `bovine-0.2.6/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 1266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 f204 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 f204 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a00 6500 a001 6502 a101 5a03  d.l.Z.e...e...Z.
 00000040: 4700 6402 6403 8400 6403 8302 5a04 6404  G.d.d...d...Z.d.
 00000050: 6405 8400 5a05 6401 5300 2906 e900 0000  d...Z.d.S.).....
 00000060: 004e 6300 0000 0000 0000 0000 0000 0000  .Nc.............
 00000070: 0000 0003 0000 0040 0000 0073 2800 0000  .......@...s(...
```

### Comparing `bovine-0.2.5/bovine/crypto/__pycache__/test.cpython-310.pyc` & `bovine-0.2.6/bovine/crypto/__pycache__/test.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 2199 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 9708 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 9708 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5300 2903 61c4 0100  Z.d.Z.d.S.).a...
 00000040: 000a 2d2d 2d2d 2d42 4547 494e 2050 5542  ..-----BEGIN PUB
 00000050: 4c49 4320 4b45 592d 2d2d 2d2d 0a4d 4949  LIC KEY-----.MII
 00000060: 4249 6a41 4e42 676b 7168 6b69 4739 7730  BIjANBgkqhkiG9w0
 00000070: 4241 5145 4641 414f 4341 5138 414d 4949  BAQEFAAOCAQ8AMII
```

### Comparing `bovine-0.2.5/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 4995 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 8313 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 8313 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 6d09 5a09 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  l.m.Z.m.Z.m.Z.m.
 00000070: 5a0e 0100 6403 6405 6c0f 6d10 5a10 0100  Z...d.d.l.m.Z...
```

### Comparing `bovine-0.2.5/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 896 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 8003 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 8003 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6403 6405  Z.m.Z.m.Z...d.d.
 00000070: 6c0d 6d0e 5a0e 6d0f 5a0f 0100 6406 6407  l.m.Z.m.Z...d.d.
```

### Comparing `bovine-0.2.5/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 5081 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 d913 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 d913 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6402 6404  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 0100 6402 6405  l.m.Z.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 0100 6406 6407 8400 5a0e  l.m.Z...d.d...Z.
```

### Comparing `bovine-0.2.5/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 1207 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 b704 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 b704 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6406 6407  Z...d.d...Z.d.d.
 00000060: 8400 5a09 6401 5300 2908 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0953 6967 6e61 7475  .....)...Signatu
```

### Comparing `bovine-0.2.5/bovine/crypto/helper.py` & `bovine-0.2.6/bovine/crypto/helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/crypto/http_signature.py` & `bovine-0.2.6/bovine/crypto/http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/crypto/signature_checker.py` & `bovine-0.2.6/bovine/crypto/signature_checker.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/crypto/signature_parser.py` & `bovine-0.2.6/bovine/crypto/signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/crypto/test.py` & `bovine-0.2.6/bovine/crypto/test.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/crypto/test_crypto.py` & `bovine-0.2.6/bovine/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/crypto/test_helper.py` & `bovine-0.2.6/bovine/crypto/test_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/crypto/test_http_signature.py` & `bovine-0.2.6/bovine/crypto/test_http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/crypto/test_signature_parser.py` & `bovine-0.2.6/bovine/crypto/test_signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/jsonld.py` & `bovine-0.2.6/bovine/jsonld.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/msg.py` & `bovine-0.2.6/bovine/msg.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/repl.py` & `bovine-0.2.6/bovine/repl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import json
 from argparse import ArgumentParser
 
+from asyncstdlib.itertools import islice
 from ptpython.repl import embed
 
 from bovine import BovineClient
 from bovine.activitystreams.utils.print import print_activity
 
 
 def build_parser():
@@ -64,15 +65,15 @@
     client: BovineClient, max_number: int = 10, summary: bool = False
 ):
     async with client:
         await display_box(await client.outbox(), max_number, summary)
 
 
 async def display_box(box, max_number: int, summary: bool):
-    async for item in box.iterate(max_number=max_number):
+    async for item in islice(box, max_number):
         if summary:
             print_activity(item)
         else:
             print(json.dumps(item, indent=2))
             print()
```

### Comparing `bovine-0.2.5/bovine/test_jsonld.py` & `bovine-0.2.6/bovine/test_jsonld.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/types.py` & `bovine-0.2.6/bovine/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     `Event Source Interface
     <https://html.spec.whatwg.org/multipage/server-sent-events.html#server-sent-events>`_.
     This is used by the event_source function
     of the BovineClient."""
 
     data: str
     event: str | None = None
-    id: int | None = None
+    id: str | None = None
     retry: int | None = None
 
     def encode(self) -> bytes:
         """Encodes the server sent event as bytes to send to the client."""
         message = f"data: {self.data}"
         if self.event is not None:
             message = f"{message}\nevent: {self.event}"
```

### Comparing `bovine-0.2.5/bovine/utils/__init__.py` & `bovine-0.2.6/bovine/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime, timezone
 from typing import Optional, Tuple
 
 
-def webfinger_response_json(name: str, url: str, domain: str) -> dict:
+def webfinger_response_json(account: str, url: str) -> dict:
     """helper to generate a webfinger response"""
     return {
-        "subject": f"acct:{name}@{domain}",
+        "subject": account,
         "links": [
             {
                 "href": url,
                 "rel": "self",
                 "type": "application/activity+json",
             }
         ],
@@ -23,11 +23,13 @@
 
     if "@" in account:
         return tuple(account.split("@", 1))
     return account, None
 
 
 def now_isoformat() -> str:
+    """Returns now in Isoformat, e.g. "2023-05-31T18:11:35Z", to be used as the value
+    of published"""
     return (
         datetime.now(tz=timezone.utc).replace(microsecond=0, tzinfo=None).isoformat()
         + "Z"
     )
```

### Comparing `bovine-0.2.5/bovine/utils/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.6/bovine/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 856 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,74 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 5803 0000  o.......5bsdX...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 a803 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
+00000020: 0007 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 6d00 5a00 6d01 5a01 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6403  d.l.m.Z.m.Z...d.
-00000050: 6505 6404 6505 6405 6505 6406 6506 6608  e.d.e.d.e.d.e.f.
-00000060: 6407 6408 8404 5a07 6409 6505 6406 6504  d.d...Z.d.e.d.e.
-00000070: 6505 6503 6505 1900 6602 1900 6604 640a  e.e.e...f...f.d.
-00000080: 640b 8404 5a08 6406 6505 6602 640c 640d  d...Z.d.e.f.d.d.
-00000090: 8404 5a09 640e 5300 290f e900 0000 0029  ..Z.d.S.)......)
-000000a0: 02da 0864 6174 6574 696d 65da 0874 696d  ...datetime..tim
-000000b0: 657a 6f6e 6529 02da 084f 7074 696f 6e61  ezone)...Optiona
-000000c0: 6cda 0554 7570 6c65 da04 6e61 6d65 da03  l..Tuple..name..
-000000d0: 7572 6cda 0664 6f6d 6169 6eda 0672 6574  url..domain..ret
-000000e0: 7572 6e63 0300 0000 0000 0000 0000 0000  urnc............
-000000f0: 0300 0000 0500 0000 4300 0000 7320 0000  ........C...s ..
-00000100: 0064 017c 009b 0064 027c 029b 009d 047c  .d.|...d.|.....|
-00000110: 0164 0364 0464 059c 0367 0164 069c 0253  .d.d.d...g.d...S
-00000120: 0029 077a 2768 656c 7065 7220 746f 2067  .).z'helper to g
-00000130: 656e 6572 6174 6520 6120 7765 6266 696e  enerate a webfin
-00000140: 6765 7220 7265 7370 6f6e 7365 7a05 6163  ger responsez.ac
-00000150: 6374 3afa 0140 da04 7365 6c66 7a19 6170  ct:..@..selfz.ap
-00000160: 706c 6963 6174 696f 6e2f 6163 7469 7669  plication/activi
-00000170: 7479 2b6a 736f 6e29 03da 0468 7265 66da  ty+json)...href.
-00000180: 0372 656c da04 7479 7065 2902 da07 7375  .rel..type)...su
-00000190: 626a 6563 74da 056c 696e 6b73 a900 2903  bject..links..).
-000001a0: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-000001b0: 1100 0000 7211 0000 00fa 4a2f 776f 6f64  ....r.....J/wood
-000001c0: 7065 636b 6572 2f73 7263 2f63 6f64 6562  pecker/src/codeb
-000001d0: 6572 672e 6f72 672f 626f 7669 6e65 2f62  erg.org/bovine/b
-000001e0: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
-000001f0: 696e 652f 7574 696c 732f 5f5f 696e 6974  ine/utils/__init
-00000200: 5f5f 2e70 79da 1777 6562 6669 6e67 6572  __.py..webfinger
-00000210: 5f72 6573 706f 6e73 655f 6a73 6f6e 0500  _response_json..
-00000220: 0000 730e 0000 000e 0302 0302 0102 0104  ..s.............
-00000230: fd02 ff06 fe72 1300 0000 da07 6163 636f  .....r......acco
-00000240: 756e 7463 0100 0000 0000 0000 0000 0000  untc............
-00000250: 0100 0000 0500 0000 4300 0000 7338 0000  ........C...s8..
-00000260: 007c 0064 0119 0064 026b 0272 0c7c 0064  .|.d...d.k.r.|.d
-00000270: 0364 0485 0219 007d 0064 027c 0076 0072  .d.....}.d.|.v.r
-00000280: 1874 007c 00a0 0164 0264 03a1 0283 0153  .t.|...d.d.....S
-00000290: 007c 0064 0466 0253 0029 057a 2a53 706c  .|.d.f.S.).z*Spl
-000002a0: 6974 7320 6665 6469 7665 7273 6520 6861  its fediverse ha
-000002b0: 6e64 6c65 2069 6e20 6e61 6d65 2061 6e64  ndle in name and
-000002c0: 2064 6f6d 6169 6e72 0100 0000 720a 0000   domainr....r...
-000002d0: 00e9 0100 0000 4e29 02da 0574 7570 6c65  ......N)...tuple
-000002e0: da05 7370 6c69 7429 0172 1400 0000 7211  ..split).r....r.
-000002f0: 0000 0072 1100 0000 7212 0000 00da 1670  ...r....r......p
-00000300: 6172 7365 5f66 6564 6976 6572 7365 5f68  arse_fediverse_h
-00000310: 616e 646c 6513 0000 0073 0a00 0000 0c02  andle....s......
-00000320: 0c01 0802 1001 0801 7218 0000 0063 0000  ........r....c..
-00000330: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00000340: 0000 4300 0000 7320 0000 0074 006a 0174  ..C...s ...t.j.t
-00000350: 026a 0364 018d 016a 0464 0264 0064 038d  .j.d...j.d.d.d..
-00000360: 02a0 05a1 0064 0417 0053 0029 054e 2901  .....d...S.).N).
-00000370: da02 747a 7201 0000 0029 02da 0b6d 6963  ..tzr....)...mic
-00000380: 726f 7365 636f 6e64 da06 747a 696e 666f  rosecond..tzinfo
-00000390: da01 5a29 0672 0200 0000 da03 6e6f 7772  ..Z).r......nowr
-000003a0: 0300 0000 da03 7574 63da 0772 6570 6c61  ......utc..repla
-000003b0: 6365 da09 6973 6f66 6f72 6d61 7472 1100  ce..isoformatr..
-000003c0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
-000003d0: 00da 0d6e 6f77 5f69 736f 666f 726d 6174  ...now_isoformat
-000003e0: 1d00 0000 7308 0000 001a 0202 0102 ff02  ....s...........
-000003f0: ff72 2100 0000 4e29 0a72 0200 0000 7203  .r!...N).r....r.
-00000400: 0000 00da 0674 7970 696e 6772 0400 0000  .....typingr....
-00000410: 7205 0000 00da 0373 7472 da04 6469 6374  r......str..dict
-00000420: 7213 0000 0072 1800 0000 7221 0000 0072  r....r....r!...r
-00000430: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00000440: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000450: 0073 0a00 0000 1000 1001 1a03 1e0e 120a  .s..............
+00000050: 6505 6404 6505 6405 6506 6606 6406 6407  e.d.e.d.e.f.d.d.
+00000060: 8404 5a07 6403 6505 6405 6504 6505 6503  ..Z.d.e.d.e.e.e.
+00000070: 6505 1900 6602 1900 6604 6408 6409 8404  e...f...f.d.d...
+00000080: 5a08 6405 6505 6602 640a 640b 8404 5a09  Z.d.e.f.d.d...Z.
+00000090: 640c 5300 290d e900 0000 0029 02da 0864  d.S.)......)...d
+000000a0: 6174 6574 696d 65da 0874 696d 657a 6f6e  atetime..timezon
+000000b0: 6529 02da 084f 7074 696f 6e61 6cda 0554  e)...Optional..T
+000000c0: 7570 6c65 da07 6163 636f 756e 74da 0375  uple..account..u
+000000d0: 726c da06 7265 7475 726e 6302 0000 0000  rl..returnc.....
+000000e0: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+000000f0: 0000 0073 1400 0000 7c00 7c01 6401 6402  ...s....|.|.d.d.
+00000100: 6403 9c03 6701 6404 9c02 5300 2905 7a27  d...g.d...S.).z'
+00000110: 6865 6c70 6572 2074 6f20 6765 6e65 7261  helper to genera
+00000120: 7465 2061 2077 6562 6669 6e67 6572 2072  te a webfinger r
+00000130: 6573 706f 6e73 65da 0473 656c 667a 1961  esponse..selfz.a
+00000140: 7070 6c69 6361 7469 6f6e 2f61 6374 6976  pplication/activ
+00000150: 6974 792b 6a73 6f6e 2903 da04 6872 6566  ity+json)...href
+00000160: da03 7265 6cda 0474 7970 6529 02da 0773  ..rel..type)...s
+00000170: 7562 6a65 6374 da05 6c69 6e6b 73a9 0029  ubject..links..)
+00000180: 0272 0600 0000 7207 0000 0072 0f00 0000  .r....r....r....
+00000190: 720f 0000 00fa 4a2f 776f 6f64 7065 636b  r.....J/woodpeck
+000001a0: 6572 2f73 7263 2f63 6f64 6562 6572 672e  er/src/codeberg.
+000001b0: 6f72 672f 626f 7669 6e65 2f62 6f76 696e  org/bovine/bovin
+000001c0: 652f 626f 7669 6e65 2f62 6f76 696e 652f  e/bovine/bovine/
+000001d0: 7574 696c 732f 5f5f 696e 6974 5f5f 2e70  utils/__init__.p
+000001e0: 79da 1777 6562 6669 6e67 6572 5f72 6573  y..webfinger_res
+000001f0: 706f 6e73 655f 6a73 6f6e 0500 0000 730e  ponse_json....s.
+00000200: 0000 0002 0302 0302 0102 0104 fd02 ff06  ................
+00000210: fe72 1100 0000 6301 0000 0000 0000 0000  .r....c.........
+00000220: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
+00000230: 3800 0000 7c00 6401 1900 6402 6b02 720c  8...|.d...d.k.r.
+00000240: 7c00 6403 6404 8502 1900 7d00 6402 7c00  |.d.d.....}.d.|.
+00000250: 7600 7218 7400 7c00 a001 6402 6403 a102  v.r.t.|...d.d...
+00000260: 8301 5300 7c00 6404 6602 5300 2905 7a2a  ..S.|.d.f.S.).z*
+00000270: 5370 6c69 7473 2066 6564 6976 6572 7365  Splits fediverse
+00000280: 2068 616e 646c 6520 696e 206e 616d 6520   handle in name 
+00000290: 616e 6420 646f 6d61 696e 7201 0000 00fa  and domainr.....
+000002a0: 0140 e901 0000 004e 2902 da05 7475 706c  .@.....N)...tupl
+000002b0: 65da 0573 706c 6974 2901 7206 0000 0072  e..split).r....r
+000002c0: 0f00 0000 720f 0000 0072 1000 0000 da16  ....r....r......
+000002d0: 7061 7273 655f 6665 6469 7665 7273 655f  parse_fediverse_
+000002e0: 6861 6e64 6c65 1300 0000 730a 0000 000c  handle....s.....
+000002f0: 020c 0108 0210 0108 0172 1600 0000 6300  .........r....c.
+00000300: 0000 0000 0000 0000 0000 0000 0000 0004  ................
+00000310: 0000 0043 0000 0073 2000 0000 7400 6a01  ...C...s ...t.j.
+00000320: 7402 6a03 6401 8d01 6a04 6402 6403 6404  t.j.d...j.d.d.d.
+00000330: 8d02 a005 a100 6405 1700 5300 2906 7a5f  ......d...S.).z_
+00000340: 5265 7475 726e 7320 6e6f 7720 696e 2049  Returns now in I
+00000350: 736f 666f 726d 6174 2c20 652e 672e 2022  soformat, e.g. "
+00000360: 3230 3233 2d30 352d 3331 5431 383a 3131  2023-05-31T18:11
+00000370: 3a33 355a 222c 2074 6f20 6265 2075 7365  :35Z", to be use
+00000380: 6420 6173 2074 6865 2076 616c 7565 0a20  d as the value. 
+00000390: 2020 206f 6620 7075 626c 6973 6865 6429     of published)
+000003a0: 01da 0274 7a72 0100 0000 4e29 02da 0b6d  ...tzr....N)...m
+000003b0: 6963 726f 7365 636f 6e64 da06 747a 696e  icrosecond..tzin
+000003c0: 666f da01 5a29 0672 0200 0000 da03 6e6f  fo..Z).r......no
+000003d0: 7772 0300 0000 da03 7574 63da 0772 6570  wr......utc..rep
+000003e0: 6c61 6365 da09 6973 6f66 6f72 6d61 7472  lace..isoformatr
+000003f0: 0f00 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
+00000400: 0000 00da 0d6e 6f77 5f69 736f 666f 726d  .....now_isoform
+00000410: 6174 1d00 0000 7308 0000 001a 0402 0102  at....s.........
+00000420: ff02 ff72 1f00 0000 4e29 0a72 0200 0000  ...r....N).r....
+00000430: 7203 0000 00da 0674 7970 696e 6772 0400  r......typingr..
+00000440: 0000 7205 0000 00da 0373 7472 da04 6469  ..r......str..di
+00000450: 6374 7211 0000 0072 1600 0000 721f 0000  ctr....r....r...
+00000460: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00000470: 7210 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000480: 0000 0073 0a00 0000 1000 1001 1603 1e0e  ...s............
+00000490: 120a                                     ..
```

### Comparing `bovine-0.2.5/bovine/utils/__pycache__/date.cpython-310.pyc` & `bovine-0.2.6/bovine/utils/__pycache__/date.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 519 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 0702 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 0702 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d00 5a00 6d01 5a01 6d02 5a02  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6505 6602 6404 6405 8404 5a06 6406 6505  e.f.d.d...Z.d.e.
 00000060: 6403 6500 6604 6407 6408 8404 5a07 640f  d.e.f.d.d...Z.d.
 00000070: 640a 6500 640b 6508 6403 6509 6606 640c  d.e.d.e.d.e.f.d.
```

### Comparing `bovine-0.2.5/bovine/utils/__pycache__/pyld_requests.cpython-310.pyc` & `bovine-0.2.6/bovine/utils/__pycache__/pyld_requests.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 4736 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 8012 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 8012 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 6d04 5a05 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6401 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100 6408  m.Z.m.Z.m.Z...d.
 00000070: 6406 6407 8401 5a0c 6402 5300 2909 6178  d.d...Z.d.S.).ax
```

### Comparing `bovine-0.2.5/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 761 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 f902 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 f902 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d06  ..m.Z...d.d.l.m.
 00000050: 5a06 6d07 5a07 6d08 5a08 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100  l.m.Z.m.Z.m.Z...
 00000070: 640c 6406 6407 8404 5a0d 640c 6408 6409  d.d.d...Z.d.d.d.
```

### Comparing `bovine-0.2.5/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 c401 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 c401 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
 00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
 00000070: 1670 6172 7365 5f66 6564 6976 6572 7365  .parse_fediverse
```

### Comparing `bovine-0.2.5/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 368 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 7001 0000  o.......5bsdp...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 7201 0000  o.........|dr...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6404 6405 8400 5a0a 6406 6407 8400 5a0b  d.d...Z.d.d...Z.
 00000070: 6401 5300 2908 e900 0000 004e e901 0000  d.S.)......N....
 00000080: 0029 02da 0d6e 6f77 5f69 736f 666f 726d  .)...now_isoform
 00000090: 6174 da17 7765 6266 696e 6765 725f 7265  at..webfinger_re
 000000a0: 7370 6f6e 7365 5f6a 736f 6e63 0000 0000  sponse_jsonc....
 000000b0: 0000 0000 0000 0000 0500 0000 0700 0000  ................
-000000c0: 4300 0000 7300 0100 0074 0064 0164 0264  C...s....t.d.d.d
-000000d0: 0383 037d 0064 047d 017c 017c 0076 007d  ...}.d.}.|.|.v.}
-000000e0: 027c 0273 3e74 01a0 0264 057c 0266 0164  .|.s>t...d.|.f.d
-000000f0: 067c 017c 0066 02a1 0474 01a0 037c 01a1  .|.|.f...t...|..
-00000100: 0164 0774 04a0 05a1 0076 0073 2774 01a0  .d.t.....v.s't..
-00000110: 067c 00a1 0172 2c74 01a0 037c 00a1 016e  .|...r,t...|...n
-00000120: 0164 0764 089c 0216 007d 0364 0964 0a7c  .d.d.....}.d.d.|
-00000130: 0369 0116 007d 0474 0774 01a0 087c 04a1  .i...}.t.t...|..
-00000140: 0183 0182 0164 0004 007d 017d 0264 0b7d  .....d...}.}.d.}
-00000150: 017c 017c 0076 007d 027c 0273 7a74 01a0  .|.|.v.}.|.szt..
-00000160: 0264 057c 0266 0164 067c 017c 0066 02a1  .d.|.f.d.|.|.f..
-00000170: 0474 01a0 037c 01a1 0164 0774 04a0 05a1  .t...|...d.t....
-00000180: 0076 0073 6374 01a0 067c 00a1 0172 6874  .v.sct...|...rht
-00000190: 01a0 037c 00a1 016e 0164 0764 089c 0216  ...|...n.d.d....
-000001a0: 007d 0364 0964 0a7c 0369 0116 007d 0474  .}.d.d.|.i...}.t
-000001b0: 0774 01a0 087c 04a1 0183 0182 0164 0004  .t...|.......d..
-000001c0: 007d 017d 0264 0053 0029 0c4e da04 6e61  .}.}.d.S.).N..na
-000001d0: 6d65 da03 7572 6cda 0664 6f6d 6169 6eda  me..url..domain.
-000001e0: 0773 7562 6a65 6374 2901 da02 696e 2901  .subject)...in).
-000001f0: 7a12 2528 7079 3129 7320 696e 2025 2870  z.%(py1)s in %(p
-00000200: 7933 2973 da08 7265 7370 6f6e 7365 2902  y3)s..response).
-00000210: da03 7079 31da 0370 7933 7a0e 6173 7365  ..py1..py3z.asse
-00000220: 7274 2025 2870 7935 2973 da03 7079 35da  rt %(py5)s..py5.
-00000230: 056c 696e 6b73 2909 7204 0000 00da 0a40  .links).r......@
-00000240: 7079 7465 7374 5f61 72da 115f 6361 6c6c  pytest_ar.._call
-00000250: 5f72 6570 7263 6f6d 7061 7265 da09 5f73  _reprcompare.._s
-00000260: 6166 6572 6570 72da 0c40 7079 5f62 7569  aferepr..@py_bui
-00000270: 6c74 696e 73da 066c 6f63 616c 73da 185f  ltins..locals.._
-00000280: 7368 6f75 6c64 5f72 6570 725f 676c 6f62  should_repr_glob
-00000290: 616c 5f6e 616d 65da 0e41 7373 6572 7469  al_name..Asserti
-000002a0: 6f6e 4572 726f 72da 135f 666f 726d 6174  onError.._format
-000002b0: 5f65 7870 6c61 6e61 7469 6f6e 2905 720a  _explanation).r.
-000002c0: 0000 00da 0b40 7079 5f61 7373 6572 7430  .....@py_assert0
-000002d0: da0b 4070 795f 6173 7365 7274 32da 0b40  ..@py_assert2..@
-000002e0: 7079 5f66 6f72 6d61 7434 da0b 4070 795f  py_format4..@py_
-000002f0: 666f 726d 6174 36a9 0072 1b00 0000 fa50  format6..r.....P
-00000300: 2f77 6f6f 6470 6563 6b65 722f 7372 632f  /woodpecker/src/
-00000310: 636f 6465 6265 7267 2e6f 7267 2f62 6f76  codeberg.org/bov
-00000320: 696e 652f 626f 7669 6e65 2f62 6f76 696e  ine/bovine/bovin
-00000330: 652f 626f 7669 6e65 2f75 7469 6c73 2f74  e/bovine/utils/t
-00000340: 6573 745f 7765 6266 696e 6765 722e 7079  est_webfinger.py
-00000350: da0e 7465 7374 5f77 6562 6669 6e67 6572  ..test_webfinger
-00000360: 0600 0000 7306 0000 000c 0178 027c 0172  ....s......x.|.r
-00000370: 1d00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000380: 0005 0000 0008 0000 0043 0000 0073 a200  .........C...s..
-00000390: 0000 7400 8300 7d00 7401 6a02 7d01 6401  ..t...}.t.j.}.d.
-000003a0: 7d02 7c01 7c02 7c00 8302 7d03 7c03 7349  }.|.|.|...}.|.sI
-000003b0: 6402 6403 7403 a004 a100 7600 731b 7405  d.d.t.....v.s.t.
-000003c0: a006 7401 a101 7220 7405 a007 7401 a101  ..t...r t...t...
-000003d0: 6e01 6403 7405 a007 7c01 a101 7405 a007  n.d.t...|...t...
-000003e0: 7c02 a101 6404 7403 a004 a100 7600 7334  |...d.t.....v.s4
-000003f0: 7405 a006 7c00 a101 7239 7405 a007 7c00  t...|...r9t...|.
-00000400: a101 6e01 6404 7405 a007 7c03 a101 6405  ..n.d.t...|...d.
-00000410: 9c05 1600 7d04 7408 7405 a009 7c04 a101  ....}.t.t...|...
-00000420: 8301 8201 6400 0400 7d01 0400 7d02 7d03  ....d...}...}.}.
-00000430: 6400 5300 2906 4e7a 265e 5c64 7b34 7d2d  d.S.).Nz&^\d{4}-
-00000440: 5c64 7b32 7d2d 5c64 7b32 7d54 5c64 7b32  \d{2}-\d{2}T\d{2
-00000450: 7d3a 5c64 7b32 7d3a 5c64 7b32 7d5a 247a  }:\d{2}:\d{2}Z$z
-00000460: 5061 7373 6572 7420 2528 7079 3729 730a  Passert %(py7)s.
-00000470: 7b25 2870 7937 2973 203d 2025 2870 7932  {%(py7)s = %(py2
-00000480: 2973 0a7b 2528 7079 3229 7320 3d20 2528  )s.{%(py2)s = %(
-00000490: 7079 3029 732e 6d61 7463 680a 7d28 2528  py0)s.match.}(%(
-000004a0: 7079 3429 732c 2025 2870 7935 2973 290a  py4)s, %(py5)s).
-000004b0: 7dda 0272 65da 0672 6573 756c 7429 05da  }..re..result)..
-000004c0: 0370 7930 da03 7079 32da 0370 7934 720d  .py0..py2..py4r.
-000004d0: 0000 00da 0370 7937 290a 7203 0000 0072  .....py7).r....r
-000004e0: 1e00 0000 da05 6d61 7463 6872 1200 0000  ......matchr....
-000004f0: 7213 0000 0072 0f00 0000 7214 0000 0072  r....r....r....r
-00000500: 1100 0000 7215 0000 0072 1600 0000 2905  ....r....r....).
-00000510: 721f 0000 00da 0b40 7079 5f61 7373 6572  r......@py_asser
-00000520: 7431 da0b 4070 795f 6173 7365 7274 33da  t1..@py_assert3.
-00000530: 0b40 7079 5f61 7373 6572 7436 da0b 4070  .@py_assert6..@p
-00000540: 795f 666f 726d 6174 3872 1b00 0000 721b  y_format8r....r.
-00000550: 0000 0072 1c00 0000 da12 7465 7374 5f6e  ...r......test_n
-00000560: 6f77 5f69 736f 666f 726d 6174 0d00 0000  ow_isoformat....
-00000570: 7350 0000 0006 0102 0102 031a fd04 0306  sP..............
-00000580: fd02 0302 fd02 0304 fd02 0302 fd04 0304  ................
-00000590: fd02 0302 fd02 0302 fd02 0302 fd02 0304  ................
-000005a0: fd04 0306 fd02 0302 fd02 0304 fd02 0302  ................
-000005b0: fd04 0304 fd02 0302 fd02 030c fd02 0302  ................
-000005c0: fd02 0314 fd72 2900 0000 290c da08 6275  .....r)...)...bu
-000005d0: 696c 7469 6e73 7212 0000 00da 195f 7079  iltinsr......_py
-000005e0: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
-000005f0: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
-00000600: 6eda 0772 6577 7269 7465 720f 0000 0072  n..rewriter....r
-00000610: 1e00 0000 da00 7203 0000 0072 0400 0000  ......r....r....
-00000620: 721d 0000 0072 2900 0000 721b 0000 0072  r....r)...r....r
-00000630: 1b00 0000 721b 0000 0072 1c00 0000 da08  ....r....r......
-00000640: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
-00000650: 0022 0010 0208 030c 07                   .".......
+000000c0: 4300 0000 73fe 0000 0074 0064 0164 0283  C...s....t.d.d..
+000000d0: 027d 0064 037d 017c 017c 0076 007d 027c  .}.d.}.|.|.v.}.|
+000000e0: 0273 3d74 01a0 0264 047c 0266 0164 057c  .s=t...d.|.f.d.|
+000000f0: 017c 0066 02a1 0474 01a0 037c 01a1 0164  .|.f...t...|...d
+00000100: 0674 04a0 05a1 0076 0073 2674 01a0 067c  .t.....v.s&t...|
+00000110: 00a1 0172 2b74 01a0 037c 00a1 016e 0164  ...r+t...|...n.d
+00000120: 0664 079c 0216 007d 0364 0864 097c 0369  .d.....}.d.d.|.i
+00000130: 0116 007d 0474 0774 01a0 087c 04a1 0183  ...}.t.t...|....
+00000140: 0182 0164 0004 007d 017d 0264 0a7d 017c  ...d...}.}.d.}.|
+00000150: 017c 0076 007d 027c 0273 7974 01a0 0264  .|.v.}.|.syt...d
+00000160: 047c 0266 0164 057c 017c 0066 02a1 0474  .|.f.d.|.|.f...t
+00000170: 01a0 037c 01a1 0164 0674 04a0 05a1 0076  ...|...d.t.....v
+00000180: 0073 6274 01a0 067c 00a1 0172 6774 01a0  .sbt...|...rgt..
+00000190: 037c 00a1 016e 0164 0664 079c 0216 007d  .|...n.d.d.....}
+000001a0: 0364 0864 097c 0369 0116 007d 0474 0774  .d.d.|.i...}.t.t
+000001b0: 01a0 087c 04a1 0183 0182 0164 0004 007d  ...|.......d...}
+000001c0: 017d 0264 0053 0029 0b4e 7a10 6163 6374  .}.d.S.).Nz.acct
+000001d0: 3a6e 616d 6540 646f 6d61 696e da03 7572  :name@domain..ur
+000001e0: 6cda 0773 7562 6a65 6374 2901 da02 696e  l..subject)...in
+000001f0: 2901 7a12 2528 7079 3129 7320 696e 2025  ).z.%(py1)s in %
+00000200: 2870 7933 2973 da08 7265 7370 6f6e 7365  (py3)s..response
+00000210: 2902 da03 7079 31da 0370 7933 7a0e 6173  )...py1..py3z.as
+00000220: 7365 7274 2025 2870 7935 2973 da03 7079  sert %(py5)s..py
+00000230: 35da 056c 696e 6b73 2909 7204 0000 00da  5..links).r.....
+00000240: 0a40 7079 7465 7374 5f61 72da 115f 6361  .@pytest_ar.._ca
+00000250: 6c6c 5f72 6570 7263 6f6d 7061 7265 da09  ll_reprcompare..
+00000260: 5f73 6166 6572 6570 72da 0c40 7079 5f62  _saferepr..@py_b
+00000270: 7569 6c74 696e 73da 066c 6f63 616c 73da  uiltins..locals.
+00000280: 185f 7368 6f75 6c64 5f72 6570 725f 676c  ._should_repr_gl
+00000290: 6f62 616c 5f6e 616d 65da 0e41 7373 6572  obal_name..Asser
+000002a0: 7469 6f6e 4572 726f 72da 135f 666f 726d  tionError.._form
+000002b0: 6174 5f65 7870 6c61 6e61 7469 6f6e 2905  at_explanation).
+000002c0: 7208 0000 00da 0b40 7079 5f61 7373 6572  r......@py_asser
+000002d0: 7430 da0b 4070 795f 6173 7365 7274 32da  t0..@py_assert2.
+000002e0: 0b40 7079 5f66 6f72 6d61 7434 da0b 4070  .@py_format4..@p
+000002f0: 795f 666f 726d 6174 36a9 0072 1900 0000  y_format6..r....
+00000300: fa50 2f77 6f6f 6470 6563 6b65 722f 7372  .P/woodpecker/sr
+00000310: 632f 636f 6465 6265 7267 2e6f 7267 2f62  c/codeberg.org/b
+00000320: 6f76 696e 652f 626f 7669 6e65 2f62 6f76  ovine/bovine/bov
+00000330: 696e 652f 626f 7669 6e65 2f75 7469 6c73  ine/bovine/utils
+00000340: 2f74 6573 745f 7765 6266 696e 6765 722e  /test_webfinger.
+00000350: 7079 da0e 7465 7374 5f77 6562 6669 6e67  py..test_webfing
+00000360: 6572 0600 0000 7306 0000 000a 0178 027c  er....s......x.|
+00000370: 0172 1b00 0000 6300 0000 0000 0000 0000  .r....c.........
+00000380: 0000 0005 0000 0008 0000 0043 0000 0073  ...........C...s
+00000390: a200 0000 7400 8300 7d00 7401 6a02 7d01  ....t...}.t.j.}.
+000003a0: 6401 7d02 7c01 7c02 7c00 8302 7d03 7c03  d.}.|.|.|...}.|.
+000003b0: 7349 6402 6403 7403 a004 a100 7600 731b  sId.d.t.....v.s.
+000003c0: 7405 a006 7401 a101 7220 7405 a007 7401  t...t...r t...t.
+000003d0: a101 6e01 6403 7405 a007 7c01 a101 7405  ..n.d.t...|...t.
+000003e0: a007 7c02 a101 6404 7403 a004 a100 7600  ..|...d.t.....v.
+000003f0: 7334 7405 a006 7c00 a101 7239 7405 a007  s4t...|...r9t...
+00000400: 7c00 a101 6e01 6404 7405 a007 7c03 a101  |...n.d.t...|...
+00000410: 6405 9c05 1600 7d04 7408 7405 a009 7c04  d.....}.t.t...|.
+00000420: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
+00000430: 7d03 6400 5300 2906 4e7a 265e 5c64 7b34  }.d.S.).Nz&^\d{4
+00000440: 7d2d 5c64 7b32 7d2d 5c64 7b32 7d54 5c64  }-\d{2}-\d{2}T\d
+00000450: 7b32 7d3a 5c64 7b32 7d3a 5c64 7b32 7d5a  {2}:\d{2}:\d{2}Z
+00000460: 247a 5061 7373 6572 7420 2528 7079 3729  $zPassert %(py7)
+00000470: 730a 7b25 2870 7937 2973 203d 2025 2870  s.{%(py7)s = %(p
+00000480: 7932 2973 0a7b 2528 7079 3229 7320 3d20  y2)s.{%(py2)s = 
+00000490: 2528 7079 3029 732e 6d61 7463 680a 7d28  %(py0)s.match.}(
+000004a0: 2528 7079 3429 732c 2025 2870 7935 2973  %(py4)s, %(py5)s
+000004b0: 290a 7dda 0272 65da 0672 6573 756c 7429  ).}..re..result)
+000004c0: 05da 0370 7930 da03 7079 32da 0370 7934  ...py0..py2..py4
+000004d0: 720b 0000 00da 0370 7937 290a 7203 0000  r......py7).r...
+000004e0: 0072 1c00 0000 da05 6d61 7463 6872 1000  .r......matchr..
+000004f0: 0000 7211 0000 0072 0d00 0000 7212 0000  ..r....r....r...
+00000500: 0072 0f00 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000510: 2905 721d 0000 00da 0b40 7079 5f61 7373  ).r......@py_ass
+00000520: 6572 7431 da0b 4070 795f 6173 7365 7274  ert1..@py_assert
+00000530: 33da 0b40 7079 5f61 7373 6572 7436 da0b  3..@py_assert6..
+00000540: 4070 795f 666f 726d 6174 3872 1900 0000  @py_format8r....
+00000550: 7219 0000 0072 1a00 0000 da12 7465 7374  r....r......test
+00000560: 5f6e 6f77 5f69 736f 666f 726d 6174 0d00  _now_isoformat..
+00000570: 0000 7350 0000 0006 0102 0102 031a fd04  ..sP............
+00000580: 0306 fd02 0302 fd02 0304 fd02 0302 fd04  ................
+00000590: 0304 fd02 0302 fd02 0302 fd02 0302 fd02  ................
+000005a0: 0304 fd04 0306 fd02 0302 fd02 0304 fd02  ................
+000005b0: 0302 fd04 0304 fd02 0302 fd02 030c fd02  ................
+000005c0: 0302 fd02 0314 fd72 2700 0000 290c da08  .......r'...)...
+000005d0: 6275 696c 7469 6e73 7210 0000 00da 195f  builtinsr......_
+000005e0: 7079 7465 7374 2e61 7373 6572 7469 6f6e  pytest.assertion
+000005f0: 2e72 6577 7269 7465 da09 6173 7365 7274  .rewrite..assert
+00000600: 696f 6eda 0772 6577 7269 7465 720d 0000  ion..rewriter...
+00000610: 0072 1c00 0000 da00 7203 0000 0072 0400  .r......r....r..
+00000620: 0000 721b 0000 0072 2700 0000 7219 0000  ..r....r'...r...
+00000630: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000640: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
+00000650: 0000 0022 0010 0208 030c 07              ...".......
```

### Comparing `bovine-0.2.5/bovine/utils/date.py` & `bovine-0.2.6/bovine/utils/date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/utils/msg/__init__.py` & `bovine-0.2.6/bovine/utils/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc` & `bovine-0.2.6/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 1432 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 9805 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 9805 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6405 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6407 6408 8400 5a09 6409  m.Z...d.d...Z.d.
 00000070: 6500 6a0a 640a 650b 640b 650b 6606 640c  e.j.d.e.d.e.f.d.
@@ -105,15 +105,15 @@
 00000680: 086d 656e 7469 6f6e 7372 2500 0000 722a  .mentionsr%...r*
 00000690: 0000 0072 0e00 0000 7219 0000 0072 0f00  ...r....r....r..
 000006a0: 0000 da07 7072 6f63 6573 731b 0000 0073  ....process....s
 000006b0: 2a00 0000 0280 0c01 1401 0a02 0e02 1a01  *...............
 000006c0: 0a02 0202 0cfe 0e04 0602 0601 0201 0401  ................
 000006d0: 0401 06fc 0607 0801 1402 1202 2eeb 722d  ..............r-
 000006e0: 0000 0029 0eda 0761 696f 6874 7470 da06  ...)...aiohttp..
-000006f0: 626f 7669 6e65 7202 0000 00da 0e62 6f76  boviner......bov
+000006f0: 626f 7669 6e65 7202 0000 005a 0e62 6f76  boviner....Z.bov
 00000700: 696e 652e 636c 6965 6e74 7372 0400 0000  ine.clientsr....
 00000710: da0c 626f 7669 6e65 2e75 7469 6c73 7205  ..bovine.utilsr.
 00000720: 0000 00da 0a76 616c 6964 6174 696f 6e72  .....validationr
 00000730: 0700 0000 7210 0000 00da 0d43 6c69 656e  ....r......Clien
 00000740: 7453 6573 7369 6f6e da03 7374 7272 1400  tSession..strr..
 00000750: 0000 722d 0000 0072 0e00 0000 720e 0000  ..r-...r....r...
 00000760: 0072 0e00 0000 720f 0000 00da 083c 6d6f  .r....r......<mo
```

### Comparing `bovine-0.2.5/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.1.pyc` & `bovine-0.2.6/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 599 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 5702 0000  o.......5bsdW...
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 5702 0000  o.........|dW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6412 6405 6406 8404 5a0a 6412 6407 6408  d.d.d...Z.d.d.d.
 00000070: 8404 5a0b 6506 6a0c a00d 6409 640a 640b  ..Z.e.j...d.d.d.
```

### Comparing `bovine-0.2.5/bovine/utils/msg/__pycache__/validation.cpython-310.pyc` & `bovine-0.2.6/bovine/utils/msg/__pycache__/validation.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun May 28 14:16:21 2023 UTC, .py size: 261 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3562 7364 0501 0000  o.......5bsd....
+00000000: 6f0d 0d0a 0000 0000 88d8 7c64 0501 0000  o.........|d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 6500 6401 4200 6602 6402 6403 8404 5a01  e.d.B.f.d.d...Z.
 00000040: 6404 6502 6602 6405 6406 8404 5a03 6401  d.e.f.d.d...Z.d.
 00000050: 5300 2907 da03 746f 734e 6301 0000 0000  S.)...tosNc.....
 00000060: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
 00000070: 0000 0073 1e00 0000 7c00 6400 7500 7206  ...s....|.d.u.r.
```

### Comparing `bovine-0.2.5/bovine/utils/msg/test_validation.py` & `bovine-0.2.6/bovine/utils/msg/test_validation.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/utils/pyld_requests.py` & `bovine-0.2.6/bovine/utils/pyld_requests.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/bovine/utils/test_date.py` & `bovine-0.2.6/bovine/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.5/pyproject.toml` & `bovine-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine"
-version = "0.2.5"
+version = "0.2.6"
 description = "Core functionality of bovine needed to build fediverse applications"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine" }]
 repository = "https://codeberg.org/bovine/bovine"
 documentation = "https://bovine.readthedocs.io/en/latest/"
@@ -18,18 +18,19 @@
 multiformats = "^0.2.1"
 aiodns = "^3.0.0"
 requests-cache = "^0.9.8"
 requests = "^2.30.0"
 pyld = "^2.0.3"
 ptpython = { version = "^3.0.23", optional = true }
 bleach = { version = "^6.0.0", optional = true}
+black = { version = "*", optional= true }
+asyncstdlib = "^3.10.7"
 
 [tool.poetry.extras]
-
-repl = ["ptpython", "bleach"]
+repl = ["ptpython", "bleach", "black"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "^4.0.0"
 behave = "^1.2.6"
```

### Comparing `bovine-0.2.5/PKG-INFO` & `bovine-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: bovine
-Version: 0.2.5
+Version: 0.2.6
 Summary: Core functionality of bovine needed to build fediverse applications
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: repl
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: asyncstdlib (>=3.10.7,<4.0.0)
+Requires-Dist: black ; extra == "repl"
 Requires-Dist: bleach (>=6.0.0,<7.0.0) ; extra == "repl"
 Requires-Dist: cryptography (>=39.0.0,<40.0.0)
 Requires-Dist: multiformats (>=0.2.1,<0.3.0)
 Requires-Dist: ptpython (>=3.0.23,<4.0.0) ; extra == "repl"
 Requires-Dist: pyld (>=2.0.3,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
```

