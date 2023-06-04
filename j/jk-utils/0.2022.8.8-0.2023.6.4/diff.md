# Comparing `tmp/jk_utils-0.2022.8.8.tar.gz` & `tmp/jk_utils-0.2023.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jk_utils-0.2022.8.8.tar", last modified: Mon Aug  8 15:42:29 2022, max compression
+gzip compressed data, was "jk_utils-0.2023.6.4.tar", last modified: Sun Jun  4 21:46:47 2023, max compression
```

## Comparing `jk_utils-0.2022.8.8.tar` & `jk_utils-0.2023.6.4.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-08 15:42:29.699586 jk_utils-0.2022.8.8/
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)    10173 2022-02-06 12:56:11.000000 jk_utils-0.2022.8.8/LICENSE.txt
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)       38 2022-08-08 15:38:21.000000 jk_utils-0.2022.8.8/MANIFEST.in
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     1653 2022-08-08 15:42:29.699586 jk_utils-0.2022.8.8/PKG-INFO
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      858 2022-02-06 12:56:11.000000 jk_utils-0.2022.8.8/README.md
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-08 15:42:29.695586 jk_utils-0.2022.8.8/jk_utils/
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     6478 2020-12-27 01:42:13.000000 jk_utils-0.2022.8.8/jk_utils/AmountOfBytes.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     7007 2018-09-23 02:51:43.000000 jk_utils-0.2022.8.8/jk_utils/AsyncRunner.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2011 2020-12-14 14:13:16.000000 jk_utils-0.2022.8.8/jk_utils/Bytes.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1011 2019-08-22 05:23:52.000000 jk_utils-0.2022.8.8/jk_utils/Cache.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     9102 2022-02-06 10:31:13.000000 jk_utils-0.2022.8.8/jk_utils/ChModValue.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      736 2019-08-22 05:23:11.000000 jk_utils-0.2022.8.8/jk_utils/ChangedFlag.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1767 2019-08-22 05:22:52.000000 jk_utils-0.2022.8.8/jk_utils/CmdLineParser.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     5669 2020-04-20 05:03:59.000000 jk_utils-0.2022.8.8/jk_utils/DataMatrix.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      795 2019-08-22 05:24:02.000000 jk_utils-0.2022.8.8/jk_utils/DelayedKeyboardInterrupt.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2640 2019-10-21 12:56:41.000000 jk_utils-0.2022.8.8/jk_utils/EnumBase.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1580 2019-08-22 05:24:17.000000 jk_utils-0.2022.8.8/jk_utils/GracefullyHandleInterrupts.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      801 2021-12-14 16:56:03.000000 jk_utils-0.2022.8.8/jk_utils/GracefullyHandleKeyboardInterrupt.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1284 2022-01-08 16:24:45.000000 jk_utils-0.2022.8.8/jk_utils/ImplementationError.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1284 2021-01-11 11:45:52.000000 jk_utils-0.2022.8.8/jk_utils/InterruptedException.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      385 2018-10-10 13:02:31.000000 jk_utils-0.2022.8.8/jk_utils/MultiCounterDict.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1051 2019-08-22 05:24:38.000000 jk_utils-0.2022.8.8/jk_utils/MutableString.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     3527 2020-10-07 22:28:01.000000 jk_utils-0.2022.8.8/jk_utils/ObservableEvent.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      353 2020-10-20 19:07:40.000000 jk_utils-0.2022.8.8/jk_utils/PIDFile.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1794 2019-04-14 11:41:42.000000 jk_utils-0.2022.8.8/jk_utils/PersistentProperties.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      598 2020-04-20 05:03:05.000000 jk_utils-0.2022.8.8/jk_utils/RandomStateID.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     3197 2018-10-02 07:11:08.000000 jk_utils-0.2022.8.8/jk_utils/RoundRobinSequence.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      993 2019-08-22 05:24:54.000000 jk_utils-0.2022.8.8/jk_utils/Stack.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     6135 2019-12-04 01:11:19.000000 jk_utils-0.2022.8.8/jk_utils/StateManager.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1617 2021-01-11 08:57:34.000000 jk_utils-0.2022.8.8/jk_utils/TerminationFlag.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     3488 2019-08-22 05:24:58.000000 jk_utils-0.2022.8.8/jk_utils/TextCanvas.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1004 2020-10-12 22:54:44.000000 jk_utils-0.2022.8.8/jk_utils/TextOutputBuffer.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)    10243 2019-08-22 05:25:03.000000 jk_utils-0.2022.8.8/jk_utils/TextTable.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2754 2018-09-23 20:59:04.000000 jk_utils-0.2022.8.8/jk_utils/TimeLimitedCache.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     5330 2021-01-11 21:34:17.000000 jk_utils-0.2022.8.8/jk_utils/TimeStamp.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      975 2019-08-22 05:25:06.000000 jk_utils-0.2022.8.8/jk_utils/Timer.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      973 2019-08-22 05:25:16.000000 jk_utils-0.2022.8.8/jk_utils/TypedValue.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1948 2020-12-24 05:45:50.000000 jk_utils-0.2022.8.8/jk_utils/VolatileValue.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2283 2022-08-08 15:39:00.000000 jk_utils-0.2022.8.8/jk_utils/__init__.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     5640 2022-01-25 17:04:31.000000 jk_utils-0.2022.8.8/jk_utils/arp.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      378 2020-10-31 23:15:42.000000 jk_utils-0.2022.8.8/jk_utils/array.py
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-08 15:42:29.695586 jk_utils-0.2022.8.8/jk_utils/async/
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      476 2021-02-16 16:06:27.000000 jk_utils-0.2022.8.8/jk_utils/async/TabularWriterMediaWiki.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      710 2021-02-16 16:06:32.000000 jk_utils-0.2022.8.8/jk_utils/async/TabularWriterSTDOUT.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)       97 2022-08-08 15:38:21.000000 jk_utils-0.2022.8.8/jk_utils/async/__init__.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     5553 2021-02-16 16:05:29.000000 jk_utils-0.2022.8.8/jk_utils/async/queues.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      487 2020-10-30 21:40:01.000000 jk_utils-0.2022.8.8/jk_utils/check.py
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-08 15:42:29.695586 jk_utils-0.2022.8.8/jk_utils/color/
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2062 2019-12-03 22:15:42.000000 jk_utils-0.2022.8.8/jk_utils/color/RGB.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      689 2019-12-03 21:55:32.000000 jk_utils-0.2022.8.8/jk_utils/color/RGBSpectrum.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1345 2019-12-03 21:44:44.000000 jk_utils-0.2022.8.8/jk_utils/color/RGBSpectrumBuilder.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      111 2022-08-08 15:38:21.000000 jk_utils-0.2022.8.8/jk_utils/color/__init__.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     5340 2019-08-22 05:23:57.000000 jk_utils-0.2022.8.8/jk_utils/datanodes.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1973 2020-04-11 10:56:04.000000 jk_utils-0.2022.8.8/jk_utils/datatypes.py
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-08 15:42:29.695586 jk_utils-0.2022.8.8/jk_utils/datetime/
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)    15319 2021-05-19 11:12:41.000000 jk_utils-0.2022.8.8/jk_utils/datetime/D.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     6005 2021-06-29 06:56:55.000000 jk_utils-0.2022.8.8/jk_utils/datetime/T1.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     4979 2021-05-08 19:27:57.000000 jk_utils-0.2022.8.8/jk_utils/datetime/T5.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     7287 2021-05-10 12:26:32.000000 jk_utils-0.2022.8.8/jk_utils/datetime/TApprox.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      173 2022-08-08 15:38:21.000000 jk_utils-0.2022.8.8/jk_utils/datetime/__init__.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      759 2020-04-11 08:38:41.000000 jk_utils-0.2022.8.8/jk_utils/datetime/dateiterator.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      409 2020-04-09 18:38:21.000000 jk_utils-0.2022.8.8/jk_utils/datetime/timeiterator5.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      331 2021-02-16 16:07:53.000000 jk_utils-0.2022.8.8/jk_utils/deferred.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      886 2021-01-11 10:53:30.000000 jk_utils-0.2022.8.8/jk_utils/deprecated.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      863 2019-08-22 05:24:09.000000 jk_utils-0.2022.8.8/jk_utils/dtutils.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     4478 2021-01-13 19:11:20.000000 jk_utils-0.2022.8.8/jk_utils/duration.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)    10004 2020-11-01 22:01:07.000000 jk_utils-0.2022.8.8/jk_utils/file_rw.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     6772 2020-12-15 13:56:42.000000 jk_utils-0.2022.8.8/jk_utils/fsutils.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1296 2019-12-03 22:00:45.000000 jk_utils-0.2022.8.8/jk_utils/hex.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2485 2022-01-25 17:04:16.000000 jk_utils-0.2022.8.8/jk_utils/ip.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      700 2022-01-25 17:03:45.000000 jk_utils-0.2022.8.8/jk_utils/mac.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      150 2020-10-27 17:16:59.000000 jk_utils-0.2022.8.8/jk_utils/oop.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2098 2018-12-07 20:30:25.000000 jk_utils-0.2022.8.8/jk_utils/pathutils.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     9557 2022-02-25 09:09:48.000000 jk_utils-0.2022.8.8/jk_utils/ping.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     4819 2022-01-14 23:43:49.000000 jk_utils-0.2022.8.8/jk_utils/processes.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1162 2020-11-09 09:45:47.000000 jk_utils-0.2022.8.8/jk_utils/python.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2361 2020-02-11 17:41:22.000000 jk_utils-0.2022.8.8/jk_utils/pythonmodules.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2191 2020-11-02 20:56:58.000000 jk_utils-0.2022.8.8/jk_utils/re.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      446 2019-08-22 05:24:49.000000 jk_utils-0.2022.8.8/jk_utils/reflection.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     4424 2018-11-08 18:02:28.000000 jk_utils-0.2022.8.8/jk_utils/rng.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2860 2021-03-16 06:38:07.000000 jk_utils-0.2022.8.8/jk_utils/showCapacityProgress.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)    16822 2020-10-12 21:09:15.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer.py
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-08 15:42:29.699586 jk_utils-0.2022.8.8/jk_utils/tokenizer2/
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     3619 2020-05-13 14:58:10.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/AbstractTokenPattern.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     7106 2020-10-12 21:09:15.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/RegExBasedTableTokenizer.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     5083 2020-10-12 21:09:15.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/RegExBasedTokenizer.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      496 2020-02-27 21:44:12.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/Token.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2521 2020-02-27 21:33:08.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPattern.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1519 2020-02-27 21:34:32.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPatternAlternatives.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1925 2020-05-15 10:46:44.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPatternDelimLoop.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1614 2020-02-27 21:33:53.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPatternRepeat.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1385 2020-05-15 10:38:35.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPatternRepeatUntilNot.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1749 2020-02-27 21:33:30.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPatternSequence.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      307 2020-05-27 06:21:52.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenizationError.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      608 2022-08-08 15:38:21.000000 jk_utils-0.2022.8.8/jk_utils/tokenizer2/__init__.py
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-08 15:42:29.699586 jk_utils-0.2022.8.8/jk_utils/typed/
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     6220 2020-12-23 22:56:03.000000 jk_utils-0.2022.8.8/jk_utils/typed/TypedList.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)       35 2022-08-08 15:38:21.000000 jk_utils-0.2022.8.8/jk_utils/typed/__init__.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     7995 2021-12-14 16:58:14.000000 jk_utils-0.2022.8.8/jk_utils/users.py
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-08 15:42:29.699586 jk_utils-0.2022.8.8/jk_utils/weakref/
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2249 2021-01-10 15:43:31.000000 jk_utils-0.2022.8.8/jk_utils/weakref/WeakRefObservableEvent.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1986 2021-01-10 15:50:13.000000 jk_utils-0.2022.8.8/jk_utils/weakref/WeakValueList.py
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)      102 2022-08-08 15:38:21.000000 jk_utils-0.2022.8.8/jk_utils/weakref/__init__.py
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-08 15:42:29.695586 jk_utils-0.2022.8.8/jk_utils.egg-info/
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1653 2022-08-08 15:42:29.000000 jk_utils-0.2022.8.8/jk_utils.egg-info/PKG-INFO
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2725 2022-08-08 15:42:29.000000 jk_utils-0.2022.8.8/jk_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)        1 2022-08-08 15:42:29.000000 jk_utils-0.2022.8.8/jk_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)        1 2019-11-06 12:11:19.000000 jk_utils-0.2022.8.8/jk_utils.egg-info/not-zip-safe
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)       53 2022-08-08 15:42:29.000000 jk_utils-0.2022.8.8/jk_utils.egg-info/requires.txt
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)        9 2022-08-08 15:42:29.000000 jk_utils-0.2022.8.8/jk_utils.egg-info/top_level.txt
--rw-rw----   0 woodoo    (1000) woodoo    (1000)       38 2022-08-08 15:42:29.699586 jk_utils-0.2022.8.8/setup.cfg
--rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1542 2022-08-08 15:38:33.000000 jk_utils-0.2022.8.8/setup.py
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-04 21:46:47.897529 jk_utils-0.2023.6.4/
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)    10173 2022-02-06 12:56:11.000000 jk_utils-0.2023.6.4/LICENSE.txt
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)       38 2022-08-08 15:38:21.000000 jk_utils-0.2023.6.4/MANIFEST.in
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)     1653 2023-06-04 21:46:47.897529 jk_utils-0.2023.6.4/PKG-INFO
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      858 2022-02-06 12:56:11.000000 jk_utils-0.2023.6.4/README.md
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-04 21:46:47.893529 jk_utils-0.2023.6.4/jk_utils/
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     6478 2020-12-27 01:42:13.000000 jk_utils-0.2023.6.4/jk_utils/AmountOfBytes.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     7007 2018-09-23 02:51:43.000000 jk_utils-0.2023.6.4/jk_utils/AsyncRunner.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2011 2020-12-14 14:13:16.000000 jk_utils-0.2023.6.4/jk_utils/Bytes.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1011 2019-08-22 05:23:52.000000 jk_utils-0.2023.6.4/jk_utils/Cache.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     9102 2022-02-06 10:31:13.000000 jk_utils-0.2023.6.4/jk_utils/ChModValue.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      736 2019-08-22 05:23:11.000000 jk_utils-0.2023.6.4/jk_utils/ChangedFlag.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1767 2019-08-22 05:22:52.000000 jk_utils-0.2023.6.4/jk_utils/CmdLineParser.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     5669 2020-04-20 05:03:59.000000 jk_utils-0.2023.6.4/jk_utils/DataMatrix.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      795 2019-08-22 05:24:02.000000 jk_utils-0.2023.6.4/jk_utils/DelayedKeyboardInterrupt.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2918 2023-04-03 20:11:17.000000 jk_utils-0.2023.6.4/jk_utils/EnumBase.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1580 2019-08-22 05:24:17.000000 jk_utils-0.2023.6.4/jk_utils/GracefullyHandleInterrupts.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      801 2021-12-14 16:56:03.000000 jk_utils-0.2023.6.4/jk_utils/GracefullyHandleKeyboardInterrupt.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1284 2022-01-08 16:24:45.000000 jk_utils-0.2023.6.4/jk_utils/ImplementationError.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1284 2021-01-11 11:45:52.000000 jk_utils-0.2023.6.4/jk_utils/InterruptedException.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      385 2018-10-10 13:02:31.000000 jk_utils-0.2023.6.4/jk_utils/MultiCounterDict.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1051 2019-08-22 05:24:38.000000 jk_utils-0.2023.6.4/jk_utils/MutableString.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     3527 2020-10-07 22:28:01.000000 jk_utils-0.2023.6.4/jk_utils/ObservableEvent.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      353 2020-10-20 19:07:40.000000 jk_utils-0.2023.6.4/jk_utils/PIDFile.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1794 2019-04-14 11:41:42.000000 jk_utils-0.2023.6.4/jk_utils/PersistentProperties.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      598 2020-04-20 05:03:05.000000 jk_utils-0.2023.6.4/jk_utils/RandomStateID.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     3197 2018-10-02 07:11:08.000000 jk_utils-0.2023.6.4/jk_utils/RoundRobinSequence.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      993 2019-08-22 05:24:54.000000 jk_utils-0.2023.6.4/jk_utils/Stack.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     6135 2019-12-04 01:11:19.000000 jk_utils-0.2023.6.4/jk_utils/StateManager.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1617 2021-01-11 08:57:34.000000 jk_utils-0.2023.6.4/jk_utils/TerminationFlag.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     3488 2019-08-22 05:24:58.000000 jk_utils-0.2023.6.4/jk_utils/TextCanvas.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1004 2020-10-12 22:54:44.000000 jk_utils-0.2023.6.4/jk_utils/TextOutputBuffer.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)    10243 2019-08-22 05:25:03.000000 jk_utils-0.2023.6.4/jk_utils/TextTable.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2754 2018-09-23 20:59:04.000000 jk_utils-0.2023.6.4/jk_utils/TimeLimitedCache.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     5330 2021-01-11 21:34:17.000000 jk_utils-0.2023.6.4/jk_utils/TimeStamp.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      975 2019-08-22 05:25:06.000000 jk_utils-0.2023.6.4/jk_utils/Timer.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      973 2019-08-22 05:25:16.000000 jk_utils-0.2023.6.4/jk_utils/TypedValue.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1948 2020-12-24 05:45:50.000000 jk_utils-0.2023.6.4/jk_utils/VolatileValue.py
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)     2283 2023-06-04 21:46:00.000000 jk_utils-0.2023.6.4/jk_utils/__init__.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     5640 2022-01-25 17:04:31.000000 jk_utils-0.2023.6.4/jk_utils/arp.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      378 2020-10-31 23:15:42.000000 jk_utils-0.2023.6.4/jk_utils/array.py
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-04 21:46:47.897529 jk_utils-0.2023.6.4/jk_utils/async/
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      476 2021-02-16 16:06:27.000000 jk_utils-0.2023.6.4/jk_utils/async/TabularWriterMediaWiki.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      710 2021-02-16 16:06:32.000000 jk_utils-0.2023.6.4/jk_utils/async/TabularWriterSTDOUT.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)       97 2022-08-08 15:38:21.000000 jk_utils-0.2023.6.4/jk_utils/async/__init__.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     5553 2021-02-16 16:05:29.000000 jk_utils-0.2023.6.4/jk_utils/async/queues.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      487 2020-10-30 21:40:01.000000 jk_utils-0.2023.6.4/jk_utils/check.py
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-04 21:46:47.897529 jk_utils-0.2023.6.4/jk_utils/color/
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2062 2019-12-03 22:15:42.000000 jk_utils-0.2023.6.4/jk_utils/color/RGB.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      689 2019-12-03 21:55:32.000000 jk_utils-0.2023.6.4/jk_utils/color/RGBSpectrum.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1345 2019-12-03 21:44:44.000000 jk_utils-0.2023.6.4/jk_utils/color/RGBSpectrumBuilder.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      111 2022-08-08 15:38:21.000000 jk_utils-0.2023.6.4/jk_utils/color/__init__.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     5340 2019-08-22 05:23:57.000000 jk_utils-0.2023.6.4/jk_utils/datanodes.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1973 2020-04-11 10:56:04.000000 jk_utils-0.2023.6.4/jk_utils/datatypes.py
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-04 21:46:47.897529 jk_utils-0.2023.6.4/jk_utils/datetime/
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)    15913 2023-06-04 21:35:09.000000 jk_utils-0.2023.6.4/jk_utils/datetime/D.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     6005 2021-06-29 06:56:55.000000 jk_utils-0.2023.6.4/jk_utils/datetime/T1.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     4979 2021-05-08 19:27:57.000000 jk_utils-0.2023.6.4/jk_utils/datetime/T5.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     7287 2021-05-10 12:26:32.000000 jk_utils-0.2023.6.4/jk_utils/datetime/TApprox.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      173 2022-08-08 15:38:21.000000 jk_utils-0.2023.6.4/jk_utils/datetime/__init__.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      759 2020-04-11 08:38:41.000000 jk_utils-0.2023.6.4/jk_utils/datetime/dateiterator.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      409 2020-04-09 18:38:21.000000 jk_utils-0.2023.6.4/jk_utils/datetime/timeiterator5.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      331 2021-02-16 16:07:53.000000 jk_utils-0.2023.6.4/jk_utils/deferred.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      886 2021-01-11 10:53:30.000000 jk_utils-0.2023.6.4/jk_utils/deprecated.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      863 2019-08-22 05:24:09.000000 jk_utils-0.2023.6.4/jk_utils/dtutils.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     4478 2021-01-13 19:11:20.000000 jk_utils-0.2023.6.4/jk_utils/duration.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)    10004 2020-11-01 22:01:07.000000 jk_utils-0.2023.6.4/jk_utils/file_rw.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     6772 2020-12-15 13:56:42.000000 jk_utils-0.2023.6.4/jk_utils/fsutils.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     1296 2019-12-03 22:00:45.000000 jk_utils-0.2023.6.4/jk_utils/hex.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2485 2022-01-25 17:04:16.000000 jk_utils-0.2023.6.4/jk_utils/ip.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      700 2022-01-25 17:03:45.000000 jk_utils-0.2023.6.4/jk_utils/mac.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      150 2020-10-27 17:16:59.000000 jk_utils-0.2023.6.4/jk_utils/oop.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2098 2018-12-07 20:30:25.000000 jk_utils-0.2023.6.4/jk_utils/pathutils.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     9557 2022-02-25 09:09:48.000000 jk_utils-0.2023.6.4/jk_utils/ping.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     4819 2022-01-14 23:43:49.000000 jk_utils-0.2023.6.4/jk_utils/processes.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1162 2020-11-09 09:45:47.000000 jk_utils-0.2023.6.4/jk_utils/python.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2361 2020-02-11 17:41:22.000000 jk_utils-0.2023.6.4/jk_utils/pythonmodules.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2191 2020-11-02 20:56:58.000000 jk_utils-0.2023.6.4/jk_utils/re.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      446 2019-08-22 05:24:49.000000 jk_utils-0.2023.6.4/jk_utils/reflection.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     4424 2018-11-08 18:02:28.000000 jk_utils-0.2023.6.4/jk_utils/rng.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2860 2021-03-16 06:38:07.000000 jk_utils-0.2023.6.4/jk_utils/showCapacityProgress.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)    16822 2020-10-12 21:09:15.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer.py
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-04 21:46:47.897529 jk_utils-0.2023.6.4/jk_utils/tokenizer2/
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     3619 2020-05-13 14:58:10.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/AbstractTokenPattern.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     7106 2020-10-12 21:09:15.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/RegExBasedTableTokenizer.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     5083 2020-10-12 21:09:15.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/RegExBasedTokenizer.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      496 2020-02-27 21:44:12.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/Token.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2521 2020-02-27 21:33:08.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPattern.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1519 2020-02-27 21:34:32.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPatternAlternatives.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1925 2020-05-15 10:46:44.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPatternDelimLoop.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1614 2020-02-27 21:33:53.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPatternRepeat.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1385 2020-05-15 10:38:35.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPatternRepeatUntilNot.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1749 2020-02-27 21:33:30.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPatternSequence.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      307 2020-05-27 06:21:52.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenizationError.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      608 2022-08-08 15:38:21.000000 jk_utils-0.2023.6.4/jk_utils/tokenizer2/__init__.py
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-04 21:46:47.897529 jk_utils-0.2023.6.4/jk_utils/typed/
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     6220 2020-12-23 22:56:03.000000 jk_utils-0.2023.6.4/jk_utils/typed/TypedList.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)       35 2022-08-08 15:38:21.000000 jk_utils-0.2023.6.4/jk_utils/typed/__init__.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     7995 2021-12-14 16:58:14.000000 jk_utils-0.2023.6.4/jk_utils/users.py
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-04 21:46:47.897529 jk_utils-0.2023.6.4/jk_utils/weakref/
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)     2249 2021-01-10 15:43:31.000000 jk_utils-0.2023.6.4/jk_utils/weakref/WeakRefObservableEvent.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1986 2021-01-10 15:50:13.000000 jk_utils-0.2023.6.4/jk_utils/weakref/WeakValueList.py
+-rw-r--r--   0 woodoo    (1000) woodoo    (1000)      102 2022-08-08 15:38:21.000000 jk_utils-0.2023.6.4/jk_utils/weakref/__init__.py
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-06-04 21:46:47.893529 jk_utils-0.2023.6.4/jk_utils.egg-info/
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)     1653 2023-06-04 21:46:47.000000 jk_utils-0.2023.6.4/jk_utils.egg-info/PKG-INFO
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)     2725 2023-06-04 21:46:47.000000 jk_utils-0.2023.6.4/jk_utils.egg-info/SOURCES.txt
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)        1 2023-06-04 21:46:47.000000 jk_utils-0.2023.6.4/jk_utils.egg-info/dependency_links.txt
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)        1 2023-06-04 21:46:47.000000 jk_utils-0.2023.6.4/jk_utils.egg-info/not-zip-safe
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)       53 2023-06-04 21:46:47.000000 jk_utils-0.2023.6.4/jk_utils.egg-info/requires.txt
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)        9 2023-06-04 21:46:47.000000 jk_utils-0.2023.6.4/jk_utils.egg-info/top_level.txt
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)       38 2023-06-04 21:46:47.897529 jk_utils-0.2023.6.4/setup.cfg
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)     1542 2023-06-04 21:45:42.000000 jk_utils-0.2023.6.4/setup.py
```

### Comparing `jk_utils-0.2022.8.8/LICENSE.txt` & `jk_utils-0.2023.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/PKG-INFO` & `jk_utils-0.2023.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jk_utils
-Version: 0.2022.8.8
+Version: 0.2023.6.4
 Summary: This python module provides various utility functions and classes.
 Home-page: UNKNOWN
 Author: Jürgen Knauth
 Author-email: pubsrc@binary-overflow.de
 License: Apache2
 Description: jk_utils
         ========
```

### Comparing `jk_utils-0.2022.8.8/README.md` & `jk_utils-0.2023.6.4/README.md`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/AmountOfBytes.py` & `jk_utils-0.2023.6.4/jk_utils/AmountOfBytes.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/AsyncRunner.py` & `jk_utils-0.2023.6.4/jk_utils/AsyncRunner.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/Bytes.py` & `jk_utils-0.2023.6.4/jk_utils/Bytes.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/Cache.py` & `jk_utils-0.2023.6.4/jk_utils/Cache.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/ChModValue.py` & `jk_utils-0.2023.6.4/jk_utils/ChModValue.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/ChangedFlag.py` & `jk_utils-0.2023.6.4/jk_utils/ChangedFlag.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/CmdLineParser.py` & `jk_utils-0.2023.6.4/jk_utils/CmdLineParser.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/DataMatrix.py` & `jk_utils-0.2023.6.4/jk_utils/DataMatrix.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/DelayedKeyboardInterrupt.py` & `jk_utils-0.2023.6.4/jk_utils/DelayedKeyboardInterrupt.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/EnumBase.py` & `jk_utils-0.2023.6.4/jk_utils/EnumBase.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,30 @@
 	def __new__(cls, value, name):
 		member = object.__new__(cls)
 		member._value_ = value
 		member.fullname = name
 		return member
 	#
 
+	def __gt__(self, other):
+		return self._value_ > int(other)
+	#
+
+	def __ge__(self, other):
+		return self._value_ >= int(other)
+	#
+
+	def __lt__(self, other):
+		return self._value_ < int(other)
+	#
+
+	def __le__(self, other):
+		return self._value_ <= int(other)
+	#
+
 	#
 	# Get an integer representation of this enumeration item.
 	#
 	def __int__(self):
 		return self._value_
 	#
```

### Comparing `jk_utils-0.2022.8.8/jk_utils/GracefullyHandleInterrupts.py` & `jk_utils-0.2023.6.4/jk_utils/GracefullyHandleInterrupts.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/GracefullyHandleKeyboardInterrupt.py` & `jk_utils-0.2023.6.4/jk_utils/GracefullyHandleKeyboardInterrupt.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/ImplementationError.py` & `jk_utils-0.2023.6.4/jk_utils/ImplementationError.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/InterruptedException.py` & `jk_utils-0.2023.6.4/jk_utils/InterruptedException.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/MutableString.py` & `jk_utils-0.2023.6.4/jk_utils/MutableString.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/ObservableEvent.py` & `jk_utils-0.2023.6.4/jk_utils/ObservableEvent.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/PersistentProperties.py` & `jk_utils-0.2023.6.4/jk_utils/PersistentProperties.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/RandomStateID.py` & `jk_utils-0.2023.6.4/jk_utils/RandomStateID.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/RoundRobinSequence.py` & `jk_utils-0.2023.6.4/jk_utils/RoundRobinSequence.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/Stack.py` & `jk_utils-0.2023.6.4/jk_utils/Stack.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/StateManager.py` & `jk_utils-0.2023.6.4/jk_utils/StateManager.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/TerminationFlag.py` & `jk_utils-0.2023.6.4/jk_utils/TerminationFlag.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/TextCanvas.py` & `jk_utils-0.2023.6.4/jk_utils/TextCanvas.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/TextOutputBuffer.py` & `jk_utils-0.2023.6.4/jk_utils/TextOutputBuffer.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/TextTable.py` & `jk_utils-0.2023.6.4/jk_utils/TextTable.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/TimeLimitedCache.py` & `jk_utils-0.2023.6.4/jk_utils/TimeLimitedCache.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/TimeStamp.py` & `jk_utils-0.2023.6.4/jk_utils/TimeStamp.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/Timer.py` & `jk_utils-0.2023.6.4/jk_utils/Timer.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/TypedValue.py` & `jk_utils-0.2023.6.4/jk_utils/TypedValue.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/VolatileValue.py` & `jk_utils-0.2023.6.4/jk_utils/VolatileValue.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/__init__.py` & `jk_utils-0.2023.6.4/jk_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿
 
 
 __author__ = "Jürgen Knauth"
-__version__ = "0.2022.8.8"
+__version__ = "0.2023.6.4"
 
 
 
 import os
 _bIsPOSIX = os.name == "posix"
```

### Comparing `jk_utils-0.2022.8.8/jk_utils/arp.py` & `jk_utils-0.2023.6.4/jk_utils/arp.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/async/TabularWriterSTDOUT.py` & `jk_utils-0.2023.6.4/jk_utils/async/TabularWriterSTDOUT.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/async/queues.py` & `jk_utils-0.2023.6.4/jk_utils/async/queues.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/color/RGB.py` & `jk_utils-0.2023.6.4/jk_utils/color/RGB.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/color/RGBSpectrum.py` & `jk_utils-0.2023.6.4/jk_utils/color/RGBSpectrum.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/color/RGBSpectrumBuilder.py` & `jk_utils-0.2023.6.4/jk_utils/color/RGBSpectrumBuilder.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/datanodes.py` & `jk_utils-0.2023.6.4/jk_utils/datanodes.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/datatypes.py` & `jk_utils-0.2023.6.4/jk_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/datetime/D.py` & `jk_utils-0.2023.6.4/jk_utils/datetime/D.py`

 * *Files 10% similar despite different names*

```diff
@@ -411,43 +411,57 @@
 	# @return		D		A new date object
 	#
 	def nextWeek(self):
 		wd = self._dt.weekday()
 		dt = self._dt.timestamp() - 24*60*60*wd
 		d = D()
 		d._dt = datetime.datetime.fromtimestamp(dt + 7 *24*60*60)
+		if d._dt.hour != 0:
+			# compensating for summer time / winter time change
+			d._dt = datetime.datetime.fromtimestamp(dt + 7 *24*60*60 + 3600)
 		return d
 	#
 
 	#
 	# @return		D		A new date object
 	#
 	def previousWeek(self):
 		wd = self._dt.weekday()
 		dt = self._dt.timestamp() - 24*60*60*wd
 		d = D()
 		d._dt = datetime.datetime.fromtimestamp(dt - 7 *24*60*60)
+		if d._dt.hour != 0:
+			# compensating for summer time / winter time change
+			d._dt = datetime.datetime.fromtimestamp(dt + 7 *24*60*60 - 3600)
 		return d
 	#
 
 	#
 	# @return		D		A new date object
 	#
 	def nextDay(self):
 		d = D()
-		d._dt = datetime.datetime.fromtimestamp(self._dt.timestamp() + 24*60*60)
+		dt = self._dt.timestamp()
+		d._dt = datetime.datetime.fromtimestamp(dt + 24*60*60)
+		if d._dt.hour != 0:
+			# compensating for summer time / winter time change
+			d._dt = datetime.datetime.fromtimestamp(dt + 24*60*60 + 3600)
 		return d
 	#
 
 	#
 	# @return		D		A new date object
 	#
 	def previousDay(self):
 		d = D()
-		d._dt = datetime.datetime.fromtimestamp(self._dt.timestamp() - 24*60*60)
+		dt = self._dt.timestamp()
+		d._dt = datetime.datetime.fromtimestamp(dt - 24*60*60)
+		if d._dt.hour != 0:
+			# compensating for summer time / winter time change
+			d._dt = datetime.datetime.fromtimestamp(dt + 24*60*60 - 3600)
 		return d
 	#
 
 	#
 	# @return		D		A new date object
 	#
 	def addMonths(self, m:int):
```

### Comparing `jk_utils-0.2022.8.8/jk_utils/datetime/T1.py` & `jk_utils-0.2023.6.4/jk_utils/datetime/T1.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/datetime/T5.py` & `jk_utils-0.2023.6.4/jk_utils/datetime/T5.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/datetime/TApprox.py` & `jk_utils-0.2023.6.4/jk_utils/datetime/TApprox.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/datetime/dateiterator.py` & `jk_utils-0.2023.6.4/jk_utils/datetime/dateiterator.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/deprecated.py` & `jk_utils-0.2023.6.4/jk_utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/dtutils.py` & `jk_utils-0.2023.6.4/jk_utils/dtutils.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/duration.py` & `jk_utils-0.2023.6.4/jk_utils/duration.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/file_rw.py` & `jk_utils-0.2023.6.4/jk_utils/file_rw.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/fsutils.py` & `jk_utils-0.2023.6.4/jk_utils/fsutils.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/hex.py` & `jk_utils-0.2023.6.4/jk_utils/hex.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/ip.py` & `jk_utils-0.2023.6.4/jk_utils/ip.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/mac.py` & `jk_utils-0.2023.6.4/jk_utils/mac.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/pathutils.py` & `jk_utils-0.2023.6.4/jk_utils/pathutils.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/ping.py` & `jk_utils-0.2023.6.4/jk_utils/ping.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/processes.py` & `jk_utils-0.2023.6.4/jk_utils/processes.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/python.py` & `jk_utils-0.2023.6.4/jk_utils/python.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/pythonmodules.py` & `jk_utils-0.2023.6.4/jk_utils/pythonmodules.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/re.py` & `jk_utils-0.2023.6.4/jk_utils/re.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/rng.py` & `jk_utils-0.2023.6.4/jk_utils/rng.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/showCapacityProgress.py` & `jk_utils-0.2023.6.4/jk_utils/showCapacityProgress.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/tokenizer.py` & `jk_utils-0.2023.6.4/jk_utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/tokenizer2/AbstractTokenPattern.py` & `jk_utils-0.2023.6.4/jk_utils/tokenizer2/AbstractTokenPattern.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/tokenizer2/RegExBasedTableTokenizer.py` & `jk_utils-0.2023.6.4/jk_utils/tokenizer2/RegExBasedTableTokenizer.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/tokenizer2/RegExBasedTokenizer.py` & `jk_utils-0.2023.6.4/jk_utils/tokenizer2/RegExBasedTokenizer.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPattern.py` & `jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPattern.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPatternAlternatives.py` & `jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPatternAlternatives.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPatternDelimLoop.py` & `jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPatternDelimLoop.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPatternRepeat.py` & `jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPatternRepeat.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPatternRepeatUntilNot.py` & `jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPatternRepeatUntilNot.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/tokenizer2/TokenPatternSequence.py` & `jk_utils-0.2023.6.4/jk_utils/tokenizer2/TokenPatternSequence.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/tokenizer2/__init__.py` & `jk_utils-0.2023.6.4/jk_utils/tokenizer2/__init__.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/typed/TypedList.py` & `jk_utils-0.2023.6.4/jk_utils/typed/TypedList.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/users.py` & `jk_utils-0.2023.6.4/jk_utils/users.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/weakref/WeakRefObservableEvent.py` & `jk_utils-0.2023.6.4/jk_utils/weakref/WeakRefObservableEvent.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils/weakref/WeakValueList.py` & `jk_utils-0.2023.6.4/jk_utils/weakref/WeakValueList.py`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/jk_utils.egg-info/PKG-INFO` & `jk_utils-0.2023.6.4/jk_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jk-utils
-Version: 0.2022.8.8
+Version: 0.2023.6.4
 Summary: This python module provides various utility functions and classes.
 Home-page: UNKNOWN
 Author: Jürgen Knauth
 Author-email: pubsrc@binary-overflow.de
 License: Apache2
 Description: jk_utils
         ========
```

### Comparing `jk_utils-0.2022.8.8/jk_utils.egg-info/SOURCES.txt` & `jk_utils-0.2023.6.4/jk_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jk_utils-0.2022.8.8/setup.py` & `jk_utils-0.2023.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,12 +47,12 @@
 		"jk_utils.datetime",
 		"jk_utils.tokenizer2",
 		"jk_utils.typed",
 		"jk_utils.weakref",
 	],
 	scripts = [
 	],
-	version = '0.2022.8.8',
+	version = '0.2023.6.4',
 	zip_safe = False,
 	long_description = readme(),
 	long_description_content_type = "text/markdown",
 )
```

