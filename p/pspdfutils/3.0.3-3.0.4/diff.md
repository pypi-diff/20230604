# Comparing `tmp/pspdfutils-3.0.3.tar.gz` & `tmp/pspdfutils-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pspdfutils-3.0.3.tar", last modified: Thu Jun  1 14:31:05 2023, max compression
+gzip compressed data, was "pspdfutils-3.0.4.tar", last modified: Sun Jun  4 21:25:49 2023, max compression
```

## Comparing `pspdfutils-3.0.3.tar` & `pspdfutils-3.0.4.tar`

### file list

```diff
@@ -1,409 +1,409 @@
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.770388 pspdfutils-3.0.3/
--rw-r-----   0 rrt       (1000) rrt       (1000)    35148 2020-01-25 13:35:25.000000 pspdfutils-3.0.3/COPYING
--rw-r-----   0 rrt       (1000) rrt       (1000)      387 2023-06-01 13:54:12.000000 pspdfutils-3.0.3/MANIFEST.in
--rw-r-----   0 rrt       (1000) rrt       (1000)     2936 2023-06-01 14:31:05.770388 pspdfutils-3.0.3/PKG-INFO
--rw-r-----   0 rrt       (1000) rrt       (1000)     2536 2023-06-01 13:42:27.000000 pspdfutils-3.0.3/README.md
--rw-r-----   0 rrt       (1000) rrt       (1000)       73 2023-05-11 20:36:26.000000 pspdfutils-3.0.3/epsffit-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)      686 2023-05-11 20:36:26.000000 pspdfutils-3.0.3/extractres-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)      620 2023-05-11 20:36:26.000000 pspdfutils-3.0.3/includeres-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)      440 2020-01-25 13:35:25.000000 pspdfutils-3.0.3/man-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)      866 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/psbook-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)      852 2023-05-22 13:02:42.000000 pspdfutils-3.0.3/psnup-include.man
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.726387 pspdfutils-3.0.3/pspdfutils.egg-info/
--rw-r-----   0 rrt       (1000) rrt       (1000)     2936 2023-06-01 14:31:05.000000 pspdfutils-3.0.3/pspdfutils.egg-info/PKG-INFO
--rw-r-----   0 rrt       (1000) rrt       (1000)    14540 2023-06-01 14:31:05.000000 pspdfutils-3.0.3/pspdfutils.egg-info/SOURCES.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)        1 2023-06-01 14:31:05.000000 pspdfutils-3.0.3/pspdfutils.egg-info/dependency_links.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)      405 2023-06-01 14:31:05.000000 pspdfutils-3.0.3/pspdfutils.egg-info/entry_points.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)       23 2023-06-01 14:31:05.000000 pspdfutils-3.0.3/pspdfutils.egg-info/requires.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)        8 2023-06-01 14:31:05.000000 pspdfutils-3.0.3/pspdfutils.egg-info/top_level.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)      298 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/psresize-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)       68 2023-05-11 20:36:26.000000 pspdfutils-3.0.3/psselect-include.man
--rw-r-----   0 rrt       (1000) rrt       (1000)     3224 2023-05-18 21:42:21.000000 pspdfutils-3.0.3/pstops-include.man
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.726387 pspdfutils-3.0.3/psutils/
--rw-r-----   0 rrt       (1000) rrt       (1000)      228 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/psutils/__init__.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     7971 2023-06-01 10:09:38.000000 pspdfutils-3.0.3/psutils/argparse.py
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.726387 pspdfutils-3.0.3/psutils/command/
--rw-r-----   0 rrt       (1000) rrt       (1000)     5829 2023-05-30 10:25:33.000000 pspdfutils-3.0.3/psutils/command/epsffit.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     4229 2023-05-30 10:25:33.000000 pspdfutils-3.0.3/psutils/command/extractres.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1917 2023-05-30 10:25:33.000000 pspdfutils-3.0.3/psutils/command/includeres.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     2872 2023-05-30 10:25:33.000000 pspdfutils-3.0.3/psutils/command/psbook.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     9503 2023-05-30 10:25:33.000000 pspdfutils-3.0.3/psutils/command/psjoin.py
--rw-r-----   0 rrt       (1000) rrt       (1000)    10565 2023-05-30 10:35:37.000000 pspdfutils-3.0.3/psutils/command/psnup.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     2173 2023-05-30 10:25:33.000000 pspdfutils-3.0.3/psutils/command/psresize.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     2685 2023-05-30 10:25:33.000000 pspdfutils-3.0.3/psutils/command/psselect.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     3425 2023-05-30 10:34:29.000000 pspdfutils-3.0.3/psutils/command/pstops.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1382 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/psutils/io.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/psutils/libpaper.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      980 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/psutils/psresources.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     5044 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/psutils/readers.py
--rw-r-----   0 rrt       (1000) rrt       (1000)    19306 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/psutils/transformers.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1930 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/psutils/types.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      913 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/psutils/warnings.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      931 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/psutils.1
--rw-r-----   0 rrt       (1000) rrt       (1000)     2808 2023-06-01 13:54:51.000000 pspdfutils-3.0.3/pyproject.toml
--rw-r-----   0 rrt       (1000) rrt       (1000)       38 2023-06-01 14:31:05.770388 pspdfutils-3.0.3/setup.cfg
--rw-r-----   0 rrt       (1000) rrt       (1000)      539 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/setup.py
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.730387 pspdfutils-3.0.3/tests/
--rw-r-----   0 rrt       (1000) rrt       (1000)      890 2023-05-30 10:33:45.000000 pspdfutils-3.0.3/tests/conftest.py
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.734387 pspdfutils-3.0.3/tests/test-files/
--rw-r-----   0 rrt       (1000) rrt       (1000)    13275 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/a3-20.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23046 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/a3-20.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     3332 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/a4-1.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    17476 2023-05-20 15:50:04.000000 pspdfutils-3.0.3/tests/test-files/a4-1.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     9028 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/a4-11.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20384 2023-05-20 15:50:04.000000 pspdfutils-3.0.3/tests/test-files/a4-11.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     3910 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/a4-2.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    17766 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/a4-2.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)    13208 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/a4-20.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23021 2023-05-21 09:11:51.000000 pspdfutils-3.0.3/tests/test-files/a4-20.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     4539 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/a4-3.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18056 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/a4-3.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     5005 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/a4-4-0.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18320 2023-05-20 15:50:04.000000 pspdfutils-3.0.3/tests/test-files/a4-4-0.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     3335 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/a5-1.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    17475 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/a5-1.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)    13277 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/a5-20.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23020 2023-05-20 15:50:04.000000 pspdfutils-3.0.3/tests/test-files/a5-20.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.710387 pspdfutils-3.0.3/tests/test-files/epsffit/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.734387 pspdfutils-3.0.3/tests/test-files/epsffit/aspect/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.734387 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.734387 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-maximize/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-maximize/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-maximize/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.734387 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-maximize-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-maximize-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-maximize-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.734387 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.734387 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-maximize/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-maximize/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-maximize/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.734387 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-maximize-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-maximize-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-maximize-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.734387 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/aspect-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.734387 pspdfutils-3.0.3/tests/test-files/epsffit/center/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/center/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78699 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/center/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.734387 pspdfutils-3.0.3/tests/test-files/epsffit/center-maximize/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/center-maximize/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78699 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/center-maximize/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.738387 pspdfutils-3.0.3/tests/test-files/epsffit/center-maximize-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/center-maximize-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78710 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/center-maximize-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.738387 pspdfutils-3.0.3/tests/test-files/epsffit/center-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/center-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78710 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/center-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.738387 pspdfutils-3.0.3/tests/test-files/epsffit/h-texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/h-texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     4432 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/h-texlive/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.738387 pspdfutils-3.0.3/tests/test-files/epsffit/m-texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/m-texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     4441 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/m-texlive/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.738387 pspdfutils-3.0.3/tests/test-files/epsffit/maximize/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/maximize/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/maximize/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.738387 pspdfutils-3.0.3/tests/test-files/epsffit/maximize-rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/maximize-rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/maximize-rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.738387 pspdfutils-3.0.3/tests/test-files/epsffit/no-options/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/no-options/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/no-options/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.738387 pspdfutils-3.0.3/tests/test-files/epsffit/rotate/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/rotate/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/rotate/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.738387 pspdfutils-3.0.3/tests/test-files/epsffit/showpage/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/showpage/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    78725 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/showpage/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.738387 pspdfutils-3.0.3/tests/test-files/epsffit/v-texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/v-texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     4433 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/epsffit/v-texlive/expected.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.710387 pspdfutils-3.0.3/tests/test-files/extractres/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.742388 pspdfutils-3.0.3/tests/test-files/extractres/sample/
--rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/extractres/sample/ISO-8859-1Encoding-expected.enc
--rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/extractres/sample/ISO-8859-1Encoding.enc
--rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02-expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01-expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/extractres/sample/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11851 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/extractres/sample/expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)      256 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/extractres/sample/includeres-expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    17478 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/extractres/sample/includeres-expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.710387 pspdfutils-3.0.3/tests/test-files/includeres/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.742388 pspdfutils-3.0.3/tests/test-files/includeres/sample/
--rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/includeres/sample/ISO-8859-1Encoding.enc
--rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/includeres/sample/a2ps-a2ps-hdr2.02.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/includeres/sample/a2ps-black+white-Prolog2.01.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)      280 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/includeres/sample/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    17476 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/includeres/sample/expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)     4334 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/plot.eps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.714387 pspdfutils-3.0.3/tests/test-files/psbook/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.742388 pspdfutils-3.0.3/tests/test-files/psbook/20/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/psbook/20/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/psbook/20/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psbook/20/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.742388 pspdfutils-3.0.3/tests/test-files/psbook/20-signature-4/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/psbook/20-signature-4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/psbook/20-signature-4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psbook/20-signature-4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.742388 pspdfutils-3.0.3/tests/test-files/psbook/3/
--rw-r-----   0 rrt       (1000) rrt       (1000)       31 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/psbook/3/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2867 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/psbook/3/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18081 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psbook/3/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.742388 pspdfutils-3.0.3/tests/test-files/psbook/3-signature-4/
--rw-r-----   0 rrt       (1000) rrt       (1000)       31 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/psbook/3-signature-4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2867 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/psbook/3-signature-4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18081 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psbook/3-signature-4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.742388 pspdfutils-3.0.3/tests/test-files/psbook/invalid-signature-size/
--rw-r-----   0 rrt       (1000) rrt       (1000)       43 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/psbook/invalid-signature-size/expected-stderr.txt
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.742388 pspdfutils-3.0.3/tests/test-files/psbook/texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)       66 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/psbook/texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     7167 2023-05-19 21:27:38.000000 pspdfutils-3.0.3/tests/test-files/psbook/texlive/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20410 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psbook/texlive/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.714387 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.742388 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:39.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-05-19 21:27:39.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19350 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.742388 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-even/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:39.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-even/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     3169 2023-05-19 21:27:39.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-even/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19502 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-even/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.746388 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-nostrip/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:39.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-nostrip/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-05-19 21:27:39.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-nostrip/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    35545 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-nostrip/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.746388 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-save/
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:39.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-save/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-05-19 21:27:39.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-save/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19474 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-save/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.718387 pspdfutils-3.0.3/tests/test-files/psnup/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.746388 pspdfutils-3.0.3/tests/test-files/psnup/20-1/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.746388 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flip/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:08:04.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flip/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13904 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flip/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30718 2023-05-20 21:10:37.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flip/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.746388 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    15184 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31098 2023-05-20 21:15:21.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.746388 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-21 09:11:54.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13244 2023-05-21 09:11:54.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-05-21 09:11:54.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.746388 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13024 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30858 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.746388 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13204 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.746388 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11029 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.746388 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-21 09:11:54.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13204 2023-05-21 09:11:54.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-05-21 09:11:54.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.750388 pspdfutils-3.0.3/tests/test-files/psnup/20-2/
--rw-r-----   0 rrt       (1000) rrt       (1000)       87 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-2/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11994 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-2/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31268 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-2/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.750388 pspdfutils-3.0.3/tests/test-files/psnup/20-2-inpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)       87 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-2-inpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11314 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-2-inpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30887 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-2-inpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.750388 pspdfutils-3.0.3/tests/test-files/psnup/20-3/
--rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11577 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.750388 pspdfutils-3.0.3/tests/test-files/psnup/20-3-impossible-tolerance/
--rw-r-----   0 rrt       (1000) rrt       (1000)       46 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3-impossible-tolerance/expected-stderr.txt
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.750388 pspdfutils-3.0.3/tests/test-files/psnup/20-3-inpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3-inpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11357 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3-inpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31678 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3-inpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.750388 pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedleft/
--rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedleft/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11577 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedleft/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedleft/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.750388 pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedright/
--rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedright/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11592 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedright/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedright/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.750388 pspdfutils-3.0.3/tests/test-files/psnup/20-4/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9162 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30986 2023-05-20 21:02:22.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.750388 pspdfutils-3.0.3/tests/test-files/psnup/20-4-297mmx210mm/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-297mmx210mm/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    11323 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-297mmx210mm/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31346 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-297mmx210mm/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.754388 pspdfutils-3.0.3/tests/test-files/psnup/20-4-border-20/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-border-20/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9652 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-border-20/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31146 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-border-20/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.754388 pspdfutils-3.0.3/tests/test-files/psnup/20-4-columnmajor/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-columnmajor/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9162 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-columnmajor/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30986 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-columnmajor/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.754388 pspdfutils-3.0.3/tests/test-files/psnup/20-4-flip/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-flip/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10423 2023-05-20 21:02:24.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-flip/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31346 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-flip/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.754388 pspdfutils-3.0.3/tests/test-files/psnup/20-4-impossible-border/
--rw-r-----   0 rrt       (1000) rrt       (1000)       28 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-impossible-border/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-impossible-border/expected.pdf
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.754388 pspdfutils-3.0.3/tests/test-files/psnup/20-4-impossible-margin/
--rw-r-----   0 rrt       (1000) rrt       (1000)       28 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-impossible-margin/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-impossible-margin/expected.pdf
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.754388 pspdfutils-3.0.3/tests/test-files/psnup/20-4-inpaper-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-inpaper-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9642 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-inpaper-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31125 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-inpaper-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.754388 pspdfutils-3.0.3/tests/test-files/psnup/20-4-margin-10/
--rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-margin-10/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9552 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-margin-10/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    31146 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/20-4-margin-10/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.758388 pspdfutils-3.0.3/tests/test-files/psnup/draw/
--rw-r-----   0 rrt       (1000) rrt       (1000)       25 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/draw/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     3397 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/draw/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    21521 2023-05-20 21:02:23.000000 pspdfutils-3.0.3/tests/test-files/psnup/draw/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.758388 pspdfutils-3.0.3/tests/test-files/psnup/texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)       53 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     7710 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/texlive/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    26045 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/texlive/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.758388 pspdfutils-3.0.3/tests/test-files/psnup/texlive2/
--rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/texlive2/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     9322 2023-05-20 21:02:25.000000 pspdfutils-3.0.3/tests/test-files/psnup/texlive2/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30184 2023-05-20 21:15:45.000000 pspdfutils-3.0.3/tests/test-files/psnup/texlive2/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.718387 pspdfutils-3.0.3/tests/test-files/psresize/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.758388 pspdfutils-3.0.3/tests/test-files/psresize/20-A3/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:42.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A3/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13424 2023-05-19 21:27:42.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A3/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30860 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A3/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.758388 pspdfutils-3.0.3/tests/test-files/psresize/20-A3in-A4/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A3in-A4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    12824 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A3in-A4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30901 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A3in-A4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.758388 pspdfutils-3.0.3/tests/test-files/psresize/20-A4/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:42.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-05-19 21:27:42.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.758388 pspdfutils-3.0.3/tests/test-files/psresize/20-A5/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:42.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A5/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13024 2023-05-19 21:27:42.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A5/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30858 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A5/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.758388 pspdfutils-3.0.3/tests/test-files/psresize/20-A5in-A4/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A5in-A4/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13204 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A5in-A4/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-A5in-A4/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.762388 pspdfutils-3.0.3/tests/test-files/psresize/20-Letter/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:42.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-Letter/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    13224 2023-05-19 21:27:42.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-Letter/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    30878 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psresize/20-Letter/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.718387 pspdfutils-3.0.3/tests/test-files/psselect/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.762388 pspdfutils-3.0.3/tests/test-files/psselect/even/
--rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/even/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     6613 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/even/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20103 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psselect/even/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.762388 pspdfutils-3.0.3/tests/test-files/psselect/even-reverse/
--rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/even-reverse/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     6613 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/even-reverse/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20103 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psselect/even-reverse/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.762388 pspdfutils-3.0.3/tests/test-files/psselect/individual-pages-and-dash-p/
--rw-r-----   0 rrt       (1000) rrt       (1000)       58 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/psselect/individual-pages-and-dash-p/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     6608 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/psselect/individual-pages-and-dash-p/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20111 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psselect/individual-pages-and-dash-p/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.762388 pspdfutils-3.0.3/tests/test-files/psselect/invalid-pagerange/
--rw-r-----   0 rrt       (1000) rrt       (1000)       69 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/psselect/invalid-pagerange/.bak.0.expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)       37 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/tests/test-files/psselect/invalid-pagerange/expected-stderr.txt
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.762388 pspdfutils-3.0.3/tests/test-files/psselect/negative-range/
--rw-r-----   0 rrt       (1000) rrt       (1000)       40 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/negative-range/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     4423 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/negative-range/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18649 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psselect/negative-range/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.762388 pspdfutils-3.0.3/tests/test-files/psselect/odd/
--rw-r-----   0 rrt       (1000) rrt       (1000)       61 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/odd/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     6609 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/odd/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20117 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psselect/odd/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.762388 pspdfutils-3.0.3/tests/test-files/psselect/options-and-complex-pagerange/
--rw-r-----   0 rrt       (1000) rrt       (1000)       47 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/psselect/options-and-complex-pagerange/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     5295 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/psselect/options-and-complex-pagerange/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19243 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psselect/options-and-complex-pagerange/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.762388 pspdfutils-3.0.3/tests/test-files/psselect/positive-negative-range/
--rw-r-----   0 rrt       (1000) rrt       (1000)       98 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/psselect/positive-negative-range/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10114 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/psselect/positive-negative-range/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    22455 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psselect/positive-negative-range/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.766388 pspdfutils-3.0.3/tests/test-files/psselect/positive-range/
--rw-r-----   0 rrt       (1000) rrt       (1000)       35 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/positive-range/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     4419 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/positive-range/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    18655 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psselect/positive-range/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.766388 pspdfutils-3.0.3/tests/test-files/psselect/psnup-texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)       97 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/psselect/psnup-texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10113 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/psselect/psnup-texlive/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    22453 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psselect/psnup-texlive/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.766388 pspdfutils-3.0.3/tests/test-files/psselect/reverse/
--rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/reverse/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-05-19 21:27:43.000000 pspdfutils-3.0.3/tests/test-files/psselect/reverse/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psselect/reverse/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.766388 pspdfutils-3.0.3/tests/test-files/psselect/texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)       66 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/psselect/texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     7048 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/psselect/texlive/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20410 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/psselect/texlive/expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)    10113 2023-06-01 09:56:59.000000 pspdfutils-3.0.3/tests/test-files/psselect-texlive-output.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    22453 2023-06-01 09:56:59.000000 pspdfutils-3.0.3/tests/test-files/psselect-texlive-output.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.722387 pspdfutils-3.0.3/tests/test-files/pstops/
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.766388 pspdfutils-3.0.3/tests/test-files/pstops/correct-angles/
--rw-r-----   0 rrt       (1000) rrt       (1000)       21 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/correct-angles/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2050 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/correct-angles/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20081 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/pstops/correct-angles/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.766388 pspdfutils-3.0.3/tests/test-files/pstops/default-paper-size/
--rw-r-----   0 rrt       (1000) rrt       (1000)       21 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/default-paper-size/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2082 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/default-paper-size/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20120 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/pstops/default-paper-size/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.766388 pspdfutils-3.0.3/tests/test-files/pstops/invalid-pagespecs/
--rw-r-----   0 rrt       (1000) rrt       (1000)      179 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/invalid-pagespecs/expected-stderr.txt
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.766388 pspdfutils-3.0.3/tests/test-files/pstops/multiple-pages/
--rw-r-----   0 rrt       (1000) rrt       (1000)       23 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/multiple-pages/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     2305 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/multiple-pages/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    20065 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/pstops/multiple-pages/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.766388 pspdfutils-3.0.3/tests/test-files/pstops/multiple-turns-and-flips/
--rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/multiple-turns-and-flips/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     1759 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/multiple-turns-and-flips/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19517 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/pstops/multiple-turns-and-flips/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.766388 pspdfutils-3.0.3/tests/test-files/pstops/negative-offsets/
--rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/negative-offsets/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     1669 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/negative-offsets/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19485 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/pstops/negative-offsets/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.770388 pspdfutils-3.0.3/tests/test-files/pstops/offsets/
--rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/offsets/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     1667 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/offsets/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    19483 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/pstops/offsets/expected.ps
-drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-01 14:31:05.770388 pspdfutils-3.0.3/tests/test-files/pstops/texlive/
--rw-r-----   0 rrt       (1000) rrt       (1000)       53 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/texlive/expected-stderr.txt
--rw-r-----   0 rrt       (1000) rrt       (1000)     7735 2023-05-19 21:27:44.000000 pspdfutils-3.0.3/tests/test-files/pstops/texlive/expected.pdf
--rw-r-----   0 rrt       (1000) rrt       (1000)    26045 2023-05-19 21:28:00.000000 pspdfutils-3.0.3/tests/test-files/pstops/texlive/expected.ps
--rw-r-----   0 rrt       (1000) rrt       (1000)    78599 2023-05-18 21:34:42.000000 pspdfutils-3.0.3/tests/test-files/tiger.eps
--rw-r-----   0 rrt       (1000) rrt       (1000)     1646 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/tests/test_epsffit.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1382 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/tests/test_extractres.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1082 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/tests/test_includeres.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      786 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/tests/test_psbook.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      957 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/tests/test_psjoin.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     3321 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/tests/test_psnup.py
--rw-r-----   0 rrt       (1000) rrt       (1000)      816 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/tests/test_psresize.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1657 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/tests/test_psselect.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     1427 2023-05-29 08:59:50.000000 pspdfutils-3.0.3/tests/test_pstops.py
--rw-r-----   0 rrt       (1000) rrt       (1000)     6952 2023-05-30 14:44:36.000000 pspdfutils-3.0.3/tests/testutils.py
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.270467 pspdfutils-3.0.4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)    35148 2020-01-25 13:35:25.000000 pspdfutils-3.0.4/COPYING
+-rw-r-----   0 rrt       (1000) rrt       (1000)      387 2023-06-01 13:54:12.000000 pspdfutils-3.0.4/MANIFEST.in
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2936 2023-06-04 21:25:49.270467 pspdfutils-3.0.4/PKG-INFO
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2536 2023-06-01 13:42:27.000000 pspdfutils-3.0.4/README.md
+-rw-r-----   0 rrt       (1000) rrt       (1000)       73 2023-05-11 20:36:26.000000 pspdfutils-3.0.4/epsffit-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)      686 2023-05-11 20:36:26.000000 pspdfutils-3.0.4/extractres-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)      620 2023-05-11 20:36:26.000000 pspdfutils-3.0.4/includeres-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)      440 2020-01-25 13:35:25.000000 pspdfutils-3.0.4/man-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)      866 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/psbook-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)      852 2023-05-22 13:02:42.000000 pspdfutils-3.0.4/psnup-include.man
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.950457 pspdfutils-3.0.4/pspdfutils.egg-info/
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2936 2023-06-04 21:25:48.000000 pspdfutils-3.0.4/pspdfutils.egg-info/PKG-INFO
+-rw-r-----   0 rrt       (1000) rrt       (1000)    14540 2023-06-04 21:25:48.000000 pspdfutils-3.0.4/pspdfutils.egg-info/SOURCES.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)        1 2023-06-04 21:25:48.000000 pspdfutils-3.0.4/pspdfutils.egg-info/dependency_links.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)      405 2023-06-04 21:25:48.000000 pspdfutils-3.0.4/pspdfutils.egg-info/entry_points.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)       23 2023-06-04 21:25:48.000000 pspdfutils-3.0.4/pspdfutils.egg-info/requires.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)        8 2023-06-04 21:25:48.000000 pspdfutils-3.0.4/pspdfutils.egg-info/top_level.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)      298 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/psresize-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)       68 2023-05-11 20:36:26.000000 pspdfutils-3.0.4/psselect-include.man
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3224 2023-05-18 21:42:21.000000 pspdfutils-3.0.4/pstops-include.man
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.958457 pspdfutils-3.0.4/psutils/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      228 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/psutils/__init__.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     8381 2023-06-04 21:23:33.000000 pspdfutils-3.0.4/psutils/argparse.py
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.962457 pspdfutils-3.0.4/psutils/command/
+-rw-r-----   0 rrt       (1000) rrt       (1000)     5829 2023-05-30 10:25:33.000000 pspdfutils-3.0.4/psutils/command/epsffit.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4229 2023-05-30 10:25:33.000000 pspdfutils-3.0.4/psutils/command/extractres.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1917 2023-05-30 10:25:33.000000 pspdfutils-3.0.4/psutils/command/includeres.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2872 2023-05-30 10:25:33.000000 pspdfutils-3.0.4/psutils/command/psbook.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     9503 2023-05-30 10:25:33.000000 pspdfutils-3.0.4/psutils/command/psjoin.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10324 2023-06-04 21:20:44.000000 pspdfutils-3.0.4/psutils/command/psnup.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2173 2023-05-30 10:25:33.000000 pspdfutils-3.0.4/psutils/command/psresize.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2685 2023-05-30 10:25:33.000000 pspdfutils-3.0.4/psutils/command/psselect.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3160 2023-06-04 21:20:48.000000 pspdfutils-3.0.4/psutils/command/pstops.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1382 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/psutils/io.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/psutils/libpaper.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      980 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/psutils/psresources.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     5044 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/psutils/readers.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19306 2023-06-04 20:30:34.000000 pspdfutils-3.0.4/psutils/transformers.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1930 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/psutils/types.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      913 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/psutils/warnings.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      931 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/psutils.1
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2808 2023-06-04 21:21:10.000000 pspdfutils-3.0.4/pyproject.toml
+-rw-r-----   0 rrt       (1000) rrt       (1000)       38 2023-06-04 21:25:49.270467 pspdfutils-3.0.4/setup.cfg
+-rw-r-----   0 rrt       (1000) rrt       (1000)      539 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/setup.py
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.970458 pspdfutils-3.0.4/tests/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      890 2023-05-30 10:33:45.000000 pspdfutils-3.0.4/tests/conftest.py
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.014459 pspdfutils-3.0.4/tests/test-files/
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13275 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/a3-20.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23046 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/a3-20.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3332 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/a4-1.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    17476 2023-05-20 15:50:04.000000 pspdfutils-3.0.4/tests/test-files/a4-1.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     9028 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/a4-11.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20384 2023-05-20 15:50:04.000000 pspdfutils-3.0.4/tests/test-files/a4-11.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3910 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/a4-2.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    17766 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/a4-2.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13208 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/a4-20.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23021 2023-05-21 09:11:51.000000 pspdfutils-3.0.4/tests/test-files/a4-20.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4539 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/a4-3.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18056 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/a4-3.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     5005 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/a4-4-0.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18320 2023-05-20 15:50:04.000000 pspdfutils-3.0.4/tests/test-files/a4-4-0.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3335 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/a5-1.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    17475 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/a5-1.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13277 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/a5-20.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23020 2023-05-20 15:50:04.000000 pspdfutils-3.0.4/tests/test-files/a5-20.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.890455 pspdfutils-3.0.4/tests/test-files/epsffit/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.018459 pspdfutils-3.0.4/tests/test-files/epsffit/aspect/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.026459 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.030460 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-maximize/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-maximize/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-maximize/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.034459 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-maximize-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-maximize-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-maximize-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.034459 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.038460 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-maximize/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-maximize/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-maximize/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.042460 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-maximize-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-maximize-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-maximize-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.042460 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/aspect-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.046460 pspdfutils-3.0.4/tests/test-files/epsffit/center/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/center/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78699 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/center/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.050460 pspdfutils-3.0.4/tests/test-files/epsffit/center-maximize/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/center-maximize/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78699 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/center-maximize/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.058460 pspdfutils-3.0.4/tests/test-files/epsffit/center-maximize-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/center-maximize-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78710 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/center-maximize-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.062460 pspdfutils-3.0.4/tests/test-files/epsffit/center-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/center-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78710 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/center-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.066460 pspdfutils-3.0.4/tests/test-files/epsffit/h-texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/h-texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4432 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/h-texlive/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.070461 pspdfutils-3.0.4/tests/test-files/epsffit/m-texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/m-texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4441 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/m-texlive/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.070461 pspdfutils-3.0.4/tests/test-files/epsffit/maximize/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/maximize/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/maximize/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.074461 pspdfutils-3.0.4/tests/test-files/epsffit/maximize-rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/maximize-rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/maximize-rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.078461 pspdfutils-3.0.4/tests/test-files/epsffit/no-options/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/no-options/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78698 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/no-options/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.082461 pspdfutils-3.0.4/tests/test-files/epsffit/rotate/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/rotate/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78709 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/rotate/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.086461 pspdfutils-3.0.4/tests/test-files/epsffit/showpage/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/showpage/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78725 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/showpage/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.090461 pspdfutils-3.0.4/tests/test-files/epsffit/v-texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/v-texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4433 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/epsffit/v-texlive/expected.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.894455 pspdfutils-3.0.4/tests/test-files/extractres/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.106462 pspdfutils-3.0.4/tests/test-files/extractres/sample/
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/extractres/sample/ISO-8859-1Encoding-expected.enc
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/extractres/sample/ISO-8859-1Encoding.enc
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02-expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01-expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/extractres/sample/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    11851 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/extractres/sample/expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)      256 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/extractres/sample/includeres-expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    17478 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/extractres/sample/includeres-expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.894455 pspdfutils-3.0.4/tests/test-files/includeres/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.106462 pspdfutils-3.0.4/tests/test-files/includeres/sample/
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2158 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/includeres/sample/ISO-8859-1Encoding.enc
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2365 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/includeres/sample/a2ps-a2ps-hdr2.02.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1253 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/includeres/sample/a2ps-black+white-Prolog2.01.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)      280 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/includeres/sample/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    17476 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/includeres/sample/expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4334 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/plot.eps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.898455 pspdfutils-3.0.4/tests/test-files/psbook/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.110462 pspdfutils-3.0.4/tests/test-files/psbook/20/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/psbook/20/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/psbook/20/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psbook/20/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.110462 pspdfutils-3.0.4/tests/test-files/psbook/20-signature-4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/psbook/20-signature-4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/psbook/20-signature-4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psbook/20-signature-4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.114462 pspdfutils-3.0.4/tests/test-files/psbook/3/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       31 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/psbook/3/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2867 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/psbook/3/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18081 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psbook/3/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.114462 pspdfutils-3.0.4/tests/test-files/psbook/3-signature-4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       31 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/psbook/3-signature-4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2867 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/psbook/3-signature-4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18081 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psbook/3-signature-4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.114462 pspdfutils-3.0.4/tests/test-files/psbook/invalid-signature-size/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       43 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/psbook/invalid-signature-size/expected-stderr.txt
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.114462 pspdfutils-3.0.4/tests/test-files/psbook/texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       66 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/psbook/texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     7167 2023-05-19 21:27:38.000000 pspdfutils-3.0.4/tests/test-files/psbook/texlive/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20410 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psbook/texlive/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.898455 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.118462 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:39.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-05-19 21:27:39.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19350 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.118462 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-even/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:39.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-even/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3169 2023-05-19 21:27:39.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-even/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19502 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-even/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.118462 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-nostrip/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:39.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-nostrip/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-05-19 21:27:39.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-nostrip/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    35545 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-nostrip/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.122462 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-save/
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-19 21:27:39.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-save/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2925 2023-05-19 21:27:39.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-save/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19474 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-save/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.914456 pspdfutils-3.0.4/tests/test-files/psnup/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.126462 pspdfutils-3.0.4/tests/test-files/psnup/20-1/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.130462 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flip/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:08:04.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flip/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13904 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flip/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30718 2023-05-20 21:10:37.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flip/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.138463 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    15184 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31098 2023-05-20 21:15:21.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.138463 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-21 09:11:54.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13244 2023-05-21 09:11:54.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-05-21 09:11:54.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.142463 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13024 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30858 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.146463 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13204 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.150463 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    11029 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.154463 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-21 09:11:54.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13204 2023-05-21 09:11:54.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-05-21 09:11:54.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.154463 pspdfutils-3.0.4/tests/test-files/psnup/20-2/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       87 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-2/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    11994 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-2/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31268 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-2/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.158463 pspdfutils-3.0.4/tests/test-files/psnup/20-2-inpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       87 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-2-inpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    11314 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-2-inpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30887 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-2-inpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.170464 pspdfutils-3.0.4/tests/test-files/psnup/20-3/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    11577 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.174464 pspdfutils-3.0.4/tests/test-files/psnup/20-3-impossible-tolerance/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       46 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3-impossible-tolerance/expected-stderr.txt
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.174464 pspdfutils-3.0.4/tests/test-files/psnup/20-3-inpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3-inpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    11357 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3-inpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31678 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3-inpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.182464 pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedleft/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedleft/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    11577 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedleft/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedleft/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.186464 pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedright/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       82 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedright/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    11592 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedright/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31679 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedright/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.194464 pspdfutils-3.0.4/tests/test-files/psnup/20-4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     9162 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30986 2023-05-20 21:02:22.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.198464 pspdfutils-3.0.4/tests/test-files/psnup/20-4-297mmx210mm/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-297mmx210mm/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    11323 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-297mmx210mm/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31346 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-297mmx210mm/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.206465 pspdfutils-3.0.4/tests/test-files/psnup/20-4-border-20/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-border-20/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     9652 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-border-20/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31146 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-border-20/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.206465 pspdfutils-3.0.4/tests/test-files/psnup/20-4-columnmajor/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-columnmajor/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     9162 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-columnmajor/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30986 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-columnmajor/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.214465 pspdfutils-3.0.4/tests/test-files/psnup/20-4-flip/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-flip/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10423 2023-05-20 21:02:24.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-flip/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31346 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-flip/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.218465 pspdfutils-3.0.4/tests/test-files/psnup/20-4-impossible-border/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       28 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-impossible-border/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-impossible-border/expected.pdf
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.222465 pspdfutils-3.0.4/tests/test-files/psnup/20-4-impossible-margin/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       28 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-impossible-margin/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)        0 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-impossible-margin/expected.pdf
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.222465 pspdfutils-3.0.4/tests/test-files/psnup/20-4-inpaper-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-inpaper-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     9642 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-inpaper-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31125 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-inpaper-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.222465 pspdfutils-3.0.4/tests/test-files/psnup/20-4-margin-10/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       76 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-margin-10/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     9552 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-margin-10/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    31146 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/20-4-margin-10/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.226465 pspdfutils-3.0.4/tests/test-files/psnup/draw/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       25 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/draw/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3397 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/draw/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    21521 2023-05-20 21:02:23.000000 pspdfutils-3.0.4/tests/test-files/psnup/draw/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.226465 pspdfutils-3.0.4/tests/test-files/psnup/texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       53 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     7710 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/texlive/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    26045 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/texlive/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.230465 pspdfutils-3.0.4/tests/test-files/psnup/texlive2/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/texlive2/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     9322 2023-05-20 21:02:25.000000 pspdfutils-3.0.4/tests/test-files/psnup/texlive2/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30184 2023-05-20 21:15:45.000000 pspdfutils-3.0.4/tests/test-files/psnup/texlive2/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.918456 pspdfutils-3.0.4/tests/test-files/psresize/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.230465 pspdfutils-3.0.4/tests/test-files/psresize/20-A3/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:42.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A3/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13424 2023-05-19 21:27:42.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A3/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30860 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A3/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.234465 pspdfutils-3.0.4/tests/test-files/psresize/20-A3in-A4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A3in-A4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    12824 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A3in-A4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30901 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A3in-A4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.234465 pspdfutils-3.0.4/tests/test-files/psresize/20-A4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:42.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-05-19 21:27:42.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23024 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.238466 pspdfutils-3.0.4/tests/test-files/psresize/20-A5/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:42.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A5/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13024 2023-05-19 21:27:42.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A5/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30858 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A5/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.238466 pspdfutils-3.0.4/tests/test-files/psresize/20-A5in-A4/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A5in-A4/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13204 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A5in-A4/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30857 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-A5in-A4/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.242466 pspdfutils-3.0.4/tests/test-files/psresize/20-Letter/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:42.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-Letter/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    13224 2023-05-19 21:27:42.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-Letter/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    30878 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psresize/20-Letter/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.922456 pspdfutils-3.0.4/tests/test-files/psselect/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.242466 pspdfutils-3.0.4/tests/test-files/psselect/even/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/even/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     6613 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/even/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20103 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psselect/even/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.246466 pspdfutils-3.0.4/tests/test-files/psselect/even-reverse/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       62 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/even-reverse/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     6613 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/even-reverse/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20103 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psselect/even-reverse/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.246466 pspdfutils-3.0.4/tests/test-files/psselect/individual-pages-and-dash-p/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       58 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/psselect/individual-pages-and-dash-p/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     6608 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/psselect/individual-pages-and-dash-p/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20111 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psselect/individual-pages-and-dash-p/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.250466 pspdfutils-3.0.4/tests/test-files/psselect/invalid-pagerange/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       69 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/psselect/invalid-pagerange/.bak.0.expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)       37 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/tests/test-files/psselect/invalid-pagerange/expected-stderr.txt
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.250466 pspdfutils-3.0.4/tests/test-files/psselect/negative-range/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       40 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/negative-range/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4423 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/negative-range/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18649 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psselect/negative-range/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.254466 pspdfutils-3.0.4/tests/test-files/psselect/odd/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       61 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/odd/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     6609 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/odd/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20117 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psselect/odd/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.254466 pspdfutils-3.0.4/tests/test-files/psselect/options-and-complex-pagerange/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       47 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/psselect/options-and-complex-pagerange/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     5295 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/psselect/options-and-complex-pagerange/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19243 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psselect/options-and-complex-pagerange/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.258466 pspdfutils-3.0.4/tests/test-files/psselect/positive-negative-range/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       98 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/psselect/positive-negative-range/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10114 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/psselect/positive-negative-range/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    22455 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psselect/positive-negative-range/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.258466 pspdfutils-3.0.4/tests/test-files/psselect/positive-range/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       35 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/positive-range/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     4419 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/positive-range/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    18655 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psselect/positive-range/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.262466 pspdfutils-3.0.4/tests/test-files/psselect/psnup-texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       97 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/psselect/psnup-texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10113 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/psselect/psnup-texlive/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    22453 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psselect/psnup-texlive/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.262466 pspdfutils-3.0.4/tests/test-files/psselect/reverse/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      107 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/reverse/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10990 2023-05-19 21:27:43.000000 pspdfutils-3.0.4/tests/test-files/psselect/reverse/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    23023 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psselect/reverse/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.262466 pspdfutils-3.0.4/tests/test-files/psselect/texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       66 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/psselect/texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     7048 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/psselect/texlive/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20410 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/psselect/texlive/expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)    10113 2023-06-01 09:56:59.000000 pspdfutils-3.0.4/tests/test-files/psselect-texlive-output.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    22453 2023-06-01 09:56:59.000000 pspdfutils-3.0.4/tests/test-files/psselect-texlive-output.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:48.930456 pspdfutils-3.0.4/tests/test-files/pstops/
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.266466 pspdfutils-3.0.4/tests/test-files/pstops/correct-angles/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       21 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/correct-angles/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2050 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/correct-angles/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20081 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/pstops/correct-angles/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.266466 pspdfutils-3.0.4/tests/test-files/pstops/default-paper-size/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       21 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/default-paper-size/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2082 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/default-paper-size/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20120 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/pstops/default-paper-size/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.266466 pspdfutils-3.0.4/tests/test-files/pstops/invalid-pagespecs/
+-rw-r-----   0 rrt       (1000) rrt       (1000)      179 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/invalid-pagespecs/expected-stderr.txt
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.266466 pspdfutils-3.0.4/tests/test-files/pstops/multiple-pages/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       23 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/multiple-pages/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     2305 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/multiple-pages/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    20065 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/pstops/multiple-pages/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.266466 pspdfutils-3.0.4/tests/test-files/pstops/multiple-turns-and-flips/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/multiple-turns-and-flips/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1759 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/multiple-turns-and-flips/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19517 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/pstops/multiple-turns-and-flips/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.270467 pspdfutils-3.0.4/tests/test-files/pstops/negative-offsets/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/negative-offsets/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1669 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/negative-offsets/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19485 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/pstops/negative-offsets/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.270467 pspdfutils-3.0.4/tests/test-files/pstops/offsets/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       19 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/offsets/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1667 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/offsets/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    19483 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/pstops/offsets/expected.ps
+drwxr-x---   0 rrt       (1000) rrt       (1000)        0 2023-06-04 21:25:49.270467 pspdfutils-3.0.4/tests/test-files/pstops/texlive/
+-rw-r-----   0 rrt       (1000) rrt       (1000)       53 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/texlive/expected-stderr.txt
+-rw-r-----   0 rrt       (1000) rrt       (1000)     7735 2023-05-19 21:27:44.000000 pspdfutils-3.0.4/tests/test-files/pstops/texlive/expected.pdf
+-rw-r-----   0 rrt       (1000) rrt       (1000)    26045 2023-05-19 21:28:00.000000 pspdfutils-3.0.4/tests/test-files/pstops/texlive/expected.ps
+-rw-r-----   0 rrt       (1000) rrt       (1000)    78599 2023-05-18 21:34:42.000000 pspdfutils-3.0.4/tests/test-files/tiger.eps
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1646 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/tests/test_epsffit.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1382 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/tests/test_extractres.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1082 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/tests/test_includeres.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      786 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/tests/test_psbook.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      957 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/tests/test_psjoin.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     3321 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/tests/test_psnup.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)      816 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/tests/test_psresize.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1657 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/tests/test_psselect.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     1427 2023-05-29 08:59:50.000000 pspdfutils-3.0.4/tests/test_pstops.py
+-rw-r-----   0 rrt       (1000) rrt       (1000)     6952 2023-06-02 19:09:18.000000 pspdfutils-3.0.4/tests/testutils.py
```

### Comparing `pspdfutils-3.0.3/COPYING` & `pspdfutils-3.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/PKG-INFO` & `pspdfutils-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspdfutils
-Version: 3.0.3
+Version: 3.0.4
 Summary: Manipulate PDF and PostScript documents
 Author-email: Reuben Thomas <rrt@sc3d.org>
 License: GPL v3 or later
 Project-URL: home_page, https://github.com/rrthomas/psutils
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `pspdfutils-3.0.3/README.md` & `pspdfutils-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/extractres-include.man` & `pspdfutils-3.0.4/extractres-include.man`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/includeres-include.man` & `pspdfutils-3.0.4/includeres-include.man`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psbook-include.man` & `pspdfutils-3.0.4/psbook-include.man`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psnup-include.man` & `pspdfutils-3.0.4/psnup-include.man`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/pspdfutils.egg-info/PKG-INFO` & `pspdfutils-3.0.4/pspdfutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pspdfutils
-Version: 3.0.3
+Version: 3.0.4
 Summary: Manipulate PDF and PostScript documents
 Author-email: Reuben Thomas <rrt@sc3d.org>
 License: GPL v3 or later
 Project-URL: home_page, https://github.com/rrthomas/psutils
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `pspdfutils-3.0.3/pspdfutils.egg-info/SOURCES.txt` & `pspdfutils-3.0.4/pspdfutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/pstops-include.man` & `pspdfutils-3.0.4/pstops-include.man`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/argparse.py` & `pspdfutils-3.0.4/psutils/argparse.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     m = re.match(r"(.+?)(|pt|in|cm|mm)$", s)
     if not m:
         raise ValueError(f"bad dimension `{s}'")
 
     return float(m[1]) * units[m[2]]
 
 
-class PaperContext:
+class PaperContext:  # pylint: disable=too-few-public-methods
     def __init__(self, size: Optional[Rectangle] = get_paper_size()) -> None:
         self.default_paper = size
 
     def dimension(
         self,
         s: str,
     ) -> float:
@@ -85,17 +85,14 @@
             if dim == "w":
                 num *= size.width
             elif dim == "h":
                 num *= size.height
 
         return num
 
-    def parsedraw(self, s: str) -> float:
-        return self.dimension(s or "1")
-
 
 def specerror() -> NoReturn:
     die(
         """bad page specification:
 
   PAGESPECS = [MODULO:]SPEC
   SPEC      = [-]PAGENO[@SCALE][L|R|U|H|V][(XOFF,YOFF)][,SPEC|+SPEC]
@@ -248,7 +245,25 @@
     )
 
     # Backwards compatibility
     parser.add_argument("-w", "--width", type=dimension, help=argparse.SUPPRESS)
     parser.add_argument("-h", "--height", type=dimension, help=argparse.SUPPRESS)
     parser.add_argument("-W", "--inwidth", type=dimension, help=argparse.SUPPRESS)
     parser.add_argument("-H", "--inheight", type=dimension, help=argparse.SUPPRESS)
+
+
+def add_draw_argument(
+    parser: argparse.ArgumentParser, paper_context: PaperContext
+) -> None:
+    parser.add_argument(
+        "-d",
+        "--draw",
+        metavar="DIMENSION",
+        nargs="?",
+        type=paper_context.dimension,
+        default=0,
+        const=1,
+        help="""\
+draw a line of given width (relative to original
+page) around each page [argument defaults to 1pt;
+default is no line; width is fixed for PDF]""",
+    )
```

### Comparing `pspdfutils-3.0.3/psutils/command/epsffit.py` & `pspdfutils-3.0.4/psutils/command/epsffit.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/command/extractres.py` & `pspdfutils-3.0.4/psutils/command/extractres.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/command/includeres.py` & `pspdfutils-3.0.4/psutils/command/includeres.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/command/psbook.py` & `pspdfutils-3.0.4/psutils/command/psbook.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/command/psjoin.py` & `pspdfutils-3.0.4/psutils/command/psjoin.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/command/psnup.py` & `pspdfutils-3.0.4/psutils/command/psnup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, List, Optional, Sequence, Tuple, Union
 
 from psutils.argparse import (
     HelpFormatter,
     PaperContext,
     add_basic_arguments,
     add_paper_arguments,
+    add_draw_argument,
     parsespecs,
 )
 from psutils.io import setup_input_and_output
 from psutils.libpaper import get_paper_size
 from psutils.readers import document_reader
 from psutils.transformers import document_transform
 from psutils.types import Rectangle
@@ -93,26 +94,15 @@
         "-b",
         "--border",
         metavar="DIMENSION",
         type=paper_context.dimension,
         default=0,
         help="width of border around each input page",
     )
-    parser.add_argument(
-        "-d",
-        "--draw",
-        metavar="DIMENSION",
-        nargs="?",
-        type=paper_context.parsedraw,
-        default=0,
-        help="""\
-draw a line of given width (relative to original
-page) around each page [argument defaults to 1pt;
-default is no line]""",
-    )
+    add_draw_argument(parser, paper_context)
     parser.add_argument(
         "-l",
         "--rotatedleft",
         action=ToggleAction,
         help="input pages are rotated left 90 degrees",
     )
     parser.add_argument(
```

### Comparing `pspdfutils-3.0.3/psutils/command/psresize.py` & `pspdfutils-3.0.4/psutils/command/psresize.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/command/psselect.py` & `pspdfutils-3.0.4/psutils/command/psselect.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/command/pstops.py` & `pspdfutils-3.0.4/psutils/command/pstops.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import List, Optional, Tuple
 
 from psutils.argparse import (
     HelpFormatter,
     PaperContext,
     add_basic_arguments,
     add_paper_arguments,
+    add_draw_argument,
     parserange,
     parsespecs,
 )
 from psutils.transformers import file_transform
 from psutils.types import Rectangle
 from psutils.warnings import simple_warning
 
@@ -63,26 +64,15 @@
     parser.add_argument(
         "-r",
         "--reverse",
         action="store_true",
         help="reverse the order of the output pages",
     )
     add_paper_arguments(parser)
-    parser.add_argument(
-        "-d",
-        "--draw",
-        metavar="DIMENSION",
-        nargs="?",
-        type=paper_context.parsedraw,
-        default=0,
-        help="""\
-draw a line of given width (relative to original
-page) around each page [argument defaults to 1pt;
-default is no line; width is fixed for PDF]""",
-    )
+    add_draw_argument(parser, paper_context)
     parser.add_argument("-b", "--nobind", help=argparse.SUPPRESS)
     add_basic_arguments(parser)
 
     return parser, paper_context
 
 
 def get_parser_manpages() -> argparse.ArgumentParser:
```

### Comparing `pspdfutils-3.0.3/psutils/io.py` & `pspdfutils-3.0.4/psutils/io.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/libpaper.py` & `pspdfutils-3.0.4/psutils/libpaper.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/psresources.py` & `pspdfutils-3.0.4/psutils/psresources.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/readers.py` & `pspdfutils-3.0.4/psutils/readers.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/transformers.py` & `pspdfutils-3.0.4/psutils/transformers.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/types.py` & `pspdfutils-3.0.4/psutils/types.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils/warnings.py` & `pspdfutils-3.0.4/psutils/warnings.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/psutils.1` & `pspdfutils-3.0.4/psutils.1`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/pyproject.toml` & `pspdfutils-3.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pspdfutils"
-version = "3.0.3"
+version = "3.0.4"
 description = "Manipulate PDF and PostScript documents"
 license = {text = "GPL v3 or later"}
 authors = [
     {name = "Reuben Thomas", email = "rrt@sc3d.org"}
 ]
 readme = "README.md"
 urls = {home_page = "https://github.com/rrthomas/psutils"}
```

### Comparing `pspdfutils-3.0.3/setup.py` & `pspdfutils-3.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/conftest.py` & `pspdfutils-3.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a3-20.pdf` & `pspdfutils-3.0.4/tests/test-files/a3-20.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a3-20.ps` & `pspdfutils-3.0.4/tests/test-files/a3-20.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-1.pdf` & `pspdfutils-3.0.4/tests/test-files/a4-1.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-1.ps` & `pspdfutils-3.0.4/tests/test-files/a4-1.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-11.pdf` & `pspdfutils-3.0.4/tests/test-files/a4-11.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-11.ps` & `pspdfutils-3.0.4/tests/test-files/a4-11.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-2.pdf` & `pspdfutils-3.0.4/tests/test-files/a4-2.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-2.ps` & `pspdfutils-3.0.4/tests/test-files/a4-2.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-20.pdf` & `pspdfutils-3.0.4/tests/test-files/a4-20.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-20.ps` & `pspdfutils-3.0.4/tests/test-files/a4-20.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-3.pdf` & `pspdfutils-3.0.4/tests/test-files/a4-3.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-3.ps` & `pspdfutils-3.0.4/tests/test-files/a4-3.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-4-0.pdf` & `pspdfutils-3.0.4/tests/test-files/a4-4-0.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a4-4-0.ps` & `pspdfutils-3.0.4/tests/test-files/a4-4-0.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a5-1.pdf` & `pspdfutils-3.0.4/tests/test-files/a5-1.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a5-1.ps` & `pspdfutils-3.0.4/tests/test-files/a5-1.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a5-20.pdf` & `pspdfutils-3.0.4/tests/test-files/a5-20.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/a5-20.ps` & `pspdfutils-3.0.4/tests/test-files/a5-20.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/aspect/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/aspect/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-maximize/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-maximize/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-maximize-rotate/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-maximize-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/aspect-center-rotate/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/aspect-center-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/aspect-maximize/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/aspect-maximize/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/aspect-maximize-rotate/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/aspect-maximize-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/aspect-rotate/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/aspect-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/center/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/center/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/center-maximize/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/center-maximize/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/center-maximize-rotate/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/center-maximize-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/center-rotate/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/center-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/h-texlive/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/h-texlive/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/m-texlive/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/m-texlive/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/maximize/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/maximize/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/maximize-rotate/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/maximize-rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/no-options/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/no-options/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/rotate/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/rotate/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/showpage/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/showpage/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/epsffit/v-texlive/expected.eps` & `pspdfutils-3.0.4/tests/test-files/epsffit/v-texlive/expected.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/extractres/sample/ISO-8859-1Encoding-expected.enc` & `pspdfutils-3.0.4/tests/test-files/extractres/sample/ISO-8859-1Encoding-expected.enc`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/extractres/sample/ISO-8859-1Encoding.enc` & `pspdfutils-3.0.4/tests/test-files/extractres/sample/ISO-8859-1Encoding.enc`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02-expected.ps` & `pspdfutils-3.0.4/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02-expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02.ps` & `pspdfutils-3.0.4/tests/test-files/extractres/sample/a2ps-a2ps-hdr2.02.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01-expected.ps` & `pspdfutils-3.0.4/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01-expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01.ps` & `pspdfutils-3.0.4/tests/test-files/extractres/sample/a2ps-black+white-Prolog2.01.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/extractres/sample/expected.ps` & `pspdfutils-3.0.4/tests/test-files/extractres/sample/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/extractres/sample/includeres-expected.ps` & `pspdfutils-3.0.4/tests/test-files/extractres/sample/includeres-expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/includeres/sample/ISO-8859-1Encoding.enc` & `pspdfutils-3.0.4/tests/test-files/includeres/sample/ISO-8859-1Encoding.enc`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/includeres/sample/a2ps-a2ps-hdr2.02.ps` & `pspdfutils-3.0.4/tests/test-files/includeres/sample/a2ps-a2ps-hdr2.02.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/includeres/sample/a2ps-black+white-Prolog2.01.ps` & `pspdfutils-3.0.4/tests/test-files/includeres/sample/a2ps-black+white-Prolog2.01.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/includeres/sample/expected.ps` & `pspdfutils-3.0.4/tests/test-files/includeres/sample/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/plot.eps` & `pspdfutils-3.0.4/tests/test-files/plot.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psbook/20/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psbook/20/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psbook/20/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psbook/20/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psbook/20-signature-4/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psbook/20-signature-4/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psbook/20-signature-4/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psbook/20-signature-4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psbook/3/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psbook/3/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psbook/3/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psbook/3/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psbook/3-signature-4/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psbook/3-signature-4/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psbook/3-signature-4/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psbook/3-signature-4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psbook/texlive/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psbook/texlive/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psbook/texlive/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psbook/texlive/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-even/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-even/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-even/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-even/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-nostrip/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-nostrip/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-nostrip/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-nostrip/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-save/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-save/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psjoin_to_file/1-2-save/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psjoin_to_file/1-2-save/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-flip/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-flip/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-flip/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-flip/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-flipped-dimensions-wrong-inpaper/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A4-outpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-outpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-1-inpaper-A5-set-inpaper/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-2/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-2/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-2/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-2/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-2-inpaper-A5/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-2-inpaper-A5/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-2-inpaper-A5/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-2-inpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-3/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-3/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-3/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-3/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-3-inpaper-A5/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-3-inpaper-A5/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-3-inpaper-A5/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-3-inpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedleft/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedleft/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedleft/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedleft/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedright/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedright/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-3-rotatedright/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-3-rotatedright/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-297mmx210mm/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-297mmx210mm/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-297mmx210mm/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-297mmx210mm/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-border-20/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-border-20/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-border-20/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-border-20/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-columnmajor/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-columnmajor/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-columnmajor/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-columnmajor/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-flip/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-flip/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-flip/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-flip/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-inpaper-A5/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-inpaper-A5/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-inpaper-A5/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-inpaper-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-margin-10/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-margin-10/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/20-4-margin-10/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/20-4-margin-10/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/draw/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/draw/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/draw/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/draw/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/texlive/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/texlive/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/texlive/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/texlive/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/texlive2/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psnup/texlive2/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psnup/texlive2/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psnup/texlive2/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-A3/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psresize/20-A3/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-A3/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psresize/20-A3/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-A3in-A4/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psresize/20-A3in-A4/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-A3in-A4/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psresize/20-A3in-A4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-A4/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psresize/20-A4/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-A4/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psresize/20-A4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-A5/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psresize/20-A5/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-A5/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psresize/20-A5/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-A5in-A4/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psresize/20-A5in-A4/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-A5in-A4/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psresize/20-A5in-A4/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-Letter/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psresize/20-Letter/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psresize/20-Letter/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psresize/20-Letter/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/even/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect/even/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/even/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psselect/even/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/even-reverse/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect/even-reverse/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/even-reverse/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psselect/even-reverse/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/individual-pages-and-dash-p/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect/individual-pages-and-dash-p/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/individual-pages-and-dash-p/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psselect/individual-pages-and-dash-p/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/negative-range/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect/negative-range/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/negative-range/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psselect/negative-range/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/odd/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect/odd/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/odd/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psselect/odd/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/options-and-complex-pagerange/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect/options-and-complex-pagerange/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/options-and-complex-pagerange/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psselect/options-and-complex-pagerange/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/positive-negative-range/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect/positive-negative-range/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/positive-negative-range/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psselect/positive-negative-range/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/positive-range/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect/positive-range/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/positive-range/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psselect/positive-range/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/psnup-texlive/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect/psnup-texlive/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/psnup-texlive/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psselect/psnup-texlive/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/reverse/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect/reverse/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/reverse/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psselect/reverse/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/texlive/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect/texlive/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect/texlive/expected.ps` & `pspdfutils-3.0.4/tests/test-files/psselect/texlive/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect-texlive-output.pdf` & `pspdfutils-3.0.4/tests/test-files/psselect-texlive-output.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/psselect-texlive-output.ps` & `pspdfutils-3.0.4/tests/test-files/psselect-texlive-output.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/correct-angles/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/pstops/correct-angles/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/correct-angles/expected.ps` & `pspdfutils-3.0.4/tests/test-files/pstops/correct-angles/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/default-paper-size/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/pstops/default-paper-size/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/default-paper-size/expected.ps` & `pspdfutils-3.0.4/tests/test-files/pstops/default-paper-size/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/multiple-pages/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/pstops/multiple-pages/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/multiple-pages/expected.ps` & `pspdfutils-3.0.4/tests/test-files/pstops/multiple-pages/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/multiple-turns-and-flips/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/pstops/multiple-turns-and-flips/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/multiple-turns-and-flips/expected.ps` & `pspdfutils-3.0.4/tests/test-files/pstops/multiple-turns-and-flips/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/negative-offsets/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/pstops/negative-offsets/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/negative-offsets/expected.ps` & `pspdfutils-3.0.4/tests/test-files/pstops/negative-offsets/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/offsets/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/pstops/offsets/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/offsets/expected.ps` & `pspdfutils-3.0.4/tests/test-files/pstops/offsets/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/texlive/expected.pdf` & `pspdfutils-3.0.4/tests/test-files/pstops/texlive/expected.pdf`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/pstops/texlive/expected.ps` & `pspdfutils-3.0.4/tests/test-files/pstops/texlive/expected.ps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test-files/tiger.eps` & `pspdfutils-3.0.4/tests/test-files/tiger.eps`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test_epsffit.py` & `pspdfutils-3.0.4/tests/test_epsffit.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test_extractres.py` & `pspdfutils-3.0.4/tests/test_extractres.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test_includeres.py` & `pspdfutils-3.0.4/tests/test_includeres.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test_psbook.py` & `pspdfutils-3.0.4/tests/test_psbook.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test_psjoin.py` & `pspdfutils-3.0.4/tests/test_psjoin.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test_psnup.py` & `pspdfutils-3.0.4/tests/test_psnup.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test_psresize.py` & `pspdfutils-3.0.4/tests/test_psresize.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test_psselect.py` & `pspdfutils-3.0.4/tests/test_psselect.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/test_pstops.py` & `pspdfutils-3.0.4/tests/test_pstops.py`

 * *Files identical despite different names*

### Comparing `pspdfutils-3.0.3/tests/testutils.py` & `pspdfutils-3.0.4/tests/testutils.py`

 * *Files identical despite different names*

