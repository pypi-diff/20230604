# Comparing `tmp/pkiviewer-0.2.0.tar.gz` & `tmp/pkiviewer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkiviewer-0.2.0.tar", max compression
+gzip compressed data, was "pkiviewer-0.2.1.tar", max compression
```

## Comparing `pkiviewer-0.2.0.tar` & `pkiviewer-0.2.1.tar`

### file list

```diff
@@ -1,105 +1,109 @@
--rw-r--r--   0        0        0    11358 2022-07-25 10:34:48.280297 pkiviewer-0.2.0/LICENSE
--rw-r--r--   0        0        0    10592 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/ReadMe.md
--rw-r--r--   0        0        0     1195 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-16 10:49:58.044884 pkiviewer-0.2.0/src/pkiviewer/__init__.py
--rw-r--r--   0        0        0     4509 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/src/pkiviewer/__main__.py
--rw-r--r--   0        0        0        0 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/src/pkiviewer/asn1/__init__.py
--rw-r--r--   0        0        0      392 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/src/pkiviewer/asn1/decode_tbs_certlist.py
--rw-r--r--   0        0        0      404 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/src/pkiviewer/asn1/load_specification.py
--rw-r--r--   0        0        0     2953 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/src/pkiviewer/asn1/specs/tbs_certlist.asn1
--rw-r--r--   0        0        0     5724 2022-07-29 11:51:39.106470 pkiviewer-0.2.0/src/pkiviewer/config.py
--rw-r--r--   0        0        0      302 2022-07-25 16:44:55.004983 pkiviewer-0.2.0/src/pkiviewer/context.py
--rw-r--r--   0        0        0     4466 2022-07-27 16:58:27.278142 pkiviewer-0.2.0/src/pkiviewer/io.py
--rw-r--r--   0        0        0     2643 2022-07-28 11:41:05.003262 pkiviewer-0.2.0/src/pkiviewer/model/__init__.py
--rw-r--r--   0        0        0     4137 2022-07-28 10:34:26.183864 pkiviewer-0.2.0/src/pkiviewer/model/certificate.py
--rw-r--r--   0        0        0     1155 2022-07-28 10:34:26.063864 pkiviewer-0.2.0/src/pkiviewer/model/common.py
--rw-r--r--   0        0        0     4636 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/src/pkiviewer/model/crl.py
--rw-r--r--   0        0        0     3835 2022-07-28 08:32:57.303096 pkiviewer-0.2.0/src/pkiviewer/model/extension/__init__.py
--rw-r--r--   0        0        0      900 2022-07-27 17:20:06.231276 pkiviewer-0.2.0/src/pkiviewer/model/extension/authority_information_access.py
--rw-r--r--   0        0        0      891 2022-07-24 08:29:19.794164 pkiviewer-0.2.0/src/pkiviewer/model/extension/authority_key_identifier.py
--rw-r--r--   0        0        0      598 2022-07-23 20:50:49.153130 pkiviewer-0.2.0/src/pkiviewer/model/extension/basic_constraints.py
--rw-r--r--   0        0        0     1382 2022-07-28 10:34:25.893864 pkiviewer-0.2.0/src/pkiviewer/model/extension/certificate_policy.py
--rw-r--r--   0        0        0     1409 2022-07-27 17:19:32.372248 pkiviewer-0.2.0/src/pkiviewer/model/extension/crl_distribution_points.py
--rw-r--r--   0        0        0      463 2022-07-24 14:35:33.974700 pkiviewer-0.2.0/src/pkiviewer/model/extension/crl_number.py
--rw-r--r--   0        0        0      520 2022-07-24 14:33:03.554881 pkiviewer-0.2.0/src/pkiviewer/model/extension/delta_crl_indicator.py
--rw-r--r--   0        0        0      628 2022-07-28 10:34:26.343864 pkiviewer-0.2.0/src/pkiviewer/model/extension/extended_key_usage.py
--rw-r--r--   0        0        0     1316 2022-07-27 17:20:41.601873 pkiviewer-0.2.0/src/pkiviewer/model/extension/freshest_crl.py
--rw-r--r--   0        0        0      517 2022-07-23 21:03:40.549742 pkiviewer-0.2.0/src/pkiviewer/model/extension/inhibit_any_policy.py
--rw-r--r--   0        0        0     1101 2022-07-24 09:29:15.280207 pkiviewer-0.2.0/src/pkiviewer/model/extension/issuer_alternative_name.py
--rw-r--r--   0        0        0     1193 2022-07-27 17:20:21.461874 pkiviewer-0.2.0/src/pkiviewer/model/extension/issuing_distribution_point.py
--rw-r--r--   0        0        0     1096 2022-07-23 20:32:00.393262 pkiviewer-0.2.0/src/pkiviewer/model/extension/key_usage.py
--rw-r--r--   0        0        0      757 2022-07-27 17:19:04.956283 pkiviewer-0.2.0/src/pkiviewer/model/extension/name_constraints.py
--rw-r--r--   0        0        0      978 2022-07-28 10:34:26.063864 pkiviewer-0.2.0/src/pkiviewer/model/extension/not_implemented_by_cryptography.py
--rw-r--r--   0        0        0      502 2022-07-26 20:00:42.823155 pkiviewer-0.2.0/src/pkiviewer/model/extension/ocsp_nocheck.py
--rw-r--r--   0        0        0     1425 2022-07-23 21:20:37.285150 pkiviewer-0.2.0/src/pkiviewer/model/extension/precertificate_signed_certificate_timestamps.py
--rw-r--r--   0        0        0      936 2022-07-27 17:00:19.936190 pkiviewer-0.2.0/src/pkiviewer/model/extension/reasons.py
--rw-r--r--   0        0        0     1005 2022-07-26 18:28:07.125831 pkiviewer-0.2.0/src/pkiviewer/model/extension/signed_certificate_timestamps.py
--rw-r--r--   0        0        0     1136 2022-07-24 09:47:09.639232 pkiviewer-0.2.0/src/pkiviewer/model/extension/subject_alternative_name.py
--rw-r--r--   0        0        0      885 2022-07-27 17:19:50.011277 pkiviewer-0.2.0/src/pkiviewer/model/extension/subject_information_access.py
--rw-r--r--   0        0        0      595 2022-07-23 20:29:06.955190 pkiviewer-0.2.0/src/pkiviewer/model/extension/subject_key_identifier.py
--rw-r--r--   0        0        0     1206 2022-07-25 10:31:00.746885 pkiviewer-0.2.0/src/pkiviewer/model/p12.py
--rw-r--r--   0        0        0     1595 2022-07-27 16:58:44.228142 pkiviewer-0.2.0/src/pkiviewer/model/public_key/__init__.py
--rw-r--r--   0        0        0      488 2022-07-28 11:41:10.793262 pkiviewer-0.2.0/src/pkiviewer/model/public_key/dh.py
--rw-r--r--   0        0        0      509 2022-07-28 11:41:14.463262 pkiviewer-0.2.0/src/pkiviewer/model/public_key/dsa.py
--rw-r--r--   0        0        0      569 2022-07-28 11:41:23.043262 pkiviewer-0.2.0/src/pkiviewer/model/public_key/ed25519.py
--rw-r--r--   0        0        0      515 2022-07-28 11:41:20.353262 pkiviewer-0.2.0/src/pkiviewer/model/public_key/ed448.py
--rw-r--r--   0        0        0      928 2022-07-28 11:41:25.923262 pkiviewer-0.2.0/src/pkiviewer/model/public_key/elliptic_curve.py
--rw-r--r--   0        0        0      574 2022-07-28 11:41:28.443262 pkiviewer-0.2.0/src/pkiviewer/model/public_key/rsa.py
--rw-r--r--   0        0        0     1462 2022-07-23 12:37:35.099932 pkiviewer-0.2.0/src/pkiviewer/model/unpack.py
--rw-r--r--   0        0        0    17186 2022-07-29 13:59:58.199663 pkiviewer-0.2.0/src/pkiviewer/oid/__init__.py
--rw-r--r--   0        0        0        0 2022-07-24 07:43:57.467308 pkiviewer-0.2.0/src/pkiviewer/py.typed
--rw-r--r--   0        0        0      781 2022-07-28 11:40:06.346429 pkiviewer-0.2.0/src/pkiviewer/types.py
--rw-r--r--   0        0        0      437 2022-07-27 11:27:38.950145 pkiviewer-0.2.0/src/pkiviewer/utils/__init__.py
--rw-r--r--   0        0        0    10558 2022-07-27 17:31:07.332720 pkiviewer-0.2.0/src/pkiviewer/utils/json_encoder.py
--rw-r--r--   0        0        0      313 2022-07-25 21:15:49.886794 pkiviewer-0.2.0/src/pkiviewer/view/__init__.py
--rw-r--r--   0        0        0      459 2022-07-24 08:12:46.201245 pkiviewer-0.2.0/src/pkiviewer/view/color.py
--rw-r--r--   0        0        0     4959 2022-07-27 17:31:07.052720 pkiviewer-0.2.0/src/pkiviewer/view/console.py
--rw-r--r--   0        0        0        0 2022-07-16 10:31:27.404896 pkiviewer-0.2.0/src/pkiviewer/view/display/__init__.py
--rw-r--r--   0        0        0    15030 2022-07-28 10:34:26.303864 pkiviewer-0.2.0/src/pkiviewer/view/display/certificate.py
--rw-r--r--   0        0        0        0 2022-07-22 18:17:01.996106 pkiviewer-0.2.0/src/pkiviewer/view/display/common.py
--rw-r--r--   0        0        0     6099 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/src/pkiviewer/view/display/crl.py
--rw-r--r--   0        0        0      278 2022-07-25 16:49:10.826792 pkiviewer-0.2.0/src/pkiviewer/view/display/csr.py
--rw-r--r--   0        0        0     4389 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/__init__.py
--rw-r--r--   0        0        0      909 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/authority_information_access.py
--rw-r--r--   0        0        0     1479 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/authority_key_identifier.py
--rw-r--r--   0        0        0      793 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/basic_constraints.py
--rw-r--r--   0        0        0     1622 2022-07-28 10:34:26.343864 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/certificate_policies.py
--rw-r--r--   0        0        0     1731 2022-07-27 17:31:07.142720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/crl_distribution_ponts.py
--rw-r--r--   0        0        0      780 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/crl_number.py
--rw-r--r--   0        0        0      697 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/extended_key_usage.py
--rw-r--r--   0        0        0     1684 2022-07-27 17:31:07.012720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/freshest_crl_display.py
--rw-r--r--   0        0        0     1241 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/header.py
--rw-r--r--   0        0        0      828 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/inhibit_any_policy.py
--rw-r--r--   0        0        0      832 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/issuer_alternative_name.py
--rw-r--r--   0        0        0     1104 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/issuing_distribution_point.py
--rw-r--r--   0        0        0      662 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/key_usage.py
--rw-r--r--   0        0        0      743 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/name_constraints.py
--rw-r--r--   0        0        0      760 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/not_implemented_by_cryptography.py
--rw-r--r--   0        0        0     2397 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/signed_certificate_timestamps.py
--rw-r--r--   0        0        0      891 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/subject_alternative_name.py
--rw-r--r--   0        0        0      846 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/subject_information_access.py
--rw-r--r--   0        0        0      839 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/extension/subject_key_identifier.py
--rw-r--r--   0        0        0     1237 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/display/p12.py
--rw-r--r--   0        0        0        0 2022-07-25 11:06:55.986106 pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/__init__.py
--rw-r--r--   0        0        0     1030 2022-07-28 07:39:55.749086 pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/dh.py
--rw-r--r--   0        0        0     1034 2022-07-28 07:40:03.600962 pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/dsa.py
--rw-r--r--   0        0        0     1061 2022-07-28 07:40:11.510962 pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/ed25519.py
--rw-r--r--   0        0        0     1051 2022-07-28 07:40:07.710962 pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/ed448.py
--rw-r--r--   0        0        0     1326 2022-07-28 07:40:15.680962 pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/elliptic_curve.py
--rw-r--r--   0        0        0     1247 2022-07-28 07:40:21.150962 pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/rsa.py
--rw-r--r--   0        0        0     1679 2022-07-22 17:09:12.905769 pkiviewer-0.2.0/src/pkiviewer/view/formatter.py
--rw-r--r--   0        0        0     1712 2022-07-27 17:31:06.882720 pkiviewer-0.2.0/src/pkiviewer/view/theme.py
--rw-r--r--   0        0        0      976 2022-07-27 14:22:08.640716 pkiviewer-0.2.0/src/pkiviewer/view/visibility.py
--rw-r--r--   0        0        0    13561 2022-07-31 08:42:32.916254 pkiviewer-0.2.0/tests/file/google.crl
--rw-r--r--   0        0        0     6775 2022-07-29 11:51:39.106470 pkiviewer-0.2.0/tests/file/microsoft.pem
--rw-r--r--   0        0        0     1490 2022-07-27 17:29:47.522403 pkiviewer-0.2.0/tests/integration/test_bad_naming_constraints.py
--rw-r--r--   0        0        0      233 2022-07-27 13:18:58.781243 pkiviewer-0.2.0/tests/unit/conftest.py
--rw-r--r--   0        0        0      663 2022-07-29 13:59:58.199663 pkiviewer-0.2.0/tests/unit/test_certificate_pem_read.py
--rw-r--r--   0        0        0      396 2022-07-26 07:55:25.900414 pkiviewer-0.2.0/tests/unit/test_config_has_key.py
--rw-r--r--   0        0        0      591 2022-07-27 17:31:07.162720 pkiviewer-0.2.0/tests/unit/test_formatting.py
--rw-r--r--   0        0        0      241 2022-07-29 11:51:39.106470 pkiviewer-0.2.0/tests/unit/test_general_name.py
--rw-r--r--   0        0        0      364 2022-07-26 09:31:29.746511 pkiviewer-0.2.0/tests/unit/test_maybe.py
--rw-r--r--   0        0        0     2021 2022-07-26 08:10:35.297685 pkiviewer-0.2.0/tests/unit/test_merge_configuration.py
--rw-r--r--   0        0        0     1338 2022-07-27 17:31:07.162720 pkiviewer-0.2.0/tests/unit/test_visibility.py
--rw-r--r--   0        0        0    12063 2022-07-31 08:43:51.316016 pkiviewer-0.2.0/setup.py
--rw-r--r--   0        0        0    11192 2022-07-31 08:43:51.316552 pkiviewer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-10-19 09:36:16.579929 pkiviewer-0.2.1/LICENSE
+-rw-r--r--   0        0        0    10780 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/ReadMe.md
+-rw-r--r--   0        0        0     1784 2023-06-04 10:56:46.070569 pkiviewer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-16 10:49:58.000000 pkiviewer-0.2.1/src/pkiviewer/__init__.py
+-rw-r--r--   0        0        0     4651 2022-10-19 09:36:16.579929 pkiviewer-0.2.1/src/pkiviewer/__main__.py
+-rw-r--r--   0        0        0        0 2022-08-04 14:38:43.000000 pkiviewer-0.2.1/src/pkiviewer/asn1/__init__.py
+-rw-r--r--   0        0        0      392 2022-07-31 08:42:32.000000 pkiviewer-0.2.1/src/pkiviewer/asn1/decode_tbs_certlist.py
+-rw-r--r--   0        0        0      625 2022-10-19 09:36:16.580930 pkiviewer-0.2.1/src/pkiviewer/asn1/load_specification.py
+-rw-r--r--   0        0        0     2953 2022-07-31 08:42:32.000000 pkiviewer-0.2.1/src/pkiviewer/asn1/specs/tbs_certlist.asn1
+-rw-r--r--   0        0        0     5724 2022-10-19 09:36:16.580930 pkiviewer-0.2.1/src/pkiviewer/config.py
+-rw-r--r--   0        0        0      379 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/context.py
+-rw-r--r--   0        0        0     4468 2022-10-19 09:36:16.580930 pkiviewer-0.2.1/src/pkiviewer/io.py
+-rw-r--r--   0        0        0     1935 2023-06-04 10:56:46.070569 pkiviewer-0.2.1/src/pkiviewer/model/__init__.py
+-rw-r--r--   0        0        0     4114 2023-06-04 10:56:46.070569 pkiviewer-0.2.1/src/pkiviewer/model/certificate.py
+-rw-r--r--   0        0        0     1155 2023-06-04 10:56:46.070569 pkiviewer-0.2.1/src/pkiviewer/model/common.py
+-rw-r--r--   0        0        0     4411 2023-06-04 10:56:46.070569 pkiviewer-0.2.1/src/pkiviewer/model/crl.py
+-rw-r--r--   0        0        0     3835 2022-10-19 09:16:54.696843 pkiviewer-0.2.1/src/pkiviewer/model/extension/__init__.py
+-rw-r--r--   0        0        0      922 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/authority_information_access.py
+-rw-r--r--   0        0        0      890 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/authority_key_identifier.py
+-rw-r--r--   0        0        0      622 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/basic_constraints.py
+-rw-r--r--   0        0        0     1407 2023-06-04 10:56:46.070569 pkiviewer-0.2.1/src/pkiviewer/model/extension/certificate_policy.py
+-rw-r--r--   0        0        0     1421 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/crl_distribution_points.py
+-rw-r--r--   0        0        0      475 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/crl_number.py
+-rw-r--r--   0        0        0      532 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/delta_crl_indicator.py
+-rw-r--r--   0        0        0      645 2023-06-04 10:56:46.070569 pkiviewer-0.2.1/src/pkiviewer/model/extension/extended_key_usage.py
+-rw-r--r--   0        0        0     1351 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/freshest_crl.py
+-rw-r--r--   0        0        0      529 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/inhibit_any_policy.py
+-rw-r--r--   0        0        0     1113 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/issuer_alternative_name.py
+-rw-r--r--   0        0        0     1261 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/issuing_distribution_point.py
+-rw-r--r--   0        0        0     1168 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/key_usage.py
+-rw-r--r--   0        0        0      801 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/name_constraints.py
+-rw-r--r--   0        0        0     1016 2023-06-04 10:56:46.070569 pkiviewer-0.2.1/src/pkiviewer/model/extension/not_implemented_by_cryptography.py
+-rw-r--r--   0        0        0      462 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/ocsp_nocheck.py
+-rw-r--r--   0        0        0     1425 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/precertificate_signed_certificate_timestamps.py
+-rw-r--r--   0        0        0      951 2022-10-19 09:36:16.580930 pkiviewer-0.2.1/src/pkiviewer/model/extension/reasons.py
+-rw-r--r--   0        0        0     1005 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/signed_certificate_timestamps.py
+-rw-r--r--   0        0        0     1148 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/subject_alternative_name.py
+-rw-r--r--   0        0        0      907 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/subject_information_access.py
+-rw-r--r--   0        0        0      620 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/extension/subject_key_identifier.py
+-rw-r--r--   0        0        0     1263 2022-10-19 09:36:16.580930 pkiviewer-0.2.1/src/pkiviewer/model/p12.py
+-rw-r--r--   0        0        0     1595 2022-10-19 09:36:16.580930 pkiviewer-0.2.1/src/pkiviewer/model/public_key/__init__.py
+-rw-r--r--   0        0        0      488 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/public_key/dh.py
+-rw-r--r--   0        0        0      509 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/public_key/dsa.py
+-rw-r--r--   0        0        0      569 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/public_key/ed25519.py
+-rw-r--r--   0        0        0      515 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/public_key/ed448.py
+-rw-r--r--   0        0        0      928 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/public_key/elliptic_curve.py
+-rw-r--r--   0        0        0      574 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/model/public_key/rsa.py
+-rw-r--r--   0        0        0     1462 2022-07-23 12:37:35.000000 pkiviewer-0.2.1/src/pkiviewer/model/unpack.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:56:46.071569 pkiviewer-0.2.1/src/pkiviewer/oid/__init__.py
+-rw-r--r--   0        0        0  4556115 2023-06-04 10:56:46.093569 pkiviewer-0.2.1/src/pkiviewer/oid/enterprise-numbers.txt
+-rw-r--r--   0        0        0    18024 2023-06-04 10:56:46.093569 pkiviewer-0.2.1/src/pkiviewer/oid/names.py
+-rw-r--r--   0        0        0     1195 2023-06-04 10:56:46.093569 pkiviewer-0.2.1/src/pkiviewer/oid/pen.py
+-rw-r--r--   0        0        0        0 2022-07-24 07:43:57.000000 pkiviewer-0.2.1/src/pkiviewer/py.typed
+-rw-r--r--   0        0        0     1544 2023-06-04 10:56:46.093569 pkiviewer-0.2.1/src/pkiviewer/types.py
+-rw-r--r--   0        0        0      437 2022-07-27 11:27:38.000000 pkiviewer-0.2.1/src/pkiviewer/utils/__init__.py
+-rw-r--r--   0        0        0      497 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/__init__.py
+-rw-r--r--   0        0        0      546 2022-10-19 09:36:16.580930 pkiviewer-0.2.1/src/pkiviewer/view/color.py
+-rw-r--r--   0        0        0     5605 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/console.py
+-rw-r--r--   0        0        0        0 2022-07-16 10:31:27.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/__init__.py
+-rw-r--r--   0        0        0    14431 2023-06-04 10:56:46.093569 pkiviewer-0.2.1/src/pkiviewer/view/display/certificate.py
+-rw-r--r--   0        0        0      841 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/common.py
+-rw-r--r--   0        0        0     5998 2023-06-04 10:56:46.093569 pkiviewer-0.2.1/src/pkiviewer/view/display/crl.py
+-rw-r--r--   0        0        0      222 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/csr.py
+-rw-r--r--   0        0        0     4203 2023-06-04 10:56:46.093569 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/__init__.py
+-rw-r--r--   0        0        0      854 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/authority_information_access.py
+-rw-r--r--   0        0        0     1480 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/authority_key_identifier.py
+-rw-r--r--   0        0        0      729 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/basic_constraints.py
+-rw-r--r--   0        0        0     1564 2023-06-04 10:56:46.093569 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/certificate_policies.py
+-rw-r--r--   0        0        0     1722 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/crl_distribution_ponts.py
+-rw-r--r--   0        0        0      780 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/crl_number.py
+-rw-r--r--   0        0        0      688 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/extended_key_usage.py
+-rw-r--r--   0        0        0     1684 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/freshest_crl_display.py
+-rw-r--r--   0        0        0     1241 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/header.py
+-rw-r--r--   0        0        0      819 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/inhibit_any_policy.py
+-rw-r--r--   0        0        0      823 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/issuer_alternative_name.py
+-rw-r--r--   0        0        0     1104 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/issuing_distribution_point.py
+-rw-r--r--   0        0        0      653 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/key_usage.py
+-rw-r--r--   0        0        0      734 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/name_constraints.py
+-rw-r--r--   0        0        0      760 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/not_implemented_by_cryptography.py
+-rw-r--r--   0        0        0     2323 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/signed_certificate_timestamps.py
+-rw-r--r--   0        0        0      836 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/subject_alternative_name.py
+-rw-r--r--   0        0        0      846 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/subject_information_access.py
+-rw-r--r--   0        0        0      775 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/extension/subject_key_identifier.py
+-rw-r--r--   0        0        0     1639 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/p12.py
+-rw-r--r--   0        0        0        0 2022-07-25 11:06:55.000000 pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/__init__.py
+-rw-r--r--   0        0        0     1030 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/dh.py
+-rw-r--r--   0        0        0     1034 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/dsa.py
+-rw-r--r--   0        0        0     1061 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/ed25519.py
+-rw-r--r--   0        0        0     1051 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/ed448.py
+-rw-r--r--   0        0        0     1326 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/elliptic_curve.py
+-rw-r--r--   0        0        0     1247 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/rsa.py
+-rw-r--r--   0        0        0     1693 2022-10-19 09:36:16.581930 pkiviewer-0.2.1/src/pkiviewer/view/formatter.py
+-rw-r--r--   0        0        0     1712 2022-07-27 17:31:06.000000 pkiviewer-0.2.1/src/pkiviewer/view/theme.py
+-rw-r--r--   0        0        0      976 2022-07-27 14:22:08.000000 pkiviewer-0.2.1/src/pkiviewer/view/visibility.py
+-rw-r--r--   0        0        0    13561 2022-07-31 08:42:32.000000 pkiviewer-0.2.1/tests/file/google.crl
+-rw-r--r--   0        0        0     6774 2022-10-19 09:36:16.582929 pkiviewer-0.2.1/tests/file/microsoft.pem
+-rw-r--r--   0        0        0      267 2022-10-19 09:36:16.582929 pkiviewer-0.2.1/tests/integration/test_asn1tools.py
+-rw-r--r--   0        0        0     1482 2022-10-19 09:36:16.582929 pkiviewer-0.2.1/tests/integration/test_bad_naming_constraints.py
+-rw-r--r--   0        0        0      233 2022-10-19 09:36:16.582929 pkiviewer-0.2.1/tests/unit/conftest.py
+-rw-r--r--   0        0        0      655 2022-10-19 09:36:16.582929 pkiviewer-0.2.1/tests/unit/test_certificate_pem_read.py
+-rw-r--r--   0        0        0      354 2022-10-19 09:36:16.582929 pkiviewer-0.2.1/tests/unit/test_config_has_key.py
+-rw-r--r--   0        0        0      591 2022-10-19 09:36:16.582929 pkiviewer-0.2.1/tests/unit/test_formatting.py
+-rw-r--r--   0        0        0      242 2022-10-19 09:36:16.582929 pkiviewer-0.2.1/tests/unit/test_general_name.py
+-rw-r--r--   0        0        0      364 2022-08-04 15:40:01.000000 pkiviewer-0.2.1/tests/unit/test_maybe.py
+-rw-r--r--   0        0        0     1992 2022-10-19 09:36:16.582929 pkiviewer-0.2.1/tests/unit/test_merge_configuration.py
+-rw-r--r--   0        0        0      623 2023-06-04 10:56:46.093569 pkiviewer-0.2.1/tests/unit/test_oid.py
+-rw-r--r--   0        0        0      191 2023-06-04 10:56:46.093569 pkiviewer-0.2.1/tests/unit/test_pen.py
+-rw-r--r--   0        0        0     1338 2022-10-19 09:36:16.582929 pkiviewer-0.2.1/tests/unit/test_visibility.py
+-rw-r--r--   0        0        0    11619 1970-01-01 00:00:00.000000 pkiviewer-0.2.1/PKG-INFO
```

### Comparing `pkiviewer-0.2.0/LICENSE` & `pkiviewer-0.2.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,7 @@
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
-
```

### Comparing `pkiviewer-0.2.0/ReadMe.md` & `pkiviewer-0.2.1/ReadMe.md`

 * *Files 2% similar despite different names*

```diff
@@ -235,7 +235,11 @@
 ".Data.Extension.PreCertificateSCTs.Value" = "normal"
 
 # Signature Information
 ".Signature" = "normal"                                        # The signature block (alogrithm + value)
 ".Signature.Algorithm" = "normal"                              # The signature algorithm
 ".Signature.Value" = "normal"                                  # The signature value
 ```
+
+## Package Info
+
+![GitHub Workflow Status](https://img.shields.io/github/workflow/status/sffjunkie/pkiviewer/pkiviewer-test) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pkiviewer)
```

### Comparing `pkiviewer-0.2.0/pyproject.toml` & `pkiviewer-0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,82 @@
 [tool.poetry]
 name = "pkiviewer"
-version = "0.2.0"
+version = "0.2.1"
 description = "PKI file viewer"
 authors = ["Simon Kennedy <sffjunkie+code@gmail.com>"]
 license = "Apache-2.0"
 readme = "ReadMe.md"
+homepage = "https://github.com/sffjunkie/pkiviewer"
+repository = "https://github.com/sffjunkie/pkiviewer"
 
 packages = [
     { include = "pkiviewer", from = "src" },
     { include = "pkiviewer/py.typed", from = "src" },
 ]
-include = [
-    { path = "tests", format = "sdist" }
-]
+include = [{ path = "tests", format = "sdist" }]
+
+[tool.poetry.urls]
+"Issue Tracker" = "https://github.com/sffjunkie/pkiviewer/issues"
 
-[project.urls]
-"Homepage" = "https://github.com/sffjunkie/pkiviewer"
-"Bug Tracker" = "https://github.com/sffjunkie/pkiviewer/issues"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.1.2"
+tox = "^3.25.1"
+typing-extensions = "^4.3.0"
+scriv = "^0.16.0"
+pytest-html = "^3.1.1"
+flake8 = "^5.0.4"
+Flake8-pyproject = "^1.1.0.post0"
+pre-commit = "^2.20.0"
+black = "^22.10.0"
+mypy = "^1.3.0"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 cryptography = "^37.0.4"
 rich = "^12.5.1"
 tomli = "^2.0.1"
 click = "^8.1.3"
 asn1tools = "^0.163.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-tox = "^3.25.1"
-typing-extensions = "^4.3.0"
-scriv = "^0.16.0"
-
 [tool.pytest.ini_options]
-pythonpath = [
-    "src"
-]
+pythonpath = ["src"]
 
 [tool.poetry.scripts]
 pkiviewer = 'pkiviewer.__main__:run'
 
 [tool.scriv]
 version = "literal: pyproject.toml: tool.poetry.version"
 format = "md"
 
+[tool.isort]
+profile = "black"
+lines_between_sections = 1
+
+[tool.flake8]
+max-line-length = 88
+exclude = [
+    ".git",
+    "__pycache__",
+    "build",
+    "dist",
+    ".venv",
+    ".ipynb_checkpoints",
+    "poetry.lock",
+]
+per-file-ignores = [
+    "src/pkiviewer/oid/__init__.py:E501",
+    "src/pkiviewer/view/display/extension/__init__.py:E501",
+    "src/pkiviewer/model/extension/__init__.py:E501",
+]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.mypy.overrides]]
 module = [
     'cryptography.*',
     'asn1tools.*',
     'pkiviewer.asn1.json_encoder',
-    'pkiviewer.model.csr'
+    'pkiviewer.model.csr',
 ]
 ignore_errors = true
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/__main__.py` & `pkiviewer-0.2.1/src/pkiviewer/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 import os
 from pathlib import Path
 
 import click
+from cryptography.hazmat.primitives.serialization.pkcs12 import PKCS12KeyAndCertificates
+from cryptography.x509 import CertificateRevocationList, CertificateSigningRequest
+from cryptography.x509.base import Certificate
 
 from pkiviewer.config import config_load
-from pkiviewer.io import load, download_pem, load_p12
-from pkiviewer.model import X509Types
-from pkiviewer.view import rich_init
-from pkiviewer.view.console import print_info
-from pkiviewer.utils import maybe
-from pkiviewer.context import _console, _config  # type: ignore
-
-from cryptography.x509.base import Certificate
+from pkiviewer.context import _console  # type: ignore
+from pkiviewer.io import download_pem, load, load_p12
 from pkiviewer.model.certificate import certiticate_parse
-from pkiviewer.view.display.certificate import (
-    certificate_display,
-    certificate_report_display,
-)
+from pkiviewer.model.crl import certiticate_revocation_list_parse
 
-# from cryptography.x509 import CertificateSigningRequest
 # from pkiviewer.model.csr import certificate_signing_request_parse
-# from pkiviewer.ui.rich.output.csr import certificate_signing_request_display
-
-from cryptography.x509 import CertificateRevocationList
-from pkiviewer.model.crl import certiticate_revocation_list_parse
+from pkiviewer.model.p12 import p12_key_and_certificates_parse
+from pkiviewer.types import X509Types
+from pkiviewer.utils import maybe
+from pkiviewer.view import rich_init
+from pkiviewer.view.console import print_info
+from pkiviewer.view.display.certificate import certificate_display
+from pkiviewer.view.display.common import report_display
 from pkiviewer.view.display.crl import certificate_revocation_list_display
 
-from cryptography.hazmat.primitives.serialization.pkcs12 import PKCS12KeyAndCertificates
-from pkiviewer.model.p12 import p12_key_and_certificates_parse
+# from pkiviewer.view.display.csr import certificate_signing_request_display
 from pkiviewer.view.display.p12 import p12_display
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 __author__ = "Simon Kennedy <sffjunkie+code@gmail.com>"
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("filename", type=click.Path())
@@ -76,68 +71,70 @@
         output_html = str(save_html)
 
     # Initialize rich
     if output_html or output_svg:
         record = True
         rich_init(
             record=record,
-            file=open(os.devnull, "wt"),
+            file=open(os.devnull, "wt", encoding="utf-8"),
             color_system="truecolor",
             width=width,
         )
     else:
         record = False
         rich_init(record=False)
 
-    con = _console.get()
-
     info: list[X509Types]
 
     fname = str(filename)
     lcname = fname.lower()
     if lcname.startswith("https://") or lcname.startswith("http://"):
         info = download_pem(fname)
         if verbose:
             print_info(f"Downloading certificate from {fname}")
     else:
-        p = Path(fname)
-        if p.suffix == ".p12":
-            info = load_p12(p)
+        x509_file_path = Path(fname)
+        if x509_file_path.suffix == ".p12":
+            info = load_p12(x509_file_path)
         else:
-            info = load(p.resolve())
+            info = load(x509_file_path.resolve())
         if verbose:
-            print_info(f"Loading RFC5280 data from {p.resolve()}")
+            print_info(f"Loading RFC5280 data from {x509_file_path.resolve()}")
 
     if info:
         element: X509Types | None
         for element in info:
             if element is None:
                 continue
 
             if isinstance(element, Certificate):
                 cert_info = certiticate_parse(element, fname)
                 certificate_display(cert_info)
-                certificate_report_display(cert_info)
+                report_display(cert_info)
 
             # TODO: Certificate Signing Request
-            # elif isinstance(element, CertificateSigningRequest):
-            #     csr_info = certificate_signing_request_parse(element, fname)
-            #     certificate_signing_request_display(csr_info)
+            elif isinstance(element, CertificateSigningRequest):
+                # csr_info = certificate_signing_request_parse(element, fname)
+                # certificate_signing_request_display(csr_info)
+                # report_display(csr_info)
+                pass
 
-            # TODO: Certificate Revocation List
             elif isinstance(element, CertificateRevocationList):  # type: ignore
                 crl_info = certiticate_revocation_list_parse(element, fname)
                 certificate_revocation_list_display(crl_info)
+                report_display(crl_info)
 
             elif isinstance(element, PKCS12KeyAndCertificates):  # type: ignore
                 p12_info = p12_key_and_certificates_parse(element, fname)
                 p12_display(p12_info)
+                report_display(p12_info)
 
     if record:
         clear = output_svg == ""
+        con = _console.get()
         if output_svg:
             con.save_svg(output_svg, clear=clear)
         if output_html:
             con.save_html(output_html)
 
 
 run()
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/asn1/specs/tbs_certlist.asn1` & `pkiviewer-0.2.1/src/pkiviewer/asn1/specs/tbs_certlist.asn1`

 * *Files identical despite different names*

### Comparing `pkiviewer-0.2.0/src/pkiviewer/config.py` & `pkiviewer-0.2.1/src/pkiviewer/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import cast, Any
+from typing import Any, cast
 
 import tomli
 
 from pkiviewer.context import _config  # type: ignore
-from pkiviewer.types import Configuration, ConfigSection, Visibility
+from pkiviewer.types import ConfigSection, Configuration, Visibility
 
 default_theme: dict[str, str] = {
     "default": "white",
     "error": "red",
     "warning": "yellow",
     "info": "green",
     "key": "blue",
@@ -160,13 +160,13 @@
 def has_key(key_path: str, config: Configuration):
     section = config
     elems = list(reversed(key_path.split(".")))
     try:
         while elem := elems.pop():
             if not isinstance(section, dict) and len(elems) == 0:
                 return False
-            if not elem in section:
+            if elem not in section:
                 return False
 
             section: Any = section[elem]
     except IndexError:
         return True
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/io.py` & `pkiviewer-0.2.1/src/pkiviewer/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-import os
 import io
+import os
 import ssl
 from pathlib import Path
 from urllib.parse import urlparse
-from cryptography.x509.base import Certificate
+
+from cryptography.hazmat.primitives.serialization.pkcs12 import load_pkcs12
 from cryptography.x509 import (
     CertificateRevocationList,
     CertificateSigningRequest,
     load_der_x509_certificate,
     load_der_x509_crl,
     load_der_x509_csr,
     load_pem_x509_certificate,
     load_pem_x509_crl,
     load_pem_x509_csr,
 )
-from cryptography.hazmat.primitives.serialization.pkcs12 import load_pkcs12
+from cryptography.x509.base import Certificate
 from rich.prompt import Prompt
 from rich.text import Text
-from pkiviewer.model import X509Types
+
 from pkiviewer.context import _theme  # type: ignore
+from pkiviewer.types import X509Types
 
 
 def download_pem(uri: str) -> list[X509Types]:
     elems = urlparse(uri, "https")
     cert = ssl.get_server_certificate((elems.netloc, 443))
     if cert:
         return [load_pem_x509_certificate(cert.encode("ascii"))]
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/__init__.py` & `pkiviewer-0.2.1/src/pkiviewer/model/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,26 @@
 from typing import Any, TypedDict
-from cryptography.x509 import (
-    CertificateSigningRequest,
-    Certificate,
-    CertificateRevocationList,
-)
-from cryptography.x509.general_name import GeneralName
+
 from cryptography.x509.extensions import AccessDescription
+from cryptography.x509.general_name import GeneralName
 from cryptography.x509.name import RelativeDistinguishedName
-from cryptography.hazmat.primitives.serialization.pkcs12 import PKCS12KeyAndCertificates
-
-from pkiviewer.oid import OidNames, Oid
 
+from pkiviewer.oid.names import OidNames
 
 GeneralNameInfo = tuple[str, Any]
 
 GeneralNameToShortName: dict[str, str] = {  # type: ignore
     "DNSName": "DNS",
     "UniformResourceIdentifier": "URI",
     "RFC822Name": "email",
     "DirectoryName": "DirectoryName",
     "IPAddress": "IP",
 }
 
 
-X509Types = (
-    Certificate
-    | CertificateRevocationList
-    | CertificateSigningRequest
-    | PKCS12KeyAndCertificates
-)
-
-
-class X509ExtensionTypeInfo(TypedDict):
-    type: str  # NOTE: type required as we can't use isinstance checks on a TypedDict
-
-
-class X509ExtensionInfo(TypedDict):
-    oid: Oid
-    name: str
-    critical: bool
-    info: X509ExtensionTypeInfo
-
-
-class PublicKeyInfo(TypedDict):
-    type: str  # NOTE: type required as we can't use isinstance checks on a TypedDict
-    name: str
-
-
 class DistributionPointInfo(TypedDict):
     names: list[GeneralNameInfo]
     reasons: list[str]
     crl_issuer: list[GeneralNameInfo]
 
 
 def general_name_parse(
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/certificate.py` & `pkiviewer-0.2.1/src/pkiviewer/model/certificate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,91 +1,73 @@
 import datetime
-from typing import TypedDict
 
-import cryptography.x509.name
 import cryptography.exceptions
-
+import cryptography.x509.name
 from cryptography.hazmat.primitives.hashes import SHA256
 from cryptography.x509 import Version
 from cryptography.x509.base import Certificate
 
-from pkiviewer.types import Warning, Error
-from pkiviewer.model import PublicKeyInfo, X509ExtensionInfo
-from pkiviewer.model.public_key import public_key_info
-from pkiviewer.model.common import sort_extensions_by_rfc_section, get_extension_for_oid
+from pkiviewer.context import _config, _console  # type: ignore
+from pkiviewer.model.common import get_extension_for_oid, sort_extensions_by_rfc_section
 from pkiviewer.model.extension import v3_extension_parse
-from pkiviewer.oid import Oid, OidNames
+from pkiviewer.model.public_key import public_key_info
+from pkiviewer.oid.names import Oid, OidNames
+from pkiviewer.types import Error, PublicKeyInfo, Warning, X509ExtensionInfo, X509Info
 from pkiviewer.view.console import print_info
-from pkiviewer.context import _console, _config  # type: ignore
 
 
 def verbose() -> bool:
     c = _config.get()
     return c["output"].get("verbose", False)
 
 
-class CertificateInfo(TypedDict, total=False):
-    filename: str
+class CertificateInfo(X509Info):
     version: Version
     serial_number: int
     signature: bytes
     signature_algorithm_oid: str
     issuer: cryptography.x509.name.Name
     not_valid_before: datetime.datetime
     not_valid_after: datetime.datetime
     subject: cryptography.x509.name.Name
     public_key: PublicKeyInfo | None
     extensions: dict[Oid, X509ExtensionInfo]
-    errors: list[Error]
-    warnings: list[Warning]
     fingerprint: bytes
 
 
 def certiticate_parse(cert: Certificate, filename: str):
-    info: CertificateInfo = {
-        "filename": filename,
-        "version": cert.version,
-        "serial_number": cert.serial_number,
-        "signature": cert.signature,
-        "signature_algorithm_oid": cert.signature_algorithm_oid.dotted_string,
-        "issuer": cert.issuer,
-        "not_valid_before": cert.not_valid_before,
-        "not_valid_after": cert.not_valid_after,
-        "subject": cert.subject,
-        "extensions": {},
-        "errors": [],
-        "warnings": [],
-        "fingerprint": cert.fingerprint(SHA256()),
-    }
+    errors: list[Error] = []
+    warnings: list[Warning] = []
 
     try:
         pk = cert.public_key()
-        info["public_key"] = public_key_info(pk)
+        pk_info = public_key_info(pk)
     except (cryptography.exceptions.UnsupportedAlgorithm, ValueError) as exc:
-        info["public_key"] = None
-        info["errors"].append(
+        pk_info = None
+        errors.append(
             Error(
                 module="cryptography",
                 text=f"Public key decode; {exc}",
             )
         )
 
+    extensions = {}
     if cert.version == Version.v3:
         try:
             se = sort_extensions_by_rfc_section(cert.extensions)
             for item in se:
                 oid = item[2]
                 extension = get_extension_for_oid(cert.extensions, oid)
                 if extension is None:
                     continue
 
                 try:
                     name = OidNames[oid].name
                 except KeyError:
-                    info["warnings"].append(
+                    warnings.append(
                         Warning(
                             module="pkiviewer",
                             text=f"Unknown extension name for oid {oid}, skipping",
                         )
                     )
                     continue
 
@@ -98,24 +80,42 @@
                         extension_info: X509ExtensionInfo = {
                             "oid": oid,
                             "name": name,
                             "critical": extension.critical,
                             "info": func(extension.value),
                         }
 
-                        info["extensions"][oid] = extension_info
-                except KeyError as exc:
+                        extensions[oid] = extension_info
+                except KeyError:
                     if oid in OidNames:
                         name = f"{OidNames[oid].name} (OID:{oid})"
                     else:
                         name = f"OID:{oid}"
-                    info["warnings"].append(
+                    warnings.append(
                         Warning(
                             module="pkiviewer",
                             text=f"Parse function for X.509 extension {name} not found",
                         )
                     )
         except ValueError as exc:
             print(exc)
             _console.get().print_exception()
 
+    info: CertificateInfo = {
+        "type": "certificate",
+        "filename": filename,
+        "version": cert.version,
+        "serial_number": cert.serial_number,
+        "signature": cert.signature,
+        "signature_algorithm_oid": cert.signature_algorithm_oid.dotted_string,
+        "issuer": cert.issuer,
+        "not_valid_before": cert.not_valid_before,
+        "not_valid_after": cert.not_valid_after,
+        "subject": cert.subject,
+        "public_key": pk_info,
+        "extensions": extensions,
+        "errors": errors,
+        "warnings": warnings,
+        "fingerprint": cert.fingerprint(SHA256()),
+    }
+
     return info
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/common.py` & `pkiviewer-0.2.1/src/pkiviewer/model/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 
-from cryptography.x509.extensions import Extensions, ExtensionType, Extension
+from cryptography.x509.extensions import Extension, Extensions, ExtensionType
 
-from pkiviewer.oid import Oid, OidNames
 from pkiviewer.model.extension import v3_extension_parse
+from pkiviewer.oid.names import Oid, OidNames
 
 
 def get_extension_for_oid(
     extensions: Extensions, oid: Oid
 ) -> Extension[ExtensionType] | None:
     for e in extensions:
         if e.oid.dotted_string == oid:
@@ -26,15 +26,15 @@
 
         rfc, s = section[0].split(" ")
         s = rfc + "".join([f"{int(e):02d}" for e in s.split(".")])
         return s
 
     a = [
         (
-            OidNames[ext.oid.dotted_string].defined_in,
+            OidNames[ext.oid.dotted_string].info,
             v3_extension_parse[ext.oid.dotted_string],
             ext.oid.dotted_string,
         )
         for ext in extensions
         if ext.oid.dotted_string in v3_extension_parse
     ]
     result: list[SortedExtensionInfo] = sorted(a, key=_section_to_key)  # type: ignore
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/crl.py` & `pkiviewer-0.2.1/src/pkiviewer/model/crl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 import datetime
-from zoneinfo import ZoneInfo
 from typing import TypedDict
+from zoneinfo import ZoneInfo
 
-from cryptography.x509 import CertificateRevocationList
-from cryptography.hazmat.primitives import hashes
-
-import cryptography.x509.name
 import cryptography.exceptions
-from asn1tools.codecs import generalized_time_to_datetime  # type: ignore
-
-from pkiviewer.model import X509ExtensionInfo
-from pkiviewer.types import Warning, Error
-from pkiviewer.oid import Oid, OidNames
-from pkiviewer.model.extension import v3_extension_parse
-from pkiviewer.context import _console  # type: ignore
+import cryptography.x509.name
+from cryptography.hazmat.primitives import hashes
+from cryptography.x509 import CertificateRevocationList
 
 from pkiviewer.asn1 import decode_tbs_certlist
+from pkiviewer.model.extension import v3_extension_parse
+from pkiviewer.oid.names import Oid, OidNames
+from pkiviewer.types import Error, Warning, X509ExtensionInfo, X509Info
 
 CertificateID = int
 
 X509RevocationDate = tuple[str, datetime.datetime]
 
 
 class X509RevocationInfo(TypedDict):
@@ -31,30 +26,25 @@
 
 
 class RevocationInfo(TypedDict):
     certificate_id: CertificateID
     revocation_date: RevokedAt
 
 
-class CertificateRevocationListInfo(TypedDict):
-    filename: str
+class CertificateRevocationListInfo(X509Info):
     signature: bytes | None
     signature_algorithm: str
     signature_algorithm_oid: str
     signature_hash_algorithm: hashes.HashAlgorithm | None
     issuer: cryptography.x509.name.Name
     last_update: datetime.datetime | None
     next_update: datetime.datetime | None
-    errors: list[Error]
-    warnings: list[Warning]
     fingerprint: bytes | None
     extensions: dict[Oid, X509ExtensionInfo]
     revoked_certificates: list[RevocationInfo]
-    errors: list[Error]
-    warnings: list[Warning]
     fingerprint: bytes | None
 
 
 def revocation_date_parse(x509_dt: X509RevocationDate) -> datetime.datetime:
     if x509_dt[0] == "utcTime":
         return x509_dt[1].replace(tzinfo=ZoneInfo("UTC"))
     else:
@@ -72,25 +62,27 @@
             "revocation_date": revocation_date_parse(dt),
         }
         info.append(rinfo)
     return info
 
 
 def certiticate_revocation_list_parse(crl: CertificateRevocationList, filename: str):
-    rl = decode_tbs_certlist.decode_crl(crl.tbs_certlist_bytes)  # type: ignore
-    revoked_certificates = revocation_info_parse(rl["revokedCertificates"])  # type: ignore
+    errors: list[Error] = []
+    warnings: list[Warning] = []
+
+    rl = decode_tbs_certlist.decode_crl(crl.tbs_certlist_bytes)
+    revoked_certificates = rl["revokedCertificates"]
+    revoked_certificates = revocation_info_parse(revoked_certificates)
 
     if crl.signature_hash_algorithm:
         fingerprint = crl.fingerprint(crl.signature_hash_algorithm)
     else:
         fingerprint = None
 
     extensions = {}
-    errors: list[Error] = []
-    warnings: list[Warning] = []
     try:
         for extension in crl.extensions:
             oid = extension.oid.dotted_string
             try:
                 name = OidNames[oid].name
             except KeyError:
                 warnings.append(
@@ -122,14 +114,15 @@
                         text=f"Parse function for X.509 extension {name} not found",
                     )
                 )
     except ValueError as exc:
         errors.append(Error(module="pkiviewer", text=exc.args[0]))
 
     info: CertificateRevocationListInfo = {
+        "type": "crl",
         "filename": filename,
         "signature": crl.signature,
         "signature_algorithm": OidNames[crl.signature_algorithm_oid.dotted_string].name,
         "signature_algorithm_oid": crl.signature_algorithm_oid.dotted_string,
         "signature_hash_algorithm": crl.signature_hash_algorithm,
         "issuer": crl.issuer,
         "last_update": crl.last_update,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/__init__.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/__init__.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from cryptography.x509.oid import ExtensionOID
 
+from pkiviewer.model.extension.authority_information_access import (
+    authority_information_access_parse,
+)
 from pkiviewer.model.extension.authority_key_identifier import (
     authority_key_identifier_parse,
 )
-from pkiviewer.model.extension.subject_key_identifier import (
-    subject_key_identifier_parse,
-)
-from pkiviewer.model.extension.certificate_policy import certificate_policies_parse
-from pkiviewer.model.extension.key_usage import key_usage_parse
-from pkiviewer.model.extension.subject_alternative_name import (
-    subject_alternative_name_parse,
-)
-from pkiviewer.model.extension.issuer_alternative_name import (
-    issuer_alternative_name_parse,
-)
 from pkiviewer.model.extension.basic_constraints import basic_constraints_parse
-from pkiviewer.model.extension.name_constraints import name_constraints_parse
-from pkiviewer.model.extension.extended_key_usage import extended_key_usage_parse
+from pkiviewer.model.extension.certificate_policy import certificate_policies_parse
 from pkiviewer.model.extension.crl_distribution_points import (
     crl_distribution_points_parse,
 )
+from pkiviewer.model.extension.crl_number import crl_number_parse
+from pkiviewer.model.extension.delta_crl_indicator import delta_crl_indicator_parse
+from pkiviewer.model.extension.extended_key_usage import extended_key_usage_parse
+from pkiviewer.model.extension.freshest_crl import freshest_crl_parse
 from pkiviewer.model.extension.inhibit_any_policy import inhibit_any_policy_parse
-from pkiviewer.model.extension.subject_information_access import (
-    subject_information_access_parse,
+from pkiviewer.model.extension.issuer_alternative_name import (
+    issuer_alternative_name_parse,
 )
-from pkiviewer.model.extension.authority_information_access import (
-    authority_information_access_parse,
+from pkiviewer.model.extension.issuing_distribution_point import (
+    issuing_distribution_point_parse,
+)
+from pkiviewer.model.extension.key_usage import key_usage_parse
+from pkiviewer.model.extension.name_constraints import name_constraints_parse
+from pkiviewer.model.extension.precertificate_signed_certificate_timestamps import (
+    precertificate_signed_certificate_timestamps_parse,
 )
 from pkiviewer.model.extension.signed_certificate_timestamps import (
     signed_certificate_timestamps_parse,
 )
-from pkiviewer.model.extension.precertificate_signed_certificate_timestamps import (
-    precertificate_signed_certificate_timestamps_parse,
+from pkiviewer.model.extension.subject_alternative_name import (
+    subject_alternative_name_parse,
 )
-from pkiviewer.model.extension.crl_number import crl_number_parse
-from pkiviewer.model.extension.issuing_distribution_point import (
-    issuing_distribution_point_parse,
+from pkiviewer.model.extension.subject_information_access import (
+    subject_information_access_parse,
+)
+from pkiviewer.model.extension.subject_key_identifier import (
+    subject_key_identifier_parse,
 )
-from pkiviewer.model.extension.delta_crl_indicator import delta_crl_indicator_parse
-from pkiviewer.model.extension.freshest_crl import freshest_crl_parse
 
 v3_extension_parse = {
     # Certificate
     ExtensionOID.AUTHORITY_KEY_IDENTIFIER.dotted_string: authority_key_identifier_parse,
     ExtensionOID.SUBJECT_KEY_IDENTIFIER.dotted_string: subject_key_identifier_parse,
     ExtensionOID.KEY_USAGE.dotted_string: (key_usage_parse),
     ExtensionOID.CERTIFICATE_POLICIES.dotted_string: certificate_policies_parse,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/authority_information_access.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/authority_information_access.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from typing import cast
 
 from cryptography.x509.extensions import AuthorityInformationAccess, ExtensionType
 
-from pkiviewer.model import (
-    X509ExtensionTypeInfo,
-    access_description_info,
-    AccessDescriptionInfo,
-)
+from pkiviewer.model import AccessDescriptionInfo, access_description_info
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 # RFC5280 4.2.2.1
 class AuthorityInformationAccessInfo(X509ExtensionTypeInfo):
     access_descriptions: list[AccessDescriptionInfo]
 
 
 def authority_information_access_parse(
     extension: ExtensionType,
 ) -> AuthorityInformationAccessInfo:
-    ext = cast(AuthorityInformationAccess, extension)
+    extension = cast(AuthorityInformationAccess, extension)
     access_descriptions: list[AccessDescriptionInfo] = []
-    for description in ext._descriptions:  # type: ignore
+    for description in extension._descriptions:  # type: ignore
         ad = access_description_info(description)
         access_descriptions.append(ad)
 
     ext_info: AuthorityInformationAccessInfo = {
         "type": "AuthorityInformationAccess",
         "access_descriptions": access_descriptions,
     }
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/authority_key_identifier.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/authority_key_identifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import cast
 
-from pkiviewer.model import X509ExtensionTypeInfo
-from pkiviewer.types import CertificateSerialNumber
-from cryptography.x509.general_name import GeneralName
 from cryptography.x509.extensions import AuthorityKeyIdentifier, ExtensionType
+from cryptography.x509.general_name import GeneralName
+
+from pkiviewer.types import CertificateSerialNumber, X509ExtensionTypeInfo
+
 
 # RFC5280 4.2.1.1
 class AuthorityKeyIdentifierInfo(X509ExtensionTypeInfo):
     cert_issuer: list[GeneralName] | None
     cert_serial_number: CertificateSerialNumber | None
     key_identifier: bytes | None
 
 
 def authority_key_identifier_parse(
     extension: ExtensionType,
 ) -> AuthorityKeyIdentifierInfo:
-    ext = cast(AuthorityKeyIdentifier, extension)
+    extension = cast(AuthorityKeyIdentifier, extension)
     ext_info: AuthorityKeyIdentifierInfo = {
         "type": "AuthorityKeyIdentifier",
-        "key_identifier": ext.key_identifier,
-        "cert_issuer": ext.authority_cert_issuer,
-        "cert_serial_number": ext.authority_cert_serial_number,
+        "key_identifier": extension.key_identifier,
+        "cert_issuer": extension.authority_cert_issuer,
+        "cert_serial_number": extension.authority_cert_serial_number,
     }
     return ext_info
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/basic_constraints.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/basic_constraints.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import cast
 
 from cryptography.x509.extensions import BasicConstraints, ExtensionType
 
-from pkiviewer.model import X509ExtensionTypeInfo
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 # RFC5280 4.2.1.9
 class BasicConstraintsInfo(X509ExtensionTypeInfo):
     ca: bool
     path_length: int
 
 
 def basic_constraints_parse(extension: ExtensionType) -> BasicConstraintsInfo:
-    ext = cast(BasicConstraints, extension)
-    path_length = ext.path_length if ext.path_length else 0
+    extension = cast(BasicConstraints, extension)
+    path_length = extension.path_length if extension.path_length else 0
     ext_info: BasicConstraintsInfo = {
         "type": "BasicConstraints",
-        "ca": ext.ca,
+        "ca": extension.ca,
         "path_length": path_length,
     }
     return ext_info
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/certificate_policy.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/certificate_policy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from typing import cast, TypedDict
+from typing import TypedDict, cast
 
 from cryptography.x509 import UserNotice
 from cryptography.x509.extensions import CertificatePolicies, ExtensionType
 
-from pkiviewer.model import X509ExtensionTypeInfo
-from pkiviewer.oid import Oid
+from pkiviewer.oid.names import Oid
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 # RFC5280 4.2.1.4
 class PolicyInfo(TypedDict):
     oid: Oid
     strings: list[str]
     user_notices: list[UserNotice]
 
 
 class CertificatePoliciesInfo(X509ExtensionTypeInfo):
     policies: list[PolicyInfo]
 
 
-def certificate_policies_parse(extension: ExtensionType) -> CertificatePoliciesInfo:
-    ext = cast(CertificatePolicies, extension)
+def certificate_policies_parse(
+    extension: ExtensionType,
+) -> CertificatePoliciesInfo:
+    extension = cast(CertificatePolicies, extension)
     policies: list[PolicyInfo] = []
-    for policy in ext._policies:  # type: ignore
+    for policy in extension._policies:  # type: ignore
         oid = policy.policy_identifier.dotted_string
 
         strings: list[str] = []
         user_notices: list[UserNotice] = []
         if policy.policy_qualifiers:
             for qual in policy.policy_qualifiers:
                 if isinstance(qual, str):
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/crl_distribution_points.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/crl_distribution_points.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import cast
 
 from cryptography.x509.extensions import CRLDistributionPoints, ExtensionType
 
 from pkiviewer.model import (
-    X509ExtensionTypeInfo,
+    DistributionPointInfo,
+    GeneralNameInfo,
     general_names_parse,
     relative_distinguished_names_parse,
-    GeneralNameInfo,
 )
 from pkiviewer.model.extension.reasons import reasons_parse
-from pkiviewer.model import DistributionPointInfo
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 # RFC5280 4.2.1.13
 class CRLDistributionPointsInfo(X509ExtensionTypeInfo):
     distribution_points: list[DistributionPointInfo]
 
 
 def crl_distribution_points_parse(
     extension: ExtensionType,
 ) -> CRLDistributionPointsInfo:
-    ext = cast(CRLDistributionPoints, extension)
+    extension = cast(CRLDistributionPoints, extension)
     distribution_points: list[DistributionPointInfo] = []
 
-    for dp in ext._distribution_points:  # type: ignore
+    for dp in extension._distribution_points:  # type: ignore
         names: list[GeneralNameInfo] = []
 
         if dp.full_name:
             names = general_names_parse(dp.full_name)
         elif dp.relative_name:
             names = relative_distinguished_names_parse(dp.relative_name)
         else:
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/delta_crl_indicator.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/delta_crl_indicator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import cast
 
 from cryptography.x509.extensions import DeltaCRLIndicator, ExtensionType
 
-from pkiviewer.model import X509ExtensionTypeInfo
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 # RFC5280 4.2.1.14
 class DeltaCRLIndicatorInfo(X509ExtensionTypeInfo):
     crl_number: int
 
 
 def delta_crl_indicator_parse(
     extension: ExtensionType,
 ) -> DeltaCRLIndicatorInfo:
-    ext = cast(DeltaCRLIndicator, extension)
+    extension = cast(DeltaCRLIndicator, extension)
     ext_info: DeltaCRLIndicatorInfo = {
         "type": "DeltaCRLIndicator",
-        "crl_number": ext.crl_number,
+        "crl_number": extension.crl_number,
     }
     return ext_info
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/extended_key_usage.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/extended_key_usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import cast
 
 from cryptography.x509.extensions import ExtendedKeyUsage, ExtensionType
 
-from pkiviewer.model import X509ExtensionTypeInfo
-from pkiviewer.oid import OidNames
+from pkiviewer.oid.names import OidNames
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 # RFC5280 4.2.1.12
 class ExtendedKeyUsageInfo(X509ExtensionTypeInfo):
     usage: list[str]
 
 
 def extended_key_usage_parse(extension: ExtensionType) -> ExtendedKeyUsageInfo:
-    ext = cast(ExtendedKeyUsage, extension)
-
+    extension = cast(ExtendedKeyUsage, extension)
     items: list[str] = []
-    for u in ext._usages:  # type: ignore
+    for u in extension._usages:  # type: ignore
         items.append(OidNames[u.dotted_string].name)
 
     ext_info: ExtendedKeyUsageInfo = {"type": "ExtendedKeyUsage", "usage": items}
     return ext_info
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/freshest_crl.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/freshest_crl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import cast
 
-from cryptography.x509.extensions import FreshestCRL, ExtensionType
+from cryptography.x509.extensions import ExtensionType, FreshestCRL
 
 from pkiviewer.model import (
-    X509ExtensionTypeInfo,
     DistributionPointInfo,
+    GeneralNameInfo,
     general_names_parse,
     relative_distinguished_names_parse,
-    GeneralNameInfo,
 )
 from pkiviewer.model.extension.reasons import reasons_parse
+from pkiviewer.types import X509ExtensionTypeInfo
+
 
 # RFC5280 4.2.1.14
 class FreshestCRLInfo(X509ExtensionTypeInfo):
     distribution_points: list[DistributionPointInfo]
 
 
 def freshest_crl_parse(
     extension: ExtensionType,
 ) -> FreshestCRLInfo:
-    ext = cast(FreshestCRL, extension)
-
+    extension = cast(FreshestCRL, extension)
     distribution_points: list[DistributionPointInfo] = []
-    for dp in ext._distribution_points:  # type: ignore
+    for dp in extension._distribution_points:  # type: ignore
         names: list[GeneralNameInfo] = []
 
         if dp.full_name:
             names = general_names_parse(dp.full_name)
         elif dp.relative_name:
             names = relative_distinguished_names_parse(dp.relative_name)
         else:
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/inhibit_any_policy.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/inhibit_any_policy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import cast
 
-from cryptography.x509.extensions import InhibitAnyPolicy, ExtensionType
+from cryptography.x509.extensions import ExtensionType, InhibitAnyPolicy
 
-from pkiviewer.model import X509ExtensionTypeInfo
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 # RFC5280 4.2.1.14
 class InhibitAnyPolicyInfo(X509ExtensionTypeInfo):
     skip_certs: int
 
 
 def inhibit_any_policy_parse(
     extension: ExtensionType,
 ) -> InhibitAnyPolicyInfo:
-    ext = cast(InhibitAnyPolicy, extension)
+    extension = cast(InhibitAnyPolicy, extension)
     ext_info: InhibitAnyPolicyInfo = {
         "type": "InhibitAnyPolicyInfo",
-        "skip_certs": ext.skip_certs,
+        "skip_certs": extension.skip_certs,
     }
     return ext_info
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/issuer_alternative_name.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/issuer_alternative_name.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from typing import cast
 
 from cryptography.x509 import general_name
-from cryptography.x509.extensions import IssuerAlternativeName, ExtensionType
+from cryptography.x509.extensions import ExtensionType, IssuerAlternativeName
 
-from pkiviewer.model import X509ExtensionTypeInfo
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 class IssuerAlternativeNameInfo(X509ExtensionTypeInfo):
     ians: dict[str, list[str]]
 
 
 # RFC5280 4.2.1.7
 def issuer_alternative_name_parse(
     extension: ExtensionType,
 ) -> IssuerAlternativeNameInfo:
-    ext = cast(IssuerAlternativeName, extension)
+    extension = cast(IssuerAlternativeName, extension)
     names = {
         general_name.DNSName: "DNS",
         general_name.RFC822Name: "email",
         general_name.UniformResourceIdentifier: "URI",
         general_name.IPAddress: "IP Address",
         general_name.RegisteredID: "Registered ID",
     }
     ians: dict[str, list[str]] = {}
     for key, value in names.items():
         ian_list: list[str] = []
-        for address in ext.get_values_for_type(type(key)):
+        for address in extension.get_values_for_type(type(key)):
             ian_list.append(str(address))
         if ian_list:
             ians[value] = ian_list
     ext_info: IssuerAlternativeNameInfo = {
         "type": "SubjectAlternativeName",
         "ians": ians,
     }
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/issuing_distribution_point.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/issuing_distribution_point.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import cast
 
-from cryptography.x509.extensions import IssuingDistributionPoint, ExtensionType
+from cryptography.x509.extensions import ExtensionType, IssuingDistributionPoint
 
-from pkiviewer.model import X509ExtensionTypeInfo, general_names_parse
+from pkiviewer.model import general_names_parse
 from pkiviewer.model.extension.reasons import reasons_parse
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 # RFC5280 4.2.1.14
 class IssuingDistributionPointInfo(X509ExtensionTypeInfo):
     full_name: list[tuple[str, str]]
     reasons: list[str]
     only_contains_attribute_certs: bool
@@ -15,22 +16,21 @@
     only_contains_user_certs: bool
     indirect_crl: bool
 
 
 def issuing_distribution_point_parse(
     extension: ExtensionType,
 ) -> IssuingDistributionPointInfo:
-    ext = cast(IssuingDistributionPoint, extension)
-
-    full_name = general_names_parse(ext.full_name)
-    reasons = reasons_parse(ext.only_some_reasons)
+    extension = cast(IssuingDistributionPoint, extension)
+    full_name = general_names_parse(extension.full_name)
+    reasons = reasons_parse(extension.only_some_reasons)
 
     ext_info: IssuingDistributionPointInfo = {
         "type": "IssuingDistributionPoint",
         "full_name": full_name,
-        "only_contains_attribute_certs": ext.only_contains_attribute_certs,
-        "only_contains_ca_certs": ext.only_contains_ca_certs,
-        "only_contains_user_certs": ext.only_contains_user_certs,
+        "only_contains_attribute_certs": extension.only_contains_attribute_certs,
+        "only_contains_ca_certs": extension.only_contains_ca_certs,
+        "only_contains_user_certs": extension.only_contains_user_certs,
         "reasons": reasons,
-        "indirect_crl": ext.indirect_crl,
+        "indirect_crl": extension.indirect_crl,
     }
     return ext_info
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/key_usage.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/key_usage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import cast
 
-from cryptography.x509.extensions import KeyUsage, ExtensionType
+from cryptography.x509.extensions import ExtensionType, KeyUsage
 
-from pkiviewer.model import X509ExtensionTypeInfo
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 # RFC5280 4.2.1.3
 class KeyUsageInfo(X509ExtensionTypeInfo):
     usage: list[str]
 
 
 def key_usage_parse(extension: ExtensionType) -> KeyUsageInfo:
+    extension = cast(KeyUsage, extension)
     items: list[str] = []
-    ext = cast(KeyUsage, extension)
-    if ext.digital_signature:
+    if extension.digital_signature:
         items.append("Digital Signature")
-    if ext.content_commitment:
+    if extension.content_commitment:
         items.append("Content Commitment (Non Repudiation)")
-    if ext.key_encipherment:
+    if extension.key_encipherment:
         items.append("Key Encipherment")
-    if ext.data_encipherment:
+    if extension.data_encipherment:
         items.append("Data Encipherment")
-    if ext.key_agreement:
+    if extension.key_agreement:
         items.append("Key Agreement")
-    if ext.key_cert_sign:
+    if extension.key_cert_sign:
         items.append("Certificate Sign")
-    if ext.crl_sign:
+    if extension.crl_sign:
         items.append("CRL Sign")
-    if ext.key_agreement and ext.encipher_only:
+    if extension.key_agreement and extension.encipher_only:
         items.append("Encipher Only")
-    if ext.key_agreement and ext.decipher_only:
+    if extension.key_agreement and extension.decipher_only:
         items.append("Decipher Only")
 
     usage: KeyUsageInfo = {"type": "KeyUsage", "usage": items}
     return usage
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/name_constraints.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/name_constraints.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import cast, Any
+from typing import Any, cast
 
-from cryptography.x509.extensions import NameConstraints, ExtensionType
+from cryptography.x509.extensions import ExtensionType, NameConstraints
 
-from pkiviewer.model import X509ExtensionTypeInfo, general_names_parse
+from pkiviewer.model import general_names_parse
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 # RFC5280 4.2.1.10
 class NameConstraintsInfo(X509ExtensionTypeInfo):
     permitted_subtrees: list[tuple[str, Any]]
     excluded_subtrees: list[tuple[str, Any]]
 
 
 def name_constraints_parse(extension: ExtensionType) -> NameConstraintsInfo:
-    ext = cast(NameConstraints, extension)
-
-    permitted = general_names_parse(ext.permitted_subtrees)
-    excluded = general_names_parse(ext.excluded_subtrees)
+    extension = cast(NameConstraints, extension)
+    permitted = general_names_parse(extension.permitted_subtrees)
+    excluded = general_names_parse(extension.excluded_subtrees)
 
     ext_info: NameConstraintsInfo = {
         "type": "NameConstraints",
         "permitted_subtrees": permitted,
         "excluded_subtrees": excluded,
     }
     return ext_info
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/precertificate_signed_certificate_timestamps.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/precertificate_signed_certificate_timestamps.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import cast
 
 from cryptography.x509.certificate_transparency import SignedCertificateTimestamp
 from cryptography.x509.extensions import (
-    PrecertificateSignedCertificateTimestamps,
     ExtensionType,
+    PrecertificateSignedCertificateTimestamps,
 )
 
-from pkiviewer.model import X509ExtensionTypeInfo
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 class PreCertificateSignedCertificateTimestampsInfo(X509ExtensionTypeInfo):
     timestamps: list[SignedCertificateTimestamp]
 
 
 # TODO Complete OreCertificateSignedCertificateTimestampsInfo
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/reasons.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/reasons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from cryptography.x509 import ReasonFlags
 
-
 Reasons: dict[ReasonFlags, str] = {
     ReasonFlags.aa_compromise: "Attribute Authority compromised",
     ReasonFlags.affiliation_changed: "Subject's name or other information has changed",
     ReasonFlags.ca_compromise: "Certificate Authority compromised",
     ReasonFlags.certificate_hold: "Certificate on hold",
     ReasonFlags.cessation_of_operation: "Certificate no longer required",
     ReasonFlags.key_compromise: "Private key was compromised",
-    ReasonFlags.privilege_withdrawn: "Privilege granted by this certificate have been withdrawn",
+    ReasonFlags.privilege_withdrawn: (
+        "Privilege granted by this certificate have been withdrawn"
+    ),
     ReasonFlags.remove_from_crl: "Certificate should be removed from the CRL",
     ReasonFlags.superseded: "Certificate superseded",
     ReasonFlags.unspecified: "Unspecified",
 }
 
 
 def reasons_parse(reasons: frozenset[ReasonFlags] | None) -> list[str]:
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/signed_certificate_timestamps.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/signed_certificate_timestamps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import cast
 
 from cryptography.x509.certificate_transparency import SignedCertificateTimestamp
-from cryptography.x509.extensions import SignedCertificateTimestamps, ExtensionType
+from cryptography.x509.extensions import ExtensionType, SignedCertificateTimestamps
 
-from pkiviewer.model import X509ExtensionTypeInfo
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 class SignedCertificateTimestampsInfo(X509ExtensionTypeInfo):
     timestamps: list[SignedCertificateTimestamp]
 
 
 # TODO Complete SignedCertificateTimestampsInfo
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/subject_alternative_name.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/subject_alternative_name.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import cast, Type
+from typing import Type, cast
 
+from cryptography.x509.extensions import ExtensionType, SubjectAlternativeName
 from cryptography.x509.general_name import (
     DNSName,
-    UniformResourceIdentifier,
     RFC822Name,
+    UniformResourceIdentifier,
 )
-from cryptography.x509.extensions import SubjectAlternativeName, ExtensionType
 
-from pkiviewer.model import X509ExtensionTypeInfo
+from pkiviewer.types import X509ExtensionTypeInfo
+
 
 # RFC5280 4.2.1.6
 class SubjectAlternativeNameInfo(X509ExtensionTypeInfo):
     sans: dict[str, list[str]]
 
 
 GeneralNameToShortName: dict[
@@ -22,20 +23,19 @@
     RFC822Name: "email",
 }
 
 
 def subject_alternative_name_parse(
     extension: ExtensionType,
 ) -> SubjectAlternativeNameInfo:
-    ext = cast(SubjectAlternativeName, extension)
-
+    extension = cast(SubjectAlternativeName, extension)
     sans: dict[str, list[str]] = {}
     for key, value in GeneralNameToShortName.items():
         san_list: list[str] = []
-        for address in ext.get_values_for_type(key):
+        for address in extension.get_values_for_type(key):
             san_list.append(str(address))
         if san_list:
             sans[value] = san_list
 
     ext_info: SubjectAlternativeNameInfo = {
         "type": "SubjectAlternativeName",
         "sans": sans,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/extension/subject_information_access.py` & `pkiviewer-0.2.1/src/pkiviewer/model/extension/subject_information_access.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from typing import cast
 
-from cryptography.x509.extensions import SubjectInformationAccess, ExtensionType
+from cryptography.x509.extensions import ExtensionType, SubjectInformationAccess
 
-from pkiviewer.model import (
-    X509ExtensionTypeInfo,
-    access_description_info,
-    AccessDescriptionInfo,
-)
+from pkiviewer.model import AccessDescriptionInfo, access_description_info
+from pkiviewer.types import X509ExtensionTypeInfo
 
 
 # RFC5280 4.2.2.2
 class SubjectInformationAccessInfo(X509ExtensionTypeInfo):
     access_descriptions: list[tuple[str, str, str]]
 
 
 def subject_information_access_parse(
     extension: ExtensionType,
 ) -> SubjectInformationAccessInfo:
-    ext = cast(SubjectInformationAccess, extension)
+    extension = cast(SubjectInformationAccess, extension)
     access_descriptions: list[AccessDescriptionInfo] = []
-    for description in ext._descriptions:  # type: ignore
+    for description in extension._descriptions:  # type: ignore
         ad = access_description_info(description)
         access_descriptions.append(ad)
 
     ext_info: SubjectInformationAccessInfo = {
         "type": "SubjectInformationAccess",
         "access_descriptions": access_descriptions,
     }
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/p12.py` & `pkiviewer-0.2.1/src/pkiviewer/model/p12.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from typing import TypedDict
-
-from cryptography.hazmat.primitives.serialization.pkcs12 import PKCS12KeyAndCertificates
 from cryptography.hazmat.primitives.asymmetric.types import PRIVATE_KEY_TYPES
+from cryptography.hazmat.primitives.serialization.pkcs12 import PKCS12KeyAndCertificates
 
 from pkiviewer.model.certificate import CertificateInfo, certiticate_parse
+from pkiviewer.types import X509Info
 
 
-class PKCS12KeyAndCertificateInfo(TypedDict):
-    filename: str
+class PKCS12KeyAndCertificateInfo(X509Info):
     name: str
     certificate: CertificateInfo | None
     private_key: PRIVATE_KEY_TYPES | None
     additional_certs: list[CertificateInfo]
 
 
 def p12_key_and_certificates_parse(
@@ -24,15 +22,18 @@
     additional_cert_info: list[CertificateInfo] = []
     for additional_cert in p12.additional_certs:
         additional_cert_info.append(
             certiticate_parse(additional_cert.certificate, filename)
         )
 
     info: PKCS12KeyAndCertificateInfo = {
+        "type": "p12",
         "filename": filename,
         "name": "PKCS12KeyAndCertificate",
         "certificate": cert_info,
         "private_key": p12.key,
         "additional_certs": additional_cert_info,
+        "errors": [],
+        "warnings": [],
     }
 
     return info
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/public_key/__init__.py` & `pkiviewer-0.2.1/src/pkiviewer/model/public_key/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from cryptography.hazmat.primitives.asymmetric.dh import DHPublicKey
 from cryptography.hazmat.primitives.asymmetric.dsa import DSAPublicKey
 from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurvePublicKey
-from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
-from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PublicKey
 from cryptography.hazmat.primitives.asymmetric.ed448 import Ed448PublicKey
+from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PublicKey
+from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
 from cryptography.hazmat.primitives.asymmetric.types import CERTIFICATE_PUBLIC_KEY_TYPES
 
-from pkiviewer.model import PublicKeyInfo
 from pkiviewer.model.public_key.dh import dh_public_key_info
 from pkiviewer.model.public_key.dsa import dsa_public_key_info
 from pkiviewer.model.public_key.ed448 import ed448_public_key_info
 from pkiviewer.model.public_key.ed25519 import ed25519_public_key_info
 from pkiviewer.model.public_key.elliptic_curve import elliptic_curve_public_key_info
 from pkiviewer.model.public_key.rsa import rsa_public_key_info
+from pkiviewer.types import PublicKeyInfo
 
 
 def public_key_info(pk: CERTIFICATE_PUBLIC_KEY_TYPES) -> PublicKeyInfo | None:
     if isinstance(pk, RSAPublicKey):
         return rsa_public_key_info(pk)
     elif isinstance(pk, EllipticCurvePublicKey):
         return elliptic_curve_public_key_info(pk)
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/public_key/ed25519.py` & `pkiviewer-0.2.1/src/pkiviewer/model/public_key/ed25519.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PublicKey
 from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
 
-from pkiviewer.model import PublicKeyInfo
+from pkiviewer.types import PublicKeyInfo
 
 
 class Ed25519PublicKeyInfo(PublicKeyInfo):
     pub: bytes
 
 
 def ed25519_public_key_info(key: Ed25519PublicKey) -> Ed25519PublicKeyInfo:
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/public_key/ed448.py` & `pkiviewer-0.2.1/src/pkiviewer/model/public_key/ed448.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cryptography.hazmat.primitives.asymmetric.ed448 import Ed448PublicKey
 from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
 
-from pkiviewer.model import PublicKeyInfo
+from pkiviewer.types import PublicKeyInfo
 
 
 class Ed448PublicKeyInfo(PublicKeyInfo):
     pub: bytes
 
 
 def ed448_public_key_info(key: Ed448PublicKey) -> Ed448PublicKeyInfo:
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/public_key/elliptic_curve.py` & `pkiviewer-0.2.1/src/pkiviewer/model/public_key/elliptic_curve.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurvePublicKey
 from cryptography.hazmat.primitives.serialization import Encoding, PublicFormat
 
-from pkiviewer.model import PublicKeyInfo
+from pkiviewer.types import PublicKeyInfo
 
 
 class EllipticCurvePublicKeyInfo(PublicKeyInfo):
     key_size: int
     x: int
     y: int
     pub: bytes
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/public_key/rsa.py` & `pkiviewer-0.2.1/src/pkiviewer/model/public_key/rsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
 
-from pkiviewer.model import PublicKeyInfo
+from pkiviewer.types import PublicKeyInfo
 
 
 class RSAPublicKeyInfo(PublicKeyInfo):
     key_size: int
     modulus: int
     exponent: int
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/model/unpack.py` & `pkiviewer-0.2.1/src/pkiviewer/model/unpack.py`

 * *Files identical despite different names*

### Comparing `pkiviewer-0.2.0/src/pkiviewer/oid/__init__.py` & `pkiviewer-0.2.1/src/pkiviewer/oid/names.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
+# flake8: noqa
 """OID to name mappings"""
 
 from typing import NamedTuple
 
+from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurveOID
 from cryptography.x509.oid import (
     AuthorityInformationAccessOID,
     ExtendedKeyUsageOID,
     ExtensionOID,
-    SignatureAlgorithmOID,
     NameOID,
+    SignatureAlgorithmOID,
 )
-from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurveOID
-
 
 Oid = str
 OidName = str
 
 
 class OidInfo(NamedTuple):
     name: OidName
-    defined_in: str | None
+    info: str | None
 
 
 OidDatabase = dict[Oid, OidInfo]
 
-
 OidNames: OidDatabase = {
     # region Name OIDs
     NameOID.BUSINESS_CATEGORY.dotted_string: OidInfo(
         "Business Category", "ITU-T X.520, RFC4519 2.1"
     ),
     NameOID.COMMON_NAME.dotted_string: OidInfo(
         "Common Name", "ITU-T X.520, RFC4519 2.3"
@@ -186,20 +185,14 @@
     ),
     ExtensionOID.PRECERT_SIGNED_CERTIFICATE_TIMESTAMPS.dotted_string: OidInfo(
         "CT Precertificate SCTs", "RFC6962 3.3"
     ),
     ExtensionOID.SIGNED_CERTIFICATE_TIMESTAMPS.dotted_string: OidInfo(
         "Certificate SCTs", "RFC6962 3.3"
     ),
-    # Microsoft Extensions
-    "1.3.6.1.4.1.311.21.7": OidInfo("Microsoft szOID_CERTIFICATE_TEMPLATE", None),
-    "1.3.6.1.4.1.311.21.10": OidInfo("Microsoft szOID_APPLICATION_CERT_POLICIES", None),
-    "1.3.6.1.4.1.311.13.2.3": OidInfo("szOID_OS_VERSION", None),
-    "1.3.6.1.4.1.311.13.2.2": OidInfo("szOID_ENROLLMENT_CSP_PROVIDER", None),
-    "1.3.6.1.4.1.311.2.1.14": OidInfo("Authenticode SPC_CERT_EXTENSIONS_OBJID", None),
     # Other extensions
     "1.2.840.113549.1.9.15": OidInfo("SMime Capabilities", "RFC8551"),
     "1.3.6.1.5.5.7.48.1.5": OidInfo("OCSP id-pkix-ocsp-nocheck extension", "RFC2560"),
     # endregion
     # region Signature Algorithm OIDs
     SignatureAlgorithmOID.DSA_WITH_SHA1.dotted_string: OidInfo(
         "DSA with SHA1", "FIPS Pub 186-4"
@@ -358,30 +351,14 @@
         "https://cabforum.org/wp-content/uploads/Baseline-Requirements-for-the-Issuance-and-Management-of-Code-Signing.v3.0.pdf",
     ),
     "2.23.140.1.31": OidInfo(
         "CA/Browser Forum onion-EV",
         "https://cabforum.org/wp-content/uploads/CA-Browser-Forum-EV-Guidelines-1.7.9.pdf",
     ),
     "2.23.140.3.1": OidInfo("CA/Browser Forum cabforganization-identifier", None),
-    "1.3.6.1.4.1.11129.2.5.3": OidInfo(
-        "Google Trust Services Certificate Policy",
-        "https://pki.goog/GTS-CP-1.3.pdf",
-    ),
-    "1.3.6.1.4.1.311.76.509.1.1": OidInfo(
-        "Microsoft PKI Services Certification Practice Statement (CPS)",
-        "https://www.microsoft.com/pkiops/Docs/Content/policy/Microsoft_PKI_Services_CPS_v3.1.2.pdf",
-    ),
-    "1.3.6.1.4.1.6449.1.2.1.5.1": OidInfo(
-        "Comodo Extended Validation (EV) Certification Practice Statement",
-        "https://www.comodo.com/repository/EV_CPS_4_JUN_07.pdf",
-    ),
-    "1.3.6.1.4.1.4146.1.20": OidInfo(
-        "GlobalSign Certificate Policy",
-        "https://www.globalsign.com/en/repository",
-    ),
     "2.16.840.1.114414.1.7.23.1": OidInfo(
         "Starfield Technologies Certificate Policy and Certification Practice Statement (CP/CPS)",
         "https://certs.starfieldtech.com/repository/certificate_practices/StarfieldCertificatePolicyandCertificationPracticeStatement.pdf",
     ),
     # endregion
     # region Hashes
     "1.2.840.113549.2.2": OidInfo("md2", None),
@@ -393,8 +370,57 @@
         "3DES in CBC mode (szOID_RSA_DES_EDE3_CBC)", "RFC8018"
     ),
     "1.3.14.3.2.7": OidInfo(
         "Single-key DES in CBC mode with padding operation", "RFC8018"
     ),
     "1.3.6.1.5.5.7.1.14": OidInfo("Proxy certification information", "RFC3820"),
     "1.2.840.113549.3.2": OidInfo("Voice encryption", "RFC8018"),
+    "1.3.6.1.4.1": OidInfo(
+        "IANA Private Enterprise Numbers",
+        "https://www.iana.org/assignments/enterprise-numbers/",
+    ),
+    # Microsoft Extensions
+    "1.3.6.1.4.1.311": OidInfo("Microsoft PEN", None),
+    "1.3.6.1.4.1.311.21.7": OidInfo("Microsoft szOID_CERTIFICATE_TEMPLATE", None),
+    "1.3.6.1.4.1.311.21.10": OidInfo("Microsoft szOID_APPLICATION_CERT_POLICIES", None),
+    "1.3.6.1.4.1.311.13.2.3": OidInfo("szOID_OS_VERSION", None),
+    "1.3.6.1.4.1.311.13.2.2": OidInfo("szOID_ENROLLMENT_CSP_PROVIDER", None),
+    "1.3.6.1.4.1.311.2.1.14": OidInfo("Authenticode SPC_CERT_EXTENSIONS_OBJID", None),
+    "1.3.6.1.4.1.311.76.509.1.1": OidInfo(
+        "Microsoft PKI Services Certification Practice Statement (CPS)",
+        "https://www.microsoft.com/pkiops/Docs/Content/policy/Microsoft_PKI_Services_CPS_v3.1.2.pdf",
+    ),
+    "1.3.6.1.4.1.4146.1.20": OidInfo(
+        "GlobalSign Certificate Policy",
+        "https://www.globalsign.com/en/repository",
+    ),
+    "1.3.6.1.4.1.6449.1.2.1.5.1": OidInfo(
+        "Comodo Extended Validation (EV) Certification Practice Statement",
+        "https://www.comodo.com/repository/EV_CPS_4_JUN_07.pdf",
+    ),
+    "1.3.6.1.4.1.11129.2.5.3": OidInfo(
+        "Google Trust Services Certificate Policy",
+        "https://pki.goog/GTS-CP-1.3.pdf",
+    ),
+    "1.3.6.1.4.1.44947.1.1.1": OidInfo(
+        "ISRG Domain Validated", "https://letsencrypt.org/documents/isrg-cps-v2.2/"
+    ),
 }
+
+
+def find_oid_or_parent(oid: str) -> OidInfo | None:
+    """Find an OID or a parent.
+
+    If an exact match is found return it
+    otherwise search up the tree for a parent and return that.
+    """
+    info = OidNames.get(oid, None)
+    if info is not None:
+        return info
+
+    elems = oid.split(".")
+    for idx in range(len(elems) - 1, 0, -1):
+        possible_id = ".".join(elems[:idx])
+        if (info := find_oid_or_parent(possible_id)) is not None:
+            return info
+
+    return None
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/console.py` & `pkiviewer-0.2.1/src/pkiviewer/view/console.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import textwrap
 from typing import Any
 
 import rich.console
 import rich.style
 import rich.theme
 
-from pkiviewer.types import Warning, Error
-from pkiviewer.view.theme import indents, INDENT_PER_LEVEL, get_style
-from pkiviewer.view.formatter import int_to_hex_short, hex_string_split
 from pkiviewer.context import _console  # type: ignore
+from pkiviewer.types import Error, Warning
+from pkiviewer.view.formatter import hex_string_split, int_to_hex_short
+from pkiviewer.view.theme import INDENT_PER_LEVEL, get_style, indents
 
 MAX_STRIDE = 24
 
 
 def print_info(text: str, indent: int = 0) -> None:
     c = _console.get()
     c.print(f"{indents[indent]}[info]{text}[/]", emoji=False, highlight=False)
 
 
 def print_hex_oneline(
     value: int,
     indent: int = 0,
     value_style: rich.style.Style | None = None,
+    c: rich.console.Console | None = None,
 ) -> None:
-    c = _console.get()
+    if c is None:
+        c = _console.get()
     text = int_to_hex_short(value)
     c.print(f"{indents[indent]}[{value_style}]{text}[/]", emoji=False, highlight=False)
 
 
 def print_hex_multiline(
     hex_str: str,
     indent: int = 0,
     stride: int = -1,
     value_style: rich.style.Style | None = None,
+    c: rich.console.Console | None = None,
 ) -> None:
-    c = _console.get()
+    if c is None:
+        c = _console.get()
     width = c.width
 
     max_stride = (width - len(indents[indent])) // 3
     max_stride = max_stride if max_stride < MAX_STRIDE else MAX_STRIDE
 
     stride = stride if stride != -1 and stride < max_stride else max_stride
 
@@ -50,41 +54,48 @@
     c.print(f"[{value_style}]{text}[/]", emoji=False, highlight=False)
 
 
 def print_key_oneline(
     key: str,
     indent: int = 0,
     key_style: rich.style.Style | None = None,
+    c: rich.console.Console | None = None,
 ) -> None:
-    c = _console.get()
+    if c is None:
+        c = _console.get()
     if key_style is None:
         key_style = get_style("key")
     c.print(f"{indents[indent]}[{key_style}]{key}[/]", emoji=False, highlight=False)
 
 
 def print_value_oneline(
     value: str,
     indent: int = 0,
     value_style: rich.style.Style | None = None,
+    c: rich.console.Console | None = None,
 ) -> None:
-    c = _console.get()
+    if c is None:
+        c = _console.get()
     if value_style is None:
         value_style = get_style("value")
     c.print(f"{indents[indent]}[{value_style}]{value}[/]", emoji=False, highlight=False)
 
 
 def print_value_multiline(
     value: str,
     indent: int = 0,
     value_style: rich.style.Style | None = None,
+    c: rich.console.Console | None = None,
 ) -> None:
+    if c is None:
+        c = _console.get()
+
     if value_style is None:
         value_style = get_style("value")
 
-    c = _console.get()
     space_left = c.width - indent * INDENT_PER_LEVEL
     if space_left < len(value):
         text = textwrap.fill(
             value,
             width=c.width,
             initial_indent=indents[indent],
             subsequent_indent=indents[indent],
@@ -94,27 +105,32 @@
         print_value_oneline(f"[{value_style}]{value}[/]", indent=indent)
 
 
 def print_multivalue_multiline(
     value: list[str],
     indent: int = 0,
     value_style: rich.style.Style | None = None,
+    c: rich.console.Console | None = None,
 ) -> None:
+    if c is None:
+        c = _console.get()
     for item in value:
-        print_value_multiline(item, indent=indent, value_style=value_style)
+        print_value_multiline(item, indent=indent, value_style=value_style, c=c)
 
 
 def print_key_value_oneline(
     key: str,
     value: Any,
     indent: int = 0,
     key_style: rich.style.Style | None = None,
     value_style: rich.style.Style | None = None,
+    c: rich.console.Console | None = None,
 ) -> None:
-    c = _console.get()
+    if c is None:
+        c = _console.get()
     if key_style is None or value_style is None:
         if key_style is None:
             key_style = get_style("key")
         if value_style is None:
             value_style = get_style("value")
 
     c.print(
@@ -126,46 +142,56 @@
 
 def print_key_value_multiline(
     key: str,
     value: Any,
     indent: int = 0,
     key_style: rich.style.Style | None = None,
     value_style: rich.style.Style | None = None,
+    c: rich.console.Console | None = None,
 ) -> None:
+    if c is None:
+        c = _console.get()
     if key_style is None or value_style is None:
         if key_style is None:
             key_style = get_style("key")
         if value_style is None:
             value_style = get_style("value")
 
-    print_key_oneline(key, indent, key_style)
-    print_value_multiline(value, indent + 1, value_style)
+    print_key_oneline(key, indent, key_style, c=c)
+    print_value_multiline(value, indent + 1, value_style, c=c)
 
 
-def print_error(filename: str, error: Error, indent: int = 0):
-    c = _console.get()
+def print_error(
+    filename: str,
+    error: Error,
+    indent: int = 0,
+    c: rich.console.Console | None = None,
+) -> None:
+    if c is None:
+        c = _console.get()
     c.print(f"{indents[indent]}[error]{filename}[/]", highlight=False)
 
     text = f"{error['module']}: {error['text']}"
     text = textwrap.fill(
         text,
         width=c.width,
         initial_indent=indents[indent + 1],
         subsequent_indent=indents[indent + 1],
     )
     c.print(f"[error]{text}[/]", highlight=False)
 
 
-def print_warning_text(text: str):
-    c = _console.get()
-    c.print(f"[warning]{text}[/]", highlight=False)
-
-
-def print_warning(filename: str, warning: Warning, indent: int = 0):
-    c = _console.get()
+def print_warning(
+    filename: str,
+    warning: Warning,
+    indent: int = 0,
+    c: rich.console.Console | None = None,
+) -> None:
+    if c is None:
+        c = _console.get()
     c.print(f"{indents[indent]}[warning]{filename}[/]", highlight=False)
 
     text = f"{warning['module']}: {warning['text']}"
     text = textwrap.fill(
         text,
         width=c.width,
         initial_indent=indents[indent + 1],
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/certificate.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/certificate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 import datetime
 from typing import cast
 
 from cryptography.x509 import Version
+
+from pkiviewer.context import _console  # type: ignore
 from pkiviewer.model.certificate import CertificateInfo
-from pkiviewer.oid import OidNames
 from pkiviewer.model.public_key.dh import DHPublicKeyInfo
 from pkiviewer.model.public_key.dsa import DSAPublicKeyInfo
 from pkiviewer.model.public_key.ed448 import Ed448PublicKeyInfo
 from pkiviewer.model.public_key.ed25519 import Ed25519PublicKeyInfo
 from pkiviewer.model.public_key.elliptic_curve import EllipticCurvePublicKeyInfo
 from pkiviewer.model.public_key.rsa import RSAPublicKeyInfo
-from pkiviewer.model import X509ExtensionInfo
-from pkiviewer.types import Warning
-from pkiviewer.view.display.public_key import dh, dsa, ed25519, ed448, elliptic_curve
-
-from pkiviewer.view.theme import (
-    get_key_style,
-    get_value_style,
-    Visibility,
-    get_key_value_styles,
-    get_style,
-)
+from pkiviewer.oid.names import OidNames
+from pkiviewer.types import ExtensionDisplayMethod, Warning, X509ExtensionInfo
 from pkiviewer.view.console import (
-    print_error,
     print_hex_multiline,
     print_key_oneline,
     print_key_value_multiline,
     print_key_value_oneline,
-    print_warning,
 )
-from pkiviewer.view.display.public_key import rsa
 from pkiviewer.view.display import extension
 from pkiviewer.view.display.extension.header import extension_header_display
+from pkiviewer.view.display.public_key import (
+    dh,
+    dsa,
+    ed448,
+    ed25519,
+    elliptic_curve,
+    rsa,
+)
 from pkiviewer.view.formatter import (
-    int_to_hex_short,
-    int_to_hex_long,
     bytes_to_hex_long,
+    format_date_time,
     format_name,
     format_version,
-    format_date_time,
+    int_to_hex_long,
+    int_to_hex_short,
 )
-from pkiviewer.view.theme import get_style, INDENT_PER_LEVEL
-from pkiviewer.view.visibility import (
+from pkiviewer.view.theme import (
+    INDENT_PER_LEVEL,
     Visibility,
+    get_key_style,
+    get_key_value_styles,
+    get_style,
+    get_value_style,
+)
+from pkiviewer.view.visibility import (
     get_element_visibility,
-    get_extension_visibility,
     get_extension_value_visibility,
+    get_extension_visibility,
 )
-from pkiviewer.types import ExtensionDisplayMethod
-from pkiviewer.context import _console  # type: ignore
 
 
 def serial_number_display(cert_info: CertificateInfo, indent: int = 0) -> None:
     visibility = get_element_visibility(".Data.SerialNumber")
     if visibility != Visibility.HIDDEN:
         key_style, value_style = get_key_value_styles(visibility)
         serial_number = cert_info.get("serial_number", None)
         if serial_number is not None:
-            if serial_number < 2 ** 32:
+            if serial_number < 2**32:
                 print_key_value_oneline(
                     "Serial Number:",
                     int_to_hex_short(serial_number),
                     indent=indent,
                     key_style=key_style,
                     value_style=value_style,
                 )
@@ -337,48 +338,39 @@
                     )
                 )
 
     fingerprint_display(cert_info, indent=indent + 1)
     extensions_display(cert_info, indent=indent + 1)
 
 
-def certificate_header_display(cert_info: CertificateInfo, indent: int = 0):
-    filename_visibility = get_element_visibility(".Header.Filename")
+def certificate_header_display(
+    cert_info: CertificateInfo, indent: int = 0, show_filename: bool = True
+):
+    if not show_filename:
+        filename_visibility = Visibility.HIDDEN
+    else:
+        filename_visibility = get_element_visibility(".Header.Filename")
     filename = cert_info.get("filename", None)
     if filename_visibility == Visibility.HIDDEN or filename is None:
         print_key_oneline("Certificate:", indent=indent)
     else:
         value_style = get_style("info")
         print_key_value_oneline(
             "Certificate:", filename, indent=indent, value_style=value_style
         )
 
 
-def certificate_display(cert_info: CertificateInfo, indent: int = 0) -> None:
+def certificate_display(
+    cert_info: CertificateInfo, indent: int = 0, show_filename: bool = True
+) -> None:
     visibility = get_element_visibility(".Header")
     if visibility != Visibility.HIDDEN:
-        certificate_header_display(cert_info, indent)
+        certificate_header_display(cert_info, indent, show_filename)
         indent = indent + 1
 
     visibility = get_element_visibility(".Data")
     if visibility != Visibility.HIDDEN:
         certificate_data_display(cert_info, indent)
 
     visibility = get_element_visibility(".Signature")
     if visibility != Visibility.HIDDEN:
         certificate_signature_display(cert_info, indent=indent)
-
-
-def certificate_report_display(cert_info: CertificateInfo) -> None:
-    errors = cert_info.get("errors", [])
-    if errors:
-        key_style = get_style("error")
-        print_key_oneline("Errors:", key_style=key_style)
-        for error in errors:
-            print_error(cert_info["filename"], error, indent=1)  # type: ignore
-
-    warnings = cert_info.get("warnings", [])
-    if warnings:
-        key_style = get_style("warning")
-        print_key_oneline("Warnings:", key_style=key_style)
-        for warning in warnings:
-            print_warning(cert_info["filename"], warning, indent=1)  # type: ignore
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/crl.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/crl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,26 @@
+from pkiviewer.context import _console  # type: ignore; type: ignore
 from pkiviewer.model.crl import CertificateRevocationListInfo
-from pkiviewer.context import _console, _theme  # type: ignore
-
-from pkiviewer.view.theme import (
-    get_key_style,
-    get_value_style,
-    Visibility,
-    get_key_value_styles,
-)
+from pkiviewer.oid.names import OidNames
 from pkiviewer.view.console import (
     print_hex_multiline,
     print_key_oneline,
     print_key_value_multiline,
     print_key_value_oneline,
 )
 from pkiviewer.view.display import extension
-from pkiviewer.view.formatter import (
-    bytes_to_hex_long,
-    format_date_time,
-    format_name,
+from pkiviewer.view.formatter import bytes_to_hex_long, format_date_time, format_name
+from pkiviewer.view.theme import (
+    INDENT_PER_LEVEL,
+    Visibility,
+    get_key_style,
+    get_key_value_styles,
+    get_value_style,
 )
-from pkiviewer.oid import OidNames
-from pkiviewer.view.theme import INDENT_PER_LEVEL
-from pkiviewer.view.visibility import get_element_visibility, Visibility
-from pkiviewer.context import _console  # type: ignore
+from pkiviewer.view.visibility import get_element_visibility
 
 
 def issuer_display(crl_info: CertificateRevocationListInfo, indent: int = 0) -> None:
     visibility = get_element_visibility(".Data.Issuer")
     if visibility != Visibility.HIDDEN:
         key_style, value_style = get_key_value_styles(visibility)
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/__init__.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,58 @@
 from cryptography.x509.oid import ExtensionOID
 
-from pkiviewer.oid import Oid
+from pkiviewer.oid.names import Oid
 from pkiviewer.types import ExtensionDisplayMethod
-
-
 from pkiviewer.view.display.extension.authority_information_access import (
     authority_information_access_display,
 )
 from pkiviewer.view.display.extension.authority_key_identifier import (
     authority_key_identifier_display,
 )
-from pkiviewer.view.display.extension.basic_constraints import (
-    basic_constraints_display,
-)
+from pkiviewer.view.display.extension.basic_constraints import basic_constraints_display
 from pkiviewer.view.display.extension.certificate_policies import (
     certificate_policies_display,
 )
 from pkiviewer.view.display.extension.crl_distribution_ponts import (
     crl_distribution_points_display,
 )
+from pkiviewer.view.display.extension.crl_number import crl_number_display
 from pkiviewer.view.display.extension.extended_key_usage import (
     extended_key_usage_display,
 )
+from pkiviewer.view.display.extension.freshest_crl_display import freshest_crl_display
+from pkiviewer.view.display.extension.inhibit_any_policy import (
+    inhibit_any_policy_display,
+)
 from pkiviewer.view.display.extension.issuer_alternative_name import (
     issuer_alternative_name_display,
 )
+from pkiviewer.view.display.extension.issuing_distribution_point import (
+    issuing_distribution_point_display,
+)
 from pkiviewer.view.display.extension.key_usage import key_usage_display
+from pkiviewer.view.display.extension.name_constraints import name_constraints_display
+from pkiviewer.view.display.extension.not_implemented_by_cryptography import (
+    policy_constraints_display,
+    policy_mappings_display,
+    subject_directory_attributes_display,
+)
 from pkiviewer.view.display.extension.signed_certificate_timestamps import (
-    signed_certificate_timestamps_display,
     precertificate_signed_certificate_timestamps_display,
+    signed_certificate_timestamps_display,
 )
 from pkiviewer.view.display.extension.subject_alternative_name import (
     subject_alternative_name_display,
 )
 from pkiviewer.view.display.extension.subject_information_access import (
     subject_information_access_display,
 )
 from pkiviewer.view.display.extension.subject_key_identifier import (
     subject_key_identifier_display,
 )
-from pkiviewer.view.display.extension.not_implemented_by_cryptography import (
-    policy_mappings_display,
-)
-from pkiviewer.view.display.extension.not_implemented_by_cryptography import (
-    subject_directory_attributes_display,
-)
-from pkiviewer.view.display.extension.name_constraints import (
-    name_constraints_display,
-)
-from pkiviewer.view.display.extension.not_implemented_by_cryptography import (
-    policy_constraints_display,
-)
-from pkiviewer.view.display.extension.inhibit_any_policy import (
-    inhibit_any_policy_display,
-)
-from pkiviewer.view.display.extension.freshest_crl_display import (
-    freshest_crl_display,
-)
-from pkiviewer.view.display.extension.crl_number import crl_number_display
-from pkiviewer.view.display.extension.issuing_distribution_point import (
-    issuing_distribution_point_display,
-)
-
 
 v3_extension_display: dict[Oid, ExtensionDisplayMethod] = {
     # RFC5280
     ExtensionOID.AUTHORITY_INFORMATION_ACCESS.dotted_string: authority_information_access_display,
     ExtensionOID.AUTHORITY_KEY_IDENTIFIER.dotted_string: authority_key_identifier_display,
     ExtensionOID.BASIC_CONSTRAINTS.dotted_string: basic_constraints_display,
     ExtensionOID.CERTIFICATE_POLICIES.dotted_string: certificate_policies_display,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/authority_information_access.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/authority_information_access.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import cast
 
 from pkiviewer.model.extension.authority_information_access import (
     AuthorityInformationAccessInfo,
 )
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_value_oneline
 from pkiviewer.view.theme import get_value_style
 from pkiviewer.view.visibility import Visibility
-from pkiviewer.context import _console  # type: ignore
 
 
 # RFC5280 4.2.2.1
 def authority_information_access_display(
     extension_info: X509ExtensionInfo,
     indent: int = 0,
     visibility: Visibility = Visibility.NORMAL,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/authority_key_identifier.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/authority_key_identifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import cast
 
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.context import _console  # type: ignore
 from pkiviewer.model.extension.authority_key_identifier import (
     AuthorityKeyIdentifierInfo,
 )
-from pkiviewer.view.formatter import bytes_to_hex_long
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import (
-    print_key_oneline,
     print_hex_multiline,
+    print_key_oneline,
     print_key_value_multiline,
 )
-from pkiviewer.view.theme import get_key_style, get_value_style, INDENT_PER_LEVEL
+from pkiviewer.view.formatter import bytes_to_hex_long
+from pkiviewer.view.theme import INDENT_PER_LEVEL, get_key_style, get_value_style
 from pkiviewer.view.visibility import Visibility
-from pkiviewer.context import _console  # type: ignore
+
 
 # RFC5280 4.2.1.1
 # TODO: authority_key_identifier_display  cert_issuer, cert_serial_number
 def authority_key_identifier_display(
     extension_info: X509ExtensionInfo,
     indent: int = 0,
     visibility: Visibility = Visibility.NORMAL,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/basic_constraints.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/basic_constraints.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from typing import cast
 
-from pkiviewer.model.extension.basic_constraints import (
-    BasicConstraintsInfo,
-)
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.model.extension.basic_constraints import BasicConstraintsInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_value_oneline
 from pkiviewer.view.theme import get_value_style
 from pkiviewer.view.visibility import Visibility
-from pkiviewer.context import _console  # type: ignore
 
 
 # RFC5280 4.2.1.9
 def basic_constraints_display(
     extension_info: X509ExtensionInfo,
     indent: int = 0,
     visibility: Visibility = Visibility.NORMAL,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/certificate_policies.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/certificate_policies.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from typing import cast
 
-from pkiviewer.model.extension.certificate_policy import (
-    CertificatePoliciesInfo,
-)
-from pkiviewer.model import X509ExtensionInfo
-from pkiviewer.oid import OidNames
-from pkiviewer.view.console import print_value_multiline, print_key_oneline
-from pkiviewer.view.theme import get_value_style, get_key_style
+from pkiviewer.model.extension.certificate_policy import CertificatePoliciesInfo
+from pkiviewer.oid.names import OidNames
+from pkiviewer.types import X509ExtensionInfo
+from pkiviewer.view.console import print_key_oneline, print_value_multiline
+from pkiviewer.view.theme import get_key_style, get_value_style
 from pkiviewer.view.visibility import Visibility
-from pkiviewer.context import _console  # type: ignore
 
 
 # RFC5280 4.2.1.4
 def policy_value_display(
     value: str,
     indent: int = 0,
     visibility: Visibility = Visibility.NORMAL,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/crl_distribution_ponts.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/crl_distribution_ponts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import cast
 
-from pkiviewer.model.extension.crl_distribution_points import (
-    CRLDistributionPointsInfo,
-)
-from pkiviewer.model import X509ExtensionInfo
-from pkiviewer.view.console import print_value_oneline, print_key_oneline
-from pkiviewer.view.theme import get_value_style, get_key_style
+from pkiviewer.model.extension.crl_distribution_points import CRLDistributionPointsInfo
+from pkiviewer.types import X509ExtensionInfo
+from pkiviewer.view.console import print_key_oneline, print_value_oneline
+from pkiviewer.view.theme import get_key_style, get_value_style
 from pkiviewer.view.visibility import Visibility
 
 
 # RFC5280 4.2.1.13
 def crl_distribution_points_display(
     extension_info: X509ExtensionInfo,
     indent: int = 0,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/crl_number.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/crl_number.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import cast
 
 from pkiviewer.model.extension.crl_number import CRLNumberInfo
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_key_value_oneline
-from pkiviewer.view.theme import get_value_style, get_key_style
+from pkiviewer.view.theme import get_key_style, get_value_style
 from pkiviewer.view.visibility import Visibility
 
 
 # RFC5280 5.2.3
 def crl_number_display(
     extension_info: X509ExtensionInfo,
     indent: int = 0,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/extended_key_usage.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/extended_key_usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from typing import cast
 
-from pkiviewer.model.extension.extended_key_usage import (
-    ExtendedKeyUsageInfo,
-)
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.model.extension.extended_key_usage import ExtendedKeyUsageInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_value_oneline
 from pkiviewer.view.theme import get_value_style
 from pkiviewer.view.visibility import Visibility
 
 
 # RFC5280 4.2.1.12
 def extended_key_usage_display(
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/freshest_crl_display.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/freshest_crl_display.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import cast
 
 from pkiviewer.model.extension.freshest_crl import FreshestCRLInfo
-from pkiviewer.model import X509ExtensionInfo
-from pkiviewer.view.console import print_value_oneline, print_key_oneline
-from pkiviewer.view.theme import get_value_style, get_key_style
+from pkiviewer.types import X509ExtensionInfo
+from pkiviewer.view.console import print_key_oneline, print_value_oneline
+from pkiviewer.view.theme import get_key_style, get_value_style
 from pkiviewer.view.visibility import Visibility
 
 
 # RFC5280 4.2.1.15
 def freshest_crl_display(
     extension_info: X509ExtensionInfo,
     indent: int = 0,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/header.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/header.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_key_value_oneline
 from pkiviewer.view.theme import get_key_style, get_style, get_value_style
 from pkiviewer.view.visibility import (
+    Visibility,
     get_element_visibility,
     get_extension_value_visibility,
-    Visibility,
 )
 
 
 def extension_header_display(extension_info: X509ExtensionInfo, indent: int):
     extension_name = extension_info["name"]
     extension_type = extension_info["info"]["type"]
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/inhibit_any_policy.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/inhibit_any_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import cast
 
-from pkiviewer.model.extension.inhibit_any_policy import (
-    InhibitAnyPolicyInfo,
-)
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.model.extension.inhibit_any_policy import InhibitAnyPolicyInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_key_value_oneline
-from pkiviewer.view.theme import get_value_style, get_key_style
+from pkiviewer.view.theme import get_key_style, get_value_style
 from pkiviewer.view.visibility import Visibility
 
 
 # RFC5280 4.2.1.14
 def inhibit_any_policy_display(
     extension_info: X509ExtensionInfo,
     indent: int = 0,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/issuer_alternative_name.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/subject_alternative_name.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import cast
 
-from pkiviewer.model.extension.issuer_alternative_name import (
-    IssuerAlternativeNameInfo,
+from pkiviewer.model.extension.subject_alternative_name import (
+    SubjectAlternativeNameInfo,
 )
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_value_multiline
 from pkiviewer.view.theme import get_value_style
 from pkiviewer.view.visibility import Visibility
 
 
-# RFC5280 4.2.1.7
-def issuer_alternative_name_display(
+# RFC5280 4.2.1.6
+def subject_alternative_name_display(
     extension_info: X509ExtensionInfo,
     indent: int = 0,
     visibility: Visibility = Visibility.NORMAL,
 ) -> None:
-    info = cast(IssuerAlternativeNameInfo, extension_info["info"])
+    info = cast(SubjectAlternativeNameInfo, extension_info["info"])
     value_style = get_value_style(visibility)
-    for name, addresses in info["ians"].items():
+    for name, addresses in info["sans"].items():
         items = [f"{name}:{address}" for address in addresses]
         text = ", ".join(items)
         print_value_multiline(text, indent=indent, value_style=value_style)
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/issuing_distribution_point.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/issuing_distribution_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import cast
 
 from pkiviewer.model.extension.issuing_distribution_point import (
     IssuingDistributionPointInfo,
 )
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_key_oneline, print_value_oneline
-from pkiviewer.view.theme import get_value_style, get_key_style
+from pkiviewer.view.theme import get_key_style, get_value_style
 from pkiviewer.view.visibility import Visibility
 
 
 # RFC5280 5.2.5
 def issuing_distribution_point_display(
     extension_info: X509ExtensionInfo,
     indent: int = 0,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/key_usage.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/key_usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from typing import cast
 
-from pkiviewer.model.extension.key_usage import (
-    KeyUsageInfo,
-)
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.model.extension.key_usage import KeyUsageInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_value_oneline
 from pkiviewer.view.theme import get_value_style
 from pkiviewer.view.visibility import Visibility
 
 
 # RFC5280 4.2.1.3
 def key_usage_display(
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/name_constraints.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/name_constraints.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from typing import cast
 
-from pkiviewer.model.extension.name_constraints import (
-    NameConstraintsInfo,
-)
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.model.extension.name_constraints import NameConstraintsInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_value_oneline
 from pkiviewer.view.theme import get_value_style
 from pkiviewer.view.visibility import Visibility
 
 
 # RFC5280 4.2.1.10
 def name_constraints_display(
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/not_implemented_by_cryptography.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/not_implemented_by_cryptography.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.visibility import Visibility
 
 # NOTE: No information provided by the cryptography module for these extensions
 # See https://github.com/pyca/cryptography/issues/1947
 
 
 # RFC5280 4.2.1.11
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/signed_certificate_timestamps.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/signed_certificate_timestamps.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 from typing import cast
 
 from cryptography.x509.certificate_transparency import SignedCertificateTimestamp
 
-from pkiviewer.model.extension.signed_certificate_timestamps import (
-    SignedCertificateTimestampsInfo,
-)
 from pkiviewer.model.extension.precertificate_signed_certificate_timestamps import (
     PreCertificateSignedCertificateTimestampsInfo,
 )
-from pkiviewer.model import X509ExtensionInfo
-from pkiviewer.view.formatter import (
-    bytes_to_hex_long,
-    format_date_time,
-    format_version,
+from pkiviewer.model.extension.signed_certificate_timestamps import (
+    SignedCertificateTimestampsInfo,
 )
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import (
+    print_hex_multiline,
     print_key_oneline,
     print_key_value_oneline,
-    print_hex_multiline,
 )
-from pkiviewer.view.theme import get_value_style, get_key_style
+from pkiviewer.view.formatter import bytes_to_hex_long, format_date_time, format_version
+from pkiviewer.view.theme import get_key_style, get_value_style
 from pkiviewer.view.visibility import Visibility
-from pkiviewer.context import _console  # type: ignore
 
 
 def sct_display(
     sct: SignedCertificateTimestamp, indent: int, visibility: Visibility
 ) -> None:
     value_style = get_value_style(visibility)
     key_style = get_key_style(visibility)
     key_indent = indent
     value_indent = key_indent + 1
     print_key_oneline("Signed Certificate Timestamp:", key_indent, key_style=key_style)
     print_key_value_oneline(
-        f"Version:",
+        "Version:",
         format_version(sct.version),
         value_indent,
         key_style=key_style,
         value_style=value_style,
     )
     log_id = bytes_to_hex_long(sct.log_id)
-    print_key_oneline(f"Log ID:", value_indent, key_style=key_style)
+    print_key_oneline("Log ID:", value_indent, key_style=key_style)
     print_hex_multiline(
         log_id, indent=value_indent + 1, stride=16, value_style=value_style
     )
     print_key_value_oneline(
         "Timestamp:",
         format_date_time(sct.timestamp),
         value_indent,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/subject_alternative_name.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/issuer_alternative_name.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from typing import cast
 
-from pkiviewer.model.extension.subject_alternative_name import (
-    SubjectAlternativeNameInfo,
-)
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.model.extension.issuer_alternative_name import IssuerAlternativeNameInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_value_multiline
 from pkiviewer.view.theme import get_value_style
 from pkiviewer.view.visibility import Visibility
-from pkiviewer.context import _console  # type: ignore
 
 
-# RFC5280 4.2.1.6
-def subject_alternative_name_display(
+# RFC5280 4.2.1.7
+def issuer_alternative_name_display(
     extension_info: X509ExtensionInfo,
     indent: int = 0,
     visibility: Visibility = Visibility.NORMAL,
 ) -> None:
-    info = cast(SubjectAlternativeNameInfo, extension_info["info"])
+    info = cast(IssuerAlternativeNameInfo, extension_info["info"])
     value_style = get_value_style(visibility)
-    for name, addresses in info["sans"].items():
+    for name, addresses in info["ians"].items():
         items = [f"{name}:{address}" for address in addresses]
         text = ", ".join(items)
         print_value_multiline(text, indent=indent, value_style=value_style)
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/subject_information_access.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/subject_information_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import cast
 
 from pkiviewer.model.extension.subject_information_access import (
     SubjectInformationAccessInfo,
 )
-from pkiviewer.model import X509ExtensionInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_value_oneline
 from pkiviewer.view.theme import get_value_style
 from pkiviewer.view.visibility import Visibility
 
 
 # RFC5280 4.2.2.2
 def subject_information_access_display(
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/extension/subject_key_identifier.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/extension/subject_key_identifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from typing import cast
 
-from pkiviewer.model.extension.subject_key_identifier import (
-    SubjectKeyIdentifierInfo,
-)
-from pkiviewer.model import X509ExtensionInfo
-from pkiviewer.view.formatter import bytes_to_hex_long
+from pkiviewer.model.extension.subject_key_identifier import SubjectKeyIdentifierInfo
+from pkiviewer.types import X509ExtensionInfo
 from pkiviewer.view.console import print_value_oneline
+from pkiviewer.view.formatter import bytes_to_hex_long
 from pkiviewer.view.theme import get_value_style
 from pkiviewer.view.visibility import Visibility
-from pkiviewer.context import _console  # type: ignore
 
 
 # RFC5280 4.2.1.2
 def subject_key_identifier_display(
     extension_info: X509ExtensionInfo,
     indent: int = 0,
     visibility: Visibility = Visibility.NORMAL,
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/p12.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/p12.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from pkiviewer.model.p12 import PKCS12KeyAndCertificateInfo
-
-from pkiviewer.view.theme import Visibility
-from pkiviewer.view.console import print_key_oneline
+from pkiviewer.view.console import print_key_oneline, print_key_value_oneline
 from pkiviewer.view.display.certificate import certificate_display
-from pkiviewer.view.visibility import get_element_visibility, Visibility
+from pkiviewer.view.theme import get_style
+from pkiviewer.view.visibility import Visibility, get_element_visibility
 
 
 def p12_display(
     p12_info: PKCS12KeyAndCertificateInfo,
 ) -> None:
-    print_key_oneline("PKCS#12:")
+    filename_visibility = get_element_visibility(".Header.Filename")
+    filename = p12_info.get("filename", None)
+    if filename_visibility == Visibility.HIDDEN or filename is None:
+        print_key_oneline("PKCS#12:", indent=0)
+    else:
+        value_style = get_style("info")
+        print_key_value_oneline("PKCS#12:", filename, indent=0, value_style=value_style)
 
     visibility = get_element_visibility(".P12.Certificate")
     cert = p12_info.get("certificate", None)
     if visibility != Visibility.HIDDEN and cert is not None:
-        certificate_display(cert, indent=1)
+        certificate_display(cert, indent=1, show_filename=False)
 
     visibility = get_element_visibility(".P12.AdditionalCertificates")
     additional_certs = p12_info.get("additional_certs", None)
     if visibility != Visibility.HIDDEN and additional_certs is not None:
         print_key_oneline("Additional Certificates:", indent=1)
         for cert in additional_certs:
-            certificate_display(cert, indent=2)
+            certificate_display(cert, indent=2, show_filename=False)
 
     visibility = get_element_visibility(".P12.PrivateKey")
 
     # TODO: Private Keys
     # private_key = p12_info.get("private_key", None)
     # if visibility != Visibility.HIDDEN and private_key is not None:
     #     print_key_oneline("Private Key:", indent=1)
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/dh.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/dh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pkiviewer.model.public_key.dh import DHPublicKeyInfo
-from pkiviewer.view.visibility import get_element_visibility, Visibility
 from pkiviewer.view.console import (
     print_hex_multiline,
     print_key_oneline,
     print_key_value_oneline,
 )
 from pkiviewer.view.formatter import int_to_hex_long
 from pkiviewer.view.theme import get_key_value_styles
+from pkiviewer.view.visibility import Visibility, get_element_visibility
 
 
 def print_dh_info(key_info: DHPublicKeyInfo, indent: int = 0):
     visibility = get_element_visibility(".Data.Subject.PublicKey.Algorithm")
     if visibility != Visibility.HIDDEN:
         key_style, value_style = get_key_value_styles(visibility)
         print_key_value_oneline(
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/dsa.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/dsa.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pkiviewer.model.public_key.dsa import DSAPublicKeyInfo
-from pkiviewer.view.visibility import get_element_visibility, Visibility
 from pkiviewer.view.console import (
     print_hex_multiline,
     print_key_oneline,
     print_key_value_oneline,
 )
 from pkiviewer.view.formatter import int_to_hex_long
 from pkiviewer.view.theme import get_key_value_styles
+from pkiviewer.view.visibility import Visibility, get_element_visibility
 
 
 def print_dsa_info(key_info: DSAPublicKeyInfo, indent: int = 0):
     visibility = get_element_visibility(".Data.Subject.PublicKey.Algorithm")
     if visibility != Visibility.HIDDEN:
         key_style, value_style = get_key_value_styles(visibility)
         print_key_value_oneline(
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/ed25519.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/ed25519.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pkiviewer.model.public_key.ed25519 import Ed25519PublicKeyInfo
-from pkiviewer.view.visibility import get_element_visibility, Visibility
 from pkiviewer.view.console import (
     print_hex_multiline,
     print_key_oneline,
     print_key_value_oneline,
 )
 from pkiviewer.view.formatter import bytes_to_hex_long
 from pkiviewer.view.theme import get_key_value_styles
+from pkiviewer.view.visibility import Visibility, get_element_visibility
 
 
 def print_ed25519_info(key_info: Ed25519PublicKeyInfo, indent: int = 0):
     visibility = get_element_visibility(".Data.Subject.PublicKey.Algorithm")
     if visibility != Visibility.HIDDEN:
         key_style, value_style = get_key_value_styles(visibility)
         print_key_value_oneline(
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/ed448.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/ed448.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pkiviewer.model.public_key.ed448 import Ed448PublicKeyInfo
-from pkiviewer.view.visibility import get_element_visibility, Visibility
 from pkiviewer.view.console import (
     print_hex_multiline,
     print_key_oneline,
     print_key_value_oneline,
 )
 from pkiviewer.view.formatter import bytes_to_hex_long
 from pkiviewer.view.theme import get_key_value_styles
+from pkiviewer.view.visibility import Visibility, get_element_visibility
 
 
 def print_ed448_info(key_info: Ed448PublicKeyInfo, indent: int = 0):
     visibility = get_element_visibility(".Data.Subject.PublicKey.Algorithm")
     if visibility != Visibility.HIDDEN:
         key_style, value_style = get_key_value_styles(visibility)
         print_key_value_oneline(
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/elliptic_curve.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/rsa.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from pkiviewer.model.public_key.elliptic_curve import EllipticCurvePublicKeyInfo
-from pkiviewer.view.visibility import get_element_visibility, Visibility
+from pkiviewer.model.public_key.rsa import RSAPublicKeyInfo
 from pkiviewer.view.console import (
-    print_key_oneline,
     print_hex_multiline,
+    print_key_oneline,
     print_key_value_oneline,
 )
-from pkiviewer.view.formatter import bytes_to_hex_long
+from pkiviewer.view.formatter import int_to_hex_long
 from pkiviewer.view.theme import get_key_value_styles
+from pkiviewer.view.visibility import Visibility, get_element_visibility
 
 
-def print_ec_info(key_info: EllipticCurvePublicKeyInfo, indent: int = 0):
+def print_rsa_info(key_info: RSAPublicKeyInfo, indent: int = 0):
     visibility = get_element_visibility(".Data.Subject.PublicKey.Algorithm")
     if visibility != Visibility.HIDDEN:
         key_style, value_style = get_key_value_styles(visibility)
         print_key_value_oneline(
             "Public Key Algorithm:",
             key_info["name"],
             indent=indent,
             key_style=key_style,
             value_style=value_style,
         )
+
         print_key_value_oneline(
-            "Public-Key", f"({key_info['key_size']} bit)", indent=indent + 1
+            "RSA Public-Key", f"({key_info['key_size']} bit)", indent=indent + 1
         )
-        print_key_oneline("pub:", indent=indent + 1)
-        hex_str = bytes_to_hex_long(key_info["pub"])
-        print_hex_multiline(hex_str, indent=indent + 2)
-
-        print_key_value_oneline("ASN1 OID:", key_info["asn1_oid"], indent=indent + 1)
+        print_key_oneline("Modulus:", indent=indent + 1)
+        print_hex_multiline(int_to_hex_long(key_info["modulus"]), indent=indent + 2)
         print_key_value_oneline(
-            "NIST CURVE:", key_info["nist_curve"], indent=indent + 1
+            "Exponent",
+            f"{key_info['exponent']} ({hex(key_info['exponent'])})",
+            indent=indent + 1,
         )
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/display/public_key/rsa.py` & `pkiviewer-0.2.1/src/pkiviewer/view/display/public_key/elliptic_curve.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from pkiviewer.model.public_key.rsa import RSAPublicKeyInfo
-from pkiviewer.view.visibility import get_element_visibility, Visibility
+from pkiviewer.model.public_key.elliptic_curve import EllipticCurvePublicKeyInfo
 from pkiviewer.view.console import (
     print_hex_multiline,
     print_key_oneline,
     print_key_value_oneline,
 )
-from pkiviewer.view.formatter import int_to_hex_long
+from pkiviewer.view.formatter import bytes_to_hex_long
 from pkiviewer.view.theme import get_key_value_styles
+from pkiviewer.view.visibility import Visibility, get_element_visibility
 
 
-def print_rsa_info(key_info: RSAPublicKeyInfo, indent: int = 0):
+def print_ec_info(key_info: EllipticCurvePublicKeyInfo, indent: int = 0):
     visibility = get_element_visibility(".Data.Subject.PublicKey.Algorithm")
     if visibility != Visibility.HIDDEN:
         key_style, value_style = get_key_value_styles(visibility)
         print_key_value_oneline(
             "Public Key Algorithm:",
             key_info["name"],
             indent=indent,
             key_style=key_style,
             value_style=value_style,
         )
-
         print_key_value_oneline(
-            "RSA Public-Key", f"({key_info['key_size']} bit)", indent=indent + 1
+            "Public-Key", f"({key_info['key_size']} bit)", indent=indent + 1
         )
-        print_key_oneline("Modulus:", indent=indent + 1)
-        print_hex_multiline(int_to_hex_long(key_info["modulus"]), indent=indent + 2)
+        print_key_oneline("pub:", indent=indent + 1)
+        hex_str = bytes_to_hex_long(key_info["pub"])
+        print_hex_multiline(hex_str, indent=indent + 2)
+
+        print_key_value_oneline("ASN1 OID:", key_info["asn1_oid"], indent=indent + 1)
         print_key_value_oneline(
-            "Exponent",
-            f"{key_info['exponent']} ({hex(key_info['exponent'])})",
-            indent=indent + 1,
+            "NIST CURVE:", key_info["nist_curve"], indent=indent + 1
         )
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/formatter.py` & `pkiviewer-0.2.1/src/pkiviewer/view/formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import datetime
 from typing import Generator
 
+import cryptography.x509.name
 from cryptography.x509 import Version as CertificateVersion
 from cryptography.x509.certificate_transparency import (
     Version as CertificateTransparencyVersion,
 )
-import cryptography.x509.name
 
 
 def _chunk(value: str, stride: int) -> Generator[str, None, None]:
     for idx in range(0, len(value), stride):
-        yield value[idx : idx + stride]
+        yield value[idx : idx + stride]  # noqa: E203
 
 
 def chunk(value: str, stride: int) -> list[str]:
     return list(_chunk(value, stride))
 
 
 def hex_string_long(value: int) -> str:
```

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/theme.py` & `pkiviewer-0.2.1/src/pkiviewer/view/theme.py`

 * *Files identical despite different names*

### Comparing `pkiviewer-0.2.0/src/pkiviewer/view/visibility.py` & `pkiviewer-0.2.1/src/pkiviewer/view/visibility.py`

 * *Files identical despite different names*

### Comparing `pkiviewer-0.2.0/tests/file/google.crl` & `pkiviewer-0.2.1/tests/file/google.crl`

 * *Files identical despite different names*

### Comparing `pkiviewer-0.2.0/tests/file/microsoft.pem` & `pkiviewer-0.2.1/tests/file/microsoft.pem`

 * *Files 0% similar despite different names*

```diff
@@ -417,8 +417,8 @@
 00001a00: 700a 6255 4354 7543 5039 732b 594f 5269  p.bUCTuCP9s+YORi
 00001a10: 4471 4152 4452 4f59 4851 582b 624b 6951  DqARDROYHQX+bKiQ
 00001a20: 3556 7178 7349 7438 6661 5779 6b47 746b  5VqxsIt8faWykGtk
 00001a30: 7451 5054 686f 4351 576c 7358 4a68 4e68  tQPThoCQWlsXJhNh
 00001a40: 6f49 0a6f 3478 6b43 416d 4b77 6472 4355  oI.o4xkCAmKwdrCU
 00001a50: 6d72 455a 7974 4f55 413d 3d0a 2d2d 2d2d  mrEZytOUA==.----
 00001a60: 2d45 4e44 2043 4552 5449 4649 4341 5445  -END CERTIFICATE
-00001a70: 2d2d 2d2d 2d0a 0a                        -----..
+00001a70: 2d2d 2d2d 2d0a                           -----.
```

### Comparing `pkiviewer-0.2.0/tests/integration/test_bad_naming_constraints.py` & `pkiviewer-0.2.1/tests/integration/test_bad_naming_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 BAUiksQ1KTiW8LyF9IRjckpkf1RH9pqBD8vVeunEpXOUPGOfseL5AAXbvYI6iN70
 aCxKkiRwqX7ZK0lL9Oh+hhaVqqdPnGxb+O3ZX/88FvKvWiicnftMx56lzv4H
 -----END CERTIFICATE-----
 """
 
 
 def test_bad_naming_constraints_no_error_when_loading():
-    _cert = load_pem_x509_certificate(bad_naming_constraints.encode("ascii"))
+    load_pem_x509_certificate(bad_naming_constraints.encode("ascii"))
 
 
 def test_bad_naming_constraints_error_when_accessing():
     cert = load_pem_x509_certificate(bad_naming_constraints.encode("ascii"))
 
     with pytest.raises(ValueError):
         for _ext in cert.extensions:
```

### Comparing `pkiviewer-0.2.0/tests/unit/test_certificate_pem_read.py` & `pkiviewer-0.2.1/tests/unit/test_certificate_pem_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
-from cryptography.x509.base import Certificate
 
 import pytest
+from cryptography.x509.base import Certificate
 
-from pkiviewer.view import rich_init
 from pkiviewer.config import config_load
 from pkiviewer.io import load
 from pkiviewer.model.certificate import certiticate_parse
+from pkiviewer.view import rich_init
 
 
 @pytest.mark.parametrize(
     "cert_file",
     ["microsoft.pem"],
 )
 def test_certificate_parsing(cert_file: str):
@@ -18,8 +18,8 @@
     rich_init()
 
     p = Path(__file__).parent
     fullpath = p / ".." / "file" / cert_file
     fullpath = fullpath.resolve()
     certificates = load(fullpath)
     if isinstance(certificates[0], Certificate):
-        _info = certiticate_parse(certificates[0], fullpath.name)
+        certiticate_parse(certificates[0], fullpath.name)
```

### Comparing `pkiviewer-0.2.0/tests/unit/test_formatting.py` & `pkiviewer-0.2.1/tests/unit/test_formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pkiviewer.view.formatter import int_to_hex_long, bytes_to_hex_long, chunk
+from pkiviewer.view.formatter import bytes_to_hex_long, chunk, int_to_hex_long
 
 
 def test_int_to_hex_long():
     assert (
         int_to_hex_long(117869795089791359327594732455184760935)
         == "58:ac:e5:94:0b:41:78:64:12:9d:53:1a:39:cb:00:67"
     )
```

### Comparing `pkiviewer-0.2.0/tests/unit/test_merge_configuration.py` & `pkiviewer-0.2.1/tests/unit/test_merge_configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
-from pkiviewer.config import merge, MergeError
+
+from pkiviewer.config import MergeError, merge
 
 
 def test_MergeEmptyConfigWithNonEmptyShouldPass():
     a = {}
     b = {"a": 1, "b": [1, 2, 3]}
 
     c = merge(a, b)
@@ -31,23 +32,23 @@
 
 
 def test_MergeValueWithListShouldFail():
     a = {"b": 2}
     b = {"b": [1, 2, 3]}
 
     with pytest.raises(MergeError):
-        _c = merge(a, b)
+        merge(a, b)
 
 
 def test_MergeValueWithDictShouldFail():
     a = {"b": 2}
     b = {"b": {"c": 1}}
 
     with pytest.raises(MergeError):
-        _c = merge(a, b)
+        merge(a, b)
 
 
 def test_MergeListWithValueShouldPass():
     a = {"b": [1, 2, 3]}
     b = {"b": 4}
 
     c = merge(a, b)
@@ -63,31 +64,31 @@
 
 
 def test_MergeListWithDictShouldFail():
     a = {"b": [1, 2, 3]}
     b = {"b": {"c": 1}}
 
     with pytest.raises(MergeError):
-        _c = merge(a, b)
+        merge(a, b)
 
 
 def test_MergeDictWithValueShouldFail():
     a = {"b": {"c": 1}}
     b = {"b": 1}
 
     with pytest.raises(MergeError):
-        _c = merge(a, b)
+        merge(a, b)
 
 
 def test_MergeDictWithListShouldFail():
     a = {"b": {"c": 1}}
     b = {"b": [1, 2, 3]}
 
     with pytest.raises(MergeError):
-        _c = merge(a, b)
+        merge(a, b)
 
 
 def test_MergeDictWithDictSameTypesShouldPass():
     a = {"b": {"c": 1}}
     b = {"b": {"d": 2}}
 
     c = merge(a, b)
@@ -101,8 +102,8 @@
 
 
 def test_MergeDictWithDictDifferentTypesShouldFail():
     a = {"b": {"c": 1}}
     b = {"b": {"c": [1, 2, 3]}}
 
     with pytest.raises(MergeError):
-        _c = merge(a, b)
+        merge(a, b)
```

### Comparing `pkiviewer-0.2.0/tests/unit/test_visibility.py` & `pkiviewer-0.2.1/tests/unit/test_visibility.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pkiviewer.config import Configuration
 from pkiviewer.view.visibility import (
     Visibility,
     get_element_visibility,
-    set_element_visibility,
-    get_extension_visibility,
     get_extension_value_visibility,
+    get_extension_visibility,
+    set_element_visibility,
 )
 
 
 def test_element_visibility_is_normal(config: Configuration):
     assert get_element_visibility(".Header") == Visibility.NORMAL
```

### Comparing `pkiviewer-0.2.0/setup.py` & `pkiviewer-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,268 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pkiviewer
+Version: 0.2.1
+Summary: PKI file viewer
+Home-page: https://github.com/sffjunkie/pkiviewer
+License: Apache-2.0
+Author: Simon Kennedy
+Author-email: sffjunkie+code@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: asn1tools (>=0.163.0,<0.164.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: cryptography (>=37.0.4,<38.0.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Project-URL: Issue Tracker, https://github.com/sffjunkie/pkiviewer/issues
+Project-URL: Repository, https://github.com/sffjunkie/pkiviewer
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# PKI Viewer
 
-packages = \
-['pkiviewer',
- 'pkiviewer.asn1',
- 'pkiviewer.model',
- 'pkiviewer.model.extension',
- 'pkiviewer.model.public_key',
- 'pkiviewer.oid',
- 'pkiviewer.utils',
- 'pkiviewer.view',
- 'pkiviewer.view.display',
- 'pkiviewer.view.display.extension',
- 'pkiviewer.view.display.public_key']
-
-package_data = \
-{'': ['*'], 'pkiviewer.asn1': ['specs/*']}
-
-modules = \
-['py']
-install_requires = \
-['asn1tools>=0.163.0,<0.164.0',
- 'click>=8.1.3,<9.0.0',
- 'cryptography>=37.0.4,<38.0.0',
- 'rich>=12.5.1,<13.0.0',
- 'tomli>=2.0.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['pkiviewer = pkiviewer.__main__:run']}
-
-setup_kwargs = {
-    'name': 'pkiviewer',
-    'version': '0.2.0',
-    'description': 'PKI file viewer',
-    'long_description': '# PKI Viewer\n\nDisplays information in the terminal from the following PKI file types\n\n- Certificates\n- PKCS#12 files\n- Certificate Signing Request (Coming Soon™)\n- Certificate Revocation List\n\nAlso Coming Soon™ is Certificate Transparency information.\n\n## Features\n\n1. Files can be in either PEM or DER formats\n\n1. If a URL is passed a certificate will be downloaded automatically\n\n1. The certificate information can be output to the terminal, an SVG file or an HTML file.\n\n1. The information that is displayed can be configured (either hidden, displayed dim or highlighted)\n\n1. The colors can be configured\n\n1. Uses [rich](https://rich.readthedocs.io/en/latest/) for the\n   fancy output/SVG & HTML generation and\n   [cryptography](https://cryptography.io/en/latest/) for the low level parsing.\n\n1. It sticks fairly closely to the output from the `openssl` binary\n\nDER format certificates should have the extension `.cer` and PKCS#12 `.p12`\n\n## PKCS#12 Files\n\nIf the PKCS#12 file is encrypted you will be prompted to enter the passsword\n\n## Usage\n\nOutput certificate information to the terminal\n\n```\npkiviewer testcert.pem   OR   pkiviewer https://bbc.com\n```\n\nFor example\n\n```\npkiviewer https://bbc.com\n```\n\nproduces the following output\n\n```\nCertificate: https://bbc.com\n    Data:\n        Version: 1 (0x0)\n        Serial Number:\n            3e:55:35:3c:c9:9b:cb:59:6e:be:fc:64\n        Signature Algorithm: RSA with SHA256\n        Issuer: C = BE, O = GlobalSign nv-sa, CN = GlobalSign RSA OV SSL CA 2018\n        Validity:\n            Not Before: Mar 04 13:51:12 2022 UTC\n            Not After:  Apr 05 13:51:11 2023 UTC\n        Subject:\n            C = GB, ST = London, L = London, O = BRITISH BROADCASTING CORPORATION, CN = www.bbc.com\n        Subject Public Key Info:\n            Public Key Algorithm: RSA\n                RSA Public-Key (2048 bit)\n                Modulus:\n                    c1:91:f9:55:15:2b:77:96:e3:a5:62:2b:1c:4b:2e:8f:e3:c9:f9:76:bd:91:d4:96:\n                    28:7e:2e:b4:a9:6a:62:71:50:74:8e:d9:ef:5d:8d:ab:fc:d9:b8:1a:f8:30:01:82:\n                    30:45:15:32:e0:f8:64:53:5d:c2:92:0b:44:29:81:5b:b0:83:bf:df:c5:b4:56:e3:\n                    7b:af:54:cf:4c:1f:6c:46:ca:b7:21:ae:bc:f5:48:93:ff:ef:f0:37:7c:16:b3:92:\n                    c1:be:36:54:78:e0:06:86:64:c1:74:4d:39:c7:79:2d:1f:e4:99:bd:fc:1b:5e:29:\n                    bc:c4:ce:8c:aa:76:81:e0:c6:30:08:ea:21:e1:b9:81:1e:08:ea:7d:31:f3:3f:b3:\n                    77:98:71:53:00:45:a6:97:a3:54:f5:25:87:eb:81:97:86:45:ef:47:3d:3e:a4:14:\n                    2c:06:9d:18:a2:4e:26:5c:bd:b8:c5:a6:53:5d:65:7b:e9:02:52:77:26:10:b5:44:\n                    e1:e0:79:a2:ef:29:d3:1b:37:46:27:67:ef:bb:5e:78:58:05:94:5b:3d:82:d8:4d:\n                    d8:28:32:b9:e8:e2:5e:65:58:f8:fc:b0:79:f8:fc:23:4f:6a:33:ff:b8:60:96:9a:\n                    bc:9b:8c:46:24:8d:fc:5d:13:19:32:ac:ff:a4:f8:91\n                Exponent 65537 (0x10001)\n                Fingerprint (SHA256):\n                    66:dd:b2:a9:e1:f4:52:2f:3b:06:e3:de:6a:76:b3:f0:18:b8:3a:e5:54:7e:71:15:\n                    83:68:5c:d7:6a:3d:17:84\n        X509v3 Extensions:\n            Authority Key Identifier:\n                keyIdentifier:\n                    f8:ef:7f:f2:cd:78:67:a8:de:6f:8f:24:8d:88:f1:87:03:02:b3:eb\n            Subject Key Identifier:\n                7c:48:b3:b1:0d:48:93:a2:d2:f0:ac:f4:f6:13:ef:75:94:cf:80:97\n            Key Usage: critical\n                Digital Signature, Key Encipherment\n            Certificate Policies:\n                Policy:\n                    GlobalSign Certificate Policy\n                    https://www.globalsign.com/en/repository\n                Policy:\n                    CA/Browser Forum organization-validated\n            Subject Alternative Name:\n                DNS:www.bbc.com, DNS:www.bbc.co.uk, DNS:bbc.co.uk, DNS:bbcrussian.com,\n                DNS:*.bbc.com, DNS:*.bbcrussian.com, DNS:bbc.com\n            Basic Constraints:\n                cA:FALSE\n            Extended Key Usage:\n                TLS Web Server Authentication, TLS Web Client Authentication\n            CRL Distribution Points:\n                Full Name:\n                    URI:http://crl.globalsign.com/gsrsaovsslca2018.crl\n            Authority Information Access:\n                CA Issuers - URI:http://secure.globalsign.com/cacert/gsrsaovsslca2018.crt\n                OCSP - URI:http://ocsp.globalsign.com/gsrsaovsslca2018\n            CT Precertificate SCTs:\n                Signed Certificate Timestamp:\n                    Version: 1 (0x0)\n                    Log ID:\n                        e8:3e:d0:da:3e:f5:06:35:32:e7:57:28:bc:89:6b:c9:\n                        03:d3:cb:d1:11:6b:ec:eb:69:e1:77:7d:6d:06:bd:6e\n                    Timestamp: Mar 04 13:51:14 2022 UTC\n                Signed Certificate Timestamp:\n                    Version: 1 (0x0)\n                    Log ID:\n                        6f:53:76:ac:31:f0:31:19:d8:99:00:a4:51:15:ff:77:\n                        15:1c:11:d9:02:c1:00:29:06:8d:b2:08:9a:37:d9:13\n                    Timestamp: Mar 04 13:51:13 2022 UTC\n                Signed Certificate Timestamp:\n                    Version: 1 (0x0)\n                    Log ID:\n                        55:81:d4:c2:16:90:36:01:4a:ea:0b:9b:57:3c:53:f0:\n                        c0:e4:38:78:70:25:08:17:2f:a3:aa:1d:07:13:d3:0c\n                    Timestamp: Mar 04 13:51:13 2022 UTC\n    Signature: RSA with SHA256\n        14:40:09:bd:42:2d:bc:29:4d:da:58:55:87:05:dc:8b:1e:1c:e9:1a:77:c4:cb:b2:\n        35:fd:b1:3b:ee:5c:97:ef:c9:b0:bb:c4:3a:9c:88:81:ff:e9:02:9e:91:9e:0e:85:\n        5d:32:4e:d5:7f:1c:cd:7b:bc:0b:7b:00:c6:07:3e:b2:c0:0a:eb:9d:f1:a5:28:cf:\n        eb:9f:12:d0:da:75:6e:f3:da:74:36:e5:6c:8a:75:41:13:4b:2b:ed:83:24:d1:d1:\n        e6:6d:85:60:86:22:b2:c7:ff:61:0d:0d:91:1c:b9:ff:18:00:ed:16:09:5d:74:dd:\n        cb:bd:85:ca:5a:46:38:f6:86:07:74:21:24:dd:be:5b:6f:43:e8:64:79:70:65:c7:\n        79:0f:44:b2:08:6f:a6:1e:73:4e:9a:e2:6f:0a:5c:ae:99:bf:f9:b3:ef:b2:f4:e6:\n        bb:1d:52:92:fd:03:14:00:24:47:0c:00:bb:3b:33:f4:2f:d9:1c:00:fc:e2:57:8d:\n        a4:bf:2f:bf:5d:94:c2:ab:48:3e:24:00:39:1f:68:29:f2:e1:ba:24:9f:96:9c:24:\n        d1:82:5d:49:70:9a:5f:56:1a:2d:14:c2:6b:02:ab:9f:f1:6b:87:c2:e9:2e:46:c1:\n        7a:08:95:94:7c:b4:3a:07:c1:c7:fe:0b:df:c3:48:68\n```\n\nOutput the certificate to an SVG file\n\n```\npkiviewer --save-svg=cert.svg testcert.pem\n```\n\nOutput the certificate to an HTML file\n\n```bash\n$ pkiviewer --save-html=cert.html testcert.pem\n```\n\nFor SVG and HTML output the number of columns to output can be set with the `--width` option\n\n## Display Configuration\n\n`pkiviewer` looks for a `pkiviewer.toml` in the current directory. See\n`pkiviewer.toml.sample` for all the options.\n\nThis file can configure what information is output and the colors.\n\n### Colors\n\nThe default colors are\n\n```toml\n[theme]\ndefault = "white"\nerror = "red"\nwarning = "yellow"\ninfo = "green"\nkey = "blue"\nvalue = "white"\nextension_critical = "yellow"\n```\n\n### Information Visibility\n\nThe following items control what is output.\n\n```toml\n[visibility]\n".Header" = "normal"                                           # Header text depending on the file type\n".Header.Filename" = "normal"                                  # The filename\n".Data" = "normal"                                             # The Data block visibility\n".Data.Version" = "normal"                                     # Certiificate version\n".Data.SerialNumber" = "normal"                                # Certificate serial number\n".Data.Issuer" = "normal"                                      # The name of the org that issued the certificate\n".Data.Fingerprint" = "normal"                                 # Fingerprint of the certificate\n".Data.Validity" = "normal"                                    # The Validity block\n".Data.Validity.Before" = "normal"                             # Date and time from which the certificate is valid\n".Data.Validity.After" = "normal"                              # Date and time after which the certificate is invalid\n".Data.Subject" = "normal"                                     # Visibility of the certificate subject block\n".Data.Subject.Name" = "normal"                                # The subject\'s name\n".Data.Subject.PublicKey" = "normal"                           # The public key\n".Data.Subject.PublicKey.Algorithm" = "normal"                 # The public key algorithm\n\n".Data.Extensions" = "normal"                                  # Visibility for all extensions\n".Data.Extension.Critical" = "normal"                          # Whether the extension is critical\n".Data.Extension.Value" = "normal"                             # Visibility of the value for all extensions\n\n# Individual extension information\n".Data.Extension.AuthorityKeyIdentifier" = "normal"\n".Data.Extension.AuthorityKeyIdentifier.Value" = "normal"\n".Data.Extension.SubjectKeyIdentifier" = "normal"\n".Data.Extension.SubjectKeyIdentifier.Value" = "normal"\n".Data.Extension.KeyUsage" = "normal"\n".Data.Extension.KeyUsage.Value" = "normal"\n".Data.Extension.CertificatePolicies" = "normal"\n".Data.Extension.CertificatePolicies.Value" = "normal"\n".Data.Extension.SubjectAlternativeName" = "normal"\n".Data.Extension.SubjectAlternativeName.Value" = "normal"\n".Data.Extension.IssuerAlternativeName" = "normal"\n".Data.Extension.IssuerAlternativeName.Value" = "normal"\n".Data.Extension.BasicConstraints" = "normal"\n".Data.Extension.BasicConstraints.Value" = "normal"\n".Data.Extension.NameConstraints" = "normal"\n".Data.Extension.NameConstraints.Value" = "normal"\n".Data.Extension.ExtendedKeyUsage" = "normal"\n".Data.Extension.ExtendedKeyUsage.Value" = "normal"\n".Data.Extension.CRLDistributionPoints" = "normal"\n".Data.Extension.CRLDistributionPoints.Value" = "normal"\n".Data.Extension.InhibitAnyPolicy" = "normal"\n".Data.Extension.InhibitAnyPolicy.Value" = "normal"\n".Data.Extension.AuthorityInformationAccess" = "normal"\n".Data.Extension.AuthorityInformationAccess.Value" = "normal"\n".Data.Extension.SubjectInformationAccess" = "normal"\n".Data.Extension.SubjectInformationAccess.Value" = "normal"\n".Data.Extension.CertificateSCTs" = "normal"\n".Data.Extension.CertificateSCTs.Value" = "normal"\n".Data.Extension.PreCertificateSCTs" = "normal"\n".Data.Extension.PreCertificateSCTs.Value" = "normal"\n\n# Signature Information\n".Signature" = "normal"                                        # The signature block (alogrithm + value)\n".Signature.Algorithm" = "normal"                              # The signature algorithm\n".Signature.Value" = "normal"                                  # The signature value\n```\n',
-    'author': 'Simon Kennedy',
-    'author_email': 'sffjunkie+code@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+Displays information in the terminal from the following PKI file types
 
+- Certificates
+- PKCS#12 files
+- Certificate Signing Request (Coming Soon™)
+- Certificate Revocation List
+
+Also Coming Soon™ is Certificate Transparency information.
+
+## Features
+
+1. Files can be in either PEM or DER formats
+
+1. If a URL is passed a certificate will be downloaded automatically
+
+1. The certificate information can be output to the terminal, an SVG file or an HTML file.
+
+1. The information that is displayed can be configured (either hidden, displayed dim or highlighted)
+
+1. The colors can be configured
+
+1. Uses [rich](https://rich.readthedocs.io/en/latest/) for the
+   fancy output/SVG & HTML generation and
+   [cryptography](https://cryptography.io/en/latest/) for the low level parsing.
+
+1. It sticks fairly closely to the output from the `openssl` binary
+
+DER format certificates should have the extension `.cer` and PKCS#12 `.p12`
+
+## PKCS#12 Files
+
+If the PKCS#12 file is encrypted you will be prompted to enter the passsword
+
+## Usage
+
+Output certificate information to the terminal
+
+```
+pkiviewer testcert.pem   OR   pkiviewer https://bbc.com
+```
+
+For example
+
+```
+pkiviewer https://bbc.com
+```
+
+produces the following output
+
+```
+Certificate: https://bbc.com
+    Data:
+        Version: 1 (0x0)
+        Serial Number:
+            3e:55:35:3c:c9:9b:cb:59:6e:be:fc:64
+        Signature Algorithm: RSA with SHA256
+        Issuer: C = BE, O = GlobalSign nv-sa, CN = GlobalSign RSA OV SSL CA 2018
+        Validity:
+            Not Before: Mar 04 13:51:12 2022 UTC
+            Not After:  Apr 05 13:51:11 2023 UTC
+        Subject:
+            C = GB, ST = London, L = London, O = BRITISH BROADCASTING CORPORATION, CN = www.bbc.com
+        Subject Public Key Info:
+            Public Key Algorithm: RSA
+                RSA Public-Key (2048 bit)
+                Modulus:
+                    c1:91:f9:55:15:2b:77:96:e3:a5:62:2b:1c:4b:2e:8f:e3:c9:f9:76:bd:91:d4:96:
+                    28:7e:2e:b4:a9:6a:62:71:50:74:8e:d9:ef:5d:8d:ab:fc:d9:b8:1a:f8:30:01:82:
+                    30:45:15:32:e0:f8:64:53:5d:c2:92:0b:44:29:81:5b:b0:83:bf:df:c5:b4:56:e3:
+                    7b:af:54:cf:4c:1f:6c:46:ca:b7:21:ae:bc:f5:48:93:ff:ef:f0:37:7c:16:b3:92:
+                    c1:be:36:54:78:e0:06:86:64:c1:74:4d:39:c7:79:2d:1f:e4:99:bd:fc:1b:5e:29:
+                    bc:c4:ce:8c:aa:76:81:e0:c6:30:08:ea:21:e1:b9:81:1e:08:ea:7d:31:f3:3f:b3:
+                    77:98:71:53:00:45:a6:97:a3:54:f5:25:87:eb:81:97:86:45:ef:47:3d:3e:a4:14:
+                    2c:06:9d:18:a2:4e:26:5c:bd:b8:c5:a6:53:5d:65:7b:e9:02:52:77:26:10:b5:44:
+                    e1:e0:79:a2:ef:29:d3:1b:37:46:27:67:ef:bb:5e:78:58:05:94:5b:3d:82:d8:4d:
+                    d8:28:32:b9:e8:e2:5e:65:58:f8:fc:b0:79:f8:fc:23:4f:6a:33:ff:b8:60:96:9a:
+                    bc:9b:8c:46:24:8d:fc:5d:13:19:32:ac:ff:a4:f8:91
+                Exponent 65537 (0x10001)
+                Fingerprint (SHA256):
+                    66:dd:b2:a9:e1:f4:52:2f:3b:06:e3:de:6a:76:b3:f0:18:b8:3a:e5:54:7e:71:15:
+                    83:68:5c:d7:6a:3d:17:84
+        X509v3 Extensions:
+            Authority Key Identifier:
+                keyIdentifier:
+                    f8:ef:7f:f2:cd:78:67:a8:de:6f:8f:24:8d:88:f1:87:03:02:b3:eb
+            Subject Key Identifier:
+                7c:48:b3:b1:0d:48:93:a2:d2:f0:ac:f4:f6:13:ef:75:94:cf:80:97
+            Key Usage: critical
+                Digital Signature, Key Encipherment
+            Certificate Policies:
+                Policy:
+                    GlobalSign Certificate Policy
+                    https://www.globalsign.com/en/repository
+                Policy:
+                    CA/Browser Forum organization-validated
+            Subject Alternative Name:
+                DNS:www.bbc.com, DNS:www.bbc.co.uk, DNS:bbc.co.uk, DNS:bbcrussian.com,
+                DNS:*.bbc.com, DNS:*.bbcrussian.com, DNS:bbc.com
+            Basic Constraints:
+                cA:FALSE
+            Extended Key Usage:
+                TLS Web Server Authentication, TLS Web Client Authentication
+            CRL Distribution Points:
+                Full Name:
+                    URI:http://crl.globalsign.com/gsrsaovsslca2018.crl
+            Authority Information Access:
+                CA Issuers - URI:http://secure.globalsign.com/cacert/gsrsaovsslca2018.crt
+                OCSP - URI:http://ocsp.globalsign.com/gsrsaovsslca2018
+            CT Precertificate SCTs:
+                Signed Certificate Timestamp:
+                    Version: 1 (0x0)
+                    Log ID:
+                        e8:3e:d0:da:3e:f5:06:35:32:e7:57:28:bc:89:6b:c9:
+                        03:d3:cb:d1:11:6b:ec:eb:69:e1:77:7d:6d:06:bd:6e
+                    Timestamp: Mar 04 13:51:14 2022 UTC
+                Signed Certificate Timestamp:
+                    Version: 1 (0x0)
+                    Log ID:
+                        6f:53:76:ac:31:f0:31:19:d8:99:00:a4:51:15:ff:77:
+                        15:1c:11:d9:02:c1:00:29:06:8d:b2:08:9a:37:d9:13
+                    Timestamp: Mar 04 13:51:13 2022 UTC
+                Signed Certificate Timestamp:
+                    Version: 1 (0x0)
+                    Log ID:
+                        55:81:d4:c2:16:90:36:01:4a:ea:0b:9b:57:3c:53:f0:
+                        c0:e4:38:78:70:25:08:17:2f:a3:aa:1d:07:13:d3:0c
+                    Timestamp: Mar 04 13:51:13 2022 UTC
+    Signature: RSA with SHA256
+        14:40:09:bd:42:2d:bc:29:4d:da:58:55:87:05:dc:8b:1e:1c:e9:1a:77:c4:cb:b2:
+        35:fd:b1:3b:ee:5c:97:ef:c9:b0:bb:c4:3a:9c:88:81:ff:e9:02:9e:91:9e:0e:85:
+        5d:32:4e:d5:7f:1c:cd:7b:bc:0b:7b:00:c6:07:3e:b2:c0:0a:eb:9d:f1:a5:28:cf:
+        eb:9f:12:d0:da:75:6e:f3:da:74:36:e5:6c:8a:75:41:13:4b:2b:ed:83:24:d1:d1:
+        e6:6d:85:60:86:22:b2:c7:ff:61:0d:0d:91:1c:b9:ff:18:00:ed:16:09:5d:74:dd:
+        cb:bd:85:ca:5a:46:38:f6:86:07:74:21:24:dd:be:5b:6f:43:e8:64:79:70:65:c7:
+        79:0f:44:b2:08:6f:a6:1e:73:4e:9a:e2:6f:0a:5c:ae:99:bf:f9:b3:ef:b2:f4:e6:
+        bb:1d:52:92:fd:03:14:00:24:47:0c:00:bb:3b:33:f4:2f:d9:1c:00:fc:e2:57:8d:
+        a4:bf:2f:bf:5d:94:c2:ab:48:3e:24:00:39:1f:68:29:f2:e1:ba:24:9f:96:9c:24:
+        d1:82:5d:49:70:9a:5f:56:1a:2d:14:c2:6b:02:ab:9f:f1:6b:87:c2:e9:2e:46:c1:
+        7a:08:95:94:7c:b4:3a:07:c1:c7:fe:0b:df:c3:48:68
+```
+
+Output the certificate to an SVG file
+
+```
+pkiviewer --save-svg=cert.svg testcert.pem
+```
+
+Output the certificate to an HTML file
+
+```bash
+$ pkiviewer --save-html=cert.html testcert.pem
+```
+
+For SVG and HTML output the number of columns to output can be set with the `--width` option
+
+## Display Configuration
+
+`pkiviewer` looks for a `pkiviewer.toml` in the current directory. See
+`pkiviewer.toml.sample` for all the options.
+
+This file can configure what information is output and the colors.
+
+### Colors
+
+The default colors are
+
+```toml
+[theme]
+default = "white"
+error = "red"
+warning = "yellow"
+info = "green"
+key = "blue"
+value = "white"
+extension_critical = "yellow"
+```
+
+### Information Visibility
+
+The following items control what is output.
+
+```toml
+[visibility]
+".Header" = "normal"                                           # Header text depending on the file type
+".Header.Filename" = "normal"                                  # The filename
+".Data" = "normal"                                             # The Data block visibility
+".Data.Version" = "normal"                                     # Certiificate version
+".Data.SerialNumber" = "normal"                                # Certificate serial number
+".Data.Issuer" = "normal"                                      # The name of the org that issued the certificate
+".Data.Fingerprint" = "normal"                                 # Fingerprint of the certificate
+".Data.Validity" = "normal"                                    # The Validity block
+".Data.Validity.Before" = "normal"                             # Date and time from which the certificate is valid
+".Data.Validity.After" = "normal"                              # Date and time after which the certificate is invalid
+".Data.Subject" = "normal"                                     # Visibility of the certificate subject block
+".Data.Subject.Name" = "normal"                                # The subject's name
+".Data.Subject.PublicKey" = "normal"                           # The public key
+".Data.Subject.PublicKey.Algorithm" = "normal"                 # The public key algorithm
+
+".Data.Extensions" = "normal"                                  # Visibility for all extensions
+".Data.Extension.Critical" = "normal"                          # Whether the extension is critical
+".Data.Extension.Value" = "normal"                             # Visibility of the value for all extensions
+
+# Individual extension information
+".Data.Extension.AuthorityKeyIdentifier" = "normal"
+".Data.Extension.AuthorityKeyIdentifier.Value" = "normal"
+".Data.Extension.SubjectKeyIdentifier" = "normal"
+".Data.Extension.SubjectKeyIdentifier.Value" = "normal"
+".Data.Extension.KeyUsage" = "normal"
+".Data.Extension.KeyUsage.Value" = "normal"
+".Data.Extension.CertificatePolicies" = "normal"
+".Data.Extension.CertificatePolicies.Value" = "normal"
+".Data.Extension.SubjectAlternativeName" = "normal"
+".Data.Extension.SubjectAlternativeName.Value" = "normal"
+".Data.Extension.IssuerAlternativeName" = "normal"
+".Data.Extension.IssuerAlternativeName.Value" = "normal"
+".Data.Extension.BasicConstraints" = "normal"
+".Data.Extension.BasicConstraints.Value" = "normal"
+".Data.Extension.NameConstraints" = "normal"
+".Data.Extension.NameConstraints.Value" = "normal"
+".Data.Extension.ExtendedKeyUsage" = "normal"
+".Data.Extension.ExtendedKeyUsage.Value" = "normal"
+".Data.Extension.CRLDistributionPoints" = "normal"
+".Data.Extension.CRLDistributionPoints.Value" = "normal"
+".Data.Extension.InhibitAnyPolicy" = "normal"
+".Data.Extension.InhibitAnyPolicy.Value" = "normal"
+".Data.Extension.AuthorityInformationAccess" = "normal"
+".Data.Extension.AuthorityInformationAccess.Value" = "normal"
+".Data.Extension.SubjectInformationAccess" = "normal"
+".Data.Extension.SubjectInformationAccess.Value" = "normal"
+".Data.Extension.CertificateSCTs" = "normal"
+".Data.Extension.CertificateSCTs.Value" = "normal"
+".Data.Extension.PreCertificateSCTs" = "normal"
+".Data.Extension.PreCertificateSCTs.Value" = "normal"
+
+# Signature Information
+".Signature" = "normal"                                        # The signature block (alogrithm + value)
+".Signature.Algorithm" = "normal"                              # The signature algorithm
+".Signature.Value" = "normal"                                  # The signature value
+```
+
+## Package Info
+
+![GitHub Workflow Status](https://img.shields.io/github/workflow/status/sffjunkie/pkiviewer/pkiviewer-test) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pkiviewer)
 
-setup(**setup_kwargs)
```

