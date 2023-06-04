# Comparing `tmp/pbtools-0.8.0.tar.gz` & `tmp/pbtools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pbtools-0.8.0.tar", last modified: Wed Sep 11 21:04:30 2019, max compression
+gzip compressed data, was "dist/pbtools-0.9.0.tar", last modified: Thu Sep 12 05:24:16 2019, max compression
```

## Comparing `pbtools-0.8.0.tar` & `pbtools-0.9.0.tar`

### file list

```diff
@@ -1,129 +1,132 @@
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-11 21:04:30.000000 pbtools-0.8.0/
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-11 21:04:30.000000 pbtools-0.8.0/pbtools.egg-info/
--rw-rw-r--   0 erik      (1000) erik      (1000)       19 2019-09-11 21:04:30.000000 pbtools-0.8.0/pbtools.egg-info/requires.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)       52 2019-09-11 21:04:30.000000 pbtools-0.8.0/pbtools.egg-info/entry_points.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)        8 2019-09-11 21:04:30.000000 pbtools-0.8.0/pbtools.egg-info/top_level.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)     3266 2019-09-11 21:04:30.000000 pbtools-0.8.0/pbtools.egg-info/SOURCES.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)        1 2019-09-11 21:04:30.000000 pbtools-0.8.0/pbtools.egg-info/dependency_links.txt
--rw-rw-r--   0 erik      (1000) erik      (1000)     5938 2019-09-11 21:04:30.000000 pbtools-0.8.0/pbtools.egg-info/PKG-INFO
--rw-rw-r--   0 erik      (1000) erik      (1000)       38 2019-09-11 21:04:30.000000 pbtools-0.8.0/setup.cfg
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-11 21:04:30.000000 pbtools-0.8.0/pbtools/
--rw-rw-r--   0 erik      (1000) erik      (1000)       22 2019-09-11 21:03:54.000000 pbtools-0.8.0/pbtools/version.py
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-11 21:04:30.000000 pbtools-0.8.0/pbtools/c_source/
--rw-rw-r--   0 erik      (1000) erik      (1000)    64395 2019-09-10 04:51:07.000000 pbtools-0.8.0/pbtools/c_source/pbtools.c
--rw-rw-r--   0 erik      (1000) erik      (1000)    32423 2019-09-11 20:56:20.000000 pbtools-0.8.0/pbtools/c_source/__init__.py
--rw-rw-r--   0 erik      (1000) erik      (1000)    25507 2019-09-10 04:31:03.000000 pbtools-0.8.0/pbtools/c_source/pbtools.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     1103 2019-08-22 05:43:41.000000 pbtools-0.8.0/pbtools/__init__.py
--rw-rw-r--   0 erik      (1000) erik      (1000)       71 2019-02-14 17:58:54.000000 pbtools-0.8.0/pbtools/__main__.py
--rw-rw-r--   0 erik      (1000) erik      (1000)    14570 2019-09-10 06:35:09.000000 pbtools-0.8.0/pbtools/parser.py
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-11 21:04:30.000000 pbtools-0.8.0/pbtools/subparsers/
--rw-rw-r--   0 erik      (1000) erik      (1000)        0 2019-02-14 17:58:54.000000 pbtools-0.8.0/pbtools/subparsers/__init__.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     1901 2019-09-10 20:32:08.000000 pbtools-0.8.0/pbtools/subparsers/generate_c_source.py
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-11 21:04:30.000000 pbtools-0.8.0/tests/
--rw-rw-r--   0 erik      (1000) erik      (1000)   111392 2019-09-01 04:57:38.000000 pbtools-0.8.0/tests/narwhal.c
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-11 21:04:30.000000 pbtools-0.8.0/tests/files/
--rw-rw-r--   0 erik      (1000) erik      (1000)       96 2019-08-26 21:13:51.000000 pbtools-0.8.0/tests/files/options.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:29:32.000000 pbtools-0.8.0/tests/files/string.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       77 2019-08-21 06:28:07.000000 pbtools-0.8.0/tests/files/int64.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      365 2019-09-02 05:26:47.000000 pbtools-0.8.0/tests/files/scalar_value_types.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      653 2019-09-11 05:22:30.000000 pbtools-0.8.0/tests/files/oneof.proto
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-11 21:04:30.000000 pbtools-0.8.0/tests/files/imports/
--rw-rw-r--   0 erik      (1000) erik      (1000)      140 2019-09-10 03:40:46.000000 pbtools-0.8.0/tests/files/imports/imported2.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:29:42.000000 pbtools-0.8.0/tests/files/uint32.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       81 2019-08-21 06:27:27.000000 pbtools-0.8.0/tests/files/fixed32.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:29:53.000000 pbtools-0.8.0/tests/files/uint64.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)    14143 2019-08-24 22:19:14.000000 pbtools-0.8.0/tests/files/main.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     1784 2019-09-08 20:17:15.000000 pbtools-0.8.0/tests/files/benchmark.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       83 2019-08-21 06:28:55.000000 pbtools-0.8.0/tests/files/sfixed32.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      282 2019-09-10 03:44:41.000000 pbtools-0.8.0/tests/files/importing.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:26:30.000000 pbtools-0.8.0/tests/files/double.proto
-drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-11 21:04:30.000000 pbtools-0.8.0/tests/files/c_source/
--rw-rw-r--   0 erik      (1000) erik      (1000)     4493 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/benchmark.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     1894 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/sfixed32.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     3324 2019-09-10 03:28:24.000000 pbtools-0.8.0/tests/files/c_source/imported.h
--rw-rw-r--   0 erik      (1000) erik      (1000)    14756 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/address_book.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     5009 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/sint32.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     2167 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/no_package.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     1867 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/uint32.h
--rw-rw-r--   0 erik      (1000) erik      (1000)    27437 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/message.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     6975 2019-09-10 04:03:34.000000 pbtools-0.8.0/tests/files/c_source/importing.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     2453 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/int32.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     8659 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/int32.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     1866 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/sint64.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     4687 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/map.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     1867 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/uint64.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     2505 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/service.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     4777 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/tags.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     5095 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/sfixed64.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     1867 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/bytes.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     5095 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/sfixed32.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     1850 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/float.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     5268 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/message.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     1894 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/sfixed64.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     1866 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/sint32.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     4984 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/bytes.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     8138 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/no_package.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     1881 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/fixed64.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     1852 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/int64.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     5009 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/double.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     1881 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/fixed32.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     3121 2019-09-10 03:58:14.000000 pbtools-0.8.0/tests/files/c_source/importing.h
--rw-rw-r--   0 erik      (1000) erik      (1000)    23848 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/benchmark.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     5009 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/uint64.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     4966 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/float.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     5016 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/string.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     5052 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/fixed64.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     7833 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/repeated.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     1877 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/options.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     5046 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/options.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     3625 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/enum.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     5052 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/fixed32.c
--rw-rw-r--   0 erik      (1000) erik      (1000)    23240 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/tags.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     1835 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/bool.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     3107 2019-09-09 20:41:27.000000 pbtools-0.8.0/tests/files/c_source/imported.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     4923 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/bool.c
--rw-rw-r--   0 erik      (1000) erik      (1000)    32290 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/oneof.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     7510 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/oneof.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     3374 2019-09-10 04:02:58.000000 pbtools-0.8.0/tests/files/c_source/imported2.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     3688 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/address_book.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     8837 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/service.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     5009 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/uint32.c
--rw-rw-r--   0 erik      (1000) erik      (1000)    12338 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/enum.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     5009 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/sint64.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     2274 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/scalar_value_types.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     8235 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/scalar_value_types.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     1805 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/map.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     1865 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/double.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     1866 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/files/c_source/string.h
--rw-rw-r--   0 erik      (1000) erik      (1000)    33968 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/repeated.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     4966 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/c_source/int64.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     3602 2019-09-10 04:03:03.000000 pbtools-0.8.0/tests/files/c_source/imported2.h
--rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:29:25.000000 pbtools-0.8.0/tests/files/sint64.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      121 2019-08-25 20:29:12.000000 pbtools-0.8.0/tests/files/int32.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       77 2019-08-21 06:26:22.000000 pbtools-0.8.0/tests/files/bytes.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       83 2019-08-21 06:29:13.000000 pbtools-0.8.0/tests/files/sfixed64.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       81 2019-08-21 06:27:46.000000 pbtools-0.8.0/tests/files/fixed64.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      417 2019-09-08 20:17:15.000000 pbtools-0.8.0/tests/files/enum.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       75 2019-08-26 21:13:51.000000 pbtools-0.8.0/tests/files/bool.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       77 2019-08-21 06:27:56.000000 pbtools-0.8.0/tests/files/float.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      965 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/files/repeated.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:29:17.000000 pbtools-0.8.0/tests/files/sint32.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      183 2019-09-08 20:17:15.000000 pbtools-0.8.0/tests/files/no_package.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      390 2019-08-18 17:37:17.000000 pbtools-0.8.0/tests/files/address_book.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      496 2019-09-09 03:27:47.000000 pbtools-0.8.0/tests/files/message.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      129 2019-09-10 03:38:03.000000 pbtools-0.8.0/tests/files/imported.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      158 2019-09-10 06:35:09.000000 pbtools-0.8.0/tests/files/map.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      231 2019-08-22 20:25:25.000000 pbtools-0.8.0/tests/files/service.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)      395 2019-08-25 06:18:15.000000 pbtools-0.8.0/tests/files/tags.proto
--rw-rw-r--   0 erik      (1000) erik      (1000)        0 2019-02-14 17:59:26.000000 pbtools-0.8.0/tests/__init__.py
--rw-rw-r--   0 erik      (1000) erik      (1000)    20801 2019-09-11 07:44:52.000000 pbtools-0.8.0/tests/test_parser.py
--rw-rw-r--   0 erik      (1000) erik      (1000)    41099 2019-09-01 04:57:38.000000 pbtools-0.8.0/tests/narwhal.h
--rw-rw-r--   0 erik      (1000) erik      (1000)     3155 2019-09-08 03:10:27.000000 pbtools-0.8.0/tests/main_fuzzer.c
--rw-rw-r--   0 erik      (1000) erik      (1000)    98631 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/main.c
--rw-rw-r--   0 erik      (1000) erik      (1000)     3591 2019-09-11 20:56:20.000000 pbtools-0.8.0/tests/test_command_line.py
--rw-rw-r--   0 erik      (1000) erik      (1000)     4155 2019-09-11 05:14:38.000000 pbtools-0.8.0/README.rst
--rw-rw-r--   0 erik      (1000) erik      (1000)      245 2019-09-01 20:54:07.000000 pbtools-0.8.0/Makefile
--rw-rw-r--   0 erik      (1000) erik      (1000)     1080 2019-08-19 06:35:22.000000 pbtools-0.8.0/LICENSE
--rw-rw-r--   0 erik      (1000) erik      (1000)     5938 2019-09-11 21:04:30.000000 pbtools-0.8.0/PKG-INFO
--rwxrwxr-x   0 erik      (1000) erik      (1000)     1035 2019-09-09 20:41:27.000000 pbtools-0.8.0/setup.py
--rw-rw-r--   0 erik      (1000) erik      (1000)      116 2019-09-09 20:41:27.000000 pbtools-0.8.0/MANIFEST.in
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-12 05:24:16.000000 pbtools-0.9.0/
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-12 05:24:16.000000 pbtools-0.9.0/pbtools.egg-info/
+-rw-rw-r--   0 erik      (1000) erik      (1000)       19 2019-09-12 05:24:16.000000 pbtools-0.9.0/pbtools.egg-info/requires.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)       52 2019-09-12 05:24:16.000000 pbtools-0.9.0/pbtools.egg-info/entry_points.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)        8 2019-09-12 05:24:16.000000 pbtools-0.9.0/pbtools.egg-info/top_level.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3357 2019-09-12 05:24:16.000000 pbtools-0.9.0/pbtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)        1 2019-09-12 05:24:16.000000 pbtools-0.9.0/pbtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5938 2019-09-12 05:24:16.000000 pbtools-0.9.0/pbtools.egg-info/PKG-INFO
+-rw-rw-r--   0 erik      (1000) erik      (1000)       38 2019-09-12 05:24:16.000000 pbtools-0.9.0/setup.cfg
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-12 05:24:16.000000 pbtools-0.9.0/pbtools/
+-rw-rw-r--   0 erik      (1000) erik      (1000)       22 2019-09-12 05:21:04.000000 pbtools-0.9.0/pbtools/version.py
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-12 05:24:16.000000 pbtools-0.9.0/pbtools/c_source/
+-rw-rw-r--   0 erik      (1000) erik      (1000)    63996 2019-09-12 04:34:52.000000 pbtools-0.9.0/pbtools/c_source/pbtools.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)    32796 2019-09-12 04:26:34.000000 pbtools-0.9.0/pbtools/c_source/__init__.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)    25385 2019-09-12 04:29:31.000000 pbtools-0.9.0/pbtools/c_source/pbtools.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1103 2019-08-22 05:43:41.000000 pbtools-0.9.0/pbtools/__init__.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)       71 2019-02-14 17:58:54.000000 pbtools-0.9.0/pbtools/__main__.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)    15860 2019-09-12 05:19:10.000000 pbtools-0.9.0/pbtools/parser.py
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-12 05:24:16.000000 pbtools-0.9.0/pbtools/subparsers/
+-rw-rw-r--   0 erik      (1000) erik      (1000)        0 2019-02-14 17:58:54.000000 pbtools-0.9.0/pbtools/subparsers/__init__.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1901 2019-09-10 20:32:08.000000 pbtools-0.9.0/pbtools/subparsers/generate_c_source.py
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-12 05:24:16.000000 pbtools-0.9.0/tests/
+-rw-rw-r--   0 erik      (1000) erik      (1000)   111392 2019-09-01 04:57:38.000000 pbtools-0.9.0/tests/narwhal.c
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-12 05:24:16.000000 pbtools-0.9.0/tests/files/
+-rw-rw-r--   0 erik      (1000) erik      (1000)       96 2019-08-26 21:13:51.000000 pbtools-0.9.0/tests/files/options.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:29:32.000000 pbtools-0.9.0/tests/files/string.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       77 2019-08-21 06:28:07.000000 pbtools-0.9.0/tests/files/int64.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      365 2019-09-02 05:26:47.000000 pbtools-0.9.0/tests/files/scalar_value_types.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      653 2019-09-11 05:22:30.000000 pbtools-0.9.0/tests/files/oneof.proto
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-12 05:24:16.000000 pbtools-0.9.0/tests/files/imports/
+-rw-rw-r--   0 erik      (1000) erik      (1000)      140 2019-09-10 03:40:46.000000 pbtools-0.9.0/tests/files/imports/imported2.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:29:42.000000 pbtools-0.9.0/tests/files/uint32.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      351 2019-09-12 04:52:11.000000 pbtools-0.9.0/tests/files/ordering.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       81 2019-08-21 06:27:27.000000 pbtools-0.9.0/tests/files/fixed32.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:29:53.000000 pbtools-0.9.0/tests/files/uint64.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)    14143 2019-08-24 22:19:14.000000 pbtools-0.9.0/tests/files/main.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1784 2019-09-08 20:17:15.000000 pbtools-0.9.0/tests/files/benchmark.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       83 2019-08-21 06:28:55.000000 pbtools-0.9.0/tests/files/sfixed32.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      282 2019-09-10 03:44:41.000000 pbtools-0.9.0/tests/files/importing.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:26:30.000000 pbtools-0.9.0/tests/files/double.proto
+drwxrwxr-x   0 erik      (1000) erik      (1000)        0 2019-09-12 05:24:16.000000 pbtools-0.9.0/tests/files/c_source/
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4493 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/benchmark.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1894 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/sfixed32.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)    16288 2019-09-12 05:19:16.000000 pbtools-0.9.0/tests/files/c_source/ordering.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3324 2019-09-10 03:28:24.000000 pbtools-0.9.0/tests/files/c_source/imported.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)    14756 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/address_book.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5009 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/sint32.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     2167 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/no_package.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1867 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/uint32.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)    27495 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/message.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3385 2019-09-12 05:19:16.000000 pbtools-0.9.0/tests/files/c_source/ordering.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     6975 2019-09-10 04:03:34.000000 pbtools-0.9.0/tests/files/c_source/importing.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     2453 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/int32.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     8659 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/int32.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1866 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/sint64.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4745 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/map.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1867 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/uint64.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     2505 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/service.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4777 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/tags.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5095 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/sfixed64.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1867 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/bytes.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5095 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/sfixed32.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1850 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/float.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5268 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/message.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1894 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/sfixed64.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1866 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/sint32.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4984 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/bytes.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     8138 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/no_package.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1881 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/fixed64.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1852 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/int64.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5009 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/double.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1881 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/fixed32.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3121 2019-09-10 03:58:14.000000 pbtools-0.9.0/tests/files/c_source/importing.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)    23848 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/benchmark.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5009 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/uint64.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4966 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/float.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5016 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/string.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5052 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/fixed64.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     7833 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/repeated.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1877 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/options.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5046 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/options.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3625 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/enum.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5052 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/fixed32.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)    23240 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/tags.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1835 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/bool.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3107 2019-09-09 20:41:27.000000 pbtools-0.9.0/tests/files/c_source/imported.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4923 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/bool.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)    32290 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/oneof.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     7510 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/oneof.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3374 2019-09-10 04:02:58.000000 pbtools-0.9.0/tests/files/c_source/imported2.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3688 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/address_book.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     8837 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/service.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5009 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/uint32.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)    12338 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/enum.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5009 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/sint64.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     2274 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/scalar_value_types.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     8235 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/scalar_value_types.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1805 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/map.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1865 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/double.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1866 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/string.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)    33968 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/repeated.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4966 2019-09-12 04:27:16.000000 pbtools-0.9.0/tests/files/c_source/int64.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3602 2019-09-10 04:03:03.000000 pbtools-0.9.0/tests/files/c_source/imported2.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:29:25.000000 pbtools-0.9.0/tests/files/sint64.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      121 2019-08-25 20:29:12.000000 pbtools-0.9.0/tests/files/int32.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       77 2019-08-21 06:26:22.000000 pbtools-0.9.0/tests/files/bytes.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       83 2019-08-21 06:29:13.000000 pbtools-0.9.0/tests/files/sfixed64.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       81 2019-08-21 06:27:46.000000 pbtools-0.9.0/tests/files/fixed64.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      417 2019-09-08 20:17:15.000000 pbtools-0.9.0/tests/files/enum.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       75 2019-08-26 21:13:51.000000 pbtools-0.9.0/tests/files/bool.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       77 2019-08-21 06:27:56.000000 pbtools-0.9.0/tests/files/float.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      965 2019-09-11 07:44:52.000000 pbtools-0.9.0/tests/files/repeated.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)       79 2019-08-21 06:29:17.000000 pbtools-0.9.0/tests/files/sint32.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      183 2019-09-08 20:17:15.000000 pbtools-0.9.0/tests/files/no_package.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      390 2019-08-18 17:37:17.000000 pbtools-0.9.0/tests/files/address_book.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      496 2019-09-09 03:27:47.000000 pbtools-0.9.0/tests/files/message.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      129 2019-09-10 03:38:03.000000 pbtools-0.9.0/tests/files/imported.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      158 2019-09-10 06:35:09.000000 pbtools-0.9.0/tests/files/map.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      231 2019-08-22 20:25:25.000000 pbtools-0.9.0/tests/files/service.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)      395 2019-08-25 06:18:15.000000 pbtools-0.9.0/tests/files/tags.proto
+-rw-rw-r--   0 erik      (1000) erik      (1000)        0 2019-02-14 17:59:26.000000 pbtools-0.9.0/tests/__init__.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)    20801 2019-09-11 07:44:52.000000 pbtools-0.9.0/tests/test_parser.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)    41099 2019-09-01 04:57:38.000000 pbtools-0.9.0/tests/narwhal.h
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3155 2019-09-08 03:10:27.000000 pbtools-0.9.0/tests/main_fuzzer.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)    98668 2019-09-12 04:54:44.000000 pbtools-0.9.0/tests/main.c
+-rw-rw-r--   0 erik      (1000) erik      (1000)     3615 2019-09-12 04:50:03.000000 pbtools-0.9.0/tests/test_command_line.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)     4155 2019-09-12 04:40:13.000000 pbtools-0.9.0/README.rst
+-rw-rw-r--   0 erik      (1000) erik      (1000)      245 2019-09-01 20:54:07.000000 pbtools-0.9.0/Makefile
+-rw-rw-r--   0 erik      (1000) erik      (1000)     1080 2019-08-19 06:35:22.000000 pbtools-0.9.0/LICENSE
+-rw-rw-r--   0 erik      (1000) erik      (1000)     5938 2019-09-12 05:24:16.000000 pbtools-0.9.0/PKG-INFO
+-rwxrwxr-x   0 erik      (1000) erik      (1000)     1035 2019-09-09 20:41:27.000000 pbtools-0.9.0/setup.py
+-rw-rw-r--   0 erik      (1000) erik      (1000)      116 2019-09-09 20:41:27.000000 pbtools-0.9.0/MANIFEST.in
```

### Comparing `pbtools-0.8.0/pbtools.egg-info/SOURCES.txt` & `pbtools-0.9.0/pbtools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 tests/files/int64.proto
 tests/files/main.py
 tests/files/map.proto
 tests/files/message.proto
 tests/files/no_package.proto
 tests/files/oneof.proto
 tests/files/options.proto
+tests/files/ordering.proto
 tests/files/repeated.proto
 tests/files/scalar_value_types.proto
 tests/files/service.proto
 tests/files/sfixed32.proto
 tests/files/sfixed64.proto
 tests/files/sint32.proto
 tests/files/sint64.proto
@@ -89,14 +90,16 @@
 tests/files/c_source/message.h
 tests/files/c_source/no_package.c
 tests/files/c_source/no_package.h
 tests/files/c_source/oneof.c
 tests/files/c_source/oneof.h
 tests/files/c_source/options.c
 tests/files/c_source/options.h
+tests/files/c_source/ordering.c
+tests/files/c_source/ordering.h
 tests/files/c_source/repeated.c
 tests/files/c_source/repeated.h
 tests/files/c_source/scalar_value_types.c
 tests/files/c_source/scalar_value_types.h
 tests/files/c_source/service.c
 tests/files/c_source/service.h
 tests/files/c_source/sfixed32.c
```

### Comparing `pbtools-0.8.0/pbtools.egg-info/PKG-INFO` & `pbtools-0.9.0/pbtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pbtools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Google Protocol Buffers tools.
 Home-page: https://github.com/eerimoq/pbtools
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: |buildstatus|_
```

### Comparing `pbtools-0.8.0/pbtools/c_source/pbtools.c` & `pbtools-0.9.0/pbtools/c_source/pbtools.c`

 * *Files 2% similar despite different names*

```diff
@@ -58,144 +58,136 @@
                                         size_t size)
 {
     struct pbtools_heap_t *heap_p;
 
     if (size >= sizeof(*heap_p)) {
         heap_p = (struct pbtools_heap_t *)buf_p;
         heap_p->buf_p = buf_p;
-        heap_p->size = size;
+        heap_p->size = (int)size;
         heap_p->pos = sizeof(*heap_p);
     } else {
         heap_p = NULL;
     }
 
     return (heap_p);
 }
 
 void *pbtools_heap_alloc(struct pbtools_heap_t *self_p,
-                         int size)
+                         size_t size)
 {
     void *buf_p;
     int left;
 
     left = (self_p->size - self_p->pos);
 
-    if (size <= left) {
+    if ((int)size <= left) {
         buf_p = &self_p->buf_p[self_p->pos];
-        self_p->pos += size;
+        self_p->pos += (int)size;
     } else {
         buf_p = NULL;
     }
 
     return (buf_p);
 }
 
 void *pbtools_decoder_heap_alloc(struct pbtools_decoder_t *self_p,
-                                 int size)
+                                 size_t size)
 {
     void *buf_p;
 
     buf_p = pbtools_heap_alloc(self_p->heap_p, size);
 
     if (buf_p == NULL) {
         pbtools_decoder_abort(self_p, PBTOOLS_OUT_OF_MEMORY);
     }
 
     return (buf_p);
 }
 
 void pbtools_encoder_init(struct pbtools_encoder_t *self_p,
                           uint8_t *buf_p,
-                          size_t size)
+                          size_t  size)
 {
     self_p->buf_p = buf_p;
-    self_p->size = size;
-    self_p->pos = (size - 1);
+    self_p->size = (int)size;
+    self_p->pos = ((int)size - 1);
 }
 
 int pbtools_encoder_get_result(struct pbtools_encoder_t *self_p)
 {
     int length;
 
-    PRINTF("pbtools_encoder_get_result(): pos: %d\n", self_p->pos);
-
     if (self_p->pos >= 0) {
         length = (self_p->size - self_p->pos - 1);
         memmove(self_p->buf_p,
                 &self_p->buf_p[self_p->pos + 1],
-                length);
+                (size_t)length);
     } else {
         length = self_p->pos;
     }
 
     return (length);
 }
 
 void pbtools_encoder_abort(struct pbtools_encoder_t *self_p,
                            int error)
 {
     if (self_p->size >= 0) {
-        PRINTF("pbtools_encoder_abort(): error: %d\n", error);
         self_p->size = -error;
         self_p->pos = -error;
     }
 }
 
 void pbtools_encoder_write(struct pbtools_encoder_t *self_p,
                            uint8_t *buf_p,
                            int size)
 {
     if (self_p->pos >= size) {
         self_p->pos -= size;
-        memcpy(&self_p->buf_p[self_p->pos + 1], buf_p, size);
+        memcpy(&self_p->buf_p[self_p->pos + 1], buf_p, (size_t)size);
     } else {
         pbtools_encoder_abort(self_p, PBTOOLS_ENCODE_BUFFER_FULL);
     }
 }
 
 void pbtools_encoder_write_tag(struct pbtools_encoder_t *self_p,
                                int field_number,
                                int wire_type)
 {
     uint8_t buf[5];
     int pos;
     uint32_t value;
 
-    value = ((field_number << 3) | wire_type);
+    value = (((uint32_t)field_number << 3) | (uint32_t)wire_type);
     pos = 0;
 
     while (value > 0) {
-        buf[pos++] = (value | 0x80);
+        buf[pos++] = (uint8_t)(value | 0x80);
         value >>= 7;
     }
 
     buf[pos - 1] &= 0x7f;
     pbtools_encoder_write(self_p, &buf[0], pos);
 }
 
 void pbtools_encoder_write_varint(struct pbtools_encoder_t *self_p,
                                   uint64_t value)
 {
     uint8_t buf[10];
     int pos;
 
-    PRINTF("pbtools_encoder_write_varint(): value: 0x%llx\n",
-           (unsigned long long)value);
-
     pos = 0;
 
     do {
-        buf[pos++] = (value | 0x80);
+        buf[pos++] = (uint8_t)(value | 0x80);
         value >>= 7;
     } while (value > 0);
 
     buf[pos - 1] &= 0x7f;
     pbtools_encoder_write(self_p, &buf[0], pos);
-
-    PRINTF("pbtools_encoder_write_varint(): done\n");
 }
 
 void pbtools_encoder_write_tagged_varint(struct pbtools_encoder_t *self_p,
                                          int field_number,
                                          int wire_type,
                                          uint64_t value)
 {
@@ -277,89 +269,73 @@
 }
 
 void pbtools_encoder_write_fixed32_value(struct pbtools_encoder_t *self_p,
                                          uint32_t value)
 {
     uint8_t buf[4];
 
-    buf[0] = (value & 0xff);
-    buf[1] = ((value >> 8) & 0xff);
-    buf[2] = ((value >> 16) & 0xff);
-    buf[3] = ((value >> 24) & 0xff);
+    buf[0] = (uint8_t)(value & 0xff);
+    buf[1] = (uint8_t)((value >> 8) & 0xff);
+    buf[2] = (uint8_t)((value >> 16) & 0xff);
+    buf[3] = (uint8_t)((value >> 24) & 0xff);
     pbtools_encoder_write(self_p, &buf[0], 4);
 }
 
 void pbtools_encoder_write_fixed32(struct pbtools_encoder_t *self_p,
                                    int field_number,
                                    uint32_t value)
 {
-    uint8_t buf[4];
-
     if (value != 0) {
-        buf[0] = (value & 0xff);
-        buf[1] = ((value >> 8) & 0xff);
-        buf[2] = ((value >> 16) & 0xff);
-        buf[3] = ((value >> 24) & 0xff);
-        pbtools_encoder_write(self_p, &buf[0], 4);
+        pbtools_encoder_write_fixed32_value(self_p, value);
         pbtools_encoder_write_tag(self_p,
                                   field_number,
                                   PBTOOLS_WIRE_TYPE_FIXED_32);
     }
 }
 
 void pbtools_encoder_write_fixed64_value(struct pbtools_encoder_t *self_p,
                                          uint64_t value)
 {
     uint8_t buf[8];
 
-    buf[0] = (value & 0xff);
-    buf[1] = ((value >> 8) & 0xff);
-    buf[2] = ((value >> 16) & 0xff);
-    buf[3] = ((value >> 24) & 0xff);
-    buf[4] = ((value >> 32) & 0xff);
-    buf[5] = ((value >> 40) & 0xff);
-    buf[6] = ((value >> 48) & 0xff);
-    buf[7] = ((value >> 56) & 0xff);
+    buf[0] = (uint8_t)(value & 0xff);
+    buf[1] = (uint8_t)((value >> 8) & 0xff);
+    buf[2] = (uint8_t)((value >> 16) & 0xff);
+    buf[3] = (uint8_t)((value >> 24) & 0xff);
+    buf[4] = (uint8_t)((value >> 32) & 0xff);
+    buf[5] = (uint8_t)((value >> 40) & 0xff);
+    buf[6] = (uint8_t)((value >> 48) & 0xff);
+    buf[7] = (uint8_t)((value >> 56) & 0xff);
     pbtools_encoder_write(self_p, &buf[0], 8);
 }
 
 void pbtools_encoder_write_fixed64(struct pbtools_encoder_t *self_p,
                                    int field_number,
                                    uint64_t value)
 {
-    uint8_t buf[8];
-
     if (value != 0) {
-        buf[0] = (value & 0xff);
-        buf[1] = ((value >> 8) & 0xff);
-        buf[2] = ((value >> 16) & 0xff);
-        buf[3] = ((value >> 24) & 0xff);
-        buf[4] = ((value >> 32) & 0xff);
-        buf[5] = ((value >> 40) & 0xff);
-        buf[6] = ((value >> 48) & 0xff);
-        buf[7] = ((value >> 56) & 0xff);
-        pbtools_encoder_write(self_p, &buf[0], 8);
+        pbtools_encoder_write_fixed64_value(self_p, value);
         pbtools_encoder_write_tag(self_p,
                                   field_number,
                                   PBTOOLS_WIRE_TYPE_FIXED_64);
     }
 }
 
 void pbtools_encoder_write_sfixed32(struct pbtools_encoder_t *self_p,
                                     int field_number,
                                     int32_t value)
 {
-    pbtools_encoder_write_fixed32(self_p, field_number, value);
+    pbtools_encoder_write_fixed32(self_p, field_number, (uint32_t)value);
 }
 
 void pbtools_encoder_write_sfixed64(struct pbtools_encoder_t *self_p,
                                     int field_number,
                                     int64_t value)
 {
-    pbtools_encoder_write_fixed64(self_p, field_number, value);
+    pbtools_encoder_write_fixed64(self_p, field_number, (uint64_t)value);
 }
 
 void pbtools_encoder_write_float(struct pbtools_encoder_t *self_p,
                                  int field_number,
                                  float value)
 {
     uint32_t data;
@@ -399,28 +375,28 @@
                                   char *value_p)
 {
     size_t length;
 
     length = strlen(value_p);
 
     if (length > 0) {
-        pbtools_encoder_write(self_p, (uint8_t *)value_p, length);
+        pbtools_encoder_write(self_p, (uint8_t *)value_p, (int)length);
         pbtools_encoder_write_tagged_varint(self_p,
                                             field_number,
                                             PBTOOLS_WIRE_TYPE_LENGTH_DELIMITED,
                                             length);
     }
 }
 
 void pbtools_encoder_write_bytes(struct pbtools_encoder_t *self_p,
                                  int field_number,
                                  struct pbtools_bytes_t *value_p)
 {
     if (value_p->size > 0) {
-        pbtools_encoder_write(self_p, value_p->buf_p, value_p->size);
+        pbtools_encoder_write(self_p, value_p->buf_p, (int)value_p->size);
         pbtools_encoder_write_tagged_varint(self_p,
                                             field_number,
                                             PBTOOLS_WIRE_TYPE_LENGTH_DELIMITED,
                                             value_p->size);
     }
 }
 
@@ -442,39 +418,41 @@
     for (i = repeated_p->length - 1; i >= 0; i--) {
         member_write(self_p, repeated_p->items_pp[i]);
     }
 
     pbtools_encoder_write_tagged_varint(self_p,
                                         field_number,
                                         PBTOOLS_WIRE_TYPE_LENGTH_DELIMITED,
-                                        pos - self_p->pos);
+                                        (uint64_t)(pos - self_p->pos));
 }
 
 static void write_repeated_int32_item(
     struct pbtools_encoder_t *self_p,
     struct pbtools_scalar_value_type_base_t *item_p)
 {
-    pbtools_encoder_write_varint(self_p,
-                                 ((struct pbtools_int32_t *)item_p)->value);
+    pbtools_encoder_write_varint(
+        self_p,
+        (uint64_t)((struct pbtools_int32_t *)item_p)->value);
 }
 
 void pbtools_encoder_write_repeated_int32(
     struct pbtools_encoder_t *self_p,
     int field_number,
     struct pbtools_repeated_int32_t *repeated_p)
 {
     WRITE_REPEATED_SCALAR_VALUE_TYPE(int32);
 }
 
 static void write_repeated_int64_item(
     struct pbtools_encoder_t *self_p,
     struct pbtools_scalar_value_type_base_t *item_p)
 {
-    pbtools_encoder_write_varint(self_p,
-                                 ((struct pbtools_int64_t *)item_p)->value);
+    pbtools_encoder_write_varint(
+        self_p,
+        (uint64_t)((struct pbtools_int64_t *)item_p)->value);
 }
 
 void pbtools_encoder_write_repeated_int64(
     struct pbtools_encoder_t *self_p,
     int field_number,
     struct pbtools_repeated_int64_t *repeated_p)
 {
@@ -597,32 +575,34 @@
     WRITE_REPEATED_SCALAR_VALUE_TYPE(fixed64);
 }
 
 static void write_repeated_sfixed32_item(
     struct pbtools_encoder_t *self_p,
     struct pbtools_scalar_value_type_base_t *item_p)
 {
-    pbtools_encoder_write_fixed32_value(self_p,
-                                        ((struct pbtools_int32_t *)item_p)->value);
+    pbtools_encoder_write_fixed32_value(
+        self_p,
+        (uint32_t)((struct pbtools_int32_t *)item_p)->value);
 }
 
 void pbtools_encoder_write_repeated_sfixed32(
     struct pbtools_encoder_t *self_p,
     int field_number,
     struct pbtools_repeated_int32_t *repeated_p)
 {
     WRITE_REPEATED_SCALAR_VALUE_TYPE(sfixed32);
 }
 
 static void write_repeated_sfixed64_item(
     struct pbtools_encoder_t *self_p,
     struct pbtools_scalar_value_type_base_t *item_p)
 {
-    pbtools_encoder_write_fixed64_value(self_p,
-                                        ((struct pbtools_int64_t *)item_p)->value);
+    pbtools_encoder_write_fixed64_value(
+        self_p,
+        (uint64_t)((struct pbtools_int64_t *)item_p)->value);
 }
 
 void pbtools_encoder_write_repeated_sfixed64(
     struct pbtools_encoder_t *self_p,
     int field_number,
     struct pbtools_repeated_int64_t *repeated_p)
 {
@@ -722,15 +702,15 @@
 
 void pbtools_decoder_init(struct pbtools_decoder_t *self_p,
                           const uint8_t *buf_p,
                           size_t size,
                           struct pbtools_heap_t *heap_p)
 {
     self_p->buf_p = buf_p;
-    self_p->size = size;
+    self_p->size = (int)size;
     self_p->pos = 0;
     self_p->heap_p = heap_p;
 }
 
 int pbtools_decoder_get_result(struct pbtools_decoder_t *self_p)
 {
     return (self_p->pos);
@@ -752,32 +732,30 @@
 
 uint8_t pbtools_decoder_get(struct pbtools_decoder_t *self_p)
 {
     uint8_t value;
 
     if (pbtools_decoder_available(self_p)) {
         value = self_p->buf_p[self_p->pos];
-        PRINTF("pbtools_decoder_get(): 0x%02x\n", value);
         self_p->pos++;
     } else {
-        PRINTF("pbtools_decoder_get(): failed\n");
         pbtools_decoder_abort(self_p, PBTOOLS_OUT_OF_DATA);
         value = 0;
     }
 
     return (value);
 }
 
 void pbtools_decoder_read(struct pbtools_decoder_t *self_p,
                           uint8_t *buf_p,
                           size_t size)
 {
-    if ((self_p->size - self_p->pos) >= size) {
+    if ((self_p->size - self_p->pos) >= (int)size) {
         memcpy(buf_p, &self_p->buf_p[self_p->pos], size);
-        self_p->pos += size;
+        self_p->pos += (int)size;
     } else {
         memset(buf_p, 0, size);
         pbtools_decoder_abort(self_p, PBTOOLS_OUT_OF_DATA);
     }
 }
 
 uint64_t pbtools_decoder_read_varint(struct pbtools_decoder_t *self_p)
@@ -792,22 +770,18 @@
     do {
         byte = pbtools_decoder_get(self_p);
         value |= (((uint64_t)byte & 0x7f) << offset);
         offset += 7;
     } while ((offset < 64) && (byte & 0x80));
 
     if (byte & 0x80) {
-        PRINTF("overflow\n");
         pbtools_decoder_abort(self_p, PBTOOLS_VARINT_OVERFLOW);
         value = 0;
     }
 
-    PRINTF("pbtools_decoder_read_varint(): value: 0x%llx\n",
-           (unsigned long long)value);
-
     return (value);
 }
 
 uint64_t pbtools_decoder_read_varint_check_wire_type(
     struct pbtools_decoder_t *self_p,
     int wire_type,
     int expected_wire_type)
@@ -833,46 +807,43 @@
 
 int pbtools_decoder_read_tag(struct pbtools_decoder_t *self_p,
                              int *wire_type_p)
 {
     uint32_t value;
     int field_number;
 
-    value = pbtools_decoder_read_varint(self_p);
-    field_number = (value >> 3);
+    value = (uint32_t)pbtools_decoder_read_varint(self_p);
+    field_number = (int)(value >> 3);
     *wire_type_p = (value & 0x7);
 
     if (field_number == 0) {
         pbtools_decoder_abort(self_p, PBTOOLS_BAD_FIELD_NUMBER);
     }
 
-    PRINTF("pbtools_decoder_read_tag(): %d %d\n",
-           field_number,
-           *wire_type_p);
-
     return (field_number);
 }
 
 int32_t pbtools_decoder_read_int32(struct pbtools_decoder_t *self_p,
                                    int wire_type)
 {
-    return (pbtools_decoder_read_int64(self_p, wire_type));
+    return ((int32_t)pbtools_decoder_read_int64(self_p, wire_type));
 }
 
 int64_t pbtools_decoder_read_int64(struct pbtools_decoder_t *self_p,
                                    int wire_type)
 {
-    return (pbtools_decoder_read_varint_check_wire_type_varint(self_p,
-                                                               wire_type));
+    return ((int64_t)pbtools_decoder_read_varint_check_wire_type_varint(
+                self_p,
+                wire_type));
 }
 
 int32_t pbtools_decoder_read_sint32(struct pbtools_decoder_t *self_p,
                                     int wire_type)
 {
-    return (pbtools_decoder_read_sint64(self_p, wire_type));
+    return ((int32_t)pbtools_decoder_read_sint64(self_p, wire_type));
 }
 
 int64_t pbtools_decoder_read_sint64(struct pbtools_decoder_t *self_p,
                                     int wire_type)
 {
     uint64_t value;
 
@@ -882,21 +853,21 @@
     if (value & 0x1) {
         value >>= 1;
         value = ~value;
     } else {
         value >>= 1;
     }
 
-    return (value);
+    return ((int64_t)value);
 }
 
 uint32_t pbtools_decoder_read_uint32(struct pbtools_decoder_t *self_p,
                                      int wire_type)
 {
-    return (pbtools_decoder_read_uint64(self_p, wire_type));
+    return ((uint32_t)pbtools_decoder_read_uint64(self_p, wire_type));
 }
 
 uint64_t pbtools_decoder_read_uint64(struct pbtools_decoder_t *self_p,
                                      int wire_type)
 {
     return (pbtools_decoder_read_varint_check_wire_type_varint(self_p,
                                                                wire_type));
@@ -979,21 +950,21 @@
 
     return (value);
 }
 
 int32_t pbtools_decoder_read_sfixed32(struct pbtools_decoder_t *self_p,
                                       int wire_type)
 {
-    return (pbtools_decoder_read_fixed32(self_p, wire_type));
+    return ((int32_t)pbtools_decoder_read_fixed32(self_p, wire_type));
 }
 
 int64_t pbtools_decoder_read_sfixed64(struct pbtools_decoder_t *self_p,
                                       int wire_type)
 {
-    return (pbtools_decoder_read_fixed64(self_p, wire_type));
+    return ((int64_t)pbtools_decoder_read_fixed64(self_p, wire_type));
 }
 
 float pbtools_decoder_read_float(struct pbtools_decoder_t *self_p,
                                  int wire_type)
 {
     uint32_t data;
     float value;
@@ -1092,18 +1063,18 @@
                             struct pbtools_heap_t *heap_p,
                             int length,
                             size_t item_size)
 {
     void *items_p;
 
     items_p = NULL;
-    *items_ppp = pbtools_heap_alloc(heap_p, sizeof(items_p) * length);
+    *items_ppp = pbtools_heap_alloc(heap_p, sizeof(items_p) * (size_t)length);
 
     if (*items_ppp != NULL) {
-        items_p = pbtools_heap_alloc(heap_p, item_size * length);
+        items_p = pbtools_heap_alloc(heap_p, item_size * (size_t)length);
     }
 
     return (items_p);
 }
 
 int pbtools_alloc_repeated_int32(struct pbtools_message_base_t *self_p,
                                  int length,
@@ -1148,15 +1119,15 @@
 
     size = pbtools_decoder_read_varint_check_wire_type(
         self_p,
         wire_type,
         PBTOOLS_WIRE_TYPE_LENGTH_DELIMITED);
     pos = self_p->pos;
 
-    while (self_p->pos < (pos + size)) {
+    while (self_p->pos < (pos + (int)size)) {
         item_p = pbtools_decoder_heap_alloc(self_p, item_size);
 
         if (item_p == NULL) {
             return;
         }
 
         member_read(self_p, item_p);
@@ -1173,15 +1144,18 @@
     }
 }
 
 static void read_repeated_int32_item(
     struct pbtools_decoder_t *self_p,
     struct pbtools_scalar_value_type_base_t *item_p)
 {
-    ((struct pbtools_int32_t *)item_p)->value = pbtools_decoder_read_varint(self_p);
+    struct pbtools_int32_t *int32_item_p;
+
+    int32_item_p = (struct pbtools_int32_t *)item_p;
+    int32_item_p->value = (int32_t)pbtools_decoder_read_varint(self_p);
 }
 
 void pbtools_decoder_read_repeated_int32(
     struct pbtools_decoder_t *self_p,
     int wire_type,
     struct pbtools_repeated_int32_t *repeated_p)
 {
@@ -1194,15 +1168,15 @@
 {
     struct pbtools_int32_t *item_p;
     int i;
 
     if (repeated_p->length > 0) {
         repeated_p->items_pp = pbtools_decoder_heap_alloc(
             self_p,
-            sizeof(item_p) * repeated_p->length);
+            sizeof(item_p) * (size_t)repeated_p->length);
 
         if (repeated_p->items_pp == NULL) {
             return;
         }
 
         item_p = repeated_p->head_p;
 
@@ -1243,15 +1217,18 @@
     return (0);
 }
 
 static void read_repeated_int64_item(
     struct pbtools_decoder_t *self_p,
     struct pbtools_scalar_value_type_base_t *item_p)
 {
-    ((struct pbtools_int64_t *)item_p)->value = pbtools_decoder_read_varint(self_p);
+    struct pbtools_int64_t *int64_item_p;
+
+    int64_item_p = (struct pbtools_int64_t *)item_p;
+    int64_item_p->value = (int64_t)pbtools_decoder_read_varint(self_p);
 }
 
 void pbtools_decoder_read_repeated_int64(
     struct pbtools_decoder_t *self_p,
     int wire_type,
     struct pbtools_repeated_int64_t *repeated_p)
 {
@@ -1264,15 +1241,15 @@
 {
     struct pbtools_int64_t *item_p;
     int i;
 
     if (repeated_p->length > 0) {
         repeated_p->items_pp = pbtools_decoder_heap_alloc(
             self_p,
-            sizeof(item_p) * repeated_p->length);
+            sizeof(item_p) * (size_t)repeated_p->length);
 
         if (repeated_p->items_pp == NULL) {
             return;
         }
 
         item_p = repeated_p->head_p;
 
@@ -1313,15 +1290,18 @@
     return (0);
 }
 
 static void read_repeated_uint32_item(
     struct pbtools_decoder_t *self_p,
     struct pbtools_scalar_value_type_base_t *item_p)
 {
-    ((struct pbtools_uint32_t *)item_p)->value = pbtools_decoder_read_varint(self_p);
+    struct pbtools_uint32_t *uint32_item_p;
+
+    uint32_item_p = (struct pbtools_uint32_t *)item_p;
+    uint32_item_p->value = (uint32_t)pbtools_decoder_read_varint(self_p);
 }
 
 void pbtools_decoder_read_repeated_uint32(
     struct pbtools_decoder_t *self_p,
     int wire_type,
     struct pbtools_repeated_uint32_t *repeated_p)
 {
@@ -1334,15 +1314,15 @@
 {
     struct pbtools_uint32_t *item_p;
     int i;
 
     if (repeated_p->length > 0) {
         repeated_p->items_pp = pbtools_decoder_heap_alloc(
             self_p,
-            sizeof(item_p) * repeated_p->length);
+            sizeof(item_p) * (size_t)repeated_p->length);
 
         if (repeated_p->items_pp == NULL) {
             return;
         }
 
         item_p = repeated_p->head_p;
 
@@ -1404,15 +1384,15 @@
 {
     struct pbtools_uint64_t *item_p;
     int i;
 
     if (repeated_p->length > 0) {
         repeated_p->items_pp = pbtools_decoder_heap_alloc(
             self_p,
-            sizeof(item_p) * repeated_p->length);
+            sizeof(item_p) * (size_t)repeated_p->length);
 
         if (repeated_p->items_pp == NULL) {
             return;
         }
 
         item_p = repeated_p->head_p;
 
@@ -1441,15 +1421,15 @@
     if (value & 0x1) {
         value >>= 1;
         value = ~value;
     } else {
         value >>= 1;
     }
 
-    ((struct pbtools_int32_t *)item_p)->value = value;
+    ((struct pbtools_int32_t *)item_p)->value = (int32_t)value;
 }
 
 void pbtools_decoder_read_repeated_sint32(
     struct pbtools_decoder_t *self_p,
     int wire_type,
     struct pbtools_repeated_int32_t *repeated_p)
 {
@@ -1481,15 +1461,15 @@
     if (value & 0x1) {
         value >>= 1;
         value = ~value;
     } else {
         value >>= 1;
     }
 
-    ((struct pbtools_int64_t *)item_p)->value = value;
+    ((struct pbtools_int64_t *)item_p)->value = (int64_t)value;
 }
 
 void pbtools_decoder_read_repeated_sint64(
     struct pbtools_decoder_t *self_p,
     int wire_type,
     struct pbtools_repeated_int64_t *repeated_p)
 {
@@ -1570,16 +1550,18 @@
     return (pbtools_alloc_repeated_int32(self_p, length, repeated_p));
 }
 
 static void read_repeated_sfixed32_item(
     struct pbtools_decoder_t *self_p,
     struct pbtools_scalar_value_type_base_t *item_p)
 {
-    ((struct pbtools_int32_t *)item_p)->value =
-        pbtools_decoder_read_fixed32_value(self_p);
+    struct pbtools_int32_t *int32_item_p;
+
+    int32_item_p = (struct pbtools_int32_t *)item_p;
+    int32_item_p->value = (int32_t)pbtools_decoder_read_fixed32_value(self_p);
 }
 
 void pbtools_decoder_read_repeated_sfixed32(
     struct pbtools_decoder_t *self_p,
     int wire_type,
     struct pbtools_repeated_int32_t *repeated_p)
 {
@@ -1600,16 +1582,18 @@
     return (pbtools_alloc_repeated_int64(self_p, length, repeated_p));
 }
 
 static void read_repeated_sfixed64_item(
     struct pbtools_decoder_t *self_p,
     struct pbtools_scalar_value_type_base_t *item_p)
 {
-    ((struct pbtools_int64_t *)item_p)->value =
-        pbtools_decoder_read_fixed64_value(self_p);
+    struct pbtools_int64_t *int64_item_p;
+
+    int64_item_p = (struct pbtools_int64_t *)item_p;
+    int64_item_p->value = (int64_t)pbtools_decoder_read_fixed64_value(self_p);
 }
 
 void pbtools_decoder_read_repeated_sfixed64(
     struct pbtools_decoder_t *self_p,
     int wire_type,
     struct pbtools_repeated_int64_t *repeated_p)
 {
@@ -1677,15 +1661,15 @@
 {
     struct pbtools_float_t *item_p;
     int i;
 
     if (repeated_p->length > 0) {
         repeated_p->items_pp = pbtools_decoder_heap_alloc(
             self_p,
-            sizeof(item_p) * repeated_p->length);
+            sizeof(item_p) * (size_t)repeated_p->length);
 
         if (repeated_p->items_pp == NULL) {
             return;
         }
 
         item_p = repeated_p->head_p;
 
@@ -1750,15 +1734,15 @@
 {
     struct pbtools_double_t *item_p;
     int i;
 
     if (repeated_p->length > 0) {
         repeated_p->items_pp = pbtools_decoder_heap_alloc(
             self_p,
-            sizeof(item_p) * repeated_p->length);
+            sizeof(item_p) * (size_t)repeated_p->length);
 
         if (repeated_p->items_pp == NULL) {
             return;
         }
 
         item_p = repeated_p->head_p;
 
@@ -1810,15 +1794,15 @@
 
     size = pbtools_decoder_read_varint_check_wire_type(
         self_p,
         wire_type,
         PBTOOLS_WIRE_TYPE_LENGTH_DELIMITED);
     pos = self_p->pos;
 
-    while (self_p->pos < (pos + size)) {
+    while (self_p->pos < (pos + (int)size)) {
         item_p = pbtools_decoder_heap_alloc(self_p, sizeof(*item_p));
 
         if (item_p == NULL) {
             return;
         }
 
         item_p->value = (pbtools_decoder_read_varint(self_p) != 0);
@@ -1841,15 +1825,15 @@
 {
     struct pbtools_bool_t *item_p;
     int i;
 
     if (repeated_p->length > 0) {
         repeated_p->items_pp = pbtools_decoder_heap_alloc(
             self_p,
-            sizeof(item_p) * repeated_p->length);
+            sizeof(item_p) * (size_t)repeated_p->length);
 
         if (repeated_p->items_pp == NULL) {
             return;
         }
 
         item_p = repeated_p->head_p;
 
@@ -1921,15 +1905,15 @@
 {
     struct pbtools_string_t *item_p;
     int i;
 
     if (repeated_p->length > 0) {
         repeated_p->items_pp = pbtools_decoder_heap_alloc(
             self_p,
-            sizeof(item_p) * repeated_p->length);
+            sizeof(item_p) * (size_t)repeated_p->length);
 
         if (repeated_p->items_pp == NULL) {
             return;
         }
 
         item_p = repeated_p->head_p;
 
@@ -2001,15 +1985,15 @@
 {
     struct pbtools_bytes_t *item_p;
     int i;
 
     if (repeated_p->length > 0) {
         repeated_p->items_pp = pbtools_decoder_heap_alloc(
             self_p,
-            sizeof(item_p) * repeated_p->length);
+            sizeof(item_p) * (size_t)repeated_p->length);
 
         if (repeated_p->items_pp == NULL) {
             return;
         }
 
         item_p = repeated_p->head_p;
 
@@ -2036,16 +2020,14 @@
 
     self_p->heap_p = parent_p->heap_p;
 }
 
 void pbtools_decoder_seek(struct pbtools_decoder_t *self_p,
                           int offset)
 {
-    PRINTF("seek: %d\n", offset);
-
     if (self_p->pos >= 0) {
         if (offset < 0) {
             pbtools_decoder_abort(self_p, -offset);
         } else if (((unsigned int)self_p->pos + (unsigned int)offset) > INT_MAX) {
             pbtools_decoder_abort(self_p, PBTOOLS_SEEK_OVERFLOW);
         } else {
             self_p->pos += offset;
@@ -2056,15 +2038,14 @@
         }
     }
 }
 
 void pbtools_decoder_skip_field(struct pbtools_decoder_t *self_p,
                                 int wire_type)
 {
-    PRINTF("pbtools_decoder_skip_field(): %d\n", wire_type);
     uint64_t value;
 
     switch (wire_type) {
 
     case PBTOOLS_WIRE_TYPE_VARINT:
         (void)pbtools_decoder_read_varint(self_p);
         break;
@@ -2178,15 +2159,15 @@
 {
     int i;
     struct pbtools_message_base_t *item_p;
     struct pbtools_message_base_t *next_item_p;
 
     repeated_p->items_pp = pbtools_heap_alloc(
         heap_p,
-        sizeof(item_p) * length);
+        sizeof(item_p) * (size_t)length);
 
     if (repeated_p->items_pp != NULL) {
         next_item_p = NULL;
 
         for (i = length - 1; i >= 0; i--) {
             item_p = pbtools_heap_alloc(heap_p, item_size);
 
@@ -2217,27 +2198,27 @@
     int pos;
 
     for (i = repeated_p->length - 1; i >= 0; i--) {
         pos = encoder_p->pos;
         message_encode_inner(encoder_p, repeated_p->items_pp[i]);
         pbtools_encoder_write_length_delimited(encoder_p,
                                                field_number,
-                                               pos - encoder_p->pos);
+                                               (uint64_t)(pos - encoder_p->pos));
     }
 }
 
 void pbtools_decode_repeated_inner(
     struct pbtools_decoder_t *decoder_p,
     int wire_type,
     struct pbtools_repeated_message_t *repeated_p,
     size_t item_size,
     pbtools_message_init_t message_init,
     pbtools_message_decode_inner_t message_decode_inner)
 {
-    size_t size;
+    int size;
     struct pbtools_decoder_t decoder;
     struct pbtools_message_base_t *item_p;
 
     if (wire_type != PBTOOLS_WIRE_TYPE_LENGTH_DELIMITED) {
         pbtools_decoder_abort(decoder_p, PBTOOLS_BAD_WIRE_TYPE);
 
         return;
@@ -2245,15 +2226,15 @@
 
     item_p = pbtools_decoder_heap_alloc(decoder_p, item_size);
 
     if (item_p == NULL) {
         return;
     }
 
-    size = pbtools_decoder_read_varint(decoder_p);
+    size = (int)pbtools_decoder_read_varint(decoder_p);
     message_init(item_p, decoder_p->heap_p, NULL);
     pbtools_decoder_init_slice(&decoder, decoder_p, size);
     message_decode_inner(&decoder, item_p);
     pbtools_decoder_seek(decoder_p, pbtools_decoder_get_result(&decoder));
     item_p->next_p = NULL;
 
     if (repeated_p->length == 0) {
@@ -2275,15 +2256,15 @@
 
     if (repeated_p->length == 0) {
         return;
     }
 
     repeated_p->items_pp = pbtools_decoder_heap_alloc(
         decoder_p,
-        sizeof(item_p) * repeated_p->length);
+        sizeof(item_p) * (size_t)repeated_p->length);
 
     if (repeated_p->items_pp == NULL) {
         return;
     }
 
     item_p = repeated_p->head_p;
 
@@ -2302,30 +2283,30 @@
     int pos;
 
     pos = self_p->pos;
     encode_inner(self_p, message_p);
     pbtools_encoder_write_tagged_varint(self_p,
                                         field_number,
                                         PBTOOLS_WIRE_TYPE_LENGTH_DELIMITED,
-                                        pos - self_p->pos);
+                                        (uint64_t)(pos - self_p->pos));
 }
 
 void pbtools_decoder_sub_message_decode(
     struct pbtools_decoder_t *self_p,
     int wire_type,
     struct pbtools_message_base_t *message_p,
     pbtools_message_decode_inner_t decode_inner)
 {
-    size_t size;
+    int size;
     struct pbtools_decoder_t decoder;
 
     if (wire_type != PBTOOLS_WIRE_TYPE_LENGTH_DELIMITED) {
         pbtools_decoder_abort(self_p, PBTOOLS_BAD_WIRE_TYPE);
 
         return;
     }
 
-    size = pbtools_decoder_read_varint(self_p);
+    size = (int)pbtools_decoder_read_varint(self_p);
     pbtools_decoder_init_slice(&decoder, self_p, size);
     decode_inner(&decoder, message_p);
     pbtools_decoder_seek(self_p, pbtools_decoder_get_result(&decoder));
 }
```

### Comparing `pbtools-0.8.0/pbtools/c_source/__init__.py` & `pbtools-0.9.0/pbtools/c_source/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,15 @@
 {encode_body}\
 }}
 
 void {name}_decode_inner(
     struct pbtools_decoder_t *decoder_p,
     struct {name}_t *self_p)
 {{
+{unused_decode}\
     int wire_type;
 
     while (pbtools_decoder_available(decoder_p)) {{
         switch (pbtools_decoder_read_tag(decoder_p, &wire_type)) {{
 
 {decode_body}
         default:
@@ -772,14 +773,20 @@
             members.append(member)
 
         for oneof in message.oneofs:
             members.append(
                 ENCODE_ONEOF_FMT.format(name=oneof.full_name_snake_case,
                                         field_name=oneof.name))
 
+        if not members:
+            members = [
+                '    (void)encoder_p;\n'
+                '    (void)self_p;\n'
+            ]
+            
         return ''.join(members)
 
     def generate_message_decode_body(self, message):
         members = []
 
         for field in message.fields:
             if field.repeated:
@@ -987,19 +994,27 @@
 
         for inner_message in message.messages:
             self.generate_message_definitions(inner_message,
                                               declarations,
                                               definitions,
                                               public=False)
 
+        decode_body = self.generate_message_decode_body(message)
+
+        if decode_body:
+            unused_decode = ''
+        else:
+            unused_decode = '    (void)self_p;\n\n'
+
         definitions.append(
             MESSAGE_STATIC_DEFINITIONS_FMT.format(
                 name=message.full_name_snake_case,
                 encode_body=self.generate_message_encode_body(message),
-                decode_body=self.generate_message_decode_body(message),
+                decode_body=decode_body,
+                unused_decode=unused_decode,
                 members_init=self.generate_message_members_init(message),
                 finalizers=self.generate_repeated_finalizers(message)))
 
         repeated = self.generate_repeated_definitions(message)
 
         if repeated:
             definitions.append(repeated)
```

### Comparing `pbtools-0.8.0/pbtools/c_source/pbtools.h` & `pbtools-0.9.0/pbtools/c_source/pbtools.h`

 * *Files 0% similar despite different names*

```diff
@@ -212,18 +212,18 @@
     struct pbtools_decoder_t *decoder_p,
     void *self_p);
 
 struct pbtools_heap_t *pbtools_heap_new(void *buf_p,
                                         size_t size);
 
 void *pbtools_heap_alloc(struct pbtools_heap_t *self_p,
-                         int size);
+                         size_t size);
 
 void *pbtools_decoder_heap_alloc(struct pbtools_decoder_t *self_p,
-                                 int size);
+                                 size_t size);
 
 void pbtools_encoder_init(struct pbtools_encoder_t *self_p,
                           uint8_t *buf_p,
                           size_t size);
 
 int pbtools_encoder_get_result(struct pbtools_encoder_t *self_p);
 
@@ -736,15 +736,8 @@
 
 void pbtools_decoder_sub_message_decode(
     struct pbtools_decoder_t *self_p,
     int wire_type,
     struct pbtools_message_base_t *message_p,
     pbtools_message_decode_inner_t decode_inner);
 
-#if 0
-#    include <stdio.h>
-#    define PRINTF(fmt, ...) printf(fmt, ##__VA_ARGS__)
-#else
-#    define PRINTF(fmt, ...)
-#endif
-
 #endif
```

### Comparing `pbtools-0.8.0/pbtools/__init__.py` & `pbtools-0.9.0/pbtools/__init__.py`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/pbtools/parser.py` & `pbtools-0.9.0/pbtools/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         map_field = Sequence('map', '<', ident, ',', message_type, '>',
                              ident, '=', 'INT',
                              Optional(Sequence('[',
                                                OneOrMore(
                                                    Sequence(ident, '=', constant)),
                                                ']')),
                              ';')
-          
+
         field = Sequence(Optional('repeated'),
                          message_type, ident, '=', 'INT',
                          Optional(Sequence('[',
                                            OneOrMore(
                                                Sequence(ident, '=', constant)),
                                            ']')),
                          ';')
@@ -345,14 +345,35 @@
     def full_name(self):
         return '.'.join(self.namespace + [self.name])
 
     @property
     def full_name_snake_case(self):
         return camel_to_snake_case(self.full_name)
 
+    def used_types(self):
+        used_types = []
+
+        for field in self.fields:
+            if field.full_type in SCALAR_VALUE_TYPES:
+                continue
+
+            used_types.append(field.full_type)
+
+        for oneof in self.oneofs:
+            for field in oneof.fields:
+                if field.full_type in SCALAR_VALUE_TYPES:
+                    continue
+
+                used_types.append(field.full_type)
+
+        for message in self.messages:
+            used_types += message.used_types()
+
+        return list(set(used_types))
+
 
 class Rpc:
 
     def __init__(self, tokens):
         self.name = tokens[1]
         self.request_type = tokens[4][1]
         self.request_stream = False
@@ -418,14 +439,15 @@
         self.options = load_options(tree)
         self.messages = load_messages(tree, namespace)
         self.services = load_services(tree)
         self.enums = load_enums(tree, namespace)
         self.messages_stack = []
         self.resolve_messages_fields_types()
         self.resolve_messages_fields_type_kinds()
+        self.messages = self.sort_messages_by_usage(self.messages)
 
     def namespace_base(self):
         if self.package is None:
             return []
         else:
             return [self.package]
 
@@ -514,14 +536,33 @@
                 if enum.name == name:
                     return enum
 
             for message in messages:
                 if message.name == name:
                     return message
 
+    def sort_messages_by_usage(self, messages):
+        reversed_sorted_messages = []
+
+        for message in messages:
+            message.messages = self.sort_messages_by_usage(message.messages)
+
+            # Insert first in the reversed list if there are no types
+            # using this type.
+            insert_index = 0
+
+            for i, sorted_message in enumerate(reversed_sorted_messages, 1):
+                if message.full_name in sorted_message.used_types():
+                    if i > insert_index:
+                        insert_index = i
+
+            reversed_sorted_messages.insert(insert_index, message)
+
+        return list(reversed(reversed_sorted_messages))
+
 
 def parse_string(text):
     return Proto(Parser().parse(text))
 
 
 def parse_file(filename):
     with open(filename, 'r') as fin:
```

### Comparing `pbtools-0.8.0/pbtools/subparsers/generate_c_source.py` & `pbtools-0.9.0/pbtools/subparsers/generate_c_source.py`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/narwhal.c` & `pbtools-0.9.0/tests/narwhal.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/oneof.proto` & `pbtools-0.9.0/tests/files/oneof.proto`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/main.py` & `pbtools-0.9.0/tests/files/main.py`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/benchmark.proto` & `pbtools-0.9.0/tests/files/benchmark.proto`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/benchmark.h` & `pbtools-0.9.0/tests/files/c_source/benchmark.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/sfixed32.h` & `pbtools-0.9.0/tests/files/c_source/sfixed32.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/imported.h` & `pbtools-0.9.0/tests/files/c_source/imported.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/address_book.c` & `pbtools-0.9.0/tests/files/c_source/address_book.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/sint32.c` & `pbtools-0.9.0/tests/files/c_source/sint32.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/no_package.h` & `pbtools-0.9.0/tests/files/c_source/no_package.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/uint32.h` & `pbtools-0.9.0/tests/files/c_source/uint32.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/message.c` & `pbtools-0.9.0/tests/files/c_source/message.c`

 * *Files 0% similar despite different names*

```diff
@@ -234,20 +234,24 @@
 
 }
 
 void message_foo_encode_inner(
     struct pbtools_encoder_t *encoder_p,
     struct message_foo_t *self_p)
 {
+    (void)encoder_p;
+    (void)self_p;
 }
 
 void message_foo_decode_inner(
     struct pbtools_decoder_t *decoder_p,
     struct message_foo_t *self_p)
 {
+    (void)self_p;
+
     int wire_type;
 
     while (pbtools_decoder_available(decoder_p)) {
         switch (pbtools_decoder_read_tag(decoder_p, &wire_type)) {
 
 
         default:
```

### Comparing `pbtools-0.8.0/tests/files/c_source/importing.c` & `pbtools-0.9.0/tests/files/c_source/importing.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/int32.h` & `pbtools-0.9.0/tests/files/c_source/int32.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/int32.c` & `pbtools-0.9.0/tests/files/c_source/int32.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/sint64.h` & `pbtools-0.9.0/tests/files/c_source/sint64.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/map.c` & `pbtools-0.9.0/tests/files/c_source/map.c`

 * *Files 2% similar despite different names*

```diff
@@ -72,20 +72,24 @@
 
 }
 
 void map_message_encode_inner(
     struct pbtools_encoder_t *encoder_p,
     struct map_message_t *self_p)
 {
+    (void)encoder_p;
+    (void)self_p;
 }
 
 void map_message_decode_inner(
     struct pbtools_decoder_t *decoder_p,
     struct map_message_t *self_p)
 {
+    (void)self_p;
+
     int wire_type;
 
     while (pbtools_decoder_available(decoder_p)) {
         switch (pbtools_decoder_read_tag(decoder_p, &wire_type)) {
 
 
         default:
```

### Comparing `pbtools-0.8.0/tests/files/c_source/uint64.h` & `pbtools-0.9.0/tests/files/c_source/uint64.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/service.h` & `pbtools-0.9.0/tests/files/c_source/service.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/tags.h` & `pbtools-0.9.0/tests/files/c_source/tags.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/sfixed64.c` & `pbtools-0.9.0/tests/files/c_source/sfixed64.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/bytes.h` & `pbtools-0.9.0/tests/files/c_source/bytes.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/sfixed32.c` & `pbtools-0.9.0/tests/files/c_source/sfixed32.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/float.h` & `pbtools-0.9.0/tests/files/c_source/float.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/message.h` & `pbtools-0.9.0/tests/files/c_source/message.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/sfixed64.h` & `pbtools-0.9.0/tests/files/c_source/sfixed64.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/sint32.h` & `pbtools-0.9.0/tests/files/c_source/sint32.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/bytes.c` & `pbtools-0.9.0/tests/files/c_source/bytes.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/no_package.c` & `pbtools-0.9.0/tests/files/c_source/no_package.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/fixed64.h` & `pbtools-0.9.0/tests/files/c_source/fixed64.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/int64.h` & `pbtools-0.9.0/tests/files/c_source/int64.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/double.c` & `pbtools-0.9.0/tests/files/c_source/double.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/fixed32.h` & `pbtools-0.9.0/tests/files/c_source/fixed32.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/importing.h` & `pbtools-0.9.0/tests/files/c_source/importing.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/benchmark.c` & `pbtools-0.9.0/tests/files/c_source/benchmark.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/uint64.c` & `pbtools-0.9.0/tests/files/c_source/uint64.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/float.c` & `pbtools-0.9.0/tests/files/c_source/float.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/string.c` & `pbtools-0.9.0/tests/files/c_source/string.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/fixed64.c` & `pbtools-0.9.0/tests/files/c_source/fixed64.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/repeated.h` & `pbtools-0.9.0/tests/files/c_source/repeated.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/options.h` & `pbtools-0.9.0/tests/files/c_source/options.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/options.c` & `pbtools-0.9.0/tests/files/c_source/options.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/enum.h` & `pbtools-0.9.0/tests/files/c_source/enum.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/fixed32.c` & `pbtools-0.9.0/tests/files/c_source/fixed32.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/tags.c` & `pbtools-0.9.0/tests/files/c_source/tags.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/bool.h` & `pbtools-0.9.0/tests/files/c_source/bool.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/imported.c` & `pbtools-0.9.0/tests/files/c_source/imported.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/bool.c` & `pbtools-0.9.0/tests/files/c_source/bool.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/oneof.c` & `pbtools-0.9.0/tests/files/c_source/oneof.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/oneof.h` & `pbtools-0.9.0/tests/files/c_source/oneof.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/imported2.c` & `pbtools-0.9.0/tests/files/c_source/imported2.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/address_book.h` & `pbtools-0.9.0/tests/files/c_source/address_book.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/service.c` & `pbtools-0.9.0/tests/files/c_source/service.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/uint32.c` & `pbtools-0.9.0/tests/files/c_source/uint32.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/enum.c` & `pbtools-0.9.0/tests/files/c_source/enum.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/sint64.c` & `pbtools-0.9.0/tests/files/c_source/sint64.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/scalar_value_types.h` & `pbtools-0.9.0/tests/files/c_source/scalar_value_types.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/scalar_value_types.c` & `pbtools-0.9.0/tests/files/c_source/scalar_value_types.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/map.h` & `pbtools-0.9.0/tests/files/c_source/map.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/double.h` & `pbtools-0.9.0/tests/files/c_source/double.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/string.h` & `pbtools-0.9.0/tests/files/c_source/string.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/repeated.c` & `pbtools-0.9.0/tests/files/c_source/repeated.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/int64.c` & `pbtools-0.9.0/tests/files/c_source/int64.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/c_source/imported2.h` & `pbtools-0.9.0/tests/files/c_source/imported2.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/files/repeated.proto` & `pbtools-0.9.0/tests/files/repeated.proto`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/test_parser.py` & `pbtools-0.9.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/narwhal.h` & `pbtools-0.9.0/tests/narwhal.h`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/main_fuzzer.c` & `pbtools-0.9.0/tests/main_fuzzer.c`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/tests/main.c` & `pbtools-0.9.0/tests/main.c`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #include "files/c_source/oneof.h"
 #include "files/c_source/repeated.h"
 #include "files/c_source/scalar_value_types.h"
 #include "files/c_source/message.h"
 #include "files/c_source/benchmark.h"
 #include "files/c_source/no_package.h"
 #include "files/c_source/importing.h"
+#include "files/c_source/ordering.h"
 
 #define membersof(a) (sizeof(a) / sizeof((a)[0]))
 
 TEST(int32)
 {
     int i;
     uint8_t encoded[128];
```

### Comparing `pbtools-0.8.0/tests/test_command_line.py` & `pbtools-0.9.0/tests/test_command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
             'int32',
             'int64',
             'message',
             'map',
             'no_package',
             'oneof',
             'options',
+            'ordering',
             'repeated',
             'scalar_value_types',
             'service',
             'sfixed32',
             'sfixed64',
             'sint32',
             'sint64',
```

### Comparing `pbtools-0.8.0/README.rst` & `pbtools-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/LICENSE` & `pbtools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pbtools-0.8.0/PKG-INFO` & `pbtools-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pbtools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Google Protocol Buffers tools.
 Home-page: https://github.com/eerimoq/pbtools
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: |buildstatus|_
```

### Comparing `pbtools-0.8.0/setup.py` & `pbtools-0.9.0/setup.py`

 * *Files identical despite different names*

