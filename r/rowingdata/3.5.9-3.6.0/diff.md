# Comparing `tmp/rowingdata-3.5.9.tar.gz` & `tmp/rowingdata-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rowingdata-3.5.9.tar", last modified: Wed Jul 20 05:15:35 2022, max compression
+gzip compressed data, was "rowingdata-3.6.0.tar", last modified: Sun Jun  4 14:57:50 2023, max compression
```

## Comparing `rowingdata-3.5.9.tar` & `rowingdata-3.6.0.tar`

### file list

```diff
@@ -1,197 +1,203 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-20 05:15:35.051932 rowingdata-3.5.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2022-07-20 05:13:27.000000 rowingdata-3.5.9/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2022-07-20 05:13:27.000000 rowingdata-3.5.9/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    31748 2022-07-20 05:15:35.051932 rowingdata-3.5.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    31386 2022-07-20 05:13:27.000000 rowingdata-3.5.9/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-20 05:15:34.983966 rowingdata-3.5.9/bin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3481 2022-07-20 05:13:27.000000 rowingdata-3.5.9/bin/crewnerddata.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)  2933658 2022-07-20 05:13:27.000000 rowingdata-3.5.9/bin/crewnerddata.tcx
--rw-rw-r--   0 travis    (2000) travis    (2000)    53177 2022-07-20 05:13:27.000000 rowingdata-3.5.9/bin/testdata.csv
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-20 05:15:34.979968 rowingdata-3.5.9/docs/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-20 05:15:34.979968 rowingdata-3.5.9/docs/_build/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-20 05:15:34.987964 rowingdata-3.5.9/docs/_build/html/
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/.buildinfo
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-20 05:15:34.987964 rowingdata-3.5.9/docs/_build/html/_images/
--rw-rw-r--   0 travis    (2000) travis    (2000)   124024 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_images/2x20min.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    85796 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_images/editrower.JPG
--rw-rw-r--   0 travis    (2000) travis    (2000)   156560 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_images/greghoc.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   118169 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_images/image001.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    42789 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_images/otwlogbook.JPG
--rw-rw-r--   0 travis    (2000) travis    (2000)    59925 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_images/otwscreenshot.JPG
--rw-rw-r--   0 travis    (2000) travis    (2000)    58348 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_images/screenshot.JPG
--rw-rw-r--   0 travis    (2000) travis    (2000)    37995 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_images/screenshotlogbook.JPG
--rw-rw-r--   0 travis    (2000) travis    (2000)   156147 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_images/woensdag.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-20 05:15:34.991962 rowingdata-3.5.9/docs/_build/html/_sources/
--rw-rw-r--   0 travis    (2000) travis    (2000)      463 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_sources/index.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_sources/modules.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3149 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_sources/rowingdata.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-20 05:15:34.995960 rowingdata-3.5.9/docs/_build/html/_static/
--rw-rw-r--   0 travis    (2000) travis    (2000)      673 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/ajax-loader.gif
--rw-rw-r--   0 travis    (2000) travis    (2000)    10507 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/alabaster.css
--rw-rw-r--   0 travis    (2000) travis    (2000)     9740 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/basic.css
--rw-rw-r--   0 travis    (2000) travis    (2000)     3500 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/comment-bright.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3578 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/comment-close.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3445 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/comment.png
--rw-rw-r--   0 travis    (2000) travis    (2000)       42 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/custom.css
--rw-rw-r--   0 travis    (2000) travis    (2000)     8166 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/doctools.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      347 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/down-pressed.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      347 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/down.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      358 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/file.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   282766 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/jquery-1.11.1.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    95786 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/jquery.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      173 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/minus.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      173 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/plus.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     4149 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 travis    (2000) travis    (2000)    18862 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/searchtools.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    35168 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    12140 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/underscore.js
--rw-rw-r--   0 travis    (2000) travis    (2000)      345 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/up-pressed.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      345 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/up.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    25351 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/_static/websupport.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    25780 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/genindex.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    68960 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/index.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     6140 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/modules.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1101 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/objects.inv
--rw-rw-r--   0 travis    (2000) travis    (2000)     7330 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/py-modindex.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    58474 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/rowingdata.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3164 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/search.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    17380 2022-07-20 05:13:27.000000 rowingdata-3.5.9/docs/_build/html/searchindex.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-20 05:15:35.003956 rowingdata-3.5.9/rowingdata/
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       36 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      289 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/boatedit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5927 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/checkdatafiles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      425 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/copystats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      758 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/crewnerdplot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      771 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/crewnerdplottime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    97689 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/csvparsers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      612 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/ergdataplot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      610 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/ergdataplottime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      623 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/ergdatatotcx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      571 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/ergstickplot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      612 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/ergstickplottime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      628 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/ergsticktotcx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1491 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/gpxtools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5327 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/gpxwrite.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      429 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/konkatenaadje.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22121 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/obsolete.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23526 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/otherparsers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      587 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/painsled_desktop_plot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      521 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/painsled_desktop_plottime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      569 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/painsled_desktop_toc2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      508 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/painsledplot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      522 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/painsledplottime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/painsledtoc2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      315 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/roweredit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   213650 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/rowingdata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      615 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/rowproplot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      609 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/rowproplottime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      615 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/speedcoachplot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      613 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/speedcoachplottime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      664 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/speedcoachtoc2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      694 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/tcxplot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      700 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/tcxplot_nogeo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      683 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/tcxplottime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      689 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/tcxplottime_nogeo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      585 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/tcxtoc2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9446 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/tcxtools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7714 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/trainingparser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3631 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1095 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/windcorrected.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10102 2022-07-20 05:13:27.000000 rowingdata-3.5.9/rowingdata/writetcx.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-20 05:15:35.003956 rowingdata-3.5.9/rowingdata.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    31748 2022-07-20 05:15:34.000000 rowingdata-3.5.9/rowingdata.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5398 2022-07-20 05:15:34.000000 rowingdata-3.5.9/rowingdata.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-07-20 05:15:34.000000 rowingdata-3.5.9/rowingdata.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-07-20 05:15:34.000000 rowingdata-3.5.9/rowingdata.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      185 2022-07-20 05:15:34.000000 rowingdata-3.5.9/rowingdata.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2022-07-20 05:15:34.000000 rowingdata-3.5.9/rowingdata.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      202 2022-07-20 05:15:35.055930 rowingdata-3.5.9/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     3846 2022-07-20 05:13:27.000000 rowingdata-3.5.9/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-07-20 05:15:35.051932 rowingdata-3.5.9/testdata/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3481 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/2016-03-25-0758.CSV
--rw-rw-r--   0 travis    (2000) travis    (2000)   416618 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/2016-03-25-0758_data.CSV
--rw-rw-r--   0 travis    (2000) travis    (2000)    56355 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/2x20min_o.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    17496 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/3km_cd_o.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   539777 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/EUBoatCoach.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    97777 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/EmpowerSpeedCoachForce.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    72367 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/NKEmporfromgreg.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   111860 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/NKLiNKv130.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)  2827124 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/NoHR.tcx
--rw-rw-r--   0 travis    (2000) travis    (2000)    70850 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/PainsledForce.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   104085 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/RP_interval.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   124341 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/RP_interval.csv_o.CSV
--rw-rw-r--   0 travis    (2000) travis    (2000)    63080 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/RP_testdata.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    98860 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/SpdCoach2_imp_inconsistent.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   159697 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/SpdCoachAmbiguous.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    62781 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/SpeedCoach GPS Workout.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    17242 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/SpeedCoach2Link_interval.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   185339 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/SpeedCoach2Linkv1.27.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    12146 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/SpeedCoach2v2.12.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     4976 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/Speedcoach2example.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    53949 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/aritmo.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   459974 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/bc1.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   340372 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/bc2.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   365508 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/bc3.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    18887 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/boatcoach.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   520154 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/boatcoach_otw.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    74347 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/correctedpainsled.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     5461 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/coxmate.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)  1479971 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/crewnerd_interval.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      381 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/crewnerddata.CSV
--rw-rw-r--   0 travis    (2000) travis    (2000)  2945286 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/crewnerddata.tcx
--rw-rw-r--   0 travis    (2000) travis    (2000)   420603 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/crewnerddata_o.CSV
--rw-rw-r--   0 travis    (2000) travis    (2000)      453 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/cumvalues.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     7424 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/ergdata_example.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    11261 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/ergdata_example.csv_o.CSV
--rw-rw-r--   0 travis    (2000) travis    (2000)   462959 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/ergstick.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   262276 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/ergstick.csv_o.CSV
--rw-rw-r--   0 travis    (2000) travis    (2000)    40411 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/ergstick2.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   231959 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/ergstick_o.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   378971 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/example.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   416716 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/example_data.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/faketcx.tcx
--rw-rw-r--   0 travis    (2000) travis    (2000)    64254 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/float.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    23400 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/herodata.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   215236 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/humon.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   157127 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/impeller_empower.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   484172 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/invalidchar.tcx
--rw-rw-r--   0 travis    (2000) travis    (2000)   115182 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/kinomap.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   397003 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/mystery.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   792595 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/nk_logbook.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    56681 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/painsled.tcx
--rw-rw-r--   0 travis    (2000) travis    (2000)   369891 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/painsled_desktop_example.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    41434 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/painsled_out_data.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   923421 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    76485 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/quiske_per_stroke_left.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   277062 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/quiske_per_stroke_right.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   511961 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/quiske_per_stroke_seat.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    20254 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/recover.tcx
--rw-rw-r--   0 travis    (2000) travis    (2000)   106145 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/ritmointervals.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    14216 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/rowingdata_eth.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)  2744646 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/rowinginmotionexample.TCX
--rw-rw-r--   0 travis    (2000) travis    (2000)   657715 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/rowinginmotionexample.TCX_o.CSV
--rw-rw-r--   0 travis    (2000) travis    (2000)   184978 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/rowperfect.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     4490 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/rowpro5.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   144225 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/rowpro_carrick.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   253794 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/rp3_curve.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   420248 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/rp3intervals.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   417209 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/rp3intervals2.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    85870 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/rp_out.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    41141 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/smartrow.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    34271 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/smartrow_intervals.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    31104 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/spdcoach2noheader.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    13731 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/speedcoach2test2.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     7840 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/speedcoach3test3.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    28352 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/speedcoachexample.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    23429 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/speedcoachexample.csv_o.CSV
--rw-rw-r--   0 travis    (2000) travis    (2000)   422653 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/summarytest.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    23885 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/testdata.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    11130 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/testdata_part1.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     9315 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/testdata_part2.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     6460 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/testdatasummary.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    19849 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/testlapidx.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)   427961 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/testtcs_210614.tcx
--rw-rw-r--   0 travis    (2000) travis    (2000)   427951 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/testtcx_210614.tcx
--rw-rw-r--   0 travis    (2000) travis    (2000)    74249 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/tim.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)    23885 2022-07-20 05:13:27.000000 rowingdata-3.5.9/testdata/划船.csv
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.843670 rowingdata-3.6.0/
+-rw-r--r--   0 sander    (1000) sander    (1000)     1074 2023-06-04 14:45:11.000000 rowingdata-3.6.0/LICENSE
+-rw-r--r--   0 sander    (1000) sander    (1000)      276 2023-06-04 14:45:11.000000 rowingdata-3.6.0/MANIFEST.in
+-rw-r--r--   0 sander    (1000) sander    (1000)    31748 2023-06-04 14:57:50.843670 rowingdata-3.6.0/PKG-INFO
+-rw-r--r--   0 sander    (1000) sander    (1000)    31386 2023-06-04 14:45:11.000000 rowingdata-3.6.0/README.rst
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.820336 rowingdata-3.6.0/bin/
+-rw-r--r--   0 sander    (1000) sander    (1000)     3481 2023-06-04 14:45:11.000000 rowingdata-3.6.0/bin/crewnerddata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  2933658 2023-06-04 14:45:11.000000 rowingdata-3.6.0/bin/crewnerddata.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    53177 2023-06-04 14:45:11.000000 rowingdata-3.6.0/bin/testdata.csv
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.820336 rowingdata-3.6.0/docs/
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.820336 rowingdata-3.6.0/docs/_build/
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.820336 rowingdata-3.6.0/docs/_build/html/
+-rw-r--r--   0 sander    (1000) sander    (1000)      166 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/.buildinfo
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.823669 rowingdata-3.6.0/docs/_build/html/_images/
+-rw-r--r--   0 sander    (1000) sander    (1000)   124024 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_images/2x20min.png
+-rw-r--r--   0 sander    (1000) sander    (1000)    85796 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_images/editrower.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)   156560 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_images/greghoc.png
+-rw-r--r--   0 sander    (1000) sander    (1000)   118169 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_images/image001.png
+-rw-r--r--   0 sander    (1000) sander    (1000)    42789 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_images/otwlogbook.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)    59925 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_images/otwscreenshot.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)    58348 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_images/screenshot.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)    37995 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_images/screenshotlogbook.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)   156147 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_images/woensdag.png
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.823669 rowingdata-3.6.0/docs/_build/html/_sources/
+-rw-r--r--   0 sander    (1000) sander    (1000)      463 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_sources/index.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)       67 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_sources/modules.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)     3149 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_sources/rowingdata.txt
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.823669 rowingdata-3.6.0/docs/_build/html/_static/
+-rw-r--r--   0 sander    (1000) sander    (1000)      673 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/ajax-loader.gif
+-rw-r--r--   0 sander    (1000) sander    (1000)    10507 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 sander    (1000) sander    (1000)     9740 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/basic.css
+-rw-r--r--   0 sander    (1000) sander    (1000)     3500 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/comment-bright.png
+-rw-r--r--   0 sander    (1000) sander    (1000)     3578 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/comment-close.png
+-rw-r--r--   0 sander    (1000) sander    (1000)     3445 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/comment.png
+-rw-r--r--   0 sander    (1000) sander    (1000)       42 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/custom.css
+-rw-r--r--   0 sander    (1000) sander    (1000)     8166 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 sander    (1000) sander    (1000)      347 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/down-pressed.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      347 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/down.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      358 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 sander    (1000) sander    (1000)   282766 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/jquery-1.11.1.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    95786 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/jquery.js
+-rw-r--r--   0 sander    (1000) sander    (1000)      173 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      173 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 sander    (1000) sander    (1000)     4149 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 sander    (1000) sander    (1000)    18862 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    35168 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    12140 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 sander    (1000) sander    (1000)      345 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/up-pressed.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      345 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/up.png
+-rw-r--r--   0 sander    (1000) sander    (1000)    25351 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/_static/websupport.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    25780 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/genindex.html
+-rw-r--r--   0 sander    (1000) sander    (1000)    68960 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/index.html
+-rw-r--r--   0 sander    (1000) sander    (1000)     6140 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/modules.html
+-rw-r--r--   0 sander    (1000) sander    (1000)     1101 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/objects.inv
+-rw-r--r--   0 sander    (1000) sander    (1000)     7330 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/py-modindex.html
+-rw-r--r--   0 sander    (1000) sander    (1000)    58474 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/rowingdata.html
+-rw-r--r--   0 sander    (1000) sander    (1000)     3164 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/search.html
+-rw-r--r--   0 sander    (1000) sander    (1000)    17380 2023-06-04 14:45:11.000000 rowingdata-3.6.0/docs/_build/html/searchindex.js
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.827003 rowingdata-3.6.0/rowingdata/
+-rw-r--r--   0 sander    (1000) sander    (1000)       27 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/__init__.py
+-rw-r--r--   0 sander    (1000) sander    (1000)       36 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/__main__.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      303 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/boatedit.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     5927 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/checkdatafiles.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      425 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/copystats.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      758 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/crewnerdplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      771 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/crewnerdplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    98695 2023-06-04 14:56:06.000000 rowingdata-3.6.0/rowingdata/csvparsers.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      612 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/ergdataplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      610 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/ergdataplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      623 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/ergdatatotcx.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      585 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/ergstickplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      612 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/ergstickplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      628 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/ergsticktotcx.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     1491 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/gpxtools.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     5327 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/gpxwrite.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      429 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/konkatenaadje.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    22121 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/obsolete.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    23544 2023-06-04 14:56:06.000000 rowingdata-3.6.0/rowingdata/otherparsers.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      587 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/painsled_desktop_plot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      521 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/painsled_desktop_plottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      569 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/painsled_desktop_toc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      508 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/painsledplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      522 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/painsledplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      441 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/painsledtoc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      315 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/roweredit.py
+-rw-r--r--   0 sander    (1000) sander    (1000)   214914 2023-06-04 14:56:06.000000 rowingdata-3.6.0/rowingdata/rowingdata.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      615 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/rowproplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      609 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/rowproplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      615 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/speedcoachplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      613 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/speedcoachplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      691 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/speedcoachtoc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      694 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/tcxplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      700 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/tcxplot_nogeo.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      683 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/tcxplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      689 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/tcxplottime_nogeo.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      585 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/tcxtoc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     9446 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/tcxtools.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     7714 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/trainingparser.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     3676 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/utils.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     1095 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/windcorrected.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    10102 2023-06-04 14:45:11.000000 rowingdata-3.6.0/rowingdata/writetcx.py
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.827003 rowingdata-3.6.0/rowingdata.egg-info/
+-rw-r--r--   0 sander    (1000) sander    (1000)    31748 2023-06-04 14:57:50.000000 rowingdata-3.6.0/rowingdata.egg-info/PKG-INFO
+-rw-r--r--   0 sander    (1000) sander    (1000)     5537 2023-06-04 14:57:50.000000 rowingdata-3.6.0/rowingdata.egg-info/SOURCES.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)        1 2023-06-04 14:57:50.000000 rowingdata-3.6.0/rowingdata.egg-info/dependency_links.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)        1 2023-06-04 14:56:39.000000 rowingdata-3.6.0/rowingdata.egg-info/not-zip-safe
+-rw-r--r--   0 sander    (1000) sander    (1000)      185 2023-06-04 14:57:50.000000 rowingdata-3.6.0/rowingdata.egg-info/requires.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)       11 2023-06-04 14:57:50.000000 rowingdata-3.6.0/rowingdata.egg-info/top_level.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)      202 2023-06-04 14:57:50.843670 rowingdata-3.6.0/setup.cfg
+-rw-r--r--   0 sander    (1000) sander    (1000)     3846 2023-06-04 14:45:11.000000 rowingdata-3.6.0/setup.py
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.843670 rowingdata-3.6.0/testdata/
+-rw-r--r--   0 sander    (1000) sander    (1000)     3481 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/2016-03-25-0758.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   416618 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/2016-03-25-0758_data.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)    56355 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/2x20min_o.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    17496 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/3km_cd_o.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   539777 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/EUBoatCoach.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    97777 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/EmpowerSpeedCoachForce.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    72367 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/NKEmporfromgreg.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   111860 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/NKLiNKv130.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  2827124 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/NoHR.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    70850 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/PainsledForce.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   104085 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/RP_interval.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   124341 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/RP_interval.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)    63080 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/RP_testdata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    98860 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/SpdCoach2_imp_inconsistent.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   159697 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/SpdCoachAmbiguous.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    62781 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/SpeedCoach GPS Workout.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    17242 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/SpeedCoach2Link_interval.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   185339 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/SpeedCoach2Linkv1.27.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    12146 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/SpeedCoach2v2.12.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     4976 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/Speedcoach2example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    53949 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/aritmo.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   459974 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/bc1.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   340372 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/bc2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   365508 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/bc3.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    18887 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/boatcoach.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    95234 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/boatcoach_fixed_distance.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   520154 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/boatcoach_otw.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    74347 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/correctedpainsled.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     5461 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/coxmate.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  1479971 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/crewnerd_interval.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)      381 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/crewnerddata.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)  2945286 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/crewnerddata.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   420603 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/crewnerddata_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)      453 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/cumvalues.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     7424 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/ergdata_example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    11261 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/ergdata_example.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   462959 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/ergstick.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   262276 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/ergstick.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)    40411 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/ergstick2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   231959 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/ergstick_o.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   378971 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   416716 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/example_data.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)       17 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/faketcx.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    64254 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/float.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23400 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/herodata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   215236 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/humon.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   157127 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/impeller_empower.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   484172 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/invalidchar.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   115182 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/kinomap.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   397003 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/mystery.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   792595 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/nk_logbook.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    56681 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/painsled.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   369891 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/painsled_desktop_example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    41434 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/painsled_out_data.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   923421 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    76485 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/quiske_per_stroke_left.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   366614 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/quiske_per_stroke_new.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   277062 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/quiske_per_stroke_right.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   511961 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/quiske_per_stroke_seat.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    20254 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/recover.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   106145 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/ritmointervals.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    14216 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/rowingdata_eth.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  2744646 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/rowinginmotionexample.TCX
+-rw-r--r--   0 sander    (1000) sander    (1000)   657715 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/rowinginmotionexample.TCX_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   184978 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/rowperfect.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     4490 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/rowpro5.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   144225 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/rowpro_carrick.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   253794 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/rp3_curve.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   420248 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/rp3intervals.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   417209 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/rp3intervals2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    85870 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/rp_out.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    41141 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/smartrow.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    34271 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/smartrow_intervals.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    31104 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/spdcoach2noheader.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    13731 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/speedcoach2test2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     7840 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/speedcoach3test3.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    28352 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/speedcoachexample.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23429 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/speedcoachexample.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   422653 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/summarytest.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23885 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/testdata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    11130 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/testdata_part1.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     9315 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/testdata_part2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     6634 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/testdatasummary.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    19849 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/testlapidx.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   427961 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/testtcs_210614.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    51127 2023-06-04 14:51:12.000000 rowingdata-3.6.0/testdata/testtcx.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   427951 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/testtcx_210614.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    74249 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/tim.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23885 2023-06-04 14:45:11.000000 rowingdata-3.6.0/testdata/划船.csv
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2023-06-04 14:57:50.843670 rowingdata-3.6.0/tests/
+-rw-r--r--   0 sander    (1000) sander    (1000)    27065 2023-06-04 14:45:11.000000 rowingdata-3.6.0/tests/test_rowingdata.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     3424 2023-06-04 14:45:11.000000 rowingdata-3.6.0/tests/testparser.py
```

### Comparing `rowingdata-3.5.9/LICENSE` & `rowingdata-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/PKG-INFO` & `rowingdata-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rowingdata
-Version: 3.5.9
+Version: 3.6.0
 Summary: The rowingdata library to create colorful plots from CrewNerd, Painsled and other rowing data tools
 Home-page: 
 Author: Sander Roosendaal
 Author-email: roosendaalsander@gmail.com
 License: MIT
 Keywords: rowing ergometer concept2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rowingdata-3.5.9/README.rst` & `rowingdata-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/bin/crewnerddata.csv` & `rowingdata-3.6.0/bin/crewnerddata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/bin/crewnerddata.tcx` & `rowingdata-3.6.0/bin/crewnerddata.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/bin/testdata.csv` & `rowingdata-3.6.0/bin/testdata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_images/2x20min.png` & `rowingdata-3.6.0/docs/_build/html/_images/2x20min.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_images/editrower.JPG` & `rowingdata-3.6.0/docs/_build/html/_images/editrower.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_images/greghoc.png` & `rowingdata-3.6.0/docs/_build/html/_images/greghoc.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_images/image001.png` & `rowingdata-3.6.0/docs/_build/html/_images/image001.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_images/otwlogbook.JPG` & `rowingdata-3.6.0/docs/_build/html/_images/otwlogbook.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_images/otwscreenshot.JPG` & `rowingdata-3.6.0/docs/_build/html/_images/otwscreenshot.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_images/screenshot.JPG` & `rowingdata-3.6.0/docs/_build/html/_images/screenshot.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_images/screenshotlogbook.JPG` & `rowingdata-3.6.0/docs/_build/html/_images/screenshotlogbook.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_images/woensdag.png` & `rowingdata-3.6.0/docs/_build/html/_images/woensdag.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_sources/rowingdata.txt` & `rowingdata-3.6.0/docs/_build/html/_sources/rowingdata.txt`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/ajax-loader.gif` & `rowingdata-3.6.0/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/alabaster.css` & `rowingdata-3.6.0/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/basic.css` & `rowingdata-3.6.0/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/comment-bright.png` & `rowingdata-3.6.0/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/comment-close.png` & `rowingdata-3.6.0/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/comment.png` & `rowingdata-3.6.0/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/doctools.js` & `rowingdata-3.6.0/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/jquery-1.11.1.js` & `rowingdata-3.6.0/docs/_build/html/_static/jquery-1.11.1.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/jquery.js` & `rowingdata-3.6.0/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/pygments.css` & `rowingdata-3.6.0/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/searchtools.js` & `rowingdata-3.6.0/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/underscore-1.3.1.js` & `rowingdata-3.6.0/docs/_build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/underscore.js` & `rowingdata-3.6.0/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/_static/websupport.js` & `rowingdata-3.6.0/docs/_build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/genindex.html` & `rowingdata-3.6.0/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/index.html` & `rowingdata-3.6.0/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/modules.html` & `rowingdata-3.6.0/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/objects.inv` & `rowingdata-3.6.0/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/py-modindex.html` & `rowingdata-3.6.0/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/rowingdata.html` & `rowingdata-3.6.0/docs/_build/html/rowingdata.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/search.html` & `rowingdata-3.6.0/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/docs/_build/html/searchindex.js` & `rowingdata-3.6.0/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/checkdatafiles.py` & `rowingdata-3.6.0/rowingdata/checkdatafiles.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/crewnerdplot.py` & `rowingdata-3.6.0/rowingdata/crewnerdplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/crewnerdplottime.py` & `rowingdata-3.6.0/rowingdata/crewnerdplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/csvparsers.py` & `rowingdata-3.6.0/rowingdata/csvparsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,17 @@
         seventhline = ''
 
     try:
         ninthline = s[8]
     except IndexError: # pragma: no cover
         ninthline = ''
 
+    if 'CatchDelay' in thirdline:
+        return 'quiskesummary'
+
     if 'Potential Split' in firstline:
         return 'hero'
 
     if 'timestamp' in firstline and 'InstaSpeed' in firstline:
         return 'nklinklogbook'
 
 
@@ -246,14 +249,17 @@
 
     if 'Stroke Number' and 'Time (seconds)' in firstline:
         return 'ergdata'
 
     if 'Number' in firstline and 'Cal/Hr' in firstline: # pragma: no cover
         return 'ergdata'
 
+    if 'Cadence (stokes/min)' in firstline:
+        return 'csv'
+
     if ' DriveTime (ms)' in firstline:
         return 'csv'
 
     if 'ElapsedTime (sec)' in firstline: # pragma: no cover
         return 'csv'
 
     if 'HR' in firstline and 'Interval' in firstline and 'Avg HR' not in firstline:
@@ -538,15 +544,15 @@
             for line in fop:
                 if 'firmware' in line.lower() and 'oar' in line.lower():
                     firmware = getfirmware(line)
 
 
 
     try:
-        firmware = np.float(firmware)
+        firmware = float(firmware)
     except ValueError:
         firmware = None
 
     return firmware
 
 def skip_variable_footer(f):
     counter = 0
@@ -1109,19 +1115,24 @@
         self.df[self.columns['TimeStamp (sec)']] = unixtimes
 
         self.to_standard()
 
 class QuiskeParser(CSVParser):
     def __init__(self, *args, **kwargs):
         kwargs['skiprows'] = 1
+        kwargs['sep'] = ';'
         if args:
             csvfile = args[0]
         else: # pragma: no cover
             csvfile = kwargs['csvfile']
 
+        firstline = get_file_line(1, csvfile)
+        if ';' not in firstline:
+            kwargs.pop('sep')
+
         super(QuiskeParser, self).__init__(*args, **kwargs)
 
         self.cols = [
             'timestamp(s)',
             'distance(m)',
             'SPM (strokes per minute)',
             '',
@@ -1556,14 +1567,20 @@
         # dump empty lines at end
         endhorizontal = self.df.loc[self.df.index[-1],
                                     self.columns[' Horizontal (meters)']]
 
         if endhorizontal == 0:
             self.df.drop(self.df.index[-1], inplace=True)
 
+        # check for decreasing dist (fixed distance workout)
+        if self.df[self.columns[' Horizontal (meters)']].is_monotonic_decreasing:
+            dist_decreasing = self.df[self.columns[' Horizontal (meters)']].copy()
+            dist_increasing = dist_decreasing.max()-dist_decreasing
+            self.df[self.columns[' Horizontal (meters)']] = dist_increasing
+
         res = make_cumvalues(self.df[self.columns[' Horizontal (meters)']])
         self.df['cumdist'] = res[0]
         maxdist = self.df['cumdist'].max()
         mask = (self.df['cumdist'] == maxdist)
         while len(self.df.loc[mask]) > 2:
             mask = (self.df['cumdist'] == maxdist)
             self.df.drop(self.df.index[-1], inplace=True)
@@ -1790,14 +1807,20 @@
         # dump empty lines at end
         endhorizontal = self.df.loc[self.df.index[-1],
                                     self.columns[' Horizontal (meters)']]
 
         if endhorizontal == 0:
             self.df.drop(self.df.index[-1], inplace=True)
 
+        # check for decreasing dist (fixed distance workout)
+        if self.df[self.columns[' Horizontal (meters)']].is_monotonic_decreasing:
+            dist_decreasing = self.df[self.columns[' Horizontal (meters)']].copy()
+            dist_increasing = dist_decreasing.max()-dist_decreasing
+            self.df[self.columns[' Horizontal (meters)']] = dist_increasing
+
         res = make_cumvalues(self.df[self.columns[' Horizontal (meters)']])
         self.df['cumdist'] = res[0]
         maxdist = self.df['cumdist'].max()
         mask = (self.df['cumdist'] == maxdist)
         while len(self.df[mask]) > 2:
             mask = (self.df['cumdist'] == maxdist)
             self.df.drop(self.df.index[-1], inplace=True)
@@ -2426,15 +2449,15 @@
 
         firmware = kwargs.get('firmware',None)
         oarlength = kwargs.get('oarlength',None)
         inboard = kwargs.get('inboard',None)
 
         if firmware is not None:
             try: # pragma: no cover
-                firmware = np.float(firmware)
+                firmware = float(firmware)
             except ValueError: # pragma: no cover
                 firmware = None
 
         super(NKLiNKLogbookParser, self).__init__(*args, **kwargs)
 
         self.cols = [
             'timestamp',
```

### Comparing `rowingdata-3.5.9/rowingdata/ergdataplot.py` & `rowingdata-3.6.0/rowingdata/ergdataplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/ergdataplottime.py` & `rowingdata-3.6.0/rowingdata/ergdataplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/ergdatatotcx.py` & `rowingdata-3.6.0/rowingdata/ergdatatotcx.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/ergstickplot.py` & `rowingdata-3.6.0/rowingdata/ergstickplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from . import rowingdata
 from sys import argv
 
 def main():
     readFile=argv[1]
 
     try:
-	rowerFile=argv[2]
+        rowerFile=argv[2]
     except IndexError:
-	rowerFile="defaultrower.txt"
+        rowerFile="defaultrower.txt"
 
     rower=rowingdata.getrower(rowerFile)
 
     csvoutput=readFile+"_o.CSV"
 
     rp=rowingdata.ErgStickParser(readFile)
     rp.write_csv(csvoutput)
 
     res=rowingdata.rowingdata(csvoutput,rowtype="On-water",
-				rower=rower)
+    rower=rower)
 
     res.plotmeters_erg()
 
     print((res.allstats()))
```

### Comparing `rowingdata-3.5.9/rowingdata/ergstickplottime.py` & `rowingdata-3.6.0/rowingdata/ergstickplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/ergsticktotcx.py` & `rowingdata-3.6.0/rowingdata/ergsticktotcx.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/gpxtools.py` & `rowingdata-3.6.0/rowingdata/gpxtools.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/gpxwrite.py` & `rowingdata-3.6.0/rowingdata/gpxwrite.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/obsolete.py` & `rowingdata-3.6.0/rowingdata/obsolete.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/otherparsers.py` & `rowingdata-3.6.0/rowingdata/otherparsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,25 +196,25 @@
 
         totaldistance = 0
         totaltime = 0
 
         dfgrouped = self.df.groupby('lapid')
         for lapcount,group in dfgrouped:
             intdist = int(
-                self.lapdf[self.lapdf['lapid']==lapcount+1]['total_distance']
+                (self.lapdf[self.lapdf['lapid']==lapcount+1]['total_distance']).iloc[0]
             )
             if np.isnan(intdist): # pragma: no cover
                 intdist = 1
             else:
                 intdist = int(intdist)
             timestamps = group['timestamp'].apply(totimestamp)
             inttime = self.lapdf[self.lapdf['lapid']==lapcount+1][
                 'total_elapsed_time'
             ]
-            inttime = float(inttime)
+            inttime = float(inttime.iloc[0])
             try:
                 intpower = int(group['power'].mean())
             except KeyError:
                 intpower = 0
             lapmin = int(inttime/60)
             lapsec = int(int(10*(inttime-lapmin*60.))/10.)
             try:
```

### Comparing `rowingdata-3.5.9/rowingdata/painsled_desktop_plot.py` & `rowingdata-3.6.0/rowingdata/painsled_desktop_plot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/painsled_desktop_plottime.py` & `rowingdata-3.6.0/rowingdata/painsled_desktop_plottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/painsled_desktop_toc2.py` & `rowingdata-3.6.0/rowingdata/painsled_desktop_toc2.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/painsledplottime.py` & `rowingdata-3.6.0/rowingdata/painsledplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/rowingdata.py` & `rowingdata-3.6.0/rowingdata/rowingdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=C0103, C0303, C0325, C0413, W0403, W0611
 
 from __future__ import absolute_import
 from __future__ import print_function
 from six.moves import range
 from six.moves import input
 
-__version__ = "3.5.9"
+__version__ = "3.6.0"
 
 from collections import Counter
 
 from matplotlib import figure
 import matplotlib
 try:
     matplotlib.use('TkCairo')
@@ -2469,20 +2469,22 @@
             latz += dlat
             lonz += dlon
             tnew.append(tz)
             latnew.append(latz)
             lonnew.append(lonz)
             unixtnew.append(unixtz)
 
-        df = df.append(pd.DataFrame({
-            'TimeStamp (sec)':unixtnew,
-            ' ElapsedTime (sec)':tnew,
-            ' latitude': latnew,
-            ' longitude': lonnew,
-        }))
+            df2 = pd.DataFrame({
+                'TimeStamp (sec)':unixtnew,
+                ' ElapsedTime (sec)':tnew,
+                ' latitude': latnew,
+                ' longitude': lonnew,
+            })
+        
+            df = pd.concat([df,df2],ignore_index=True)
 
         df.interpolate(inplace=True)
         df = df.fillna(method='ffill',axis=1)
         df['index'] = range(len(df))
         df.set_index('index',inplace=True)
 
         self.df = df
@@ -2597,19 +2599,65 @@
     def set_instroke_metrics(self): # pragma: no cover
         cols = self.get_instroke_columns()
         for c in cols:
             self.add_instroke_metrics(str(c))
             self.add_instroke_diff(str(c))
             self.add_instroke_maxminpos(str(c))
 
-    def get_instroke_data(self,column_name,spm_min=0,spm_max=100):
-        df = self.df[self.df[' Cadence (stokes/min)']>=spm_min]
+    def add_instroke_speed(self,accel='boat accelerator curve',factor=9.80665):
+        accel = self.df[accel].str[1:-1].str.split(',',expand=True)
+        accel = accel.apply(pd.to_numeric, errors='coerce')
+        spms = self.df[' Cadence (stokes/min)']
+        velo = []
+        for index, row in accel.iterrows():
+
+            a = factor*row.values
+            v = np.cumsum(a)
+            stroke_rate = spms[index]
+            stroke_time = 60./stroke_rate
+            dt = stroke_time/len(a)
+
+            v = dt*v
+            v = v - v.mean()
+            vstr = ''
+            for vv in v:
+                vstr += '{a},'.format(a=vv)
+
+            velo.append(vstr)
+
+        
+
+        self.df['instroke boat speed'] = velo
+
+
+        return 1
+
+
+    def get_instroke_data(self,column_name,spm_min=0,spm_max=100,
+                          activeminutesmin=0,activeminutesmax=0,factor=1):
+
+        df = self.df.copy()
+        df['TimeStamp (sec)'] -= df.loc[:,'TimeStamp (sec)'].iloc[0]
+        if activeminutesmin > 0:
+            df = df[df['TimeStamp (sec)']>=activeminutesmin*60.]
+        if activeminutesmax > 0:
+            df = df[df['TimeStamp (sec)']<=activeminutesmax*60.]
+
+        df = df[df[' Cadence (stokes/min)']>=spm_min]
         df = df[df[' Cadence (stokes/min)']<=spm_max]
+
+        if df.empty:
+            return df
+
+
+
+
         df = df[column_name].str[1:-1].str.split(',',expand=True)
         df = df.apply(pd.to_numeric, errors = 'coerce')
+        df = factor*df
 
         return df
 
     def plot_instroke(self,column_name,spm_min=0,spm_max=100): # pragma: no cover
         df  = self.get_instroke_data(column_name,spm_min=spm_min,spm_max=spm_max)
         df_pos = (df+abs(df))/2.
         df_min = -(-df+abs(-df))/2.
@@ -3392,15 +3440,15 @@
         if mode == 'split':
             self.df[' WorkoutState'] = 5
 
         return vals, units, typ
 
     def updateinterval_range(self, metricname,
                              valuelow,valuehigh, unit='seconds',
-                             mode='split',
+                             #mode='split',
                              debug=False,
                              smoothwindow = 60.,
                              activewindow = []): # pragma: no cover
 
         if self.empty:
             return None, None, None
 
@@ -3543,16 +3591,16 @@
             vals.append(startelapsed-previouselapsed)
 
             if df.loc[startindex,' WorkoutState'] == 3: # replaced ix with loc
                 tt = 'rest'
             else:
                 tt = 'work'
 
-            if mode == 'split':
-                tt = 'work'
+            #if mode == 'split':
+            #    tt = 'work'
 
             typ.append(tt)
 
             if debug: # pragma: no cover
                 print(startindex,startelapsed-previouselapsed,unit,tt)
 
             previouselapsed = startelapsed
@@ -3568,16 +3616,16 @@
         vals.append(startelapsed-previouselapsed)
 
         if df.loc[startindex,' WorkoutState'] == 3: # replaced ix with loc
             tt = 'rest'
         else:
             tt = 'work'
 
-        if mode == 'split':
-            tt = 'work'
+        #if mode == 'split':
+        #    tt = 'work'
 
         typ.append(tt)
 
         if debug: # pragma: no cover
             print(startindex,startelapsed-previouselapsed,unit,tt)
 
         if debug: # pragma: no cover
@@ -3588,16 +3636,16 @@
 
 
         if debug: # pragma: no cover
             print(vals)
             print(units)
             print(typ)
 
-        if mode == 'split':
-            self.df[' WorkoutState'] = 5
+        #if mode == 'split':
+        #    self.df[' WorkoutState'] = 5
 
         return vals, units, typ
 
 
     def updateinterval_string(self, s, debug=False):
         res = trainingparser.parse(s)
         res = trainingparser.cleanzeros(res)
```

### Comparing `rowingdata-3.5.9/rowingdata/rowproplot.py` & `rowingdata-3.6.0/rowingdata/rowproplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/rowproplottime.py` & `rowingdata-3.6.0/rowingdata/rowproplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/speedcoachplot.py` & `rowingdata-3.6.0/rowingdata/speedcoachplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/speedcoachplottime.py` & `rowingdata-3.6.0/rowingdata/speedcoachplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/speedcoachtoc2.py` & `rowingdata-3.6.0/rowingdata/speedcoachtoc2.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import time
 from sys import argv
 
 def main():
     readFile=argv[1]
 
     try:
-	rowerFile=argv[2]
+        rowerFile=argv[2]
     except IndexError:
-	rowerFile="defaultrower.txt"
+        rowerFile="defaultrower.txt"
 
     try:
-	datestring=argv[3]
+        datestring=argv[3]
     except IndexError:
-	datestring=time.strftime("%c")
+        datestring=time.strftime("%c")
 
     rower=rowingdata.getrower(rowerFile)
-	
+
 
     res=rowingdata.speedcoachParser(readFile,row_date=datestring)
 
     file2=readFile+"_o.csv"
 
     res.write_csv(file2)
```

### Comparing `rowingdata-3.5.9/rowingdata/tcxplot.py` & `rowingdata-3.6.0/rowingdata/tcxplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/tcxplot_nogeo.py` & `rowingdata-3.6.0/rowingdata/tcxplot_nogeo.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/tcxplottime.py` & `rowingdata-3.6.0/rowingdata/tcxplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/tcxplottime_nogeo.py` & `rowingdata-3.6.0/rowingdata/tcxplottime_nogeo.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/tcxtoc2.py` & `rowingdata-3.6.0/rowingdata/tcxtoc2.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/tcxtools.py` & `rowingdata-3.6.0/rowingdata/tcxtools.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/trainingparser.py` & `rowingdata-3.6.0/rowingdata/trainingparser.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/utils.py` & `rowingdata-3.6.0/rowingdata/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,11 +123,13 @@
 def wavg(group, avg_name, weight_name):
     """ http://stackoverflow.com/questions/10951341/pandas-dataframe-aggregate-function-using-multiple-columns
     In rare instance, we may not have weights, so just return the mean. Customize this if your business case
     should return otherwise.
     """
     d = group[avg_name]
     w = group[weight_name]
+    if w.sum() == 0:
+        return d.mean()
     try:
         return (d * w).sum() / w.sum()
     except ZeroDivisionError:
         return d.mean()
```

### Comparing `rowingdata-3.5.9/rowingdata/windcorrected.py` & `rowingdata-3.6.0/rowingdata/windcorrected.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata/writetcx.py` & `rowingdata-3.6.0/rowingdata/writetcx.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/rowingdata.egg-info/PKG-INFO` & `rowingdata-3.6.0/rowingdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rowingdata
-Version: 3.5.9
+Version: 3.6.0
 Summary: The rowingdata library to create colorful plots from CrewNerd, Painsled and other rowing data tools
 Home-page: 
 Author: Sander Roosendaal
 Author-email: roosendaalsander@gmail.com
 License: MIT
 Keywords: rowing ergometer concept2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rowingdata-3.5.9/rowingdata.egg-info/SOURCES.txt` & `rowingdata-3.6.0/rowingdata.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 testdata/SpeedCoach2v2.12.csv
 testdata/Speedcoach2example.csv
 testdata/aritmo.csv
 testdata/bc1.csv
 testdata/bc2.csv
 testdata/bc3.csv
 testdata/boatcoach.csv
+testdata/boatcoach_fixed_distance.csv
 testdata/boatcoach_otw.csv
 testdata/correctedpainsled.csv
 testdata/coxmate.csv
 testdata/crewnerd_interval.csv
 testdata/crewnerddata.CSV
 testdata/crewnerddata.tcx
 testdata/crewnerddata_o.CSV
@@ -148,14 +149,15 @@
 testdata/mystery.csv
 testdata/nk_logbook.csv
 testdata/painsled.tcx
 testdata/painsled_desktop_example.csv
 testdata/painsled_out_data.csv
 testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv
 testdata/quiske_per_stroke_left.csv
+testdata/quiske_per_stroke_new.csv
 testdata/quiske_per_stroke_right.csv
 testdata/quiske_per_stroke_seat.csv
 testdata/recover.tcx
 testdata/ritmointervals.csv
 testdata/rowingdata_eth.csv
 testdata/rowinginmotionexample.TCX
 testdata/rowinginmotionexample.TCX_o.CSV
@@ -176,10 +178,13 @@
 testdata/summarytest.csv
 testdata/testdata.csv
 testdata/testdata_part1.csv
 testdata/testdata_part2.csv
 testdata/testdatasummary.csv
 testdata/testlapidx.csv
 testdata/testtcs_210614.tcx
+testdata/testtcx.tcx
 testdata/testtcx_210614.tcx
 testdata/tim.csv
-testdata/划船.csv
+testdata/划船.csv
+tests/test_rowingdata.py
+tests/testparser.py
```

### Comparing `rowingdata-3.5.9/setup.py` & `rowingdata-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/2016-03-25-0758.CSV` & `rowingdata-3.6.0/testdata/2016-03-25-0758.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/2016-03-25-0758_data.CSV` & `rowingdata-3.6.0/testdata/2016-03-25-0758_data.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/2x20min_o.csv` & `rowingdata-3.6.0/testdata/2x20min_o.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/3km_cd_o.csv` & `rowingdata-3.6.0/testdata/3km_cd_o.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/EUBoatCoach.csv` & `rowingdata-3.6.0/testdata/EUBoatCoach.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/EmpowerSpeedCoachForce.csv` & `rowingdata-3.6.0/testdata/EmpowerSpeedCoachForce.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/NKEmporfromgreg.csv` & `rowingdata-3.6.0/testdata/NKEmporfromgreg.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/NKLiNKv130.csv` & `rowingdata-3.6.0/testdata/NKLiNKv130.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/NoHR.tcx` & `rowingdata-3.6.0/testdata/NoHR.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/PainsledForce.csv` & `rowingdata-3.6.0/testdata/PainsledForce.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/RP_interval.csv` & `rowingdata-3.6.0/testdata/RP_interval.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/RP_interval.csv_o.CSV` & `rowingdata-3.6.0/testdata/RP_interval.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/RP_testdata.csv` & `rowingdata-3.6.0/testdata/RP_testdata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/SpdCoach2_imp_inconsistent.csv` & `rowingdata-3.6.0/testdata/SpdCoach2_imp_inconsistent.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/SpdCoachAmbiguous.csv` & `rowingdata-3.6.0/testdata/SpdCoachAmbiguous.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/SpeedCoach GPS Workout.csv` & `rowingdata-3.6.0/testdata/SpeedCoach GPS Workout.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/SpeedCoach2Link_interval.csv` & `rowingdata-3.6.0/testdata/SpeedCoach2Link_interval.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/SpeedCoach2Linkv1.27.csv` & `rowingdata-3.6.0/testdata/SpeedCoach2Linkv1.27.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/SpeedCoach2v2.12.csv` & `rowingdata-3.6.0/testdata/SpeedCoach2v2.12.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/Speedcoach2example.csv` & `rowingdata-3.6.0/testdata/Speedcoach2example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/aritmo.csv` & `rowingdata-3.6.0/testdata/aritmo.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/bc1.csv` & `rowingdata-3.6.0/testdata/bc1.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/bc2.csv` & `rowingdata-3.6.0/testdata/bc2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/bc3.csv` & `rowingdata-3.6.0/testdata/bc3.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/boatcoach.csv` & `rowingdata-3.6.0/testdata/boatcoach.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/boatcoach_otw.csv` & `rowingdata-3.6.0/testdata/boatcoach_otw.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/correctedpainsled.csv` & `rowingdata-3.6.0/testdata/correctedpainsled.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/coxmate.csv` & `rowingdata-3.6.0/testdata/coxmate.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/crewnerd_interval.csv` & `rowingdata-3.6.0/testdata/crewnerd_interval.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/crewnerddata.tcx` & `rowingdata-3.6.0/testdata/crewnerddata.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/crewnerddata_o.CSV` & `rowingdata-3.6.0/testdata/crewnerddata_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/ergdata_example.csv` & `rowingdata-3.6.0/testdata/ergdata_example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/ergdata_example.csv_o.CSV` & `rowingdata-3.6.0/testdata/ergdata_example.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/ergstick.csv` & `rowingdata-3.6.0/testdata/ergstick.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/ergstick.csv_o.CSV` & `rowingdata-3.6.0/testdata/ergstick.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/ergstick2.csv` & `rowingdata-3.6.0/testdata/ergstick2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/ergstick_o.csv` & `rowingdata-3.6.0/testdata/ergstick_o.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/example.csv` & `rowingdata-3.6.0/testdata/example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/example_data.csv` & `rowingdata-3.6.0/testdata/example_data.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/float.csv` & `rowingdata-3.6.0/testdata/float.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/herodata.csv` & `rowingdata-3.6.0/testdata/herodata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/humon.csv` & `rowingdata-3.6.0/testdata/humon.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/impeller_empower.csv` & `rowingdata-3.6.0/testdata/impeller_empower.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/invalidchar.tcx` & `rowingdata-3.6.0/testdata/invalidchar.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/kinomap.csv` & `rowingdata-3.6.0/testdata/kinomap.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/mystery.csv` & `rowingdata-3.6.0/testdata/mystery.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/nk_logbook.csv` & `rowingdata-3.6.0/testdata/nk_logbook.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/painsled.tcx` & `rowingdata-3.6.0/testdata/painsled.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/painsled_desktop_example.csv` & `rowingdata-3.6.0/testdata/painsled_desktop_example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/painsled_out_data.csv` & `rowingdata-3.6.0/testdata/painsled_out_data.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv` & `rowingdata-3.6.0/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/quiske_per_stroke_left.csv` & `rowingdata-3.6.0/testdata/quiske_per_stroke_left.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/quiske_per_stroke_right.csv` & `rowingdata-3.6.0/testdata/quiske_per_stroke_right.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/quiske_per_stroke_seat.csv` & `rowingdata-3.6.0/testdata/quiske_per_stroke_seat.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/recover.tcx` & `rowingdata-3.6.0/testdata/recover.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/ritmointervals.csv` & `rowingdata-3.6.0/testdata/ritmointervals.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/rowingdata_eth.csv` & `rowingdata-3.6.0/testdata/rowingdata_eth.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/rowinginmotionexample.TCX` & `rowingdata-3.6.0/testdata/rowinginmotionexample.TCX`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/rowinginmotionexample.TCX_o.CSV` & `rowingdata-3.6.0/testdata/rowinginmotionexample.TCX_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/rowperfect.csv` & `rowingdata-3.6.0/testdata/rowperfect.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/rowpro5.csv` & `rowingdata-3.6.0/testdata/rowpro5.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/rowpro_carrick.csv` & `rowingdata-3.6.0/testdata/rowpro_carrick.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/rp3_curve.csv` & `rowingdata-3.6.0/testdata/rp3_curve.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/rp3intervals.csv` & `rowingdata-3.6.0/testdata/rp3intervals.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/rp3intervals2.csv` & `rowingdata-3.6.0/testdata/rp3intervals2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/rp_out.csv` & `rowingdata-3.6.0/testdata/rp_out.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/smartrow.csv` & `rowingdata-3.6.0/testdata/smartrow.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/smartrow_intervals.csv` & `rowingdata-3.6.0/testdata/smartrow_intervals.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/spdcoach2noheader.csv` & `rowingdata-3.6.0/testdata/spdcoach2noheader.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/speedcoach2test2.csv` & `rowingdata-3.6.0/testdata/speedcoach2test2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/speedcoach3test3.csv` & `rowingdata-3.6.0/testdata/speedcoach3test3.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/speedcoachexample.csv` & `rowingdata-3.6.0/testdata/speedcoachexample.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/speedcoachexample.csv_o.CSV` & `rowingdata-3.6.0/testdata/speedcoachexample.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/summarytest.csv` & `rowingdata-3.6.0/testdata/summarytest.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/testdata.csv` & `rowingdata-3.6.0/testdata/testdata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/testdata_part1.csv` & `rowingdata-3.6.0/testdata/testdata_part1.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/testdata_part2.csv` & `rowingdata-3.6.0/testdata/testdata_part2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/testdatasummary.csv` & `rowingdata-3.6.0/testdata/testdatasummary.csv`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 filename,type,nr_lines,year,month,day,hour,minute,second,dist,seconds,nrintervals,lap 1 time,lap 1 dist,timezone,,,,,,
+quiske_per_stroke_new.csv,quiske,139,2022,11,7,7,58,35,930,382,1,382,930,UTC,,,,,,
+boatcoach_fixed_distance.csv,boatcoach,493,2022,6,13,12,31,37,1996,495,4,109,494,UTC,,,,,,
 smartrow_intervals.csv,smartrow,739,0,0,0,0,0,0,6979,2335,1,2335,6979,UTC,,,,,,
 smartrow.csv,smartrow,878,0,0,0,0,0,0,7836,3005,1,3005,7836,UTC,,,,,,
 rowpro_carrick.csv,rp,1212,2022,1,19,17,33,0,10023,3608,10,422,1495,UTC,,,,,,
 fromnk.csv.gz,nklinklogbook,430,2021,7,7,17,33,28,3005,1062,12,60,250,UTC,,,,,,
 herodata.csv,hero,300,2021,4,26,13,37,33,3512,896,1,896,3512,UTC,,,,,,
 nk_logbook.csv,nklinklogbook,1613,2021,3,30,11,13,4,12155,3901,1,3901,12155,UTC,,,,,,
 SpdCoachAmbiguous.csv,speedcoach2,0,2021,0,0,0,0,0,0,0,0,0,0,UTC,,,,,,
```

### Comparing `rowingdata-3.5.9/testdata/testlapidx.csv` & `rowingdata-3.6.0/testdata/testlapidx.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/testtcs_210614.tcx` & `rowingdata-3.6.0/testdata/testtcs_210614.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/testtcx_210614.tcx` & `rowingdata-3.6.0/testdata/testtcx_210614.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/tim.csv` & `rowingdata-3.6.0/testdata/tim.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.5.9/testdata/划船.csv` & `rowingdata-3.6.0/testdata/划船.csv`

 * *Files identical despite different names*

