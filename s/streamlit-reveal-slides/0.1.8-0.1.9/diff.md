# Comparing `tmp/streamlit-reveal-slides-0.1.8.tar.gz` & `tmp/streamlit-reveal-slides-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-reveal-slides-0.1.8.tar", last modified: Sat Jun  3 19:29:55 2023, max compression
+gzip compressed data, was "streamlit-reveal-slides-0.1.9.tar", last modified: Sat Jun  3 23:48:52 2023, max compression
```

## Comparing `streamlit-reveal-slides-0.1.8.tar` & `streamlit-reveal-slides-0.1.9.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 19:29:55.318663 streamlit-reveal-slides-0.1.8/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1063 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.8/LICENSE
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       49 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.8/MANIFEST.in
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-03 19:29:55.318663 streamlit-reveal-slides-0.1.8/PKG-INFO
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2218 2023-05-23 23:10:19.000000 streamlit-reveal-slides-0.1.8/README.md
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 19:29:55.268663 streamlit-reveal-slides-0.1.8/reveal_slides/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    15013 2023-06-03 05:59:45.000000 streamlit-reveal-slides-0.1.8/reveal_slides/__init__.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 19:29:55.258663 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 19:29:55.268663 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6479 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/asset-manifest.json
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   197459 2023-06-03 19:29:00.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/bootstrap.min.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4356 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/index.html
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 19:29:55.258663 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 19:29:55.278663 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7201 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11924 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7253 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11744 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6477 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20354 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/13.74908590.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11911 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11713 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7184 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11931 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6719 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11404 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      405 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      580 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1666 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1954 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5699 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10009 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    47158 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60673 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6543 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20560 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6560 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20701 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6057 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19287 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5695 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18239 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5701 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18662 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5826 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19077 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5825 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18776 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 19:29:55.308663 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/15.7665d197.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/15.7665d197.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1847219 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2767 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.LICENSE.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  3896922 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/6.e9192981.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/6.e9192981.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/7.be794506.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/7.be794506.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4751 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/main.639deb8d.chunk.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19445 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/main.639deb8d.chunk.js.map
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3774 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17321 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 19:29:55.308663 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    30764 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25696 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64256 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   238084 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75720 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98556 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    88070 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   288008 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   114324 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   284640 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    89897 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   115648 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   240944 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98816 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75706 2023-06-03 19:29:27.000000 streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       38 2023-06-03 19:29:55.318663 streamlit-reveal-slides-0.1.8/setup.cfg
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      764 2023-06-03 19:27:34.000000 streamlit-reveal-slides-0.1.8/setup.py
-drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 19:29:55.318663 streamlit-reveal-slides-0.1.8/streamlit_reveal_slides.egg-info/
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-03 19:29:55.000000 streamlit-reveal-slides-0.1.8/streamlit_reveal_slides.egg-info/PKG-INFO
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6450 2023-06-03 19:29:55.000000 streamlit-reveal-slides-0.1.8/streamlit_reveal_slides.egg-info/SOURCES.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)        1 2023-06-03 19:29:55.000000 streamlit-reveal-slides-0.1.8/streamlit_reveal_slides.egg-info/dependency_links.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-06-03 19:29:55.000000 streamlit-reveal-slides-0.1.8/streamlit_reveal_slides.egg-info/requires.txt
--rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       14 2023-06-03 19:29:55.000000 streamlit-reveal-slides-0.1.8/streamlit_reveal_slides.egg-info/top_level.txt
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 23:48:52.557556 streamlit-reveal-slides-0.1.9/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1063 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.9/LICENSE
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       49 2023-05-23 07:31:54.000000 streamlit-reveal-slides-0.1.9/MANIFEST.in
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-03 23:48:52.547556 streamlit-reveal-slides-0.1.9/PKG-INFO
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2218 2023-05-23 23:10:19.000000 streamlit-reveal-slides-0.1.9/README.md
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 23:48:52.447556 streamlit-reveal-slides-0.1.9/reveal_slides/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    16377 2023-06-03 23:48:04.000000 streamlit-reveal-slides-0.1.9/reveal_slides/__init__.py
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 23:48:52.437556 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 23:48:52.447556 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6479 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/asset-manifest.json
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   197459 2023-06-03 23:47:27.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/bootstrap.min.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4356 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/index.html
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 23:48:52.437556 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 23:48:52.467556 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7201 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11924 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7253 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11744 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6477 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20354 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/13.74908590.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11911 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7194 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11713 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     7184 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11931 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6719 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    11404 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      405 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      580 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1666 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     1954 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5699 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    10009 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    47158 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    60673 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6543 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20560 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6560 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    20701 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6057 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19287 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5695 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18239 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5701 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18662 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5826 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19077 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     5825 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    18776 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 23:48:52.527556 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/10.442a54e9.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/10.442a54e9.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/11.6dd2762e.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/11.6dd2762e.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/12.b5132789.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/12.b5132789.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/13.155b252b.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/13.155b252b.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/14.124342a7.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/14.124342a7.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/15.1df3933b.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/15.1df3933b.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/16.e98baccf.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/16.e98baccf.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/17.f47ed1b3.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/17.f47ed1b3.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/18.bbe30a24.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/18.bbe30a24.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      180 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/19.63982437.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      107 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/19.63982437.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  1847821 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/2.971d039e.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     2767 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/2.971d039e.chunk.js.LICENSE.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)  3897921 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/2.971d039e.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/3.a17c1b63.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/3.a17c1b63.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/4.c8e4936c.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/4.c8e4936c.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/5.ab74786f.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/5.ab74786f.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/6.7f9bbd64.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/6.7f9bbd64.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/7.887bb0a8.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/7.887bb0a8.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/8.0121e917.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/8.0121e917.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      178 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/9.e6c78b5a.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      106 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/9.e6c78b5a.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     4761 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/main.18f5a848.chunk.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    19491 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/main.18f5a848.chunk.js.map
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     3774 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/runtime-main.887ff237.js
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    17321 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/runtime-main.887ff237.js.map
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 23:48:52.547556 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    30764 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    25696 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    64256 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   238084 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75720 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98556 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    88070 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   288008 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   114324 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   284640 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    89897 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   115648 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)   240944 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    98816 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)    75706 2023-06-03 23:48:08.000000 streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       38 2023-06-03 23:48:52.557556 streamlit-reveal-slides-0.1.9/setup.cfg
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      764 2023-06-03 23:48:39.000000 streamlit-reveal-slides-0.1.9/setup.py
+drwxr-xr-x   0 anasbouzid  (1000) anasbouzid  (1000)        0 2023-06-03 23:48:52.547556 streamlit-reveal-slides-0.1.9/streamlit_reveal_slides.egg-info/
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)      393 2023-06-03 23:48:52.000000 streamlit-reveal-slides-0.1.9/streamlit_reveal_slides.egg-info/PKG-INFO
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)     6450 2023-06-03 23:48:52.000000 streamlit-reveal-slides-0.1.9/streamlit_reveal_slides.egg-info/SOURCES.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)        1 2023-06-03 23:48:52.000000 streamlit-reveal-slides-0.1.9/streamlit_reveal_slides.egg-info/dependency_links.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       16 2023-06-03 23:48:52.000000 streamlit-reveal-slides-0.1.9/streamlit_reveal_slides.egg-info/requires.txt
+-rw-r--r--   0 anasbouzid  (1000) anasbouzid  (1000)       14 2023-06-03 23:48:52.000000 streamlit-reveal-slides-0.1.9/streamlit_reveal_slides.egg-info/top_level.txt
```

### Comparing `streamlit-reveal-slides-0.1.8/LICENSE` & `streamlit-reveal-slides-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/README.md` & `streamlit-reveal-slides-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/__init__.py` & `streamlit-reveal-slides-0.1.9/reveal_slides/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -239,701 +239,786 @@
 00000ee0: 7472 6561 6d6c 6974 2072 756e 2073 6c69  treamlit run sli
 00000ef0: 6465 732f 5f5f 696e 6974 5f5f 2e70 7960  des/__init__.py`
 00000f00: 0a69 6620 6e6f 7420 5f52 454c 4541 5345  .if not _RELEASE
 00000f10: 3a0a 2020 2020 696d 706f 7274 2073 7472  :.    import str
 00000f20: 6561 6d6c 6974 2061 7320 7374 0a0a 2020  eamlit as st..  
 00000f30: 2020 7361 6d70 6c65 5f68 746d 6c20 3d20    sample_html = 
 00000f40: 7222 2222 3c73 6563 7469 6f6e 2064 6174  r"""<section dat
-00000f50: 612d 6261 636b 6772 6f75 6e64 2d63 6f6c  a-background-col
-00000f60: 6f72 3d22 2337 3832 3831 4622 203e 3c68  or="#78281F" ><h
-00000f70: 313e 5265 7665 616c 2e6a 7320 2b20 5374  1>Reveal.js + St
-00000f80: 7265 616d 6c69 743c 2f68 313e 3c2f 7365  reamlit</h1></se
-00000f90: 6374 696f 6e3e 0a3c 7365 6374 696f 6e3e  ction>.<section>
-00000fa0: 536c 6964 6520 323c 2f73 6563 7469 6f6e  Slide 2</section
-00000fb0: 3e22 2222 0a20 2020 200a 2020 2020 2320  >""".    .    # 
-00000fc0: 4e6f 7465 2074 6861 7420 6576 656e 2074  Note that even t
-00000fd0: 686f 7567 6820 7765 2070 7574 206d 6172  hough we put mar
-00000fe0: 6b64 6f77 6e20 696e 2061 2072 6177 2073  kdown in a raw s
-00000ff0: 7472 696e 672c 2077 6520 7374 696c 6c20  tring, we still 
-00001000: 6e65 6564 2074 6f20 6573 6361 7065 2074  need to escape t
-00001010: 6865 2062 6163 6b73 6c61 7368 6573 0a20  he backslashes. 
-00001020: 2020 2023 2054 6869 7320 6973 2077 6879     # This is why
-00001030: 2077 6520 7573 6520 3420 6261 636b 736c   we use 4 backsl
-00001040: 6173 6865 7320 746f 2067 6574 2032 2062  ashes to get 2 b
-00001050: 6163 6b73 6c61 7368 6573 2069 6e20 7468  ackslashes in th
-00001060: 6520 6c61 7465 7820 6d61 7468 2063 6f64  e latex math cod
-00001070: 650a 2020 2020 7361 6d70 6c65 5f6d 6172  e.    sample_mar
-00001080: 6b64 6f77 6e20 3d20 7222 2222 0a23 2052  kdown = r""".# R
-00001090: 6576 6561 6c2e 6a73 202b 2053 7472 6561  eveal.js + Strea
-000010a0: 6d6c 6974 0a41 6464 203c 6120 7461 7267  mlit.Add <a targ
-000010b0: 6574 3d22 5f62 6c61 6e6b 2220 6872 6566  et="_blank" href
-000010c0: 3d22 6874 7470 733a 2f2f 7265 7665 616c  ="https://reveal
-000010d0: 6a73 2e63 6f6d 2f22 3e52 6576 6561 6c2e  js.com/">Reveal.
-000010e0: 6a73 3c2f 613e 2070 7265 7365 6e74 6174  js</a> presentat
-000010f0: 696f 6e73 2074 6f20 796f 7572 2053 7472  ions to your Str
-00001100: 6561 6d6c 6974 2061 7070 2e0a 2d2d 2d0a  eamlit app..---.
-00001110: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
-00001120: 6070 6970 2069 6e73 7461 6c6c 2073 7472  `pip install str
-00001130: 6561 6d6c 6974 2d72 6576 6561 6c2d 736c  eamlit-reveal-sl
-00001140: 6964 6573 600a 0a5c 5b5b 4769 7448 7562  ides`..\[[GitHub
-00001150: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001160: 2e63 6f6d 2f62 6f75 7a69 6461 6e61 732f  .com/bouzidanas/
-00001170: 7374 7265 616d 6c69 742e 696f 2f74 7265  streamlit.io/tre
-00001180: 652f 3737 3438 6332 6139 3766 3463 6135  e/7748c2a97f4ca5
-00001190: 3463 6534 6238 3132 3061 3035 3464 3663  4ce4b8120a054d6c
-000011a0: 3636 6538 6265 3239 3664 2f73 7472 6561  66e8be296d/strea
-000011b0: 6d6c 6974 2d72 6576 6561 6c2d 736c 6964  mlit-reveal-slid
-000011c0: 6573 295c 5d20 5c5b 5b50 7950 495d 2868  es)\] \[[PyPI](h
-000011d0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-000011e0: 7072 6f6a 6563 742f 7374 7265 616d 6c69  project/streamli
-000011f0: 742d 7265 7665 616c 2d73 6c69 6465 732f  t-reveal-slides/
-00001200: 295c 5d0a 2d2d 2d0a 2323 2050 7265 7365  )\].---.## Prese
-00001210: 6e74 6174 696f 6e20 4665 6174 7572 6573  ntation Features
-00001220: 0a2d 2043 7265 6174 6520 736c 6964 6573  .- Create slides
-00001230: 2066 726f 6d20 6d61 726b 646f 776e 206f   from markdown o
-00001240: 7220 6d61 726b 7570 203c 212d 2d20 2e65  r markup <!-- .e
-00001250: 6c65 6d65 6e74 3a20 636c 6173 733d 2266  lement: class="f
-00001260: 7261 676d 656e 7422 2064 6174 612d 6672  ragment" data-fr
-00001270: 6167 6d65 6e74 2d69 6e64 6578 3d22 3022  agment-index="0"
-00001280: 202d 2d3e 0a2d 2054 6f75 6368 2c20 6d6f   -->.- Touch, mo
-00001290: 7573 652c 2061 6e64 206b 6579 626f 6172  use, and keyboar
-000012a0: 6420 6e61 7669 6761 7469 6f6e 203c 212d  d navigation <!-
-000012b0: 2d20 2e65 6c65 6d65 6e74 3a20 636c 6173  - .element: clas
-000012c0: 733d 2266 7261 676d 656e 7422 2064 6174  s="fragment" dat
-000012d0: 612d 6672 6167 6d65 6e74 2d69 6e64 6578  a-fragment-index
-000012e0: 3d22 3122 202d 2d3e 0a2d 2046 756c 6c73  ="1" -->.- Fulls
-000012f0: 6372 6565 6e20 616e 6420 6f76 6572 7669  creen and overvi
-00001300: 6577 206d 6f64 6573 203c 212d 2d20 2e65  ew modes <!-- .e
-00001310: 6c65 6d65 6e74 3a20 636c 6173 733d 2266  lement: class="f
-00001320: 7261 676d 656e 7422 2064 6174 612d 6672  ragment" data-fr
-00001330: 6167 6d65 6e74 2d69 6e64 6578 3d22 3222  agment-index="2"
-00001340: 202d 2d3e 0a2d 2053 6561 7263 6820 616e   -->.- Search an
-00001350: 6420 5a6f 6f6d 2028 706c 7567 696e 7329  d Zoom (plugins)
-00001360: 203c 212d 2d20 2e65 6c65 6d65 6e74 3a20   <!-- .element: 
-00001370: 636c 6173 733d 2266 7261 676d 656e 7422  class="fragment"
-00001380: 2064 6174 612d 6672 6167 6d65 6e74 2d69   data-fragment-i
-00001390: 6e64 6578 3d22 3322 202d 2d3e 0a2d 2044  ndex="3" -->.- D
-000013a0: 6973 706c 6179 204c 6154 6558 2061 6e64  isplay LaTeX and
-000013b0: 2073 796e 7461 7820 6869 6768 6c69 6768   syntax highligh
-000013c0: 7465 6420 636f 6465 2028 706c 7567 696e  ted code (plugin
-000013d0: 7329 203c 212d 2d20 2e65 6c65 6d65 6e74  s) <!-- .element
-000013e0: 3a20 636c 6173 733d 2266 7261 676d 656e  : class="fragmen
-000013f0: 7422 2064 6174 612d 6672 6167 6d65 6e74  t" data-fragment
-00001400: 2d69 6e64 6578 3d22 3422 202d 2d3e 0a2d  -index="4" -->.-
-00001410: 2d2d 0a23 2320 536c 6964 6520 436f 6e74  --.## Slide Cont
-00001420: 656e 7420 4372 6561 7469 6f6e 0a41 2070  ent Creation.A p
-00001430: 6172 6167 7261 7068 2077 6974 6820 736f  aragraph with so
-00001440: 6d65 2074 6578 7420 616e 6420 6120 6d61  me text and a ma
-00001450: 726b 646f 776e 205b 6c69 6e6b 5d28 6874  rkdown [link](ht
-00001460: 7470 733a 2f2f 6861 6b69 6d2e 7365 292e  tps://hakim.se).
-00001470: 200a 4d61 726b 646f 776e 206c 696e 6b73   .Markdown links
-00001480: 2067 6574 2064 6973 706c 6179 6564 2077   get displayed w
-00001490: 6974 6869 6e20 7468 6520 7061 7265 6e74  ithin the parent
-000014a0: 2069 6672 616d 652e 0a2d 2d0a 416e 6f74   iframe..--.Anot
-000014b0: 6865 7220 7061 7261 6772 6170 6820 636f  her paragraph co
-000014c0: 6e74 6169 6e69 6e67 2074 6865 2073 616d  ntaining the sam
-000014d0: 6520 3c61 2074 6172 6765 743d 225f 626c  e <a target="_bl
-000014e0: 616e 6b22 2068 7265 663d 2268 7474 7073  ank" href="https
-000014f0: 3a2f 2f68 616b 696d 2e73 6522 3e6c 696e  ://hakim.se">lin
-00001500: 6b3c 2f61 3e2e 0a48 6f77 6576 6572 2c20  k</a>..However, 
-00001510: 7468 6973 206c 696e 6b20 7769 6c6c 206f  this link will o
-00001520: 7065 6e20 696e 2061 206e 6577 2074 6162  pen in a new tab
-00001530: 2069 6e73 7465 6164 2e20 0a54 6869 7320   instead. .This 
-00001540: 6973 2064 6f6e 6520 7573 696e 6720 616e  is done using an
-00001550: 2048 544d 4c20 603c 613e 6020 7461 6720   HTML `<a>` tag 
-00001560: 7769 7468 2060 7461 7267 6574 3d22 5f62  with `target="_b
-00001570: 6c61 6e6b 2260 2e0a 2d2d 2d0a 2323 2042  lank"`..---.## B
-00001580: 6163 6b67 726f 756e 6473 0a52 6576 6561  ackgrounds.Revea
-00001590: 6c20 7375 7070 6f72 7473 2066 6f75 7220  l supports four 
-000015a0: 6469 6666 6572 656e 7420 7479 7065 7320  different types 
-000015b0: 6f66 2062 6163 6b67 726f 756e 6473 3a20  of backgrounds: 
-000015c0: 636f 6c6f 722c 2069 6d61 6765 2c20 7669  color, image, vi
-000015d0: 6465 6f20 616e 6420 6966 7261 6d65 2e0a  deo and iframe..
-000015e0: 2d2d 0a3c 212d 2d20 2e73 6c69 6465 3a20  --.<!-- .slide: 
-000015f0: 6461 7461 2d62 6163 6b67 726f 756e 642d  data-background-
-00001600: 636f 6c6f 723d 2223 3238 3337 3437 2220  color="#283747" 
-00001610: 2d2d 3e0a 4368 616e 6765 2074 6865 2062  -->.Change the b
-00001620: 6163 6b67 726f 756e 6420 746f 2061 2073  ackground to a s
-00001630: 6f6c 6964 2063 6f6c 6f72 2075 7369 6e67  olid color using
-00001640: 2074 6865 2060 6461 7461 2d62 6163 6b67   the `data-backg
-00001650: 726f 756e 642d 636f 6c6f 7260 2061 7474  round-color` att
-00001660: 7269 6275 7465 2e0a 2d2d 0a3c 212d 2d20  ribute..--.<!-- 
-00001670: 2e73 6c69 6465 3a20 6461 7461 2d62 6163  .slide: data-bac
-00001680: 6b67 726f 756e 642d 7669 6465 6f3d 2268  kground-video="h
-00001690: 7474 7073 3a2f 2f62 6f75 7a69 6461 6e61  ttps://bouzidana
-000016a0: 732e 6769 7468 7562 2e69 6f2f 7669 6465  s.github.io/vide
-000016b0: 6f73 2f70 6578 656c 732d 636f 7474 6f6e  os/pexels-cotton
-000016c0: 6272 6f2d 3936 3635 3233 352e 6d70 3422  bro-9665235.mp4"
-000016d0: 2064 6174 612d 6261 636b 6772 6f75 6e64   data-background
-000016e0: 2d76 6964 656f 2d6c 6f6f 7020 6461 7461  -video-loop data
-000016f0: 2d62 6163 6b67 726f 756e 642d 7669 6465  -background-vide
-00001700: 6f2d 6d75 7465 6420 2d2d 3e0a 4164 6420  o-muted -->.Add 
-00001710: 6120 7669 6465 6f20 6173 2074 6865 2062  a video as the b
-00001720: 6163 6b67 726f 756e 6420 7573 696e 6720  ackground using 
-00001730: 7468 6520 6064 6174 612d 6261 636b 6772  the `data-backgr
-00001740: 6f75 6e64 2d76 6964 656f 6020 6174 7472  ound-video` attr
-00001750: 6962 7574 652e 2041 6464 2060 6461 7461  ibute. Add `data
-00001760: 2d62 6163 6b67 726f 756e 642d 7669 6465  -background-vide
-00001770: 6f2d 6c6f 6f70 6020 746f 206c 6f6f 7020  o-loop` to loop 
-00001780: 7468 6520 7669 6465 6f20 696e 2074 6865  the video in the
-00001790: 2062 6163 6b67 726f 756e 6420 616e 6420   background and 
-000017a0: 6164 6420 6064 6174 612d 6261 636b 6772  add `data-backgr
-000017b0: 6f75 6e64 2d76 6964 656f 2d6d 7574 6564  ound-video-muted
-000017c0: 6020 746f 206d 7574 6520 6974 2e0a 2d2d  ` to mute it..--
-000017d0: 2d0a 2323 204d 6174 6820 4578 7072 6573  -.## Math Expres
-000017e0: 7369 6f6e 730a 5468 6973 2066 6f6c 6c6f  sions.This follo
-000017f0: 7769 6e67 2069 7320 616e 2065 7861 6d70  wing is an examp
-00001800: 6c65 206f 6620 616e 2069 6e6c 696e 6520  le of an inline 
-00001810: 6d61 7468 2065 7175 6174 696f 6e3a 2024  math equation: $
-00001820: 655e 7b69 5c70 697d 202b 2031 203d 2030  e^{i\pi} + 1 = 0
-00001830: 242e 0a2d 2d0a 2323 2054 6865 204c 6f72  $..--.## The Lor
-00001840: 656e 7a20 4571 7561 7469 6f6e 730a 0a24  enz Equations..$
-00001850: 240a 5c62 6567 696e 7b61 6c69 676e 6564  $.\begin{aligned
-00001860: 7d0a 5c64 6f74 7b78 7d20 2620 3d20 5c73  }.\dot{x} & = \s
-00001870: 6967 6d61 2879 2d78 2920 5c5c 5c5c 0a5c  igma(y-x) \\\\.\
-00001880: 646f 747b 797d 2026 203d 205c 7268 6f20  dot{y} & = \rho 
-00001890: 7820 2d20 7920 2d20 787a 205c 5c5c 5c0a  x - y - xz \\\\.
-000018a0: 5c64 6f74 7b7a 7d20 2620 3d20 2d5c 6265  \dot{z} & = -\be
-000018b0: 7461 207a 202b 2078 790a 5c65 6e64 7b61  ta z + xy.\end{a
-000018c0: 6c69 676e 6564 7d0a 2424 0a2d 2d2d 0a23  ligned}.$$.---.#
-000018d0: 2320 436f 6465 2062 6c6f 636b 730a 6060  # Code blocks.``
-000018e0: 606a 7320 5b31 2d32 7c33 7c34 5d0a 6c65  `js [1-2|3|4].le
-000018f0: 7420 6120 3d20 313b 0a6c 6574 2062 203d  t a = 1;.let b =
-00001900: 2032 3b0a 6c65 7420 6320 3d20 7820 3d3e   2;.let c = x =>
-00001910: 2031 202b 2032 202b 2078 3b0a 6328 3329   1 + 2 + x;.c(3)
-00001920: 3b0a 6060 600a 2d2d 2d0a 2323 2053 6c69  ;.```.---.## Sli
-00001930: 6465 2046 7261 676d 656e 7473 0a54 6869  de Fragments.Thi
-00001940: 7320 7365 6e74 656e 6365 2069 7320 706c  s sentence is pl
-00001950: 6163 6564 2069 6e20 6120 6672 6167 6d65  aced in a fragme
-00001960: 6e74 2077 6974 6820 6064 6174 612d 6672  nt with `data-fr
-00001970: 6167 6d65 6e74 2d69 6e64 6578 3d22 3022  agment-index="0"
-00001980: 6020 0a3c 212d 2d20 2e65 6c65 6d65 6e74  ` .<!-- .element
-00001990: 3a20 636c 6173 733d 2266 7261 676d 656e  : class="fragmen
-000019a0: 7422 2064 6174 612d 6672 6167 6d65 6e74  t" data-fragment
-000019b0: 2d69 6e64 6578 3d22 3022 202d 2d3e 0a0a  -index="0" -->..
-000019c0: 5468 6973 2069 7320 7468 6520 7468 6972  This is the thir
-000019d0: 6420 6672 6167 6d65 6e74 2069 6e20 7468  d fragment in th
-000019e0: 6520 736c 6964 6520 7468 6174 2077 696c  e slide that wil
-000019f0: 6c20 6170 7065 6172 2062 6563 6175 7365  l appear because
-00001a00: 2060 6461 7461 2d66 7261 676d 656e 742d   `data-fragment-
-00001a10: 696e 6465 7860 2069 7320 7365 7420 746f  index` is set to
-00001a20: 2060 3160 200a 3c21 2d2d 202e 656c 656d   `1` .<!-- .elem
-00001a30: 656e 743a 2063 6c61 7373 3d22 6672 6167  ent: class="frag
-00001a40: 6d65 6e74 2220 6461 7461 2d66 7261 676d  ment" data-fragm
-00001a50: 656e 742d 696e 6465 783d 2231 2220 2d2d  ent-index="1" --
-00001a60: 3e0a 0a54 6869 7320 7365 6e74 656e 6365  >..This sentence
-00001a70: 2061 7070 6561 7273 2062 7920 6465 6661   appears by defa
-00001a80: 756c 7420 7768 656e 2079 6f75 2074 7261  ult when you tra
-00001a90: 6e73 6974 696f 6e20 696e 746f 2061 6e64  nsition into and
-00001aa0: 206f 7574 206f 6620 7468 6973 2073 6c69   out of this sli
-00001ab0: 6465 200a 2d2d 2d0a 2323 2043 6f6e 6669  de .---.## Confi
-00001ac0: 6775 7269 6e67 2074 6865 2050 7265 7365  guring the Prese
-00001ad0: 6e74 6174 696f 6e0a 5468 6520 7072 6573  ntation.The pres
-00001ae0: 656e 7461 7469 6f6e 2063 616e 2062 6520  entation can be 
-00001af0: 636f 6e66 6967 7572 6564 2075 7369 6e67  configured using
-00001b00: 2074 6865 2060 636f 6e66 6967 6020 7061   the `config` pa
-00001b10: 7261 6d65 7465 722e 2049 7473 2061 7320  rameter. Its as 
-00001b20: 7369 6d70 6c65 2061 7320 7061 7373 696e  simple as passin
-00001b30: 6720 6120 6469 6374 696f 6e61 7279 2077  g a dictionary w
-00001b40: 6974 6820 7468 6520 7265 7665 616c 2063  ith the reveal c
-00001b50: 6f6e 6669 6775 7261 7469 6f6e 206f 7074  onfiguration opt
-00001b60: 696f 6e73 2e0a 2d2d 2d0a 2323 204c 6120  ions..---.## La 
-00001b70: 6669 6e0a 2222 220a 2020 2020 7374 2e6d  fin.""".    st.m
-00001b80: 6172 6b64 6f77 6e28 2223 2320 5354 5245  arkdown("## STRE
-00001b90: 414d 4c49 5420 5245 5645 414c 2e4a 5320  AMLIT REVEAL.JS 
-00001ba0: 434f 4d50 4f4e 454e 5422 290a 2020 2020  COMPONENT").    
-00001bb0: 7769 7468 2073 742e 7369 6465 6261 723a  with st.sidebar:
-00001bc0: 0a20 2020 2020 2020 2073 742e 6865 6164  .        st.head
-00001bd0: 6572 2822 436f 6d70 6f6e 656e 7420 5061  er("Component Pa
-00001be0: 7261 6d65 7465 7273 2229 0a20 2020 2020  rameters").     
-00001bf0: 2020 2074 6865 6d65 203d 2073 742e 7365     theme = st.se
-00001c00: 6c65 6374 626f 7828 2254 6865 6d65 222c  lectbox("Theme",
-00001c10: 205b 2262 6c61 636b 222c 2022 626c 6163   ["black", "blac
-00001c20: 6b2d 636f 6e74 7261 7374 222c 2022 626c  k-contrast", "bl
-00001c30: 6f6f 6422 2c20 2264 7261 6375 6c61 222c  ood", "dracula",
-00001c40: 2022 6d6f 6f6e 222c 2022 7768 6974 6522   "moon", "white"
-00001c50: 2c20 2277 6869 7465 2d63 6f6e 7472 6173  , "white-contras
-00001c60: 7422 2c20 226c 6561 6775 6522 2c20 2262  t", "league", "b
-00001c70: 6569 6765 222c 2022 736b 7922 2c20 226e  eige", "sky", "n
-00001c80: 6967 6874 222c 2022 7365 7269 6622 2c20  ight", "serif", 
-00001c90: 2273 696d 706c 6522 2c20 2273 6f6c 6172  "simple", "solar
-00001ca0: 697a 6564 225d 290a 2020 2020 2020 2020  ized"]).        
-00001cb0: 6865 6967 6874 203d 2073 742e 6e75 6d62  height = st.numb
-00001cc0: 6572 5f69 6e70 7574 2822 4865 6967 6874  er_input("Height
-00001cd0: 222c 2076 616c 7565 3d35 3030 290a 2020  ", value=500).  
-00001ce0: 2020 2020 2020 7374 2e73 7562 6865 6164        st.subhead
-00001cf0: 6572 2822 536c 6964 6520 436f 6e66 6967  er("Slide Config
-00001d00: 7572 6174 696f 6e22 290a 2020 2020 2020  uration").      
-00001d10: 2020 636f 6e74 656e 745f 6865 6967 6874    content_height
-00001d20: 203d 2073 742e 6e75 6d62 6572 5f69 6e70   = st.number_inp
-00001d30: 7574 2822 436f 6e74 656e 7420 4865 6967  ut("Content Heig
-00001d40: 6874 222c 2076 616c 7565 3d39 3030 290a  ht", value=900).
-00001d50: 2020 2020 2020 2020 636f 6e74 656e 745f          content_
-00001d60: 7769 6474 6820 3d20 7374 2e6e 756d 6265  width = st.numbe
-00001d70: 725f 696e 7075 7428 2243 6f6e 7465 6e74  r_input("Content
-00001d80: 2057 6964 7468 222c 2076 616c 7565 3d39   Width", value=9
-00001d90: 3030 290a 2020 2020 2020 2020 7363 616c  00).        scal
-00001da0: 655f 7261 6e67 6520 3d20 7374 2e73 6c69  e_range = st.sli
-00001db0: 6465 7228 2253 6361 6c65 2052 616e 6765  der("Scale Range
-00001dc0: 222c 206d 696e 5f76 616c 7565 3d30 2e30  ", min_value=0.0
-00001dd0: 2c20 6d61 785f 7661 6c75 653d 352e 302c  , max_value=5.0,
-00001de0: 2076 616c 7565 3d5b 302e 312c 2030 2e35   value=[0.1, 0.5
-00001df0: 5d2c 2073 7465 703d 302e 3129 0a20 2020  ], step=0.1).   
-00001e00: 2020 2020 206d 6172 6769 6e20 3d20 7374       margin = st
-00001e10: 2e73 6c69 6465 7228 224d 6172 6769 6e22  .slider("Margin"
-00001e20: 2c20 6d69 6e5f 7661 6c75 653d 302e 302c  , min_value=0.0,
-00001e30: 206d 6178 5f76 616c 7565 3d30 2e38 2c20   max_value=0.8, 
-00001e40: 7661 6c75 653d 302e 312c 2073 7465 703d  value=0.1, step=
-00001e50: 302e 3035 290a 2020 2020 2020 2020 706c  0.05).        pl
-00001e60: 7567 696e 7320 3d20 7374 2e6d 756c 7469  ugins = st.multi
-00001e70: 7365 6c65 6374 2822 506c 7567 696e 7322  select("Plugins"
-00001e80: 2c20 5b22 6869 6768 6c69 6768 7422 2c20  , ["highlight", 
-00001e90: 226b 6174 6578 222c 2022 6d61 7468 6a61  "katex", "mathja
-00001ea0: 7832 222c 2022 6d61 7468 6a61 7833 222c  x2", "mathjax3",
-00001eb0: 2022 6e6f 7465 7322 2c20 2273 6561 7263   "notes", "searc
-00001ec0: 6822 2c20 227a 6f6f 6d22 5d2c 205b 5d29  h", "zoom"], [])
-00001ed0: 0a20 2020 2020 2020 2073 742e 7375 6268  .        st.subh
-00001ee0: 6561 6465 7228 2249 6e69 7469 616c 2053  eader("Initial S
-00001ef0: 7461 7465 2229 0a20 2020 2020 2020 2068  tate").        h
-00001f00: 736c 6964 6550 6f73 203d 2073 742e 6e75  slidePos = st.nu
-00001f10: 6d62 6572 5f69 6e70 7574 2822 486f 7269  mber_input("Hori
-00001f20: 7a6f 6e74 616c 2053 6c69 6465 2050 6f73  zontal Slide Pos
-00001f30: 6974 696f 6e22 2c20 7661 6c75 653d 3029  ition", value=0)
-00001f40: 0a20 2020 2020 2020 2076 736c 6964 6550  .        vslideP
-00001f50: 6f73 203d 2073 742e 6e75 6d62 6572 5f69  os = st.number_i
-00001f60: 6e70 7574 2822 5665 7274 6963 616c 2053  nput("Vertical S
-00001f70: 6c69 6465 2050 6f73 6974 696f 6e22 2c20  lide Position", 
-00001f80: 7661 6c75 653d 3029 0a20 2020 2020 2020  value=0).       
-00001f90: 2066 7261 6750 6f73 203d 2073 742e 6e75   fragPos = st.nu
-00001fa0: 6d62 6572 5f69 6e70 7574 2822 4672 6167  mber_input("Frag
-00001fb0: 6d65 6e74 2050 6f73 6974 696f 6e22 2c20  ment Position", 
-00001fc0: 7661 6c75 653d 2d31 290a 2020 2020 2020  value=-1).      
-00001fd0: 2020 6f76 6572 7669 6577 203d 2073 742e    overview = st.
-00001fe0: 6368 6563 6b62 6f78 2822 5368 6f77 204f  checkbox("Show O
-00001ff0: 7665 7276 6965 7722 2c20 7661 6c75 653d  verview", value=
-00002000: 4661 6c73 6529 0a20 2020 2020 2020 2070  False).        p
-00002010: 6175 7365 6420 3d20 7374 2e63 6865 636b  aused = st.check
-00002020: 626f 7828 2250 6175 7365 222c 2076 616c  box("Pause", val
-00002030: 7565 3d46 616c 7365 290a 0a20 2020 2023  ue=False)..    #
-00002040: 2041 6464 2074 6865 2073 7472 6561 6d6c   Add the streaml
-00002050: 6974 2d72 6576 6561 6c2d 736c 6964 6520  it-reveal-slide 
-00002060: 636f 6d70 6f6e 656e 7420 746f 2074 6865  component to the
-00002070: 2053 7472 6561 6d6c 6974 2061 7070 2e20   Streamlit app. 
-00002080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002090: 2020 200a 2020 2020 6375 7272 5374 6174     .    currStat
-000020a0: 6520 3d20 736c 6964 6573 2873 616d 706c  e = slides(sampl
-000020b0: 655f 6d61 726b 646f 776e 2c20 0a20 2020  e_markdown, .   
-000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020d0: 2020 2020 6865 6967 6874 3d68 6569 6768      height=heigh
-000020e0: 742c 200a 2020 2020 2020 2020 2020 2020  t, .            
-000020f0: 2020 2020 2020 2020 2020 2074 6865 6d65             theme
-00002100: 3d74 6865 6d65 2c20 0a20 2020 2020 2020  =theme, .       
-00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002120: 636f 6e66 6967 3d7b 0a20 2020 2020 2020  config={.       
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 2020 2020 2020 2277 6964 7468 223a          "width":
-00002150: 2063 6f6e 7465 6e74 5f77 6964 7468 2c20   content_width, 
-00002160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2268 6569 6768 7422 3a20 636f 6e74 656e  "height": conten
-00002190: 745f 6865 6967 6874 2c20 0a20 2020 2020  t_height, .     
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021b0: 2020 2020 2020 2020 2020 226d 696e 5363            "minSc
-000021c0: 616c 6522 3a20 7363 616c 655f 7261 6e67  ale": scale_rang
-000021d0: 655b 305d 2c20 0a20 2020 2020 2020 2020  e[0], .         
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021f0: 2020 2020 2020 2263 656e 7465 7222 3a20        "center": 
-00002200: 5472 7565 2c20 0a20 2020 2020 2020 2020  True, .         
-00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002220: 2020 2020 2020 226d 6178 5363 616c 6522        "maxScale"
-00002230: 3a20 7363 616c 655f 7261 6e67 655b 315d  : scale_range[1]
-00002240: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2020 226d 6172 6769 6e22 3a20 6d61 7267    "margin": marg
-00002270: 696e 2c20 0a20 2020 2020 2020 2020 2020  in, .           
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2020 2270 6c75 6769 6e73 223a 2070      "plugins": p
-000022a0: 6c75 6769 6e73 0a20 2020 2020 2020 2020  lugins.         
-000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022c0: 2020 2020 2020 7d2c 200a 2020 2020 2020        }, .      
-000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022e0: 2069 6e69 7469 616c 5f73 7461 7465 3d7b   initial_state={
-000022f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002310: 2020 2020 2020 2022 696e 6465 7868 223a         "indexh":
-00002320: 2068 736c 6964 6550 6f73 2c20 0a20 2020   hslidePos, .   
-00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002350: 2020 2022 696e 6465 7876 223a 2076 736c     "indexv": vsl
-00002360: 6964 6550 6f73 2c20 0a20 2020 2020 2020  idePos, .       
+00000f50: 612d 6d61 726b 646f 776e 3d22 2220 6461  a-markdown="" da
+00000f60: 7461 2d73 6570 6172 6174 6f72 2d76 6572  ta-separator-ver
+00000f70: 7469 6361 6c3d 225e 2d2d 2422 203e 0a3c  tical="^--$" >.<
+00000f80: 7363 7269 7074 2074 7970 653d 2274 6578  script type="tex
+00000f90: 742f 7465 6d70 6c61 7465 223e 0a23 2320  t/template">.## 
+00000fa0: 5b57 656c 636f 6d65 2074 6f20 4149 204a  [Welcome to AI J
+00000fb0: 656f 7061 7264 7921 5d28 232f 3129 0a3c  eopardy!](#/1).<
+00000fc0: 2f73 6372 6970 743e 0a3c 2f73 6563 7469  /script>.</secti
+00000fd0: 6f6e 3e0a 3c73 6372 6970 7420 7479 7065  on>.<script type
+00000fe0: 3d22 6170 706c 6963 6174 696f 6e2f 6a61  ="application/ja
+00000ff0: 7661 7363 7269 7074 223e 0a20 2020 2066  vascript">.    f
+00001000: 756e 6374 696f 6e20 6669 6e64 4c69 6e6b  unction findLink
+00001010: 2865 6c29 207b 0a20 2020 2020 2020 2069  (el) {.        i
+00001020: 6620 2865 6c2e 7461 674e 616d 6520 3d3d  f (el.tagName ==
+00001030: 2027 4127 2026 2620 656c 2e68 7265 6629   'A' && el.href)
+00001040: 207b 0a20 2020 2020 2020 2020 2020 2072   {.            r
+00001050: 6574 7572 6e20 656c 2e68 7265 663b 0a20  eturn el.href;. 
+00001060: 2020 2020 2020 207d 2065 6c73 6520 6966         } else if
+00001070: 2028 656c 2e70 6172 656e 7445 6c65 6d65   (el.parentEleme
+00001080: 6e74 2920 7b0a 2020 2020 2020 2020 2020  nt) {.          
+00001090: 2020 7265 7475 726e 2066 696e 644c 696e    return findLin
+000010a0: 6b28 656c 2e70 6172 656e 7445 6c65 6d65  k(el.parentEleme
+000010b0: 6e74 293b 0a20 2020 2020 2020 207d 2065  nt);.        } e
+000010c0: 6c73 6520 7b0a 2020 2020 2020 2020 2020  lse {.          
+000010d0: 2020 7265 7475 726e 206e 756c 6c3b 0a20    return null;. 
+000010e0: 2020 2020 2020 207d 0a20 2020 207d 3b0a         }.    };.
+000010f0: 0a20 2020 2066 756e 6374 696f 6e20 6361  .    function ca
+00001100: 6c6c 6261 636b 2865 2920 7b0a 2020 2020  llback(e) {.    
+00001110: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
+00001120: 2243 6c69 636b 2064 6574 6563 7465 6421  "Click detected!
+00001130: 2229 3b0a 2020 2020 2020 2020 636f 6e73  ");.        cons
+00001140: 7420 6c69 6e6b 203d 2066 696e 644c 696e  t link = findLin
+00001150: 6b28 652e 7461 7267 6574 293b 0a20 2020  k(e.target);.   
+00001160: 2020 2020 2069 6620 286c 696e 6b20 3d3d       if (link ==
+00001170: 206e 756c 6c29 207b 2072 6574 7572 6e3b   null) { return;
+00001180: 207d 0a20 2020 2020 2020 2065 2e70 7265   }.        e.pre
+00001190: 7665 6e74 4465 6661 756c 7428 293b 0a20  ventDefault();. 
+000011a0: 2020 2020 2020 2063 6f6e 736f 6c65 2e6c         console.l
+000011b0: 6f67 2822 4c69 6e6b 2063 6c69 636b 6564  og("Link clicked
+000011c0: 2122 2c20 6c69 6e6b 293b 0a20 2020 207d  !", link);.    }
+000011d0: 3b0a 2020 2020 636f 6e73 6f6c 652e 6c6f  ;.    console.lo
+000011e0: 6728 2241 6464 696e 6720 636c 6963 6b20  g("Adding click 
+000011f0: 6c69 7374 656e 6572 2229 3b0a 2020 2020  listener");.    
+00001200: 646f 6375 6d65 6e74 2e61 6464 4576 656e  document.addEven
+00001210: 744c 6973 7465 6e65 7228 2763 6c69 636b  tListener('click
+00001220: 272c 2063 616c 6c62 6163 6b2c 2066 616c  ', callback, fal
+00001230: 7365 293b 0a3c 2f73 6372 6970 743e 2222  se);.</script>""
+00001240: 220a 2020 2020 0a20 2020 2023 204e 6f74  ".    .    # Not
+00001250: 6520 7468 6174 2065 7665 6e20 7468 6f75  e that even thou
+00001260: 6768 2077 6520 7075 7420 6d61 726b 646f  gh we put markdo
+00001270: 776e 2069 6e20 6120 7261 7720 7374 7269  wn in a raw stri
+00001280: 6e67 2c20 7765 2073 7469 6c6c 206e 6565  ng, we still nee
+00001290: 6420 746f 2065 7363 6170 6520 7468 6520  d to escape the 
+000012a0: 6261 636b 736c 6173 6865 730a 2020 2020  backslashes.    
+000012b0: 2320 5468 6973 2069 7320 7768 7920 7765  # This is why we
+000012c0: 2075 7365 2034 2062 6163 6b73 6c61 7368   use 4 backslash
+000012d0: 6573 2074 6f20 6765 7420 3220 6261 636b  es to get 2 back
+000012e0: 736c 6173 6865 7320 696e 2074 6865 206c  slashes in the l
+000012f0: 6174 6578 206d 6174 6820 636f 6465 0a20  atex math code. 
+00001300: 2020 2073 616d 706c 655f 6d61 726b 646f     sample_markdo
+00001310: 776e 203d 2072 2222 220a 2320 5265 7665  wn = r""".# Reve
+00001320: 616c 2e6a 7320 2b20 5374 7265 616d 6c69  al.js + Streamli
+00001330: 740a 4164 6420 3c61 2074 6172 6765 743d  t.Add <a target=
+00001340: 225f 626c 616e 6b22 2068 7265 663d 2268  "_blank" href="h
+00001350: 7474 7073 3a2f 2f72 6576 6561 6c6a 732e  ttps://revealjs.
+00001360: 636f 6d2f 223e 5265 7665 616c 2e6a 733c  com/">Reveal.js<
+00001370: 2f61 3e20 7072 6573 656e 7461 7469 6f6e  /a> presentation
+00001380: 7320 746f 2079 6f75 7220 5374 7265 616d  s to your Stream
+00001390: 6c69 7420 6170 702e 0a2d 2d2d 0a23 2320  lit app..---.## 
+000013a0: 496e 7374 616c 6c61 7469 6f6e 0a60 7069  Installation.`pi
+000013b0: 7020 696e 7374 616c 6c20 7374 7265 616d  p install stream
+000013c0: 6c69 742d 7265 7665 616c 2d73 6c69 6465  lit-reveal-slide
+000013d0: 7360 0a0a 5c5b 5b47 6974 4875 625d 2868  s`..\[[GitHub](h
+000013e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000013f0: 6d2f 626f 757a 6964 616e 6173 2f73 7472  m/bouzidanas/str
+00001400: 6561 6d6c 6974 2e69 6f2f 7472 6565 2f37  eamlit.io/tree/7
+00001410: 3734 3863 3261 3937 6634 6361 3534 6365  748c2a97f4ca54ce
+00001420: 3462 3831 3230 6130 3534 6436 6336 3665  4b8120a054d6c66e
+00001430: 3862 6532 3936 642f 7374 7265 616d 6c69  8be296d/streamli
+00001440: 742d 7265 7665 616c 2d73 6c69 6465 7329  t-reveal-slides)
+00001450: 5c5d 205c 5b5b 5079 5049 5d28 6874 7470  \] \[[PyPI](http
+00001460: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00001470: 6a65 6374 2f73 7472 6561 6d6c 6974 2d72  ject/streamlit-r
+00001480: 6576 6561 6c2d 736c 6964 6573 2f29 5c5d  eveal-slides/)\]
+00001490: 0a2d 2d2d 0a23 2320 5072 6573 656e 7461  .---.## Presenta
+000014a0: 7469 6f6e 2046 6561 7475 7265 730a 2d20  tion Features.- 
+000014b0: 4372 6561 7465 2073 6c69 6465 7320 6672  Create slides fr
+000014c0: 6f6d 206d 6172 6b64 6f77 6e20 6f72 206d  om markdown or m
+000014d0: 6172 6b75 7020 3c21 2d2d 202e 656c 656d  arkup <!-- .elem
+000014e0: 656e 743a 2063 6c61 7373 3d22 6672 6167  ent: class="frag
+000014f0: 6d65 6e74 2220 6461 7461 2d66 7261 676d  ment" data-fragm
+00001500: 656e 742d 696e 6465 783d 2230 2220 2d2d  ent-index="0" --
+00001510: 3e0a 2d20 546f 7563 682c 206d 6f75 7365  >.- Touch, mouse
+00001520: 2c20 616e 6420 6b65 7962 6f61 7264 206e  , and keyboard n
+00001530: 6176 6967 6174 696f 6e20 3c21 2d2d 202e  avigation <!-- .
+00001540: 656c 656d 656e 743a 2063 6c61 7373 3d22  element: class="
+00001550: 6672 6167 6d65 6e74 2220 6461 7461 2d66  fragment" data-f
+00001560: 7261 676d 656e 742d 696e 6465 783d 2231  ragment-index="1
+00001570: 2220 2d2d 3e0a 2d20 4675 6c6c 7363 7265  " -->.- Fullscre
+00001580: 656e 2061 6e64 206f 7665 7276 6965 7720  en and overview 
+00001590: 6d6f 6465 7320 3c21 2d2d 202e 656c 656d  modes <!-- .elem
+000015a0: 656e 743a 2063 6c61 7373 3d22 6672 6167  ent: class="frag
+000015b0: 6d65 6e74 2220 6461 7461 2d66 7261 676d  ment" data-fragm
+000015c0: 656e 742d 696e 6465 783d 2232 2220 2d2d  ent-index="2" --
+000015d0: 3e0a 2d20 5365 6172 6368 2061 6e64 205a  >.- Search and Z
+000015e0: 6f6f 6d20 2870 6c75 6769 6e73 2920 3c21  oom (plugins) <!
+000015f0: 2d2d 202e 656c 656d 656e 743a 2063 6c61  -- .element: cla
+00001600: 7373 3d22 6672 6167 6d65 6e74 2220 6461  ss="fragment" da
+00001610: 7461 2d66 7261 676d 656e 742d 696e 6465  ta-fragment-inde
+00001620: 783d 2233 2220 2d2d 3e0a 2d20 4469 7370  x="3" -->.- Disp
+00001630: 6c61 7920 4c61 5465 5820 616e 6420 7379  lay LaTeX and sy
+00001640: 6e74 6178 2068 6967 686c 6967 6874 6564  ntax highlighted
+00001650: 2063 6f64 6520 2870 6c75 6769 6e73 2920   code (plugins) 
+00001660: 3c21 2d2d 202e 656c 656d 656e 743a 2063  <!-- .element: c
+00001670: 6c61 7373 3d22 6672 6167 6d65 6e74 2220  lass="fragment" 
+00001680: 6461 7461 2d66 7261 676d 656e 742d 696e  data-fragment-in
+00001690: 6465 783d 2234 2220 2d2d 3e0a 2d2d 2d0a  dex="4" -->.---.
+000016a0: 2323 2053 6c69 6465 2043 6f6e 7465 6e74  ## Slide Content
+000016b0: 2043 7265 6174 696f 6e0a 4120 7061 7261   Creation.A para
+000016c0: 6772 6170 6820 7769 7468 2073 6f6d 6520  graph with some 
+000016d0: 7465 7874 2061 6e64 2061 206d 6172 6b64  text and a markd
+000016e0: 6f77 6e20 5b6c 696e 6b5d 2868 7474 7073  own [link](https
+000016f0: 3a2f 2f68 616b 696d 2e73 6529 2e20 0a4d  ://hakim.se). .M
+00001700: 6172 6b64 6f77 6e20 6c69 6e6b 7320 6765  arkdown links ge
+00001710: 7420 6469 7370 6c61 7965 6420 7769 7468  t displayed with
+00001720: 696e 2074 6865 2070 6172 656e 7420 6966  in the parent if
+00001730: 7261 6d65 2e0a 2d2d 0a41 6e6f 7468 6572  rame..--.Another
+00001740: 2070 6172 6167 7261 7068 2063 6f6e 7461   paragraph conta
+00001750: 696e 696e 6720 7468 6520 7361 6d65 203c  ining the same <
+00001760: 6120 7461 7267 6574 3d22 5f62 6c61 6e6b  a target="_blank
+00001770: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
+00001780: 6861 6b69 6d2e 7365 223e 6c69 6e6b 3c2f  hakim.se">link</
+00001790: 613e 2e0a 486f 7765 7665 722c 2074 6869  a>..However, thi
+000017a0: 7320 6c69 6e6b 2077 696c 6c20 6f70 656e  s link will open
+000017b0: 2069 6e20 6120 6e65 7720 7461 6220 696e   in a new tab in
+000017c0: 7374 6561 642e 200a 5468 6973 2069 7320  stead. .This is 
+000017d0: 646f 6e65 2075 7369 6e67 2061 6e20 4854  done using an HT
+000017e0: 4d4c 2060 3c61 3e60 2074 6167 2077 6974  ML `<a>` tag wit
+000017f0: 6820 6074 6172 6765 743d 225f 626c 616e  h `target="_blan
+00001800: 6b22 602e 0a2d 2d2d 0a23 2320 4261 636b  k"`..---.## Back
+00001810: 6772 6f75 6e64 730a 5265 7665 616c 2073  grounds.Reveal s
+00001820: 7570 706f 7274 7320 666f 7572 2064 6966  upports four dif
+00001830: 6665 7265 6e74 2074 7970 6573 206f 6620  ferent types of 
+00001840: 6261 636b 6772 6f75 6e64 733a 2063 6f6c  backgrounds: col
+00001850: 6f72 2c20 696d 6167 652c 2076 6964 656f  or, image, video
+00001860: 2061 6e64 2069 6672 616d 652e 0a2d 2d0a   and iframe..--.
+00001870: 3c21 2d2d 202e 736c 6964 653a 2064 6174  <!-- .slide: dat
+00001880: 612d 6261 636b 6772 6f75 6e64 2d63 6f6c  a-background-col
+00001890: 6f72 3d22 2332 3833 3734 3722 202d 2d3e  or="#283747" -->
+000018a0: 0a43 6861 6e67 6520 7468 6520 6261 636b  .Change the back
+000018b0: 6772 6f75 6e64 2074 6f20 6120 736f 6c69  ground to a soli
+000018c0: 6420 636f 6c6f 7220 7573 696e 6720 7468  d color using th
+000018d0: 6520 6064 6174 612d 6261 636b 6772 6f75  e `data-backgrou
+000018e0: 6e64 2d63 6f6c 6f72 6020 6174 7472 6962  nd-color` attrib
+000018f0: 7574 652e 0a2d 2d0a 3c21 2d2d 202e 736c  ute..--.<!-- .sl
+00001900: 6964 653a 2064 6174 612d 6261 636b 6772  ide: data-backgr
+00001910: 6f75 6e64 2d76 6964 656f 3d22 6874 7470  ound-video="http
+00001920: 733a 2f2f 626f 757a 6964 616e 6173 2e67  s://bouzidanas.g
+00001930: 6974 6875 622e 696f 2f76 6964 656f 732f  ithub.io/videos/
+00001940: 7065 7865 6c73 2d63 6f74 746f 6e62 726f  pexels-cottonbro
+00001950: 2d39 3636 3532 3335 2e6d 7034 2220 6461  -9665235.mp4" da
+00001960: 7461 2d62 6163 6b67 726f 756e 642d 7669  ta-background-vi
+00001970: 6465 6f2d 6c6f 6f70 2064 6174 612d 6261  deo-loop data-ba
+00001980: 636b 6772 6f75 6e64 2d76 6964 656f 2d6d  ckground-video-m
+00001990: 7574 6564 202d 2d3e 0a41 6464 2061 2076  uted -->.Add a v
+000019a0: 6964 656f 2061 7320 7468 6520 6261 636b  ideo as the back
+000019b0: 6772 6f75 6e64 2075 7369 6e67 2074 6865  ground using the
+000019c0: 2060 6461 7461 2d62 6163 6b67 726f 756e   `data-backgroun
+000019d0: 642d 7669 6465 6f60 2061 7474 7269 6275  d-video` attribu
+000019e0: 7465 2e20 4164 6420 6064 6174 612d 6261  te. Add `data-ba
+000019f0: 636b 6772 6f75 6e64 2d76 6964 656f 2d6c  ckground-video-l
+00001a00: 6f6f 7060 2074 6f20 6c6f 6f70 2074 6865  oop` to loop the
+00001a10: 2076 6964 656f 2069 6e20 7468 6520 6261   video in the ba
+00001a20: 636b 6772 6f75 6e64 2061 6e64 2061 6464  ckground and add
+00001a30: 2060 6461 7461 2d62 6163 6b67 726f 756e   `data-backgroun
+00001a40: 642d 7669 6465 6f2d 6d75 7465 6460 2074  d-video-muted` t
+00001a50: 6f20 6d75 7465 2069 742e 0a2d 2d2d 0a23  o mute it..---.#
+00001a60: 2320 4d61 7468 2045 7870 7265 7373 696f  # Math Expressio
+00001a70: 6e73 0a54 6869 7320 666f 6c6c 6f77 696e  ns.This followin
+00001a80: 6720 6973 2061 6e20 6578 616d 706c 6520  g is an example 
+00001a90: 6f66 2061 6e20 696e 6c69 6e65 206d 6174  of an inline mat
+00001aa0: 6820 6571 7561 7469 6f6e 3a20 2465 5e7b  h equation: $e^{
+00001ab0: 695c 7069 7d20 2b20 3120 3d20 3024 2e0a  i\pi} + 1 = 0$..
+00001ac0: 2d2d 0a23 2320 5468 6520 4c6f 7265 6e7a  --.## The Lorenz
+00001ad0: 2045 7175 6174 696f 6e73 0a0a 2424 0a5c   Equations..$$.\
+00001ae0: 6265 6769 6e7b 616c 6967 6e65 647d 0a5c  begin{aligned}.\
+00001af0: 646f 747b 787d 2026 203d 205c 7369 676d  dot{x} & = \sigm
+00001b00: 6128 792d 7829 205c 5c5c 5c0a 5c64 6f74  a(y-x) \\\\.\dot
+00001b10: 7b79 7d20 2620 3d20 5c72 686f 2078 202d  {y} & = \rho x -
+00001b20: 2079 202d 2078 7a20 5c5c 5c5c 0a5c 646f   y - xz \\\\.\do
+00001b30: 747b 7a7d 2026 203d 202d 5c62 6574 6120  t{z} & = -\beta 
+00001b40: 7a20 2b20 7879 0a5c 656e 647b 616c 6967  z + xy.\end{alig
+00001b50: 6e65 647d 0a24 240a 2d2d 2d0a 2323 2043  ned}.$$.---.## C
+00001b60: 6f64 6520 626c 6f63 6b73 0a60 6060 6a73  ode blocks.```js
+00001b70: 205b 312d 327c 337c 345d 0a6c 6574 2061   [1-2|3|4].let a
+00001b80: 203d 2031 3b0a 6c65 7420 6220 3d20 323b   = 1;.let b = 2;
+00001b90: 0a6c 6574 2063 203d 2078 203d 3e20 3120  .let c = x => 1 
+00001ba0: 2b20 3220 2b20 783b 0a63 2833 293b 0a60  + 2 + x;.c(3);.`
+00001bb0: 6060 0a2d 2d2d 0a23 2320 536c 6964 6520  ``.---.## Slide 
+00001bc0: 4672 6167 6d65 6e74 730a 5468 6973 2073  Fragments.This s
+00001bd0: 656e 7465 6e63 6520 6973 2070 6c61 6365  entence is place
+00001be0: 6420 696e 2061 2066 7261 676d 656e 7420  d in a fragment 
+00001bf0: 7769 7468 2060 6461 7461 2d66 7261 676d  with `data-fragm
+00001c00: 656e 742d 696e 6465 783d 2230 2260 200a  ent-index="0"` .
+00001c10: 3c21 2d2d 202e 656c 656d 656e 743a 2063  <!-- .element: c
+00001c20: 6c61 7373 3d22 6672 6167 6d65 6e74 2220  lass="fragment" 
+00001c30: 6461 7461 2d66 7261 676d 656e 742d 696e  data-fragment-in
+00001c40: 6465 783d 2230 2220 2d2d 3e0a 0a54 6869  dex="0" -->..Thi
+00001c50: 7320 6973 2074 6865 2074 6869 7264 2066  s is the third f
+00001c60: 7261 676d 656e 7420 696e 2074 6865 2073  ragment in the s
+00001c70: 6c69 6465 2074 6861 7420 7769 6c6c 2061  lide that will a
+00001c80: 7070 6561 7220 6265 6361 7573 6520 6064  ppear because `d
+00001c90: 6174 612d 6672 6167 6d65 6e74 2d69 6e64  ata-fragment-ind
+00001ca0: 6578 6020 6973 2073 6574 2074 6f20 6031  ex` is set to `1
+00001cb0: 6020 0a3c 212d 2d20 2e65 6c65 6d65 6e74  ` .<!-- .element
+00001cc0: 3a20 636c 6173 733d 2266 7261 676d 656e  : class="fragmen
+00001cd0: 7422 2064 6174 612d 6672 6167 6d65 6e74  t" data-fragment
+00001ce0: 2d69 6e64 6578 3d22 3122 202d 2d3e 0a0a  -index="1" -->..
+00001cf0: 5468 6973 2073 656e 7465 6e63 6520 6170  This sentence ap
+00001d00: 7065 6172 7320 6279 2064 6566 6175 6c74  pears by default
+00001d10: 2077 6865 6e20 796f 7520 7472 616e 7369   when you transi
+00001d20: 7469 6f6e 2069 6e74 6f20 616e 6420 6f75  tion into and ou
+00001d30: 7420 6f66 2074 6869 7320 736c 6964 6520  t of this slide 
+00001d40: 0a2d 2d2d 0a23 2320 436f 6e66 6967 7572  .---.## Configur
+00001d50: 696e 6720 7468 6520 5072 6573 656e 7461  ing the Presenta
+00001d60: 7469 6f6e 0a54 6865 2070 7265 7365 6e74  tion.The present
+00001d70: 6174 696f 6e20 6361 6e20 6265 2063 6f6e  ation can be con
+00001d80: 6669 6775 7265 6420 7573 696e 6720 7468  figured using th
+00001d90: 6520 6063 6f6e 6669 6760 2070 6172 616d  e `config` param
+00001da0: 6574 6572 2e20 4974 7320 6173 2073 696d  eter. Its as sim
+00001db0: 706c 6520 6173 2070 6173 7369 6e67 2061  ple as passing a
+00001dc0: 2064 6963 7469 6f6e 6172 7920 7769 7468   dictionary with
+00001dd0: 2074 6865 2072 6576 6561 6c20 636f 6e66   the reveal conf
+00001de0: 6967 7572 6174 696f 6e20 6f70 7469 6f6e  iguration option
+00001df0: 732e 0a2d 2d2d 0a23 2320 4c61 2066 696e  s..---.## La fin
+00001e00: 0a22 2222 0a20 2020 2073 742e 6d61 726b  .""".    st.mark
+00001e10: 646f 776e 2822 2323 2053 5452 4541 4d4c  down("## STREAML
+00001e20: 4954 2052 4556 4541 4c2e 4a53 2043 4f4d  IT REVEAL.JS COM
+00001e30: 504f 4e45 4e54 2229 0a20 2020 2077 6974  PONENT").    wit
+00001e40: 6820 7374 2e73 6964 6562 6172 3a0a 2020  h st.sidebar:.  
+00001e50: 2020 2020 2020 7374 2e68 6561 6465 7228        st.header(
+00001e60: 2243 6f6d 706f 6e65 6e74 2050 6172 616d  "Component Param
+00001e70: 6574 6572 7322 290a 2020 2020 2020 2020  eters").        
+00001e80: 7468 656d 6520 3d20 7374 2e73 656c 6563  theme = st.selec
+00001e90: 7462 6f78 2822 5468 656d 6522 2c20 5b22  tbox("Theme", ["
+00001ea0: 626c 6163 6b22 2c20 2262 6c61 636b 2d63  black", "black-c
+00001eb0: 6f6e 7472 6173 7422 2c20 2262 6c6f 6f64  ontrast", "blood
+00001ec0: 222c 2022 6472 6163 756c 6122 2c20 226d  ", "dracula", "m
+00001ed0: 6f6f 6e22 2c20 2277 6869 7465 222c 2022  oon", "white", "
+00001ee0: 7768 6974 652d 636f 6e74 7261 7374 222c  white-contrast",
+00001ef0: 2022 6c65 6167 7565 222c 2022 6265 6967   "league", "beig
+00001f00: 6522 2c20 2273 6b79 222c 2022 6e69 6768  e", "sky", "nigh
+00001f10: 7422 2c20 2273 6572 6966 222c 2022 7369  t", "serif", "si
+00001f20: 6d70 6c65 222c 2022 736f 6c61 7269 7a65  mple", "solarize
+00001f30: 6422 5d29 0a20 2020 2020 2020 2068 6569  d"]).        hei
+00001f40: 6768 7420 3d20 7374 2e6e 756d 6265 725f  ght = st.number_
+00001f50: 696e 7075 7428 2248 6569 6768 7422 2c20  input("Height", 
+00001f60: 7661 6c75 653d 3530 3029 0a20 2020 2020  value=500).     
+00001f70: 2020 2073 742e 7375 6268 6561 6465 7228     st.subheader(
+00001f80: 2253 6c69 6465 2043 6f6e 6669 6775 7261  "Slide Configura
+00001f90: 7469 6f6e 2229 0a20 2020 2020 2020 2063  tion").        c
+00001fa0: 6f6e 7465 6e74 5f68 6569 6768 7420 3d20  ontent_height = 
+00001fb0: 7374 2e6e 756d 6265 725f 696e 7075 7428  st.number_input(
+00001fc0: 2243 6f6e 7465 6e74 2048 6569 6768 7422  "Content Height"
+00001fd0: 2c20 7661 6c75 653d 3930 3029 0a20 2020  , value=900).   
+00001fe0: 2020 2020 2063 6f6e 7465 6e74 5f77 6964       content_wid
+00001ff0: 7468 203d 2073 742e 6e75 6d62 6572 5f69  th = st.number_i
+00002000: 6e70 7574 2822 436f 6e74 656e 7420 5769  nput("Content Wi
+00002010: 6474 6822 2c20 7661 6c75 653d 3930 3029  dth", value=900)
+00002020: 0a20 2020 2020 2020 2073 6361 6c65 5f72  .        scale_r
+00002030: 616e 6765 203d 2073 742e 736c 6964 6572  ange = st.slider
+00002040: 2822 5363 616c 6520 5261 6e67 6522 2c20  ("Scale Range", 
+00002050: 6d69 6e5f 7661 6c75 653d 302e 302c 206d  min_value=0.0, m
+00002060: 6178 5f76 616c 7565 3d35 2e30 2c20 7661  ax_value=5.0, va
+00002070: 6c75 653d 5b30 2e31 2c20 302e 355d 2c20  lue=[0.1, 0.5], 
+00002080: 7374 6570 3d30 2e31 290a 2020 2020 2020  step=0.1).      
+00002090: 2020 6d61 7267 696e 203d 2073 742e 736c    margin = st.sl
+000020a0: 6964 6572 2822 4d61 7267 696e 222c 206d  ider("Margin", m
+000020b0: 696e 5f76 616c 7565 3d30 2e30 2c20 6d61  in_value=0.0, ma
+000020c0: 785f 7661 6c75 653d 302e 382c 2076 616c  x_value=0.8, val
+000020d0: 7565 3d30 2e31 2c20 7374 6570 3d30 2e30  ue=0.1, step=0.0
+000020e0: 3529 0a20 2020 2020 2020 2070 6c75 6769  5).        plugi
+000020f0: 6e73 203d 2073 742e 6d75 6c74 6973 656c  ns = st.multisel
+00002100: 6563 7428 2250 6c75 6769 6e73 222c 205b  ect("Plugins", [
+00002110: 2268 6967 686c 6967 6874 222c 2022 6b61  "highlight", "ka
+00002120: 7465 7822 2c20 226d 6174 686a 6178 3222  tex", "mathjax2"
+00002130: 2c20 226d 6174 686a 6178 3322 2c20 226e  , "mathjax3", "n
+00002140: 6f74 6573 222c 2022 7365 6172 6368 222c  otes", "search",
+00002150: 2022 7a6f 6f6d 225d 2c20 5b5d 290a 2020   "zoom"], []).  
+00002160: 2020 2020 2020 7374 2e73 7562 6865 6164        st.subhead
+00002170: 6572 2822 496e 6974 6961 6c20 5374 6174  er("Initial Stat
+00002180: 6522 290a 2020 2020 2020 2020 6873 6c69  e").        hsli
+00002190: 6465 506f 7320 3d20 7374 2e6e 756d 6265  dePos = st.numbe
+000021a0: 725f 696e 7075 7428 2248 6f72 697a 6f6e  r_input("Horizon
+000021b0: 7461 6c20 536c 6964 6520 506f 7369 7469  tal Slide Positi
+000021c0: 6f6e 222c 2076 616c 7565 3d30 290a 2020  on", value=0).  
+000021d0: 2020 2020 2020 7673 6c69 6465 506f 7320        vslidePos 
+000021e0: 3d20 7374 2e6e 756d 6265 725f 696e 7075  = st.number_inpu
+000021f0: 7428 2256 6572 7469 6361 6c20 536c 6964  t("Vertical Slid
+00002200: 6520 506f 7369 7469 6f6e 222c 2076 616c  e Position", val
+00002210: 7565 3d30 290a 2020 2020 2020 2020 6672  ue=0).        fr
+00002220: 6167 506f 7320 3d20 7374 2e6e 756d 6265  agPos = st.numbe
+00002230: 725f 696e 7075 7428 2246 7261 676d 656e  r_input("Fragmen
+00002240: 7420 506f 7369 7469 6f6e 222c 2076 616c  t Position", val
+00002250: 7565 3d2d 3129 0a20 2020 2020 2020 206f  ue=-1).        o
+00002260: 7665 7276 6965 7720 3d20 7374 2e63 6865  verview = st.che
+00002270: 636b 626f 7828 2253 686f 7720 4f76 6572  ckbox("Show Over
+00002280: 7669 6577 222c 2076 616c 7565 3d46 616c  view", value=Fal
+00002290: 7365 290a 2020 2020 2020 2020 7061 7573  se).        paus
+000022a0: 6564 203d 2073 742e 6368 6563 6b62 6f78  ed = st.checkbox
+000022b0: 2822 5061 7573 6522 2c20 7661 6c75 653d  ("Pause", value=
+000022c0: 4661 6c73 6529 0a20 2020 200a 2020 2020  False).    .    
+000022d0: 2323 2041 6464 2074 6865 2073 7472 6561  ## Add the strea
+000022e0: 6d6c 6974 2d72 6576 6561 6c2d 736c 6964  mlit-reveal-slid
+000022f0: 6520 636f 6d70 6f6e 656e 7420 746f 2074  e component to t
+00002300: 6865 2053 7472 6561 6d6c 6974 2061 7070  he Streamlit app
+00002310: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002320: 2020 2020 2020 0a20 2020 2023 2320 4874        .    ## Ht
+00002330: 6d6c 206d 6172 6b75 7020 6578 616d 706c  ml markup exampl
+00002340: 650a 2020 2020 2320 6375 7272 5374 6174  e.    # currStat
+00002350: 6520 3d20 736c 6964 6573 2873 616d 706c  e = slides(sampl
+00002360: 655f 6874 6d6c 2c20 0a20 2020 2023 2020  e_html, .    #  
 00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002380: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002390: 696e 6465 7866 223a 2066 7261 6750 6f73  indexf": fragPos
-000023a0: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 2020 2020 2020 2020 2022 7061 7573 6564           "paused
-000023d0: 223a 2070 6175 7365 642c 200a 2020 2020  ": paused, .    
-000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002400: 2020 226f 7665 7276 6965 7722 3a20 6f76    "overview": ov
-00002410: 6572 7669 6577 200a 2020 2020 2020 2020  erview .        
-00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002430: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00002440: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00002450: 2020 2020 2020 2020 206d 6172 6b64 6f77           markdow
-00002460: 6e5f 7072 6f70 733d 7b22 6461 7461 2d73  n_props={"data-s
-00002470: 6570 6172 6174 6f72 2d76 6572 7469 6361  eparator-vertica
-00002480: 6c22 3a22 5e2d 2d24 227d 2c20 0a20 2020  l":"^--$"}, .   
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2020 2020 6373 733d 7222 626f 6479 2e72      css=r"body.r
-000024b0: 6576 6561 6c2d 7669 6577 706f 7274 207b  eveal-viewport {
-000024c0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-000024d0: 3a20 626c 7565 3b7d 222c 0a20 2020 2020  : blue;}",.     
-000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024f0: 2020 6469 7370 6c61 795f 6f6e 6c79 3d54    display_only=T
-00002500: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00002510: 2020 2020 2020 2020 2020 2020 6b65 793d              key=
-00002520: 2272 6576 6561 6c5f 736c 6964 6573 2229  "reveal_slides")
-00002530: 0a0a 2020 2020 6966 2063 7572 7253 7461  ..    if currSta
-00002540: 7465 5b22 696e 6465 7868 225d 203d 3d20  te["indexh"] == 
-00002550: 303a 0a20 2020 2020 2020 2073 742e 6d61  0:.        st.ma
-00002560: 726b 646f 776e 2822 5265 7665 616c 2e6a  rkdown("Reveal.j
-00002570: 7320 6973 2061 6e20 6f70 656e 2073 6f75  s is an open sou
-00002580: 7263 6520 4854 4d4c 2070 7265 7365 6e74  rce HTML present
-00002590: 6174 696f 6e20 6672 616d 6577 6f72 6b2e  ation framework.
-000025a0: 2049 7420 656e 6162 6c65 7320 616e 796f   It enables anyo
-000025b0: 6e65 2077 6974 6820 6120 7765 6220 6272  ne with a web br
-000025c0: 6f77 7365 7220 746f 2063 7265 6174 6520  owser to create 
-000025d0: 6675 6c6c 792d 6665 6174 7572 6564 2061  fully-featured a
-000025e0: 6e64 2062 6561 7574 6966 756c 2070 7265  nd beautiful pre
-000025f0: 7365 6e74 6174 696f 6e73 2066 6f72 2066  sentations for f
-00002600: 7265 652e 205c 6e5c 6e54 6865 2066 7261  ree. \n\nThe fra
-00002610: 6d65 776f 726b 2063 6f6d 6573 2077 6974  mework comes wit
-00002620: 6820 6120 6272 6f61 6420 7261 6e67 6520  h a broad range 
-00002630: 6f66 2066 6561 7475 7265 7320 696e 636c  of features incl
-00002640: 7564 696e 6720 6e65 7374 6564 2073 6c69  uding nested sli
-00002650: 6465 732c 204d 6172 6b64 6f77 6e20 7375  des, Markdown su
-00002660: 7070 6f72 742c 2041 7574 6f2d 416e 696d  pport, Auto-Anim
-00002670: 6174 652c 2050 4446 2065 7870 6f72 742c  ate, PDF export,
-00002680: 2073 7065 616b 6572 206e 6f74 6573 2c20   speaker notes, 
-00002690: 4c61 5465 5820 7375 7070 6f72 7420 616e  LaTeX support an
-000026a0: 6420 7379 6e74 6178 2068 6967 686c 6967  d syntax highlig
-000026b0: 6874 6564 2063 6f64 652e 2229 0a20 2020  hted code.").   
-000026c0: 2065 6c69 6620 6375 7272 5374 6174 655b   elif currState[
-000026d0: 2269 6e64 6578 6822 5d20 3d3d 2032 3a0a  "indexh"] == 2:.
-000026e0: 2020 2020 2020 2020 6966 2063 7572 7253          if currS
-000026f0: 7461 7465 5b22 696e 6465 7866 225d 203d  tate["indexf"] =
-00002700: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00002710: 2073 742e 6d61 726b 646f 776e 2822 5f28   st.markdown("_(
-00002720: 7365 6520 6c61 7465 7220 736c 6964 6573  see later slides
-00002730: 2066 6f72 2064 6574 6169 6c73 2061 6e64   for details and
-00002740: 2065 7861 6d70 6c65 7329 5f22 290a 2020   examples)_").  
-00002750: 2020 2020 2020 656c 6966 2063 7572 7253        elif currS
-00002760: 7461 7465 5b22 696e 6465 7866 225d 203d  tate["indexf"] =
-00002770: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-00002780: 2073 742e 6d61 726b 646f 776e 2822 2d20   st.markdown("- 
-00002790: 596f 7520 6361 6e20 7377 6970 6520 686f  You can swipe ho
-000027a0: 7269 7a6f 6e74 616c 6c79 206f 7220 7665  rizontally or ve
-000027b0: 7274 6963 616c 6c79 2074 6f20 6e61 7669  rtically to navi
-000027c0: 6761 7465 2074 6872 6f75 6768 2061 2070  gate through a p
-000027d0: 7265 7365 6e74 6174 696f 6e20 6f6e 2061  resentation on a
-000027e0: 6e79 2074 6f75 6368 2d65 6e61 626c 6564  ny touch-enabled
-000027f0: 2064 6576 6963 652e 205c 6e2d 2059 6f75   device. \n- You
-00002800: 2063 616e 2075 7365 2074 6865 2061 7272   can use the arr
-00002810: 6f77 206b 6579 7320 6f6e 2079 6f75 7220  ow keys on your 
-00002820: 6b65 7962 6f61 7264 2074 6f20 6e61 7669  keyboard to navi
-00002830: 6761 7465 2061 7320 7765 6c6c 2e20 5c6e  gate as well. \n
-00002840: 2d20 4e61 7669 6761 7469 6e67 2077 6974  - Navigating wit
-00002850: 6820 7468 6520 6d6f 7573 6520 6973 2061  h the mouse is a
-00002860: 7320 7369 6d70 6c65 2061 7320 636c 6963  s simple as clic
-00002870: 6b69 6e67 2074 6865 2064 6972 6563 7469  king the directi
-00002880: 6f6e 616c 2061 7272 6f77 7320 6e65 6172  onal arrows near
-00002890: 2074 6865 2065 6467 6573 206f 7220 636f   the edges or co
-000028a0: 726e 6572 7320 6f66 2074 6865 2073 6c69  rners of the sli
-000028b0: 6465 732e 2229 0a20 2020 2020 2020 2065  des.").        e
-000028c0: 6c69 6620 6375 7272 5374 6174 655b 2269  lif currState["i
-000028d0: 6e64 6578 6622 5d20 3d3d 2032 3a0a 2020  ndexf"] == 2:.  
-000028e0: 2020 2020 2020 2020 2020 7374 2e6d 6172            st.mar
-000028f0: 6b64 6f77 6e28 222d 2050 7265 7373 2074  kdown("- Press t
-00002900: 6865 2060 4660 206b 6579 206f 6e20 796f  he `F` key on yo
-00002910: 7572 206b 6579 626f 6172 6420 746f 2065  ur keyboard to e
-00002920: 6e74 6572 2066 756c 6c2d 7363 7265 656e  nter full-screen
-00002930: 206d 6f64 652e 2050 7265 7373 2060 4553   mode. Press `ES
-00002940: 4360 2074 6f20 6578 6974 2066 756c 6c2d  C` to exit full-
-00002950: 7363 7265 656e 206d 6f64 652e 205c 6e2d  screen mode. \n-
-00002960: 2050 7265 7373 2074 6865 2060 4f60 206f   Press the `O` o
-00002970: 6620 6045 5343 6020 6b65 7920 746f 2065  f `ESC` key to e
-00002980: 6e74 6572 2061 6e64 2065 7869 7420 6f76  nter and exit ov
-00002990: 6572 7669 6577 206d 6f64 6522 290a 2020  erview mode").  
-000029a0: 2020 2020 2020 656c 6966 2063 7572 7253        elif currS
-000029b0: 7461 7465 5b22 696e 6465 7866 225d 203d  tate["indexf"] =
-000029c0: 3d20 333a 0a20 2020 2020 2020 2020 2020  = 3:.           
-000029d0: 2073 742e 7772 6974 6528 223a 6172 726f   st.write(":arro
-000029e0: 775f 6c65 6674 3a20 4d61 6b65 2073 7572  w_left: Make sur
-000029f0: 6520 746f 2061 6464 2074 6865 2073 6561  e to add the sea
-00002a00: 7263 6820 616e 6420 7a6f 6f6d 2070 6c75  rch and zoom plu
-00002a10: 6769 6e73 2074 6f20 6163 7469 7661 7465  gins to activate
-00002a20: 2074 6865 7365 2066 6561 7475 7265 732e   these features.
-00002a30: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-00002a40: 742e 6d61 726b 646f 776e 2822 2d20 5072  t.markdown("- Pr
-00002a50: 6573 7320 6043 7472 6c60 202b 2060 5368  ess `Ctrl` + `Sh
-00002a60: 6966 7460 202b 2060 4660 206b 6579 7320  ift` + `F` keys 
-00002a70: 6f6e 2079 6f75 7220 6b65 7962 6f61 7264  on your keyboard
-00002a80: 2074 6f20 6f70 656e 2061 6e64 2063 6c6f   to open and clo
-00002a90: 7365 2074 6865 2073 6561 7263 6820 6469  se the search di
-00002aa0: 616c 6f67 2e20 5c6e 2d20 5072 6573 7320  alog. \n- Press 
-00002ab0: 7468 6520 6041 6c74 6020 6b65 7920 616e  the `Alt` key an
-00002ac0: 6420 7269 6768 7420 636c 6963 6b20 746f  d right click to
-00002ad0: 207a 6f6f 6d20 696e 2061 6e64 206f 7574   zoom in and out
-00002ae0: 206f 6e20 7468 6520 7265 6769 6f6e 2074   on the region t
-00002af0: 6865 206d 6f75 7365 2069 7320 686f 7665  he mouse is hove
-00002b00: 7269 6e67 206f 7665 722e 2229 0a20 2020  ring over.").   
-00002b10: 2020 2020 2065 6c69 6620 6375 7272 5374       elif currSt
-00002b20: 6174 655b 2269 6e64 6578 6622 5d20 3d3d  ate["indexf"] ==
-00002b30: 2034 3a0a 2020 2020 2020 2020 2020 2020   4:.            
-00002b40: 7374 2e6d 6172 6b64 6f77 6e28 225f 2873  st.markdown("_(s
-00002b50: 6565 206c 6174 6572 2073 6c69 6465 7320  ee later slides 
-00002b60: 666f 7220 6465 7461 696c 7320 616e 6420  for details and 
-00002b70: 6578 616d 706c 6573 295f 2229 0a20 2020  examples)_").   
-00002b80: 2065 6c69 6620 6375 7272 5374 6174 655b   elif currState[
-00002b90: 2269 6e64 6578 6822 5d20 3d3d 2033 3a0a  "indexh"] == 3:.
-00002ba0: 2020 2020 2020 2020 7374 2e6d 6172 6b64          st.markd
-00002bb0: 6f77 6e28 2727 2754 6869 7320 636f 6d70  own('''This comp
-00002bc0: 6f6e 656e 7420 616c 6c6f 7773 2066 6f72  onent allows for
-00002bd0: 2074 776f 2077 6179 7320 6f66 2063 7265   two ways of cre
-00002be0: 6174 696e 6720 7265 7665 616c 2e6a 7320  ating reveal.js 
-00002bf0: 7072 6573 656e 7461 7469 6f6e 732e 205c  presentations. \
-00002c00: 6e31 2e20 5b4d 6172 6b64 6f77 6e5d 2868  n1. [Markdown](h
-00002c10: 7474 7073 3a2f 2f72 6576 6561 6c6a 732e  ttps://revealjs.
-00002c20: 636f 6d2f 6d61 726b 646f 776e 2f29 205c  com/markdown/) \
-00002c30: 6e32 2e20 5b4d 6172 6b75 705d 2868 7474  n2. [Markup](htt
-00002c40: 7073 3a2f 2f72 6576 6561 6c6a 732e 636f  ps://revealjs.co
-00002c50: 6d2f 6d61 726b 7570 2f29 205c 6e5c 6e54  m/markup/) \n\nT
-00002c60: 6865 2070 7269 6d61 7279 2077 6179 2069  he primary way i
-00002c70: 7320 7573 696e 6720 6d61 726b 646f 776e  s using markdown
-00002c80: 2e20 4279 2064 6566 6175 6c74 2c20 7468  . By default, th
-00002c90: 6520 636f 6d70 6f6e 656e 7420 6073 6c69  e component `sli
-00002ca0: 6465 6020 6675 6e63 7469 6f6e 2061 6363  de` function acc
-00002cb0: 6570 7473 2061 2073 7472 696e 6720 636f  epts a string co
-00002cc0: 6e74 6169 6e69 6e67 206d 6172 6b64 6f77  ntaining markdow
-00002cd0: 6e20 6173 2069 6e70 7574 2e20 4e6f 7465  n as input. Note
-00002ce0: 2074 6861 7420 7468 6973 2073 7472 6561   that this strea
-00002cf0: 6d6c 6974 2063 6f6d 706f 6e65 6e74 2074  mlit component t
-00002d00: 616b 6573 2063 6172 6520 6f66 2074 6865  akes care of the
-00002d10: 2068 746d 6c20 7461 6773 2028 603c 7365   html tags (`<se
-00002d20: 6374 696f 6e3e 602c 2060 3c74 6578 7461  ction>`, `<texta
-00002d30: 7265 613e 602c 2060 3c73 6372 6970 743e  rea>`, `<script>
-00002d40: 6029 2066 6f72 2079 6f75 2073 6f20 796f  `) for you so yo
-00002d50: 7520 6f6e 6c79 2068 6176 6520 746f 2077  u only have to w
-00002d60: 6f72 7279 2061 626f 7574 2074 6865 206d  orry about the m
-00002d70: 6172 6b64 6f77 6e20 636f 6e74 656e 742e  arkdown content.
-00002d80: 2054 6865 2066 6f6c 6c6f 7769 6e67 2069   The following i
-00002d90: 7320 7369 6d70 6c65 2065 7861 6d70 6c65  s simple example
-00002da0: 206f 6620 6d61 726b 646f 776e 2066 6f72   of markdown for
-00002db0: 2061 2070 7265 7365 6e74 6174 696f 6e20   a presentation 
-00002dc0: 7769 7468 2074 6872 6565 2073 6c69 6465  with three slide
-00002dd0: 733a 2027 2727 290a 2020 2020 2020 2020  s: ''').        
-00002de0: 7361 6d70 6c65 5f6d 6172 6b64 6f77 6e20  sample_markdown 
-00002df0: 3d20 2727 2723 2320 536c 6964 6520 310a  = '''## Slide 1.
-00002e00: 4120 7061 7261 6772 6170 6820 7769 7468  A paragraph with
-00002e10: 2073 6f6d 6520 7465 7874 2061 6e64 2061   some text and a
-00002e20: 205b 6c69 6e6b 5d28 6874 7470 733a 2f2f   [link](https://
-00002e30: 6861 6b69 6d2e 7365 292e 0a2d 2d2d 0a23  hakim.se)..---.#
-00002e40: 2320 536c 6964 6520 320a 2d2d 2d0a 2323  # Slide 2.---.##
-00002e50: 2053 6c69 6465 2033 2727 270a 2020 2020   Slide 3'''.    
-00002e60: 2020 2020 7374 2e63 6f64 6528 7361 6d70      st.code(samp
-00002e70: 6c65 5f6d 6172 6b64 6f77 6e2c 206c 616e  le_markdown, lan
-00002e80: 6775 6167 653d 226d 6422 290a 2020 2020  guage="md").    
-00002e90: 2020 2020 7374 2e6d 6172 6b64 6f77 6e28      st.markdown(
-00002ea0: 2727 2754 6865 2073 6563 6f6e 6420 7761  '''The second wa
-00002eb0: 7920 6973 2062 7920 7072 6f76 6964 696e  y is by providin
-00002ec0: 6720 6120 7374 7269 6e67 2063 6f6e 7461  g a string conta
-00002ed0: 696e 696e 6720 7468 6520 6d61 726b 7570  ining the markup
-00002ee0: 2074 6861 7420 676f 6573 2069 6e73 6964   that goes insid
-00002ef0: 6520 7468 6520 603c 6469 7620 636c 6173  e the `<div clas
-00002f00: 733d 2273 6c69 6465 7322 3e60 2065 6c65  s="slides">` ele
-00002f10: 6d65 6e74 2061 6e64 2073 6574 7469 6e67  ment and setting
-00002f20: 2074 6865 2060 736c 6964 6560 2066 756e   the `slide` fun
-00002f30: 6374 696f 6e27 7320 6061 6c6c 6f77 5f75  ction's `allow_u
-00002f40: 6e73 6166 655f 6874 6d6c 6020 6172 6775  nsafe_html` argu
-00002f50: 6d65 6e74 2074 6f20 6054 7275 6560 2e20  ment to `True`. 
-00002f60: 5468 6520 6c61 7474 6572 2069 7320 7768  The latter is wh
-00002f70: 6174 2074 656c 6c73 2074 6865 2063 6f6d  at tells the com
-00002f80: 706f 6e65 6e74 2074 6f20 6578 7065 6374  ponent to expect
-00002f90: 206d 6172 6b75 7020 696e 7374 6561 6420   markup instead 
-00002fa0: 6f66 206d 6172 6b64 6f77 6e2e 2727 2729  of markdown.''')
-00002fb0: 0a20 2020 2020 2020 2073 616d 706c 655f  .        sample_
-00002fc0: 6874 6d6c 203d 2027 2727 3c64 6976 2063  html = '''<div c
-00002fd0: 6c61 7373 3d22 7265 7665 616c 223e 0a20  lass="reveal">. 
-00002fe0: 203c 6469 7620 636c 6173 733d 2273 6c69   <div class="sli
-00002ff0: 6465 7322 3e0a 2020 2020 3c73 6563 7469  des">.    <secti
-00003000: 6f6e 3e48 6f72 697a 6f6e 7461 6c20 536c  on>Horizontal Sl
-00003010: 6964 653c 2f73 6563 7469 6f6e 3e0a 2020  ide</section>.  
-00003020: 2020 3c73 6563 7469 6f6e 3e0a 2020 2020    <section>.    
-00003030: 2020 3c73 6563 7469 6f6e 3e56 6572 7469    <section>Verti
-00003040: 6361 6c20 536c 6964 6520 313c 2f73 6563  cal Slide 1</sec
-00003050: 7469 6f6e 3e0a 2020 2020 2020 3c73 6563  tion>.      <sec
-00003060: 7469 6f6e 3e56 6572 7469 6361 6c20 536c  tion>Vertical Sl
-00003070: 6964 6520 323c 2f73 6563 7469 6f6e 3e0a  ide 2</section>.
-00003080: 2020 2020 3c2f 7365 6374 696f 6e3e 0a20      </section>. 
-00003090: 203c 2f64 6976 3e0a 3c2f 6469 763e 2727   </div>.</div>''
-000030a0: 270a 2020 2020 2020 2020 7374 2e63 6f64  '.        st.cod
-000030b0: 6528 7361 6d70 6c65 5f68 746d 6c2c 206c  e(sample_html, l
-000030c0: 616e 6775 6167 653d 2268 746d 6c22 290a  anguage="html").
-000030d0: 2020 2020 2020 2020 7374 2e77 6172 6e69          st.warni
-000030e0: 6e67 2822 5741 524e 494e 4721 2120 5468  ng("WARNING!! Th
-000030f0: 6520 6d61 726b 7570 2079 6f75 2070 726f  e markup you pro
-00003100: 7669 6465 2069 7320 6469 7265 6374 6c79  vide is directly
-00003110: 2069 6e6a 6563 7465 6420 7669 6120 7468   injected via th
-00003120: 6520 6064 616e 6765 726f 7573 6c79 5365  e `dangerouslySe
-00003130: 7449 6e6e 6572 4854 4d4c 6020 7072 6f70  tInnerHTML` prop
-00003140: 6572 7479 206f 6620 7468 6520 656e 636c  erty of the encl
-00003150: 6f73 696e 6720 6064 6976 602e 2054 6869  osing `div`. Thi
-00003160: 7320 6d65 616e 7320 7468 6174 2079 6f75  s means that you
-00003170: 2061 7265 2072 6573 706f 6e73 6962 6c65   are responsible
-00003180: 2066 6f72 2065 6e73 7572 696e 6720 7468   for ensuring th
-00003190: 6174 2074 6865 206d 6172 6b75 7020 6973  at the markup is
-000031a0: 2073 6166 6520 616e 6420 646f 6573 206e   safe and does n
-000031b0: 6f74 2063 6f6e 7461 696e 2061 6e79 206d  ot contain any m
-000031c0: 616c 6963 696f 7573 2063 6f64 652e 2054  alicious code. T
-000031d0: 6865 2063 6f6d 706f 6e65 6e74 2064 6f65  he component doe
-000031e0: 7320 6e6f 7420 646f 2061 6e79 2073 616e  s not do any san
-000031f0: 6974 697a 6174 696f 6e20 6f66 2074 6865  itization of the
-00003200: 206d 6172 6b75 702e 2229 0a20 2020 2065   markup.").    e
-00003210: 6c69 6620 6375 7272 5374 6174 655b 2269  lif currState["i
-00003220: 6e64 6578 6822 5d20 3d3d 2034 3a0a 2020  ndexh"] == 4:.  
-00003230: 2020 2020 2020 7374 2e6d 6172 6b64 6f77        st.markdow
-00003240: 6e28 2246 6f72 206d 6f72 6520 6578 616d  n("For more exam
-00003250: 706c 6573 206f 6620 6261 636b 6772 6f75  ples of backgrou
-00003260: 6e64 732c 2073 6565 205b 6865 7265 5d28  nds, see [here](
-00003270: 6874 7470 733a 2f2f 7265 7665 616c 6a73  https://revealjs
-00003280: 2e63 6f6d 2f62 6163 6b67 726f 756e 6473  .com/backgrounds
-00003290: 2f29 2e22 290a 2020 2020 2020 2020 7374  /).").        st
-000032a0: 2e6d 6172 6b64 6f77 6e28 2254 6f20 6368  .markdown("To ch
-000032b0: 616e 6765 2074 6865 2062 6163 6b67 726f  ange the backgro
-000032c0: 756e 6420 696e 206d 6172 6b64 6f77 6e2c  und in markdown,
-000032d0: 2061 6464 2061 2063 6f6d 6d65 6e74 2074   add a comment t
-000032e0: 6f20 7468 6520 736c 6964 6520 7468 6174  o the slide that
-000032f0: 206f 6265 7973 2074 6865 2066 6f6c 6c6f   obeys the follo
-00003300: 7769 6e67 2073 796e 7461 783a 2229 0a20  wing syntax:"). 
-00003310: 2020 2020 2020 2073 742e 636f 6465 2827         st.code('
-00003320: 3c21 2d2d 202e 736c 6964 653a 2064 6174  <!-- .slide: dat
-00003330: 612d 6261 636b 6772 6f75 6e64 2d63 6f6c  a-background-col
-00003340: 6f72 3d22 2332 3833 3734 3722 202d 2d3e  or="#283747" -->
-00003350: 272c 206c 616e 6775 6167 653d 226d 6422  ', language="md"
-00003360: 290a 2020 2020 2020 2020 7374 2e6d 6172  ).        st.mar
-00003370: 6b64 6f77 6e28 224d 616b 6520 7375 7265  kdown("Make sure
-00003380: 2074 6f20 6164 6420 616c 6c20 7468 6520   to add all the 
-00003390: 6064 6174 612d 6020 6174 7472 6962 7574  `data-` attribut
-000033a0: 6573 2079 6f75 2072 6571 7569 7265 2061  es you require a
-000033b0: 6674 6572 2074 6865 2060 2e73 6c69 6465  fter the `.slide
-000033c0: 3a60 2229 0a20 2020 2065 6c69 6620 6375  :`").    elif cu
-000033d0: 7272 5374 6174 655b 2269 6e64 6578 6822  rrState["indexh"
-000033e0: 5d20 3d3d 2035 3a0a 2020 2020 2020 2020  ] == 5:.        
-000033f0: 7374 2e77 7269 7465 2822 3a61 7272 6f77  st.write(":arrow
-00003400: 5f6c 6566 743a 204d 616b 6520 7375 7265  _left: Make sure
-00003410: 2074 6f20 6164 642f 696e 636c 7564 6520   to add/include 
-00003420: 7468 6520 6d61 7468 2070 6c75 6769 6e20  the math plugin 
-00003430: 736f 2074 6861 7420 7468 6520 6c61 7465  so that the late
-00003440: 7820 6973 2070 726f 7065 726c 7920 7072  x is properly pr
-00003450: 6f63 6573 7365 6420 616e 6420 7265 6e64  ocessed and rend
-00003460: 6572 6564 2e20 5468 6572 6520 6172 6520  ered. There are 
-00003470: 7468 7265 6520 6275 696c 742d 696e 2070  three built-in p
-00003480: 6c75 6769 6e73 2074 6861 7420 7072 6f63  lugins that proc
-00003490: 6573 7320 6c61 7465 783a 2229 0a20 2020  ess latex:").   
-000034a0: 2020 2020 2073 742e 7772 6974 6528 2231       st.write("1
-000034b0: 2e20 606b 6174 6578 6020 2d20 7573 6573  . `katex` - uses
-000034c0: 204b 6154 6558 2074 6f20 7265 6e64 6572   KaTeX to render
-000034d0: 206d 6174 6820 6571 7561 7469 6f6e 732e   math equations.
-000034e0: 205c 6e32 2e20 606d 6174 686a 6178 3260   \n2. `mathjax2`
-000034f0: 202d 2075 7365 7320 4d61 7468 4a61 7832   - uses MathJax2
-00003500: 2074 6f20 7265 6e64 6572 206d 6174 6820   to render math 
-00003510: 6571 7561 7469 6f6e 732e 205c 6e33 2e20  equations. \n3. 
-00003520: 606d 6174 686a 6178 3360 202d 2075 7365  `mathjax3` - use
-00003530: 7320 4d61 7468 4a61 7833 2074 6f20 7265  s MathJax3 to re
-00003540: 6e64 6572 206d 6174 6820 6571 7561 7469  nder math equati
-00003550: 6f6e 732e 2229 0a20 2020 2020 2020 2073  ons.").        s
-00003560: 742e 7761 726e 696e 6728 2257 4152 4e49  t.warning("WARNI
-00003570: 4e47 2121 204f 6e6c 7920 6f6e 6520 6d61  NG!! Only one ma
-00003580: 7468 2070 6c75 6769 6e20 6361 6e20 6265  th plugin can be
-00003590: 2075 7365 6420 6174 2061 2074 696d 652e   used at a time.
-000035a0: 2049 6e63 6c75 6469 6e67 206d 6f72 6520   Including more 
-000035b0: 7468 616e 206f 6e65 2070 6c75 6769 6e20  than one plugin 
-000035c0: 7769 6c6c 2072 6573 756c 7420 696e 2061  will result in a
-000035d0: 6e20 6572 726f 722e 2229 0a20 2020 2065  n error.").    e
-000035e0: 6c69 6620 6375 7272 5374 6174 655b 2269  lif currState["i
-000035f0: 6e64 6578 6822 5d20 3d3d 2036 3a0a 2020  ndexh"] == 6:.  
-00003600: 2020 2020 2020 7374 2e6d 6172 6b64 6f77        st.markdow
-00003610: 6e28 223a 6172 726f 775f 6c65 6674 3a20  n(":arrow_left: 
-00003620: 4d61 6b65 2073 7572 6520 746f 2061 6464  Make sure to add
-00003630: 2f69 6e63 6c75 6465 2074 6865 2068 6967  /include the hig
-00003640: 686c 6967 6874 2070 6c75 6769 6e20 666f  hlight plugin fo
-00003650: 7220 7379 6e74 6178 2068 6967 686c 6967  r syntax highlig
-00003660: 6874 696e 672e 2022 290a 2020 2020 2020  hting. ").      
-00003670: 2020 7374 2e6d 6172 6b64 6f77 6e28 2246    st.markdown("F
-00003680: 6f72 2069 6e64 6976 6964 7561 6c20 6c69  or individual li
-00003690: 6e65 2068 6967 686c 6967 6874 696e 672c  ne highlighting,
-000036a0: 2061 6464 206c 696e 6520 6e75 6d62 6572   add line number
-000036b0: 7320 2873 6570 6172 6174 6564 2062 7920  s (separated by 
-000036c0: 6120 636f 6d6d 6120 6966 206e 6f74 2063  a comma if not c
-000036d0: 6f6e 7365 6375 7469 7665 2920 7269 6768  onsecutive) righ
-000036e0: 7420 6166 7465 7220 7468 6520 7468 7265  t after the thre
-000036f0: 6520 6261 636b 7469 636b 7320 616e 6420  e backticks and 
-00003700: 7468 6520 7072 6f67 7261 6d6d 696e 6720  the programming 
-00003710: 6c61 6e67 7561 6765 2074 6865 2063 6f64  language the cod
-00003720: 6520 6973 2077 7269 7474 656e 2069 6e2e  e is written in.
-00003730: 2046 6f72 2065 7861 6d70 6c65 2c20 746f   For example, to
-00003740: 2068 6967 686c 6967 6874 206c 696e 6573   highlight lines
-00003750: 2031 2c20 322c 2033 2c20 616e 6420 353a   1, 2, 3, and 5:
-00003760: 2229 0a20 2020 2020 2020 2073 742e 636f  ").        st.co
-00003770: 6465 2822 6060 606a 6176 6173 6372 6970  de("```javascrip
-00003780: 7420 5b31 2d33 2c35 5d22 2c20 6c61 6e67  t [1-3,5]", lang
-00003790: 7561 6765 3d22 6d64 2229 0a20 2020 2020  uage="md").     
-000037a0: 2020 2073 742e 6d61 726b 646f 776e 2822     st.markdown("
-000037b0: 596f 7520 6361 6e20 6561 7369 6c79 2067  You can easily g
-000037c0: 656e 6572 6174 6520 6672 6167 6d65 6e74  enerate fragment
-000037d0: 7320 7468 6174 2073 7465 7020 7468 726f  s that step thro
-000037e0: 7567 6820 6469 6666 6572 656e 7420 6869  ugh different hi
-000037f0: 6768 6c69 6768 7465 6420 6c69 6e65 7320  ghlighted lines 
-00003800: 6f66 2063 6f64 6520 6279 2063 6861 696e  of code by chain
-00003810: 696e 6720 7365 7473 206f 6620 6c69 6e65  ing sets of line
-00003820: 206e 756d 6265 7273 2074 6f67 6574 6865   numbers togethe
-00003830: 7220 7573 696e 6720 6120 607c 6020 6368  r using a `|` ch
-00003840: 6172 6163 7465 722e 2054 6865 2066 6f6c  aracter. The fol
-00003850: 6c6f 7769 6e67 2065 7861 6d70 6c65 2068  lowing example h
-00003860: 6967 686c 6967 6874 7320 6c69 6e65 7320  ighlights lines 
-00003870: 312d 3320 616e 6420 7468 656e 2032 2d34  1-3 and then 2-4
-00003880: 2069 6e20 7468 6520 6e65 7874 2066 7261   in the next fra
-00003890: 676d 656e 743a 2229 0a20 2020 2020 2020  gment:").       
-000038a0: 2073 616d 706c 655f 636f 6465 5f6d 6172   sample_code_mar
-000038b0: 6b64 6f77 6e20 3d20 2260 6060 6a61 7661  kdown = "```java
-000038c0: 7363 7269 7074 205b 312d 337c 322d 345d  script [1-3|2-4]
-000038d0: 220a 2020 2020 2020 2020 7374 2e63 6f64  ".        st.cod
-000038e0: 6528 7361 6d70 6c65 5f63 6f64 655f 6d61  e(sample_code_ma
-000038f0: 726b 646f 776e 2c20 6c61 6e67 7561 6765  rkdown, language
-00003900: 3d22 6d61 726b 646f 776e 2229 0a20 2020  ="markdown").   
-00003910: 2020 2020 2073 742e 6d61 726b 646f 776e       st.markdown
-00003920: 2822 416c 736f 2c20 6d61 6b65 2073 7572  ("Also, make sur
-00003930: 6520 746f 2063 6c6f 7365 2074 6865 2063  e to close the c
-00003940: 6f64 6520 626c 6f63 6b20 7769 7468 2074  ode block with t
-00003950: 6872 6565 206d 6f72 6520 6261 636b 7469  hree more backti
-00003960: 636b 7320 6f6e 2061 6e20 656d 7074 7920  cks on an empty 
-00003970: 6c69 6e65 2061 6674 6572 2074 6865 206c  line after the l
-00003980: 6173 7420 6c69 6e65 206f 6620 636f 6465  ast line of code
-00003990: 2e22 290a 2020 2020 656c 6966 2063 7572  .").    elif cur
-000039a0: 7253 7461 7465 5b22 696e 6465 7868 225d  rState["indexh"]
-000039b0: 203d 3d20 383a 0a20 2020 2020 2020 2073   == 8:.        s
-000039c0: 742e 6d61 726b 646f 776e 2822 416e 7920  t.markdown("Any 
-000039d0: 6f70 7469 6f6e 2074 6861 7420 796f 7520  option that you 
-000039e0: 6361 6e20 7061 7373 2074 6f20 7468 6520  can pass to the 
-000039f0: 6052 6576 6561 6c2e 696e 6974 6961 6c69  `Reveal.initiali
-00003a00: 7a65 6020 616e 6420 6052 6576 6561 6c2e  ze` and `Reveal.
-00003a10: 636f 6e66 6967 7572 6560 2066 756e 6374  configure` funct
-00003a20: 696f 6e73 2063 616e 2062 6520 7061 7373  ions can be pass
-00003a30: 6564 2074 6f20 7468 6520 636f 6d70 6f6e  ed to the compon
-00003a40: 656e 7420 2874 6f20 636f 6e66 6967 7572  ent (to configur
-00003a50: 6520 7468 6520 7072 6573 656e 7461 7469  e the presentati
-00003a60: 6f6e 2920 7669 6120 7468 6520 6063 6f6e  on) via the `con
-00003a70: 6669 6760 2061 7267 756d 656e 7420 6f66  fig` argument of
-00003a80: 2074 6865 2063 6f6d 706f 6e65 6e74 2773   the component's
-00003a90: 2060 736c 6964 6573 6020 6675 6e63 7469   `slides` functi
-00003aa0: 6f6e 2e22 29                             on.")
+00002380: 2020 6865 6967 6874 3d68 6569 6768 742c    height=height,
+00002390: 200a 2020 2020 2320 2020 2020 2020 2020   .    #         
+000023a0: 2020 2020 2020 2020 2020 2074 6865 6d65             theme
+000023b0: 3d74 6865 6d65 2c20 2020 2020 2020 2020  =theme,         
+000023c0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+000023d0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+000023e0: 2020 2020 2063 6f6e 6669 673d 7b0a 2020       config={.  
+000023f0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+00002400: 2020 2020 2020 2020 2020 2020 2277 6964              "wid
+00002410: 7468 223a 2063 6f6e 7465 6e74 5f77 6964  th": content_wid
+00002420: 7468 2c20 0a20 2020 2023 2020 2020 2020  th, .    #      
+00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002440: 2020 2022 6865 6967 6874 223a 2063 6f6e     "height": con
+00002450: 7465 6e74 5f68 6569 6768 742c 200a 2020  tent_height, .  
+00002460: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+00002470: 2020 2020 2020 2020 2020 2020 226d 696e              "min
+00002480: 5363 616c 6522 3a20 7363 616c 655f 7261  Scale": scale_ra
+00002490: 6e67 655b 305d 2c20 0a20 2020 2023 2020  nge[0], .    #  
+000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024b0: 2020 2020 2020 2022 6365 6e74 6572 223a         "center":
+000024c0: 2054 7275 652c 200a 2020 2020 2320 2020   True, .    #   
+000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024e0: 2020 2020 2020 226d 6178 5363 616c 6522        "maxScale"
+000024f0: 3a20 7363 616c 655f 7261 6e67 655b 315d  : scale_range[1]
+00002500: 2c20 0a20 2020 2023 2020 2020 2020 2020  , .    #        
+00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002520: 2022 6d61 7267 696e 223a 206d 6172 6769   "margin": margi
+00002530: 6e2c 200a 2020 2020 2320 2020 2020 2020  n, .    #       
+00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002550: 2020 2270 6c75 6769 6e73 223a 205b 226d    "plugins": ["m
+00002560: 6172 6b64 6f77 6e22 5d0a 2020 2020 2320  arkdown"].    # 
+00002570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002580: 2020 2020 2020 2020 7d2c 2061 6c6c 6f77          }, allow
+00002590: 5f75 6e73 6166 655f 6874 6d6c 3d54 7275  _unsafe_html=Tru
+000025a0: 652c 0a20 2020 2023 2020 2020 2020 2020  e,.    #        
+000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025c0: 206b 6579 3d22 7265 7665 616c 2229 0a20   key="reveal"). 
+000025d0: 2020 2020 200a 2020 2020 2323 204d 6172       .    ## Mar
+000025e0: 6b64 6f77 6e20 6578 616d 706c 650a 2020  kdown example.  
+000025f0: 2020 6375 7272 5374 6174 6520 3d20 736c    currState = sl
+00002600: 6964 6573 2873 616d 706c 655f 6d61 726b  ides(sample_mark
+00002610: 646f 776e 2c20 0a20 2020 2020 2020 2020  down, .         
+00002620: 2020 2020 2020 2020 2020 2020 2020 6865                he
+00002630: 6967 6874 3d68 6569 6768 742c 200a 2020  ight=height, .  
+00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002650: 2020 2020 2074 6865 6d65 3d74 6865 6d65       theme=theme
+00002660: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
+00002670: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00002680: 3d7b 0a20 2020 2020 2020 2020 2020 2020  ={.             
+00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026a0: 2020 2277 6964 7468 223a 2063 6f6e 7465    "width": conte
+000026b0: 6e74 5f77 6964 7468 2c20 0a20 2020 2020  nt_width, .     
+000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026d0: 2020 2020 2020 2020 2020 2268 6569 6768            "heigh
+000026e0: 7422 3a20 636f 6e74 656e 745f 6865 6967  t": content_heig
+000026f0: 6874 2c20 0a20 2020 2020 2020 2020 2020  ht, .           
+00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002710: 2020 2020 226d 696e 5363 616c 6522 3a20      "minScale": 
+00002720: 7363 616c 655f 7261 6e67 655b 305d 2c20  scale_range[0], 
+00002730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002750: 2263 656e 7465 7222 3a20 5472 7565 2c20  "center": True, 
+00002760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002780: 226d 6178 5363 616c 6522 3a20 7363 616c  "maxScale": scal
+00002790: 655f 7261 6e67 655b 315d 2c20 0a20 2020  e_range[1], .   
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027b0: 2020 2020 2020 2020 2020 2020 226d 6172              "mar
+000027c0: 6769 6e22 3a20 6d61 7267 696e 2c20 0a20  gin": margin, . 
+000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027e0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+000027f0: 6c75 6769 6e73 223a 2070 6c75 6769 6e73  lugins": plugins
+00002800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002820: 7d2c 200a 2020 2020 2020 2020 2020 2020  }, .            
+00002830: 2020 2020 2020 2020 2020 2069 6e69 7469             initi
+00002840: 616c 5f73 7461 7465 3d7b 0a20 2020 2020  al_state={.     
+00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 2022 696e 6465 7868 223a 2068 736c 6964   "indexh": hslid
+00002880: 6550 6f73 2c20 0a20 2020 2020 2020 2020  ePos, .         
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2020 2020 2020 2020 2020 2020 2022 696e               "in
+000028b0: 6465 7876 223a 2076 736c 6964 6550 6f73  dexv": vslidePos
+000028c0: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
+000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028e0: 2020 2020 2020 2020 2022 696e 6465 7866           "indexf
+000028f0: 223a 2066 7261 6750 6f73 2c20 0a20 2020  ": fragPos, .   
+00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002920: 2020 2022 7061 7573 6564 223a 2070 6175     "paused": pau
+00002930: 7365 642c 200a 2020 2020 2020 2020 2020  sed, .          
+00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002950: 2020 2020 2020 2020 2020 2020 226f 7665              "ove
+00002960: 7276 6965 7722 3a20 6f76 6572 7669 6577  rview": overview
+00002970: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002990: 2020 2020 2020 2020 7d2c 200a 2020 2020          }, .    
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029b0: 2020 206d 6172 6b64 6f77 6e5f 7072 6f70     markdown_prop
+000029c0: 733d 7b22 6461 7461 2d73 6570 6172 6174  s={"data-separat
+000029d0: 6f72 2d76 6572 7469 6361 6c22 3a22 5e2d  or-vertical":"^-
+000029e0: 2d24 227d 2c20 0a20 2020 2020 2020 2020  -$"}, .         
+000029f0: 2020 2020 2020 2020 2020 2020 2020 6373                cs
+00002a00: 733d 7222 626f 6479 2e72 6576 6561 6c2d  s=r"body.reveal-
+00002a10: 7669 6577 706f 7274 207b 6261 636b 6772  viewport {backgr
+00002a20: 6f75 6e64 2d63 6f6c 6f72 3a20 626c 7565  ound-color: blue
+00002a30: 3b7d 222c 0a20 2020 2020 2020 2020 2020  ;}",.           
+00002a40: 2020 2020 2020 2020 2020 2020 6469 7370              disp
+00002a50: 6c61 795f 6f6e 6c79 3d54 7275 652c 0a20  lay_only=True,. 
+00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a70: 2020 2020 2020 6b65 793d 2272 6576 6561        key="revea
+00002a80: 6c5f 736c 6964 6573 2229 0a0a 2020 2020  l_slides")..    
+00002a90: 6966 2063 7572 7253 7461 7465 5b22 696e  if currState["in
+00002aa0: 6465 7868 225d 203d 3d20 303a 0a20 2020  dexh"] == 0:.   
+00002ab0: 2020 2020 2073 742e 6d61 726b 646f 776e       st.markdown
+00002ac0: 2822 5265 7665 616c 2e6a 7320 6973 2061  ("Reveal.js is a
+00002ad0: 6e20 6f70 656e 2073 6f75 7263 6520 4854  n open source HT
+00002ae0: 4d4c 2070 7265 7365 6e74 6174 696f 6e20  ML presentation 
+00002af0: 6672 616d 6577 6f72 6b2e 2049 7420 656e  framework. It en
+00002b00: 6162 6c65 7320 616e 796f 6e65 2077 6974  ables anyone wit
+00002b10: 6820 6120 7765 6220 6272 6f77 7365 7220  h a web browser 
+00002b20: 746f 2063 7265 6174 6520 6675 6c6c 792d  to create fully-
+00002b30: 6665 6174 7572 6564 2061 6e64 2062 6561  featured and bea
+00002b40: 7574 6966 756c 2070 7265 7365 6e74 6174  utiful presentat
+00002b50: 696f 6e73 2066 6f72 2066 7265 652e 205c  ions for free. \
+00002b60: 6e5c 6e54 6865 2066 7261 6d65 776f 726b  n\nThe framework
+00002b70: 2063 6f6d 6573 2077 6974 6820 6120 6272   comes with a br
+00002b80: 6f61 6420 7261 6e67 6520 6f66 2066 6561  oad range of fea
+00002b90: 7475 7265 7320 696e 636c 7564 696e 6720  tures including 
+00002ba0: 6e65 7374 6564 2073 6c69 6465 732c 204d  nested slides, M
+00002bb0: 6172 6b64 6f77 6e20 7375 7070 6f72 742c  arkdown support,
+00002bc0: 2041 7574 6f2d 416e 696d 6174 652c 2050   Auto-Animate, P
+00002bd0: 4446 2065 7870 6f72 742c 2073 7065 616b  DF export, speak
+00002be0: 6572 206e 6f74 6573 2c20 4c61 5465 5820  er notes, LaTeX 
+00002bf0: 7375 7070 6f72 7420 616e 6420 7379 6e74  support and synt
+00002c00: 6178 2068 6967 686c 6967 6874 6564 2063  ax highlighted c
+00002c10: 6f64 652e 2229 0a20 2020 2065 6c69 6620  ode.").    elif 
+00002c20: 6375 7272 5374 6174 655b 2269 6e64 6578  currState["index
+00002c30: 6822 5d20 3d3d 2032 3a0a 2020 2020 2020  h"] == 2:.      
+00002c40: 2020 6966 2063 7572 7253 7461 7465 5b22    if currState["
+00002c50: 696e 6465 7866 225d 203d 3d20 303a 0a20  indexf"] == 0:. 
+00002c60: 2020 2020 2020 2020 2020 2073 742e 6d61             st.ma
+00002c70: 726b 646f 776e 2822 5f28 7365 6520 6c61  rkdown("_(see la
+00002c80: 7465 7220 736c 6964 6573 2066 6f72 2064  ter slides for d
+00002c90: 6574 6169 6c73 2061 6e64 2065 7861 6d70  etails and examp
+00002ca0: 6c65 7329 5f22 290a 2020 2020 2020 2020  les)_").        
+00002cb0: 656c 6966 2063 7572 7253 7461 7465 5b22  elif currState["
+00002cc0: 696e 6465 7866 225d 203d 3d20 313a 0a20  indexf"] == 1:. 
+00002cd0: 2020 2020 2020 2020 2020 2073 742e 6d61             st.ma
+00002ce0: 726b 646f 776e 2822 2d20 596f 7520 6361  rkdown("- You ca
+00002cf0: 6e20 7377 6970 6520 686f 7269 7a6f 6e74  n swipe horizont
+00002d00: 616c 6c79 206f 7220 7665 7274 6963 616c  ally or vertical
+00002d10: 6c79 2074 6f20 6e61 7669 6761 7465 2074  ly to navigate t
+00002d20: 6872 6f75 6768 2061 2070 7265 7365 6e74  hrough a present
+00002d30: 6174 696f 6e20 6f6e 2061 6e79 2074 6f75  ation on any tou
+00002d40: 6368 2d65 6e61 626c 6564 2064 6576 6963  ch-enabled devic
+00002d50: 652e 205c 6e2d 2059 6f75 2063 616e 2075  e. \n- You can u
+00002d60: 7365 2074 6865 2061 7272 6f77 206b 6579  se the arrow key
+00002d70: 7320 6f6e 2079 6f75 7220 6b65 7962 6f61  s on your keyboa
+00002d80: 7264 2074 6f20 6e61 7669 6761 7465 2061  rd to navigate a
+00002d90: 7320 7765 6c6c 2e20 5c6e 2d20 4e61 7669  s well. \n- Navi
+00002da0: 6761 7469 6e67 2077 6974 6820 7468 6520  gating with the 
+00002db0: 6d6f 7573 6520 6973 2061 7320 7369 6d70  mouse is as simp
+00002dc0: 6c65 2061 7320 636c 6963 6b69 6e67 2074  le as clicking t
+00002dd0: 6865 2064 6972 6563 7469 6f6e 616c 2061  he directional a
+00002de0: 7272 6f77 7320 6e65 6172 2074 6865 2065  rrows near the e
+00002df0: 6467 6573 206f 7220 636f 726e 6572 7320  dges or corners 
+00002e00: 6f66 2074 6865 2073 6c69 6465 732e 2229  of the slides.")
+00002e10: 0a20 2020 2020 2020 2065 6c69 6620 6375  .        elif cu
+00002e20: 7272 5374 6174 655b 2269 6e64 6578 6622  rrState["indexf"
+00002e30: 5d20 3d3d 2032 3a0a 2020 2020 2020 2020  ] == 2:.        
+00002e40: 2020 2020 7374 2e6d 6172 6b64 6f77 6e28      st.markdown(
+00002e50: 222d 2050 7265 7373 2074 6865 2060 4660  "- Press the `F`
+00002e60: 206b 6579 206f 6e20 796f 7572 206b 6579   key on your key
+00002e70: 626f 6172 6420 746f 2065 6e74 6572 2066  board to enter f
+00002e80: 756c 6c2d 7363 7265 656e 206d 6f64 652e  ull-screen mode.
+00002e90: 2050 7265 7373 2060 4553 4360 2074 6f20   Press `ESC` to 
+00002ea0: 6578 6974 2066 756c 6c2d 7363 7265 656e  exit full-screen
+00002eb0: 206d 6f64 652e 205c 6e2d 2050 7265 7373   mode. \n- Press
+00002ec0: 2074 6865 2060 4f60 206f 6620 6045 5343   the `O` of `ESC
+00002ed0: 6020 6b65 7920 746f 2065 6e74 6572 2061  ` key to enter a
+00002ee0: 6e64 2065 7869 7420 6f76 6572 7669 6577  nd exit overview
+00002ef0: 206d 6f64 6522 290a 2020 2020 2020 2020   mode").        
+00002f00: 656c 6966 2063 7572 7253 7461 7465 5b22  elif currState["
+00002f10: 696e 6465 7866 225d 203d 3d20 333a 0a20  indexf"] == 3:. 
+00002f20: 2020 2020 2020 2020 2020 2073 742e 7772             st.wr
+00002f30: 6974 6528 223a 6172 726f 775f 6c65 6674  ite(":arrow_left
+00002f40: 3a20 4d61 6b65 2073 7572 6520 746f 2061  : Make sure to a
+00002f50: 6464 2074 6865 2073 6561 7263 6820 616e  dd the search an
+00002f60: 6420 7a6f 6f6d 2070 6c75 6769 6e73 2074  d zoom plugins t
+00002f70: 6f20 6163 7469 7661 7465 2074 6865 7365  o activate these
+00002f80: 2066 6561 7475 7265 732e 2229 0a20 2020   features.").   
+00002f90: 2020 2020 2020 2020 2073 742e 6d61 726b           st.mark
+00002fa0: 646f 776e 2822 2d20 5072 6573 7320 6043  down("- Press `C
+00002fb0: 7472 6c60 202b 2060 5368 6966 7460 202b  trl` + `Shift` +
+00002fc0: 2060 4660 206b 6579 7320 6f6e 2079 6f75   `F` keys on you
+00002fd0: 7220 6b65 7962 6f61 7264 2074 6f20 6f70  r keyboard to op
+00002fe0: 656e 2061 6e64 2063 6c6f 7365 2074 6865  en and close the
+00002ff0: 2073 6561 7263 6820 6469 616c 6f67 2e20   search dialog. 
+00003000: 5c6e 2d20 5072 6573 7320 7468 6520 6041  \n- Press the `A
+00003010: 6c74 6020 6b65 7920 616e 6420 7269 6768  lt` key and righ
+00003020: 7420 636c 6963 6b20 746f 207a 6f6f 6d20  t click to zoom 
+00003030: 696e 2061 6e64 206f 7574 206f 6e20 7468  in and out on th
+00003040: 6520 7265 6769 6f6e 2074 6865 206d 6f75  e region the mou
+00003050: 7365 2069 7320 686f 7665 7269 6e67 206f  se is hovering o
+00003060: 7665 722e 2229 0a20 2020 2020 2020 2065  ver.").        e
+00003070: 6c69 6620 6375 7272 5374 6174 655b 2269  lif currState["i
+00003080: 6e64 6578 6622 5d20 3d3d 2034 3a0a 2020  ndexf"] == 4:.  
+00003090: 2020 2020 2020 2020 2020 7374 2e6d 6172            st.mar
+000030a0: 6b64 6f77 6e28 225f 2873 6565 206c 6174  kdown("_(see lat
+000030b0: 6572 2073 6c69 6465 7320 666f 7220 6465  er slides for de
+000030c0: 7461 696c 7320 616e 6420 6578 616d 706c  tails and exampl
+000030d0: 6573 295f 2229 0a20 2020 2065 6c69 6620  es)_").    elif 
+000030e0: 6375 7272 5374 6174 655b 2269 6e64 6578  currState["index
+000030f0: 6822 5d20 3d3d 2033 3a0a 2020 2020 2020  h"] == 3:.      
+00003100: 2020 7374 2e6d 6172 6b64 6f77 6e28 2727    st.markdown(''
+00003110: 2754 6869 7320 636f 6d70 6f6e 656e 7420  'This component 
+00003120: 616c 6c6f 7773 2066 6f72 2074 776f 2077  allows for two w
+00003130: 6179 7320 6f66 2063 7265 6174 696e 6720  ays of creating 
+00003140: 7265 7665 616c 2e6a 7320 7072 6573 656e  reveal.js presen
+00003150: 7461 7469 6f6e 732e 205c 6e31 2e20 5b4d  tations. \n1. [M
+00003160: 6172 6b64 6f77 6e5d 2868 7474 7073 3a2f  arkdown](https:/
+00003170: 2f72 6576 6561 6c6a 732e 636f 6d2f 6d61  /revealjs.com/ma
+00003180: 726b 646f 776e 2f29 205c 6e32 2e20 5b4d  rkdown/) \n2. [M
+00003190: 6172 6b75 705d 2868 7474 7073 3a2f 2f72  arkup](https://r
+000031a0: 6576 6561 6c6a 732e 636f 6d2f 6d61 726b  evealjs.com/mark
+000031b0: 7570 2f29 205c 6e5c 6e54 6865 2070 7269  up/) \n\nThe pri
+000031c0: 6d61 7279 2077 6179 2069 7320 7573 696e  mary way is usin
+000031d0: 6720 6d61 726b 646f 776e 2e20 4279 2064  g markdown. By d
+000031e0: 6566 6175 6c74 2c20 7468 6520 636f 6d70  efault, the comp
+000031f0: 6f6e 656e 7420 6073 6c69 6465 6020 6675  onent `slide` fu
+00003200: 6e63 7469 6f6e 2061 6363 6570 7473 2061  nction accepts a
+00003210: 2073 7472 696e 6720 636f 6e74 6169 6e69   string containi
+00003220: 6e67 206d 6172 6b64 6f77 6e20 6173 2069  ng markdown as i
+00003230: 6e70 7574 2e20 4e6f 7465 2074 6861 7420  nput. Note that 
+00003240: 7468 6973 2073 7472 6561 6d6c 6974 2063  this streamlit c
+00003250: 6f6d 706f 6e65 6e74 2074 616b 6573 2063  omponent takes c
+00003260: 6172 6520 6f66 2074 6865 2068 746d 6c20  are of the html 
+00003270: 7461 6773 2028 603c 7365 6374 696f 6e3e  tags (`<section>
+00003280: 602c 2060 3c74 6578 7461 7265 613e 602c  `, `<textarea>`,
+00003290: 2060 3c73 6372 6970 743e 6029 2066 6f72   `<script>`) for
+000032a0: 2079 6f75 2073 6f20 796f 7520 6f6e 6c79   you so you only
+000032b0: 2068 6176 6520 746f 2077 6f72 7279 2061   have to worry a
+000032c0: 626f 7574 2074 6865 206d 6172 6b64 6f77  bout the markdow
+000032d0: 6e20 636f 6e74 656e 742e 2054 6865 2066  n content. The f
+000032e0: 6f6c 6c6f 7769 6e67 2069 7320 7369 6d70  ollowing is simp
+000032f0: 6c65 2065 7861 6d70 6c65 206f 6620 6d61  le example of ma
+00003300: 726b 646f 776e 2066 6f72 2061 2070 7265  rkdown for a pre
+00003310: 7365 6e74 6174 696f 6e20 7769 7468 2074  sentation with t
+00003320: 6872 6565 2073 6c69 6465 733a 2027 2727  hree slides: '''
+00003330: 290a 2020 2020 2020 2020 7361 6d70 6c65  ).        sample
+00003340: 5f6d 6172 6b64 6f77 6e20 3d20 2727 2723  _markdown = '''#
+00003350: 2320 536c 6964 6520 310a 4120 7061 7261  # Slide 1.A para
+00003360: 6772 6170 6820 7769 7468 2073 6f6d 6520  graph with some 
+00003370: 7465 7874 2061 6e64 2061 205b 6c69 6e6b  text and a [link
+00003380: 5d28 6874 7470 733a 2f2f 6861 6b69 6d2e  ](https://hakim.
+00003390: 7365 292e 0a2d 2d2d 0a53 6c69 6465 2032  se)..---.Slide 2
+000033a0: 0a2d 2d2d 0a53 6c69 6465 2033 2727 270a  .---.Slide 3'''.
+000033b0: 2020 2020 2020 2020 7374 2e63 6f64 6528          st.code(
+000033c0: 7361 6d70 6c65 5f6d 6172 6b64 6f77 6e2c  sample_markdown,
+000033d0: 206c 616e 6775 6167 653d 226d 6422 290a   language="md").
+000033e0: 2020 2020 2020 2020 7374 2e6d 6172 6b64          st.markd
+000033f0: 6f77 6e28 2727 2754 6865 2073 6563 6f6e  own('''The secon
+00003400: 6420 7761 7920 6973 2062 7920 7072 6f76  d way is by prov
+00003410: 6964 696e 6720 6120 7374 7269 6e67 2063  iding a string c
+00003420: 6f6e 7461 696e 696e 6720 7468 6520 6d61  ontaining the ma
+00003430: 726b 7570 2074 6861 7420 676f 6573 2069  rkup that goes i
+00003440: 6e73 6964 6520 7468 6520 603c 6469 7620  nside the `<div 
+00003450: 636c 6173 733d 2273 6c69 6465 7322 3e60  class="slides">`
+00003460: 2065 6c65 6d65 6e74 2061 6e64 2073 6574   element and set
+00003470: 7469 6e67 2074 6865 2060 736c 6964 6560  ting the `slide`
+00003480: 2066 756e 6374 696f 6e27 7320 6061 6c6c   function's `all
+00003490: 6f77 5f75 6e73 6166 655f 6874 6d6c 6020  ow_unsafe_html` 
+000034a0: 6172 6775 6d65 6e74 2074 6f20 6054 7275  argument to `Tru
+000034b0: 6560 2e20 5468 6520 6c61 7474 6572 2069  e`. The latter i
+000034c0: 7320 7768 6174 2074 656c 6c73 2074 6865  s what tells the
+000034d0: 2063 6f6d 706f 6e65 6e74 2074 6f20 6578   component to ex
+000034e0: 7065 6374 206d 6172 6b75 7020 696e 7374  pect markup inst
+000034f0: 6561 6420 6f66 206d 6172 6b64 6f77 6e2e  ead of markdown.
+00003500: 2727 2729 0a20 2020 2020 2020 2073 616d  ''').        sam
+00003510: 706c 655f 6874 6d6c 203d 2027 2727 3c64  ple_html = '''<d
+00003520: 6976 2063 6c61 7373 3d22 7265 7665 616c  iv class="reveal
+00003530: 223e 0a20 203c 6469 7620 636c 6173 733d  ">.  <div class=
+00003540: 2273 6c69 6465 7322 3e0a 2020 2020 3c73  "slides">.    <s
+00003550: 6563 7469 6f6e 3e48 6f72 697a 6f6e 7461  ection>Horizonta
+00003560: 6c20 536c 6964 653c 2f73 6563 7469 6f6e  l Slide</section
+00003570: 3e0a 2020 2020 3c73 6563 7469 6f6e 3e0a  >.    <section>.
+00003580: 2020 2020 2020 3c73 6563 7469 6f6e 3e56        <section>V
+00003590: 6572 7469 6361 6c20 536c 6964 6520 313c  ertical Slide 1<
+000035a0: 2f73 6563 7469 6f6e 3e0a 2020 2020 2020  /section>.      
+000035b0: 3c73 6563 7469 6f6e 3e56 6572 7469 6361  <section>Vertica
+000035c0: 6c20 536c 6964 6520 323c 2f73 6563 7469  l Slide 2</secti
+000035d0: 6f6e 3e0a 2020 2020 3c2f 7365 6374 696f  on>.    </sectio
+000035e0: 6e3e 0a20 203c 2f64 6976 3e0a 3c2f 6469  n>.  </div>.</di
+000035f0: 763e 2727 270a 2020 2020 2020 2020 7374  v>'''.        st
+00003600: 2e63 6f64 6528 7361 6d70 6c65 5f68 746d  .code(sample_htm
+00003610: 6c2c 206c 616e 6775 6167 653d 2268 746d  l, language="htm
+00003620: 6c22 290a 2020 2020 2020 2020 7374 2e77  l").        st.w
+00003630: 6172 6e69 6e67 2822 5741 524e 494e 4721  arning("WARNING!
+00003640: 2120 5468 6520 6d61 726b 7570 2079 6f75  ! The markup you
+00003650: 2070 726f 7669 6465 2069 7320 6469 7265   provide is dire
+00003660: 6374 6c79 2069 6e6a 6563 7465 6420 7669  ctly injected vi
+00003670: 6120 7468 6520 6064 616e 6765 726f 7573  a the `dangerous
+00003680: 6c79 5365 7449 6e6e 6572 4854 4d4c 6020  lySetInnerHTML` 
+00003690: 7072 6f70 6572 7479 206f 6620 7468 6520  property of the 
+000036a0: 656e 636c 6f73 696e 6720 6064 6976 602e  enclosing `div`.
+000036b0: 2054 6869 7320 6d65 616e 7320 7468 6174   This means that
+000036c0: 2079 6f75 2061 7265 2072 6573 706f 6e73   you are respons
+000036d0: 6962 6c65 2066 6f72 2065 6e73 7572 696e  ible for ensurin
+000036e0: 6720 7468 6174 2074 6865 206d 6172 6b75  g that the marku
+000036f0: 7020 6973 2073 6166 6520 616e 6420 646f  p is safe and do
+00003700: 6573 206e 6f74 2063 6f6e 7461 696e 2061  es not contain a
+00003710: 6e79 206d 616c 6963 696f 7573 2063 6f64  ny malicious cod
+00003720: 652e 2054 6865 2063 6f6d 706f 6e65 6e74  e. The component
+00003730: 2064 6f65 7320 6e6f 7420 646f 2061 6e79   does not do any
+00003740: 2073 616e 6974 697a 6174 696f 6e20 6f66   sanitization of
+00003750: 2074 6865 206d 6172 6b75 702e 2229 0a20   the markup."). 
+00003760: 2020 2065 6c69 6620 6375 7272 5374 6174     elif currStat
+00003770: 655b 2269 6e64 6578 6822 5d20 3d3d 2034  e["indexh"] == 4
+00003780: 3a0a 2020 2020 2020 2020 7374 2e6d 6172  :.        st.mar
+00003790: 6b64 6f77 6e28 2246 6f72 206d 6f72 6520  kdown("For more 
+000037a0: 6578 616d 706c 6573 206f 6620 6261 636b  examples of back
+000037b0: 6772 6f75 6e64 732c 2073 6565 205b 6865  grounds, see [he
+000037c0: 7265 5d28 6874 7470 733a 2f2f 7265 7665  re](https://reve
+000037d0: 616c 6a73 2e63 6f6d 2f62 6163 6b67 726f  aljs.com/backgro
+000037e0: 756e 6473 2f29 2e22 290a 2020 2020 2020  unds/).").      
+000037f0: 2020 7374 2e6d 6172 6b64 6f77 6e28 2254    st.markdown("T
+00003800: 6f20 6368 616e 6765 2074 6865 2062 6163  o change the bac
+00003810: 6b67 726f 756e 6420 696e 206d 6172 6b64  kground in markd
+00003820: 6f77 6e2c 2061 6464 2061 2063 6f6d 6d65  own, add a comme
+00003830: 6e74 2074 6f20 7468 6520 736c 6964 6520  nt to the slide 
+00003840: 7468 6174 206f 6265 7973 2074 6865 2066  that obeys the f
+00003850: 6f6c 6c6f 7769 6e67 2073 796e 7461 783a  ollowing syntax:
+00003860: 2229 0a20 2020 2020 2020 2073 742e 636f  ").        st.co
+00003870: 6465 2827 3c21 2d2d 202e 736c 6964 653a  de('<!-- .slide:
+00003880: 2064 6174 612d 6261 636b 6772 6f75 6e64   data-background
+00003890: 2d63 6f6c 6f72 3d22 2332 3833 3734 3722  -color="#283747"
+000038a0: 202d 2d3e 272c 206c 616e 6775 6167 653d   -->', language=
+000038b0: 226d 6422 290a 2020 2020 2020 2020 7374  "md").        st
+000038c0: 2e6d 6172 6b64 6f77 6e28 224d 616b 6520  .markdown("Make 
+000038d0: 7375 7265 2074 6f20 6164 6420 616c 6c20  sure to add all 
+000038e0: 7468 6520 6064 6174 612d 6020 6174 7472  the `data-` attr
+000038f0: 6962 7574 6573 2079 6f75 2072 6571 7569  ibutes you requi
+00003900: 7265 2061 6674 6572 2074 6865 2060 2e73  re after the `.s
+00003910: 6c69 6465 3a60 2229 0a20 2020 2065 6c69  lide:`").    eli
+00003920: 6620 6375 7272 5374 6174 655b 2269 6e64  f currState["ind
+00003930: 6578 6822 5d20 3d3d 2035 3a0a 2020 2020  exh"] == 5:.    
+00003940: 2020 2020 7374 2e77 7269 7465 2822 3a61      st.write(":a
+00003950: 7272 6f77 5f6c 6566 743a 204d 616b 6520  rrow_left: Make 
+00003960: 7375 7265 2074 6f20 6164 642f 696e 636c  sure to add/incl
+00003970: 7564 6520 7468 6520 6d61 7468 2070 6c75  ude the math plu
+00003980: 6769 6e20 736f 2074 6861 7420 7468 6520  gin so that the 
+00003990: 6c61 7465 7820 6973 2070 726f 7065 726c  latex is properl
+000039a0: 7920 7072 6f63 6573 7365 6420 616e 6420  y processed and 
+000039b0: 7265 6e64 6572 6564 2e20 5468 6572 6520  rendered. There 
+000039c0: 6172 6520 7468 7265 6520 6275 696c 742d  are three built-
+000039d0: 696e 2070 6c75 6769 6e73 2074 6861 7420  in plugins that 
+000039e0: 7072 6f63 6573 7320 6c61 7465 783a 2229  process latex:")
+000039f0: 0a20 2020 2020 2020 2073 742e 7772 6974  .        st.writ
+00003a00: 6528 2231 2e20 606b 6174 6578 6020 2d20  e("1. `katex` - 
+00003a10: 7573 6573 204b 6154 6558 2074 6f20 7265  uses KaTeX to re
+00003a20: 6e64 6572 206d 6174 6820 6571 7561 7469  nder math equati
+00003a30: 6f6e 732e 205c 6e32 2e20 606d 6174 686a  ons. \n2. `mathj
+00003a40: 6178 3260 202d 2075 7365 7320 4d61 7468  ax2` - uses Math
+00003a50: 4a61 7832 2074 6f20 7265 6e64 6572 206d  Jax2 to render m
+00003a60: 6174 6820 6571 7561 7469 6f6e 732e 205c  ath equations. \
+00003a70: 6e33 2e20 606d 6174 686a 6178 3360 202d  n3. `mathjax3` -
+00003a80: 2075 7365 7320 4d61 7468 4a61 7833 2074   uses MathJax3 t
+00003a90: 6f20 7265 6e64 6572 206d 6174 6820 6571  o render math eq
+00003aa0: 7561 7469 6f6e 732e 2229 0a20 2020 2020  uations.").     
+00003ab0: 2020 2073 742e 7761 726e 696e 6728 2257     st.warning("W
+00003ac0: 4152 4e49 4e47 2121 204f 6e6c 7920 6f6e  ARNING!! Only on
+00003ad0: 6520 6d61 7468 2070 6c75 6769 6e20 6361  e math plugin ca
+00003ae0: 6e20 6265 2075 7365 6420 6174 2061 2074  n be used at a t
+00003af0: 696d 652e 2049 6e63 6c75 6469 6e67 206d  ime. Including m
+00003b00: 6f72 6520 7468 616e 206f 6e65 2070 6c75  ore than one plu
+00003b10: 6769 6e20 7769 6c6c 2072 6573 756c 7420  gin will result 
+00003b20: 696e 2061 6e20 6572 726f 722e 2229 0a20  in an error."). 
+00003b30: 2020 2065 6c69 6620 6375 7272 5374 6174     elif currStat
+00003b40: 655b 2269 6e64 6578 6822 5d20 3d3d 2036  e["indexh"] == 6
+00003b50: 3a0a 2020 2020 2020 2020 7374 2e6d 6172  :.        st.mar
+00003b60: 6b64 6f77 6e28 223a 6172 726f 775f 6c65  kdown(":arrow_le
+00003b70: 6674 3a20 4d61 6b65 2073 7572 6520 746f  ft: Make sure to
+00003b80: 2061 6464 2f69 6e63 6c75 6465 2074 6865   add/include the
+00003b90: 2068 6967 686c 6967 6874 2070 6c75 6769   highlight plugi
+00003ba0: 6e20 666f 7220 7379 6e74 6178 2068 6967  n for syntax hig
+00003bb0: 686c 6967 6874 696e 672e 2022 290a 2020  hlighting. ").  
+00003bc0: 2020 2020 2020 7374 2e6d 6172 6b64 6f77        st.markdow
+00003bd0: 6e28 2246 6f72 2069 6e64 6976 6964 7561  n("For individua
+00003be0: 6c20 6c69 6e65 2068 6967 686c 6967 6874  l line highlight
+00003bf0: 696e 672c 2061 6464 206c 696e 6520 6e75  ing, add line nu
+00003c00: 6d62 6572 7320 2873 6570 6172 6174 6564  mbers (separated
+00003c10: 2062 7920 6120 636f 6d6d 6120 6966 206e   by a comma if n
+00003c20: 6f74 2063 6f6e 7365 6375 7469 7665 2920  ot consecutive) 
+00003c30: 7269 6768 7420 6166 7465 7220 7468 6520  right after the 
+00003c40: 7468 7265 6520 6261 636b 7469 636b 7320  three backticks 
+00003c50: 616e 6420 7468 6520 7072 6f67 7261 6d6d  and the programm
+00003c60: 696e 6720 6c61 6e67 7561 6765 2074 6865  ing language the
+00003c70: 2063 6f64 6520 6973 2077 7269 7474 656e   code is written
+00003c80: 2069 6e2e 2046 6f72 2065 7861 6d70 6c65   in. For example
+00003c90: 2c20 746f 2068 6967 686c 6967 6874 206c  , to highlight l
+00003ca0: 696e 6573 2031 2c20 322c 2033 2c20 616e  ines 1, 2, 3, an
+00003cb0: 6420 353a 2229 0a20 2020 2020 2020 2073  d 5:").        s
+00003cc0: 742e 636f 6465 2822 6060 606a 6176 6173  t.code("```javas
+00003cd0: 6372 6970 7420 5b31 2d33 2c35 5d22 2c20  cript [1-3,5]", 
+00003ce0: 6c61 6e67 7561 6765 3d22 6d64 2229 0a20  language="md"). 
+00003cf0: 2020 2020 2020 2073 742e 6d61 726b 646f         st.markdo
+00003d00: 776e 2822 596f 7520 6361 6e20 6561 7369  wn("You can easi
+00003d10: 6c79 2067 656e 6572 6174 6520 6672 6167  ly generate frag
+00003d20: 6d65 6e74 7320 7468 6174 2073 7465 7020  ments that step 
+00003d30: 7468 726f 7567 6820 6469 6666 6572 656e  through differen
+00003d40: 7420 6869 6768 6c69 6768 7465 6420 6c69  t highlighted li
+00003d50: 6e65 7320 6f66 2063 6f64 6520 6279 2063  nes of code by c
+00003d60: 6861 696e 696e 6720 7365 7473 206f 6620  haining sets of 
+00003d70: 6c69 6e65 206e 756d 6265 7273 2074 6f67  line numbers tog
+00003d80: 6574 6865 7220 7573 696e 6720 6120 607c  ether using a `|
+00003d90: 6020 6368 6172 6163 7465 722e 2054 6865  ` character. The
+00003da0: 2066 6f6c 6c6f 7769 6e67 2065 7861 6d70   following examp
+00003db0: 6c65 2068 6967 686c 6967 6874 7320 6c69  le highlights li
+00003dc0: 6e65 7320 312d 3320 616e 6420 7468 656e  nes 1-3 and then
+00003dd0: 2032 2d34 2069 6e20 7468 6520 6e65 7874   2-4 in the next
+00003de0: 2066 7261 676d 656e 743a 2229 0a20 2020   fragment:").   
+00003df0: 2020 2020 2073 616d 706c 655f 636f 6465       sample_code
+00003e00: 5f6d 6172 6b64 6f77 6e20 3d20 2260 6060  _markdown = "```
+00003e10: 6a61 7661 7363 7269 7074 205b 312d 337c  javascript [1-3|
+00003e20: 322d 345d 220a 2020 2020 2020 2020 7374  2-4]".        st
+00003e30: 2e63 6f64 6528 7361 6d70 6c65 5f63 6f64  .code(sample_cod
+00003e40: 655f 6d61 726b 646f 776e 2c20 6c61 6e67  e_markdown, lang
+00003e50: 7561 6765 3d22 6d61 726b 646f 776e 2229  uage="markdown")
+00003e60: 0a20 2020 2020 2020 2073 742e 6d61 726b  .        st.mark
+00003e70: 646f 776e 2822 416c 736f 2c20 6d61 6b65  down("Also, make
+00003e80: 2073 7572 6520 746f 2063 6c6f 7365 2074   sure to close t
+00003e90: 6865 2063 6f64 6520 626c 6f63 6b20 7769  he code block wi
+00003ea0: 7468 2074 6872 6565 206d 6f72 6520 6261  th three more ba
+00003eb0: 636b 7469 636b 7320 6f6e 2061 6e20 656d  ckticks on an em
+00003ec0: 7074 7920 6c69 6e65 2061 6674 6572 2074  pty line after t
+00003ed0: 6865 206c 6173 7420 6c69 6e65 206f 6620  he last line of 
+00003ee0: 636f 6465 2e22 290a 2020 2020 656c 6966  code.").    elif
+00003ef0: 2063 7572 7253 7461 7465 5b22 696e 6465   currState["inde
+00003f00: 7868 225d 203d 3d20 383a 0a20 2020 2020  xh"] == 8:.     
+00003f10: 2020 2073 742e 6d61 726b 646f 776e 2822     st.markdown("
+00003f20: 416e 7920 6f70 7469 6f6e 2074 6861 7420  Any option that 
+00003f30: 796f 7520 6361 6e20 7061 7373 2074 6f20  you can pass to 
+00003f40: 7468 6520 6052 6576 6561 6c2e 696e 6974  the `Reveal.init
+00003f50: 6961 6c69 7a65 6020 616e 6420 6052 6576  ialize` and `Rev
+00003f60: 6561 6c2e 636f 6e66 6967 7572 6560 2066  eal.configure` f
+00003f70: 756e 6374 696f 6e73 2063 616e 2062 6520  unctions can be 
+00003f80: 7061 7373 6564 2074 6f20 7468 6520 636f  passed to the co
+00003f90: 6d70 6f6e 656e 7420 2874 6f20 636f 6e66  mponent (to conf
+00003fa0: 6967 7572 6520 7468 6520 7072 6573 656e  igure the presen
+00003fb0: 7461 7469 6f6e 2920 7669 6120 7468 6520  tation) via the 
+00003fc0: 6063 6f6e 6669 6760 2061 7267 756d 656e  `config` argumen
+00003fd0: 7420 6f66 2074 6865 2063 6f6d 706f 6e65  t of the compone
+00003fe0: 6e74 2773 2060 736c 6964 6573 6020 6675  nt's `slides` fu
+00003ff0: 6e63 7469 6f6e 2e22 29                   nction.")
```

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/asset-manifest.json` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/asset-manifest.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6233211233211233%*

 * *Differences: {"'entrypoints'": "{insert: [(0, 'static/js/runtime-main.887ff237.js'), (2, "*

 * *                  "'static/js/2.971d039e.chunk.js'), (3, 'static/js/main.18f5a848.chunk.js')], "*

 * *                  'delete: [3, 2, 0]}',*

 * * "'files'": "{'main.js': './static/js/main.18f5a848.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.18f5a848.chunk.js.map', 'runtime-main.js': "*

 * *            "'./static/js/runtime-main.887ff237.js', 'runtime-main.js.map': "*

 * *            "'./static/js/runtime-main.887ff237.js.map', 'stati […]*

```diff
@@ -1,20 +1,20 @@
 {
     "entrypoints": [
-        "static/js/runtime-main.eaac28ce.js",
+        "static/js/runtime-main.887ff237.js",
         "static/css/2.5029ddca.chunk.css",
-        "static/js/2.5c1e1a04.chunk.js",
-        "static/js/main.639deb8d.chunk.js"
+        "static/js/2.971d039e.chunk.js",
+        "static/js/main.18f5a848.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.639deb8d.chunk.js",
-        "main.js.map": "./static/js/main.639deb8d.chunk.js.map",
-        "runtime-main.js": "./static/js/runtime-main.eaac28ce.js",
-        "runtime-main.js.map": "./static/js/runtime-main.eaac28ce.js.map",
+        "main.js": "./static/js/main.18f5a848.chunk.js",
+        "main.js.map": "./static/js/main.18f5a848.chunk.js.map",
+        "runtime-main.js": "./static/js/runtime-main.887ff237.js",
+        "runtime-main.js.map": "./static/js/runtime-main.887ff237.js.map",
         "static/css/10.1f3244e3.chunk.css": "./static/css/10.1f3244e3.chunk.css",
         "static/css/10.1f3244e3.chunk.css.map": "./static/css/10.1f3244e3.chunk.css.map",
         "static/css/11.cb699f02.chunk.css": "./static/css/11.cb699f02.chunk.css",
         "static/css/11.cb699f02.chunk.css.map": "./static/css/11.cb699f02.chunk.css.map",
         "static/css/12.158b51eb.chunk.css": "./static/css/12.158b51eb.chunk.css",
         "static/css/12.158b51eb.chunk.css.map": "./static/css/12.158b51eb.chunk.css.map",
         "static/css/13.74908590.chunk.css": "./static/css/13.74908590.chunk.css",
@@ -43,48 +43,48 @@
         "static/css/6.1b9cee33.chunk.css.map": "./static/css/6.1b9cee33.chunk.css.map",
         "static/css/7.4e275de2.chunk.css": "./static/css/7.4e275de2.chunk.css",
         "static/css/7.4e275de2.chunk.css.map": "./static/css/7.4e275de2.chunk.css.map",
         "static/css/8.eb5abf62.chunk.css": "./static/css/8.eb5abf62.chunk.css",
         "static/css/8.eb5abf62.chunk.css.map": "./static/css/8.eb5abf62.chunk.css.map",
         "static/css/9.1253a161.chunk.css": "./static/css/9.1253a161.chunk.css",
         "static/css/9.1253a161.chunk.css.map": "./static/css/9.1253a161.chunk.css.map",
-        "static/js/10.18fc5a6d.chunk.js": "./static/js/10.18fc5a6d.chunk.js",
-        "static/js/10.18fc5a6d.chunk.js.map": "./static/js/10.18fc5a6d.chunk.js.map",
-        "static/js/11.e2b8452b.chunk.js": "./static/js/11.e2b8452b.chunk.js",
-        "static/js/11.e2b8452b.chunk.js.map": "./static/js/11.e2b8452b.chunk.js.map",
-        "static/js/12.6c6d4448.chunk.js": "./static/js/12.6c6d4448.chunk.js",
-        "static/js/12.6c6d4448.chunk.js.map": "./static/js/12.6c6d4448.chunk.js.map",
-        "static/js/13.c5f703d1.chunk.js": "./static/js/13.c5f703d1.chunk.js",
-        "static/js/13.c5f703d1.chunk.js.map": "./static/js/13.c5f703d1.chunk.js.map",
-        "static/js/14.39efed4e.chunk.js": "./static/js/14.39efed4e.chunk.js",
-        "static/js/14.39efed4e.chunk.js.map": "./static/js/14.39efed4e.chunk.js.map",
-        "static/js/15.7665d197.chunk.js": "./static/js/15.7665d197.chunk.js",
-        "static/js/15.7665d197.chunk.js.map": "./static/js/15.7665d197.chunk.js.map",
-        "static/js/16.4a5a2671.chunk.js": "./static/js/16.4a5a2671.chunk.js",
-        "static/js/16.4a5a2671.chunk.js.map": "./static/js/16.4a5a2671.chunk.js.map",
-        "static/js/17.e0e3c073.chunk.js": "./static/js/17.e0e3c073.chunk.js",
-        "static/js/17.e0e3c073.chunk.js.map": "./static/js/17.e0e3c073.chunk.js.map",
-        "static/js/18.b265fc2b.chunk.js": "./static/js/18.b265fc2b.chunk.js",
-        "static/js/18.b265fc2b.chunk.js.map": "./static/js/18.b265fc2b.chunk.js.map",
-        "static/js/19.5ba3da56.chunk.js": "./static/js/19.5ba3da56.chunk.js",
-        "static/js/19.5ba3da56.chunk.js.map": "./static/js/19.5ba3da56.chunk.js.map",
-        "static/js/2.5c1e1a04.chunk.js": "./static/js/2.5c1e1a04.chunk.js",
-        "static/js/2.5c1e1a04.chunk.js.LICENSE.txt": "./static/js/2.5c1e1a04.chunk.js.LICENSE.txt",
-        "static/js/2.5c1e1a04.chunk.js.map": "./static/js/2.5c1e1a04.chunk.js.map",
-        "static/js/3.d30f1cfd.chunk.js": "./static/js/3.d30f1cfd.chunk.js",
-        "static/js/3.d30f1cfd.chunk.js.map": "./static/js/3.d30f1cfd.chunk.js.map",
-        "static/js/4.ec7a53ea.chunk.js": "./static/js/4.ec7a53ea.chunk.js",
-        "static/js/4.ec7a53ea.chunk.js.map": "./static/js/4.ec7a53ea.chunk.js.map",
-        "static/js/5.e42b3133.chunk.js": "./static/js/5.e42b3133.chunk.js",
-        "static/js/5.e42b3133.chunk.js.map": "./static/js/5.e42b3133.chunk.js.map",
-        "static/js/6.e9192981.chunk.js": "./static/js/6.e9192981.chunk.js",
-        "static/js/6.e9192981.chunk.js.map": "./static/js/6.e9192981.chunk.js.map",
-        "static/js/7.be794506.chunk.js": "./static/js/7.be794506.chunk.js",
-        "static/js/7.be794506.chunk.js.map": "./static/js/7.be794506.chunk.js.map",
-        "static/js/8.15dd3b20.chunk.js": "./static/js/8.15dd3b20.chunk.js",
-        "static/js/8.15dd3b20.chunk.js.map": "./static/js/8.15dd3b20.chunk.js.map",
-        "static/js/9.119f08fa.chunk.js": "./static/js/9.119f08fa.chunk.js",
-        "static/js/9.119f08fa.chunk.js.map": "./static/js/9.119f08fa.chunk.js.map",
+        "static/js/10.442a54e9.chunk.js": "./static/js/10.442a54e9.chunk.js",
+        "static/js/10.442a54e9.chunk.js.map": "./static/js/10.442a54e9.chunk.js.map",
+        "static/js/11.6dd2762e.chunk.js": "./static/js/11.6dd2762e.chunk.js",
+        "static/js/11.6dd2762e.chunk.js.map": "./static/js/11.6dd2762e.chunk.js.map",
+        "static/js/12.b5132789.chunk.js": "./static/js/12.b5132789.chunk.js",
+        "static/js/12.b5132789.chunk.js.map": "./static/js/12.b5132789.chunk.js.map",
+        "static/js/13.155b252b.chunk.js": "./static/js/13.155b252b.chunk.js",
+        "static/js/13.155b252b.chunk.js.map": "./static/js/13.155b252b.chunk.js.map",
+        "static/js/14.124342a7.chunk.js": "./static/js/14.124342a7.chunk.js",
+        "static/js/14.124342a7.chunk.js.map": "./static/js/14.124342a7.chunk.js.map",
+        "static/js/15.1df3933b.chunk.js": "./static/js/15.1df3933b.chunk.js",
+        "static/js/15.1df3933b.chunk.js.map": "./static/js/15.1df3933b.chunk.js.map",
+        "static/js/16.e98baccf.chunk.js": "./static/js/16.e98baccf.chunk.js",
+        "static/js/16.e98baccf.chunk.js.map": "./static/js/16.e98baccf.chunk.js.map",
+        "static/js/17.f47ed1b3.chunk.js": "./static/js/17.f47ed1b3.chunk.js",
+        "static/js/17.f47ed1b3.chunk.js.map": "./static/js/17.f47ed1b3.chunk.js.map",
+        "static/js/18.bbe30a24.chunk.js": "./static/js/18.bbe30a24.chunk.js",
+        "static/js/18.bbe30a24.chunk.js.map": "./static/js/18.bbe30a24.chunk.js.map",
+        "static/js/19.63982437.chunk.js": "./static/js/19.63982437.chunk.js",
+        "static/js/19.63982437.chunk.js.map": "./static/js/19.63982437.chunk.js.map",
+        "static/js/2.971d039e.chunk.js": "./static/js/2.971d039e.chunk.js",
+        "static/js/2.971d039e.chunk.js.LICENSE.txt": "./static/js/2.971d039e.chunk.js.LICENSE.txt",
+        "static/js/2.971d039e.chunk.js.map": "./static/js/2.971d039e.chunk.js.map",
+        "static/js/3.a17c1b63.chunk.js": "./static/js/3.a17c1b63.chunk.js",
+        "static/js/3.a17c1b63.chunk.js.map": "./static/js/3.a17c1b63.chunk.js.map",
+        "static/js/4.c8e4936c.chunk.js": "./static/js/4.c8e4936c.chunk.js",
+        "static/js/4.c8e4936c.chunk.js.map": "./static/js/4.c8e4936c.chunk.js.map",
+        "static/js/5.ab74786f.chunk.js": "./static/js/5.ab74786f.chunk.js",
+        "static/js/5.ab74786f.chunk.js.map": "./static/js/5.ab74786f.chunk.js.map",
+        "static/js/6.7f9bbd64.chunk.js": "./static/js/6.7f9bbd64.chunk.js",
+        "static/js/6.7f9bbd64.chunk.js.map": "./static/js/6.7f9bbd64.chunk.js.map",
+        "static/js/7.887bb0a8.chunk.js": "./static/js/7.887bb0a8.chunk.js",
+        "static/js/7.887bb0a8.chunk.js.map": "./static/js/7.887bb0a8.chunk.js.map",
+        "static/js/8.0121e917.chunk.js": "./static/js/8.0121e917.chunk.js",
+        "static/js/8.0121e917.chunk.js.map": "./static/js/8.0121e917.chunk.js.map",
+        "static/js/9.e6c78b5a.chunk.js": "./static/js/9.e6c78b5a.chunk.js",
+        "static/js/9.e6c78b5a.chunk.js.map": "./static/js/9.e6c78b5a.chunk.js.map",
         "static/media/solarized.css": "./static/media/league-gothic.6ae91382.ttf",
         "static/media/white_contrast_compact_verbatim_headers.css": "./static/media/source-sans-pro-semibolditalic.fb03c660.eot"
     }
 }
```

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/bootstrap.min.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/index.html` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/2.5029ddca.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root" class="reveal"></div><script>!function(e){function t(t){for(var n,o,c=t[0],i=t[1],f=t[2],l=0,d=[];l<c.length;l++)o=c[l],Object.prototype.hasOwnProperty.call(a,o)&&a[o]&&d.push(a[o][0]),a[o]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(s&&s(t);d.length;)d.shift()();return u.push.apply(u,f||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,o=1;o<r.length;o++){var i=r[o];0!==a[i]&&(n=!1)}n&&(u.splice(t--,1),e=c(c.s=r[0]))}return e}var n={},o={1:0},a={1:0},u=[];function c(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,c),r.l=!0,r.exports}c.e=function(e){var t=[];o[e]?t.push(o[e]):0!==o[e]&&{3:1,4:1,5:1,6:1,7:1,8:1,9:1,10:1,11:1,12:1,13:1,14:1,15:1,16:1,17:1,18:1,19:1}[e]&&t.push(o[e]=new Promise((function(t,r){for(var n="static/css/"+({}[e]||e)+"."+{3:"11f8848d",4:"2fe0cb1b",5:"5a2b8ee3",6:"1b9cee33",7:"4e275de2",8:"eb5abf62",9:"1253a161",10:"1f3244e3",11:"cb699f02",12:"158b51eb",13:"74908590",14:"e64fc659",15:"3adba626",16:"b573d318",17:"10a8300f",18:"4eb3e38a",19:"74b97645"}[e]+".chunk.css",a=c.p+n,u=document.getElementsByTagName("link"),i=0;i<u.length;i++){var f=(s=u[i]).getAttribute("data-href")||s.getAttribute("href");if("stylesheet"===s.rel&&(f===n||f===a))return t()}var l=document.getElementsByTagName("style");for(i=0;i<l.length;i++){var s;if((f=(s=l[i]).getAttribute("data-href"))===n||f===a)return t()}var d=document.createElement("link");d.rel="stylesheet",d.type="text/css",d.onload=t,d.onerror=function(t){var n=t&&t.target&&t.target.src||a,u=new Error("Loading CSS chunk "+e+" failed.\n("+n+")");u.code="CSS_CHUNK_LOAD_FAILED",u.request=n,delete o[e],d.parentNode.removeChild(d),r(u)},d.href=a,document.getElementsByTagName("head")[0].appendChild(d)})).then((function(){o[e]=0})));var r=a[e];if(0!==r)if(r)t.push(r[2]);else{var n=new Promise((function(t,n){r=a[e]=[t,n]}));t.push(r[2]=n);var u,i=document.createElement("script");i.charset="utf-8",i.timeout=120,c.nc&&i.setAttribute("nonce",c.nc),i.src=function(e){return c.p+"static/js/"+({}[e]||e)+"."+{3:"d30f1cfd",4:"ec7a53ea",5:"e42b3133",6:"e9192981",7:"be794506",8:"15dd3b20",9:"119f08fa",10:"18fc5a6d",11:"e2b8452b",12:"6c6d4448",13:"c5f703d1",14:"39efed4e",15:"7665d197",16:"4a5a2671",17:"e0e3c073",18:"b265fc2b",19:"5ba3da56"}[e]+".chunk.js"}(e);var f=new Error;u=function(t){i.onerror=i.onload=null,clearTimeout(l);var r=a[e];if(0!==r){if(r){var n=t&&("load"===t.type?"missing":t.type),o=t&&t.target&&t.target.src;f.message="Loading chunk "+e+" failed.\n("+n+": "+o+")",f.name="ChunkLoadError",f.type=n,f.request=o,r[1](f)}a[e]=void 0}};var l=setTimeout((function(){u({type:"timeout",target:i})}),12e4);i.onerror=i.onload=u,document.head.appendChild(i)}return Promise.all(t)},c.m=e,c.c=n,c.d=function(e,t,r){c.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},c.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},c.t=function(e,t){if(1&t&&(e=c(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(c.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)c.d(r,n,function(t){return e[t]}.bind(null,n));return r},c.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return c.d(t,"a",t),t},c.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},c.p="./",c.oe=function(e){throw console.error(e),e};var i=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],f=i.push.bind(i);i.push=t,i=i.slice();for(var l=0;l<i.length;l++)t(i[l]);var s=f;r()}([])</script><script src="./static/js/2.5c1e1a04.chunk.js"></script><script src="./static/js/main.639deb8d.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/2.5029ddca.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root" class="reveal"></div><script>!function(e){function t(t){for(var n,o,c=t[0],i=t[1],l=t[2],f=0,d=[];f<c.length;f++)o=c[f],Object.prototype.hasOwnProperty.call(a,o)&&a[o]&&d.push(a[o][0]),a[o]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(s&&s(t);d.length;)d.shift()();return u.push.apply(u,l||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,o=1;o<r.length;o++){var i=r[o];0!==a[i]&&(n=!1)}n&&(u.splice(t--,1),e=c(c.s=r[0]))}return e}var n={},o={1:0},a={1:0},u=[];function c(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,c),r.l=!0,r.exports}c.e=function(e){var t=[];o[e]?t.push(o[e]):0!==o[e]&&{3:1,4:1,5:1,6:1,7:1,8:1,9:1,10:1,11:1,12:1,13:1,14:1,15:1,16:1,17:1,18:1,19:1}[e]&&t.push(o[e]=new Promise((function(t,r){for(var n="static/css/"+({}[e]||e)+"."+{3:"11f8848d",4:"2fe0cb1b",5:"5a2b8ee3",6:"1b9cee33",7:"4e275de2",8:"eb5abf62",9:"1253a161",10:"1f3244e3",11:"cb699f02",12:"158b51eb",13:"74908590",14:"e64fc659",15:"3adba626",16:"b573d318",17:"10a8300f",18:"4eb3e38a",19:"74b97645"}[e]+".chunk.css",a=c.p+n,u=document.getElementsByTagName("link"),i=0;i<u.length;i++){var l=(s=u[i]).getAttribute("data-href")||s.getAttribute("href");if("stylesheet"===s.rel&&(l===n||l===a))return t()}var f=document.getElementsByTagName("style");for(i=0;i<f.length;i++){var s;if((l=(s=f[i]).getAttribute("data-href"))===n||l===a)return t()}var d=document.createElement("link");d.rel="stylesheet",d.type="text/css",d.onload=t,d.onerror=function(t){var n=t&&t.target&&t.target.src||a,u=new Error("Loading CSS chunk "+e+" failed.\n("+n+")");u.code="CSS_CHUNK_LOAD_FAILED",u.request=n,delete o[e],d.parentNode.removeChild(d),r(u)},d.href=a,document.getElementsByTagName("head")[0].appendChild(d)})).then((function(){o[e]=0})));var r=a[e];if(0!==r)if(r)t.push(r[2]);else{var n=new Promise((function(t,n){r=a[e]=[t,n]}));t.push(r[2]=n);var u,i=document.createElement("script");i.charset="utf-8",i.timeout=120,c.nc&&i.setAttribute("nonce",c.nc),i.src=function(e){return c.p+"static/js/"+({}[e]||e)+"."+{3:"a17c1b63",4:"c8e4936c",5:"ab74786f",6:"7f9bbd64",7:"887bb0a8",8:"0121e917",9:"e6c78b5a",10:"442a54e9",11:"6dd2762e",12:"b5132789",13:"155b252b",14:"124342a7",15:"1df3933b",16:"e98baccf",17:"f47ed1b3",18:"bbe30a24",19:"63982437"}[e]+".chunk.js"}(e);var l=new Error;u=function(t){i.onerror=i.onload=null,clearTimeout(f);var r=a[e];if(0!==r){if(r){var n=t&&("load"===t.type?"missing":t.type),o=t&&t.target&&t.target.src;l.message="Loading chunk "+e+" failed.\n("+n+": "+o+")",l.name="ChunkLoadError",l.type=n,l.request=o,r[1](l)}a[e]=void 0}};var f=setTimeout((function(){u({type:"timeout",target:i})}),12e4);i.onerror=i.onload=u,document.head.appendChild(i)}return Promise.all(t)},c.m=e,c.c=n,c.d=function(e,t,r){c.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},c.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},c.t=function(e,t){if(1&t&&(e=c(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(c.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)c.d(r,n,function(t){return e[t]}.bind(null,n));return r},c.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return c.d(t,"a",t),t},c.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},c.p="./",c.oe=function(e){throw console.error(e),e};var i=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],l=i.push.bind(i);i.push=t,i=i.slice();for(var f=0;f<i.length;f++)t(i[f]);var s=l;r()}([])</script><script src="./static/js/2.971d039e.chunk.js"></script><script src="./static/js/main.18f5a848.chunk.js"></script></body></html>
```

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/10.1f3244e3.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/11.cb699f02.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/12.158b51eb.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/13.74908590.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/13.74908590.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/13.74908590.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/14.e64fc659.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/15.3adba626.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/16.b573d318.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/17.10a8300f.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/18.4eb3e38a.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/19.74b97645.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/2.5029ddca.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/3.11f8848d.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/4.2fe0cb1b.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/5.5a2b8ee3.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/2.971d039e.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 2.5c1e1a04.chunk.js.LICENSE.txt */
+/*! For license information please see 2.971d039e.chunk.js.LICENSE.txt */
 (this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || []).push([
     [2],
     [function(e, t, n) {
         "use strict";
 
         function r(e, t) {
             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
@@ -435,15 +435,15 @@
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
     }, function(e, t, n) {
         "use strict";
-        e.exports = n(43)
+        e.exports = n(44)
     }, function(e, t, n) {
         "use strict";
         var r = n(2),
             i = n(4),
             a = n(3),
             o = n(5),
             s = n(0),
@@ -3441,15 +3441,15 @@
                 enumerable: !0,
                 configurable: !0,
                 writable: !0
             }) : e[t] = n, e
         }
     }, function(e, t, n) {
         "use strict";
-        e.exports = n(69)
+        e.exports = n(70)
     }, function(e, t, n) {
         "use strict";
         n.d(t, "b", (function() {
             return pc
         })), n.d(t, "a", (function() {
             return lc
         }));
@@ -21137,15 +21137,15 @@
                         if (u) throw o
                     }
                 }
             }
         }, e.exports.__esModule = !0, e.exports.default = e.exports
     }, function(e, t, n) {
         "use strict";
-        e.exports = n(47)
+        e.exports = n(48)
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return i
         }));
         var r = n(11);
 
@@ -21159,17 +21159,17 @@
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return ("string" === t ? String : Number)(e)
             }(e, "string");
             return "symbol" === Object(r.a)(t) ? t : String(t)
         }
     }, function(e, t, n) {
-        var r = n(65).default,
+        var r = n(66).default,
             i = n(17).default,
-            a = n(66).default,
+            a = n(67).default,
             o = n(30).default,
             s = n(28).default,
             u = ["local", "version", "extensions"];
         e.exports = function() {
             "use strict";
             var e = function() {
                     var e, t = {
@@ -21350,18 +21350,18 @@
             if (e) {
                 if ("string" === typeof e) return r(e, t);
                 var n = Object.prototype.toString.call(e).slice(8, -1);
                 return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? r(e, t) : void 0
             }
         }, e.exports.__esModule = !0, e.exports.default = e.exports
     }, function(e, t, n) {
-        var r = n(51),
-            i = n(52),
+        var r = n(52),
+            i = n(53),
             a = n(21),
-            o = n(53);
+            o = n(54);
         e.exports = function(e, t) {
             return r(e) || i(e, t) || a(e, t) || o()
         }, e.exports.__esModule = !0, e.exports.default = e.exports
     }, function(e, t) {
         e.exports = function(e, t) {
             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
         }, e.exports.__esModule = !0, e.exports.default = e.exports
@@ -21433,15 +21433,15 @@
                     o = r(n);
                     for (var c = 0; c < o.length; c++) a.call(n, o[c]) && (s[o[c]] = n[o[c]])
                 }
             }
             return s
         }
     }, function(e, t, n) {
-        var r = n(48);
+        var r = n(49);
 
         function i(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
@@ -21458,21 +21458,21 @@
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }, e.exports.__esModule = !0, e.exports.default = e.exports
     }, function(e, t, n) {
         var r = n(16).default,
-            i = n(49);
+            i = n(50);
         e.exports = function(e) {
             var t = i(e, "string");
             return "symbol" === r(t) ? t : String(t)
         }, e.exports.__esModule = !0, e.exports.default = e.exports
     }, function(e, t, n) {
-        var r = n(50);
+        var r = n(51);
         e.exports = function(e, t) {
             if (null == e) return {};
             var n, i, a = r(e, t);
             if (Object.getOwnPropertySymbols) {
                 var o = Object.getOwnPropertySymbols(e);
                 for (i = 0; i < o.length; i++) n = o[i], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (a[n] = e[n])
             }
@@ -21506,22 +21506,50 @@
         "use strict";
         ! function e() {
             if ("undefined" !== typeof __REACT_DEVTOOLS_GLOBAL_HOOK__ && "function" === typeof __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE) try {
                 __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE(e)
             } catch (t) {
                 console.error(t)
             }
-        }(), e.exports = n(44)
+        }(), e.exports = n(45)
+    }, function(e, t, n) {
+        "use strict";
+        var r = n(6),
+            i = n.n(r),
+            a = Object.assign || function(e) {
+                for (var t = 1; t < arguments.length; t++) {
+                    var n = arguments[t];
+                    for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
+                }
+                return e
+            };
+        t.a = function(e) {
+            var t = e.html,
+                n = function(e, t) {
+                    var n = {};
+                    for (var r in e) t.indexOf(r) >= 0 || Object.prototype.hasOwnProperty.call(e, r) && (n[r] = e[r]);
+                    return n
+                }(e, ["html"]),
+                o = Object(r.useRef)(null);
+            return Object(r.useEffect)((function() {
+                if (t) {
+                    var e = document.createRange().createContextualFragment(t);
+                    o.current.innerHTML = "", o.current.appendChild(e)
+                }
+            }), [t]), i.a.createElement("div", a({}, n, {
+                ref: o
+            }))
+        }
     }, function(e, t, n) {
         var r = n(17).default,
-            i = n(54).default,
+            i = n(55).default,
             a = n(22).default,
-            o = n(57).default,
-            s = n(58).default,
-            u = n(61).default,
+            o = n(58).default,
+            s = n(59).default,
+            u = n(62).default,
             l = n(23).default,
             c = n(24).default;
         e.exports = function() {
             "use strict";
             var e = {
                 exports: {}
             };
@@ -38189,18 +38217,18 @@
         (function(e) {
             n.d(t, "a", (function() {
                 return Fe
             }));
             var r = n(18),
                 i = n(6),
                 a = n.n(i),
-                o = n(40),
+                o = n(41),
                 s = n.n(o),
-                u = n(41),
-                l = n(42),
+                u = n(42),
+                l = n(43),
                 c = n(26),
                 d = n(13),
                 p = n.n(d);
 
             function _() {
                 return (_ = Object.assign || function(e) {
                     for (var t = 1; t < arguments.length; t++) {
@@ -38974,15 +39002,15 @@
                     return this.sealed ? T(2) : a.a.createElement(ue, {
                         sheet: this.instance
                     }, e)
                 }, t.interleaveWithNodeStream = function(e) {
                     return T(3)
                 }
             }()
-        }).call(this, n(70))
+        }).call(this, n(71))
     }, function(e, t) {
         e.exports = function(e, t, n, r) {
             var i = n ? n.call(r, e, t) : void 0;
             if (void 0 !== i) return !!i;
             if (e === t) return !0;
             if ("object" !== typeof e || !e || "object" !== typeof t || !t) return !1;
             var a = Object.keys(e),
@@ -39776,15 +39804,15 @@
         }, t.useState = function(e) {
             return G().useState(e)
         }, t.version = "16.14.0"
     }, function(e, t, n) {
         "use strict";
         var r = n(6),
             i = n(27),
-            a = n(45);
+            a = n(46);
 
         function o(e) {
             for (var t = "https://reactjs.org/docs/error-decoder.html?invariant=" + e, n = 1; n < arguments.length; n++) t += "&args[]=" + encodeURIComponent(arguments[n]);
             return "Minified React error #" + e + "; visit " + t + " for the full message or use the non-minified dev environment for full errors and additional helpful warnings."
         }
         if (!r) throw Error(o(227));
 
@@ -45015,15 +45043,15 @@
         }, t.unstable_renderSubtreeIntoContainer = function(e, t, n, r) {
             if (!il(n)) throw Error(o(200));
             if (null == e || void 0 === e._reactInternalFiber) throw Error(o(38));
             return al(e, t, n, !1, r)
         }, t.version = "16.14.0"
     }, function(e, t, n) {
         "use strict";
-        e.exports = n(46)
+        e.exports = n(47)
     }, function(e, t, n) {
         "use strict";
         var r, i, a, o, s;
         if ("undefined" === typeof window || "function" !== typeof MessageChannel) {
             var u = null,
                 l = null,
                 c = function e() {
@@ -45426,16 +45454,16 @@
     }, function(e, t) {
         e.exports = function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }, e.exports.__esModule = !0, e.exports.default = e.exports
     }, function(e, t, n) {
         var r = n(32),
             i = n(25),
-            a = n(55),
-            o = n(56);
+            a = n(56),
+            o = n(57);
 
         function s(t) {
             var n = "function" === typeof Map ? new Map : void 0;
             return e.exports = s = function(e) {
                 if (null === e || !a(e)) return e;
                 if ("function" !== typeof e) throw new TypeError("Super expression must either be null or a function");
                 if ("undefined" !== typeof n) {
@@ -45487,44 +45515,44 @@
             }), Object.defineProperty(e, "prototype", {
                 writable: !1
             }), t && r(e, t)
         }, e.exports.__esModule = !0, e.exports.default = e.exports
     }, function(e, t, n) {
         var r = n(32),
             i = n(33),
-            a = n(59);
+            a = n(60);
         e.exports = function(e) {
             var t = i();
             return function() {
                 var n, i = r(e);
                 if (t) {
                     var o = r(this).constructor;
                     n = Reflect.construct(i, arguments, o)
                 } else n = i.apply(this, arguments);
                 return a(this, n)
             }
         }, e.exports.__esModule = !0, e.exports.default = e.exports
     }, function(e, t, n) {
         var r = n(16).default,
-            i = n(60);
+            i = n(61);
         e.exports = function(e, t) {
             if (t && ("object" === r(t) || "function" === typeof t)) return t;
             if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
             return i(e)
         }, e.exports.__esModule = !0, e.exports.default = e.exports
     }, function(e, t) {
         e.exports = function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }, e.exports.__esModule = !0, e.exports.default = e.exports
     }, function(e, t, n) {
-        var r = n(62),
-            i = n(63),
+        var r = n(63),
+            i = n(64),
             a = n(21),
-            o = n(64);
+            o = n(65);
         e.exports = function(e) {
             return r(e) || i(e) || a(e) || o()
         }, e.exports.__esModule = !0, e.exports.default = e.exports
     }, function(e, t, n) {
         var r = n(31);
         e.exports = function(e) {
             if (Array.isArray(e)) return r(e)
@@ -46014,8 +46042,8 @@
         }, i.chdir = function(e) {
             throw new Error("process.chdir is not supported")
         }, i.umask = function() {
             return 0
         }
     }]
 ]);
-//# sourceMappingURL=2.5c1e1a04.chunk.js.map
+//# sourceMappingURL=2.971d039e.chunk.js.map
```

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.LICENSE.txt` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/2.971d039e.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/2.971d039e.chunk.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8564523727033935%*

 * *Differences: {"'file'": "'static/js/2.971d039e.chunk.js'",*

 * * "'mappings'": "';0IAAe,SAASA,EAAgBC,EAAUC,GAChD,KAAMD,aAAoBC,GACxB,MAAM,IAAIC,UAAU,oCAExB,CAJA,iC,+BCAA,8CACA,SAASC,EAAkBC,EAAQC,GACjC,IAAK,IAAIC,EAAI,EAAGA,EAAID,EAAME,OAAQD,IAAK,CACrC,IAAIE,EAAaH,EAAMC,GACvBE,EAAWC,WAAaD,EAAWC,aAAc,EACjDD,EAAWE,cAAe,EACtB,UAAWF,IAAYA,EAAWG,UAAW,GACjDC,OAAOC,eAAeT,EAAQ,YAAcI,EAAWM,KAAMN,EAC/D,CACF,CACe,SAASO,EAAad,EAAae,EAAYC,GAM5D,OALID,GAAYb,EAAkBF,EAAYiB,UAAWF,GACrDC,GAAad,EAAkBF,EAAagB,GAChDL,OAAOC,eAAeZ,EAAa,YAAa,CAC9CU,U […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/2.5c1e1a04.chunk.js",
+    "file": "static/js/2.971d039e.chunk.js",
     "names": [
         "_classCallCheck",
         "instance",
         "Constructor",
         "TypeError",
         "_defineProperties",
         "target",
@@ -3350,14 +3350,22 @@
         "test3",
         "letter",
         "shouldUseNative",
         "toObject",
         "objectWithoutPropertiesLoose",
         "checkDCE",
         "__REACT_DEVTOOLS_GLOBAL_HOOK__",
+        "objectWithoutProperties",
+        "divRef",
+        "useRef",
+        "slotHtml",
+        "createRange",
+        "createContextualFragment",
+        "_extends",
+        "ref",
         "Set",
         "isFrozen",
         "isMatchIgnored",
         "scope",
         "sublanguage",
         "language",
         "classPrefix",
@@ -3846,15 +3854,14 @@
         "attrs",
         "parentComponentId",
         "shouldForwardProp",
         "componentStyle",
         "foldedComponentIds",
         "$as",
         "as",
-        "ref",
         "forwardRef",
         "withComponent",
         "_foldedDefaultProps",
         "withConfig",
         "createStyles",
         "removeStyles",
         "renderStyles",
@@ -3960,15 +3967,14 @@
         "useContext",
         "useDebugValue",
         "useEffect",
         "useImperativeHandle",
         "useLayoutEffect",
         "useMemo",
         "useReducer",
-        "useRef",
         "useState",
         "onError",
         "extractEvents",
         "eventTypes",
         "phasedRegistrationNames",
         "registrationName",
         "stateNode",
@@ -4610,15 +4616,14 @@
         "firstSuspendedTime",
         "rangeCount",
         "wb",
         "activeElementDetached",
         "focusedElem",
         "selectionRange",
         "Tj",
-        "createRange",
         "setStart",
         "removeAllRanges",
         "addRange",
         "setEnd",
         "vb",
         "Uj",
         "Vj",
@@ -4941,14 +4946,15 @@
         "../node_modules/@babel/runtime/helpers/objectSpread2.js",
         "../node_modules/@babel/runtime/helpers/toPropertyKey.js",
         "../node_modules/@babel/runtime/helpers/objectWithoutProperties.js",
         "../node_modules/@babel/runtime/helpers/arrayLikeToArray.js",
         "../node_modules/@babel/runtime/helpers/getPrototypeOf.js",
         "../node_modules/@babel/runtime/helpers/isNativeReflectConstruct.js",
         "../node_modules/react-dom/index.js",
+        "../../src/index.js",
         "../node_modules/reveal.js/plugin/highlight/highlight.js",
         "../node_modules/reveal.js/plugin/search/search.js",
         "../node_modules/reveal.js/plugin/notes/notes.js",
         "../node_modules/reveal.js/plugin/zoom/zoom.js",
         "../../src/utils/interleave.js",
         "../../src/utils/isPlainObject.js",
         "../../src/utils/empties.js",
@@ -5214,14 +5220,15 @@
         "var defineProperty = require(\"./defineProperty.js\");\nfunction ownKeys(object, enumerableOnly) {\n  var keys = Object.keys(object);\n  if (Object.getOwnPropertySymbols) {\n    var symbols = Object.getOwnPropertySymbols(object);\n    enumerableOnly && (symbols = symbols.filter(function (sym) {\n      return Object.getOwnPropertyDescriptor(object, sym).enumerable;\n    })), keys.push.apply(keys, symbols);\n  }\n  return keys;\n}\nfunction _objectSpread2(target) {\n  for (var i = 1; i < arguments.length; i++) {\n    var source = null != arguments[i] ? arguments[i] : {};\n    i % 2 ? ownKeys(Object(source), !0).forEach(function (key) {\n      defineProperty(target, key, source[key]);\n    }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)) : ownKeys(Object(source)).forEach(function (key) {\n      Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key));\n    });\n  }\n  return target;\n}\nmodule.exports = _objectSpread2, module.exports.__esModule = true, module.exports[\"default\"] = module.exports;",
         "var _typeof = require(\"./typeof.js\")[\"default\"];\nvar toPrimitive = require(\"./toPrimitive.js\");\nfunction _toPropertyKey(arg) {\n  var key = toPrimitive(arg, \"string\");\n  return _typeof(key) === \"symbol\" ? key : String(key);\n}\nmodule.exports = _toPropertyKey, module.exports.__esModule = true, module.exports[\"default\"] = module.exports;",
         "var objectWithoutPropertiesLoose = require(\"./objectWithoutPropertiesLoose.js\");\nfunction _objectWithoutProperties(source, excluded) {\n  if (source == null) return {};\n  var target = objectWithoutPropertiesLoose(source, excluded);\n  var key, i;\n  if (Object.getOwnPropertySymbols) {\n    var sourceSymbolKeys = Object.getOwnPropertySymbols(source);\n    for (i = 0; i < sourceSymbolKeys.length; i++) {\n      key = sourceSymbolKeys[i];\n      if (excluded.indexOf(key) >= 0) continue;\n      if (!Object.prototype.propertyIsEnumerable.call(source, key)) continue;\n      target[key] = source[key];\n    }\n  }\n  return target;\n}\nmodule.exports = _objectWithoutProperties, module.exports.__esModule = true, module.exports[\"default\"] = module.exports;",
         "function _arrayLikeToArray(arr, len) {\n  if (len == null || len > arr.length) len = arr.length;\n  for (var i = 0, arr2 = new Array(len); i < len; i++) arr2[i] = arr[i];\n  return arr2;\n}\nmodule.exports = _arrayLikeToArray, module.exports.__esModule = true, module.exports[\"default\"] = module.exports;",
         "function _getPrototypeOf(o) {\n  module.exports = _getPrototypeOf = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function _getPrototypeOf(o) {\n    return o.__proto__ || Object.getPrototypeOf(o);\n  }, module.exports.__esModule = true, module.exports[\"default\"] = module.exports;\n  return _getPrototypeOf(o);\n}\nmodule.exports = _getPrototypeOf, module.exports.__esModule = true, module.exports[\"default\"] = module.exports;",
         "function _isNativeReflectConstruct() {\n  if (typeof Reflect === \"undefined\" || !Reflect.construct) return false;\n  if (Reflect.construct.sham) return false;\n  if (typeof Proxy === \"function\") return true;\n  try {\n    Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function () {}));\n    return true;\n  } catch (e) {\n    return false;\n  }\n}\nmodule.exports = _isNativeReflectConstruct, module.exports.__esModule = true, module.exports[\"default\"] = module.exports;",
         "'use strict';\n\nfunction checkDCE() {\n  /* global __REACT_DEVTOOLS_GLOBAL_HOOK__ */\n  if (\n    typeof __REACT_DEVTOOLS_GLOBAL_HOOK__ === 'undefined' ||\n    typeof __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE !== 'function'\n  ) {\n    return;\n  }\n  if (process.env.NODE_ENV !== 'production') {\n    // This branch is unreachable because this function is only called\n    // in production, but the condition is true only in development.\n    // Therefore if the branch is still here, dead code elimination wasn't\n    // properly applied.\n    // Don't change the message. React DevTools relies on it. Also make sure\n    // this message doesn't occur elsewhere in this function, or it will cause\n    // a false positive.\n    throw new Error('^_^');\n  }\n  try {\n    // Verify that the code above has been dead code eliminated (DCE'd).\n    __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE(checkDCE);\n  } catch (err) {\n    // DevTools shouldn't crash React, no matter what.\n    // We should still report in case we break this code.\n    console.error(err);\n  }\n}\n\nif (process.env.NODE_ENV === 'production') {\n  // DCE check should happen before ReactDOM bundle executes so that\n  // DevTools can report bad minification during injection.\n  checkDCE();\n  module.exports = require('./cjs/react-dom.production.min.js');\n} else {\n  module.exports = require('./cjs/react-dom.development.js');\n}\n",
+        "import React, { useEffect, useRef } from 'react'\n\nfunction DangerouslySetHtmlContent(props) {\n  const { html, ...rest } = props\n  const divRef = useRef(null)\n\n  useEffect(() => {\n    if (!html) return\n\n    const slotHtml = document.createRange().createContextualFragment(html) // Create a 'tiny' document and parse the html string\n    divRef.current.innerHTML = '' // Clear the container\n    divRef.current.appendChild(slotHtml) // Append the new content\n  }, [html])\n\n\n  return (\n    <div {...rest} ref={divRef}></div>\n  )\n}\n\nexport default DangerouslySetHtmlContent\n",
         "!function(e,t){\"object\"==typeof exports&&\"undefined\"!=typeof module?module.exports=t():\"function\"==typeof define&&define.amd?define(t):(e=\"undefined\"!=typeof globalThis?globalThis:e||self).RevealSearch=t()}(this,(function(){\"use strict\";\n/*!\n\t * Handles finding a text string anywhere in the slides and showing the next occurrence to the user\n\t * by navigatating to that slide and highlighting it.\n\t *\n\t * @author Jon Snyder <snyder.jon@gmail.com>, February 2013\n\t */return()=>{let e,t,n,l,o,i,r;function s(){t=document.createElement(\"div\"),t.classList.add(\"searchbox\"),t.style.position=\"absolute\",t.style.top=\"10px\",t.style.right=\"10px\",t.style.zIndex=10,t.innerHTML='<input type=\"search\" class=\"searchinput\" placeholder=\"Search...\" style=\"vertical-align: top;\"/>\\n\\t\\t</span>',n=t.querySelector(\".searchinput\"),n.style.width=\"240px\",n.style.fontSize=\"14px\",n.style.padding=\"4px 6px\",n.style.color=\"#000\",n.style.background=\"#fff\",n.style.borderRadius=\"2px\",n.style.border=\"0\",n.style.outline=\"0\",n.style.boxShadow=\"0 2px 18px rgba(0, 0, 0, 0.2)\",n.style[\"-webkit-appearance\"]=\"none\",e.getRevealElement().appendChild(t),n.addEventListener(\"keyup\",(function(t){if(13===t.keyCode)t.preventDefault(),function(){if(i){var t=n.value;\"\"===t?(r&&r.remove(),l=null):(r=new c(\"slidecontent\"),l=r.apply(t),o=0)}l&&(l.length&&l.length<=o&&(o=0),l.length>o&&(e.slide(l[o].h,l[o].v),o++))}(),i=!1;else i=!0}),!1),d()}function a(){t||s(),t.style.display=\"inline\",n.focus(),n.select()}function d(){t||s(),t.style.display=\"none\",r&&r.remove()}function c(t,n){var l=document.getElementById(t)||document.body,o=n||\"EM\",i=new RegExp(\"^(?:\"+o+\"|SCRIPT|FORM)$\"),r=[\"#ff6\",\"#a0ffff\",\"#9f9\",\"#f99\",\"#f6f\"],s=[],a=0,d=\"\",c=[];this.setRegex=function(e){e=e.replace(/^[^\\w]+|[^\\w]+$/g,\"\").replace(/[^\\w'-]+/g,\"|\"),d=new RegExp(\"(\"+e+\")\",\"i\")},this.getRegex=function(){return d.toString().replace(/^\\/\\\\b\\(|\\)\\\\b\\/i$/g,\"\").replace(/\\|/g,\" \")},this.hiliteWords=function(t){if(null!=t&&t&&d&&!i.test(t.nodeName)){if(t.hasChildNodes())for(var n=0;n<t.childNodes.length;n++)this.hiliteWords(t.childNodes[n]);var l,f;if(3==t.nodeType)if((l=t.nodeValue)&&(f=d.exec(l))){for(var p=t;null!=p&&\"SECTION\"!=p.nodeName;)p=p.parentNode;var u=e.getIndices(p),h=c.length,y=!1;for(n=0;n<h;n++)c[n].h===u.h&&c[n].v===u.v&&(y=!0);y||c.push(u),s[f[0].toLowerCase()]||(s[f[0].toLowerCase()]=r[a++%r.length]);var g=document.createElement(o);g.appendChild(document.createTextNode(f[0])),g.style.backgroundColor=s[f[0].toLowerCase()],g.style.fontStyle=\"inherit\",g.style.color=\"#000\";var v=t.splitText(f.index);v.nodeValue=v.nodeValue.substring(f[0].length),t.parentNode.insertBefore(g,v)}}},this.remove=function(){for(var e,t=document.getElementsByTagName(o);t.length&&(e=t[0]);)e.parentNode.replaceChild(e.firstChild,e)},this.apply=function(e){if(null!=e&&e)return this.remove(),this.setRegex(e),this.hiliteWords(l),c}}return{id:\"search\",init:n=>{e=n,e.registerKeyboardShortcut(\"CTRL + Shift + F\",\"Search\"),document.addEventListener(\"keydown\",(function(e){\"F\"==e.key&&(e.ctrlKey||e.metaKey)&&(e.preventDefault(),t||s(),\"inline\"!==t.style.display?a():d())}),!1)},open:a}}}));\n",
         "!function(t,e){\"object\"==typeof exports&&\"undefined\"!=typeof module?module.exports=e():\"function\"==typeof define&&define.amd?define(e):(t=\"undefined\"!=typeof globalThis?globalThis:t||self).RevealNotes=e()}(this,(function(){\"use strict\";function t(){return{baseUrl:null,breaks:!1,extensions:null,gfm:!0,headerIds:!0,headerPrefix:\"\",highlight:null,langPrefix:\"language-\",mangle:!0,pedantic:!1,renderer:null,sanitize:!1,sanitizer:null,silent:!1,smartLists:!1,smartypants:!1,tokenizer:null,walkTokens:null,xhtml:!1}}let e={baseUrl:null,breaks:!1,extensions:null,gfm:!0,headerIds:!0,headerPrefix:\"\",highlight:null,langPrefix:\"language-\",mangle:!0,pedantic:!1,renderer:null,sanitize:!1,sanitizer:null,silent:!1,smartLists:!1,smartypants:!1,tokenizer:null,walkTokens:null,xhtml:!1};const n=/[&<>\"']/,i=/[&<>\"']/g,s=/[<>\"']|&(?!#?\\w+;)/,r=/[<>\"']|&(?!#?\\w+;)/g,a={\"&\":\"&amp;\",\"<\":\"&lt;\",\">\":\"&gt;\",'\"':\"&quot;\",\"'\":\"&#39;\"},l=t=>a[t];function o(t,e){if(e){if(n.test(t))return t.replace(i,l)}else if(s.test(t))return t.replace(r,l);return t}const c=/&(#(?:\\d+)|(?:#x[0-9A-Fa-f]+)|(?:\\w+));?/gi;function p(t){return t.replace(c,((t,e)=>\"colon\"===(e=e.toLowerCase())?\":\":\"#\"===e.charAt(0)?\"x\"===e.charAt(1)?String.fromCharCode(parseInt(e.substring(2),16)):String.fromCharCode(+e.substring(1)):\"\"))}const u=/(^|[^\\[])\\^/g;function d(t,e){t=t.source||t,e=e||\"\";const n={replace:(e,i)=>(i=(i=i.source||i).replace(u,\"$1\"),t=t.replace(e,i),n),getRegex:()=>new RegExp(t,e)};return n}const h=/[^\\w:]/g,g=/^$|^[a-z][a-z0-9+.-]*:|^[?#]/i;function m(t,e,n){if(t){let t;try{t=decodeURIComponent(p(n)).replace(h,\"\").toLowerCase()}catch(t){return null}if(0===t.indexOf(\"javascript:\")||0===t.indexOf(\"vbscript:\")||0===t.indexOf(\"data:\"))return null}e&&!g.test(n)&&(n=function(t,e){f[\" \"+t]||(k.test(t)?f[\" \"+t]=t+\"/\":f[\" \"+t]=S(t,\"/\",!0));t=f[\" \"+t];const n=-1===t.indexOf(\":\");return\"//\"===e.substring(0,2)?n?e:t.replace(w,\"$1\")+e:\"/\"===e.charAt(0)?n?e:t.replace(x,\"$1\")+e:t+e}(e,n));try{n=encodeURI(n).replace(/%25/g,\"%\")}catch(t){return null}return n}const f={},k=/^[^:]+:\\/*[^/]*$/,w=/^([^:]+:)[\\s\\S]*$/,x=/^([^:]+:\\/*[^/]*)[\\s\\S]*$/;const b={exec:function(){}};function y(t){let e,n,i=1;for(;i<arguments.length;i++)for(n in e=arguments[i],e)Object.prototype.hasOwnProperty.call(e,n)&&(t[n]=e[n]);return t}function v(t,e){const n=t.replace(/\\|/g,((t,e,n)=>{let i=!1,s=e;for(;--s>=0&&\"\\\\\"===n[s];)i=!i;return i?\"|\":\" |\"})).split(/ \\|/);let i=0;if(n[0].trim()||n.shift(),n.length>0&&!n[n.length-1].trim()&&n.pop(),n.length>e)n.splice(e);else for(;n.length<e;)n.push(\"\");for(;i<n.length;i++)n[i]=n[i].trim().replace(/\\\\\\|/g,\"|\");return n}function S(t,e,n){const i=t.length;if(0===i)return\"\";let s=0;for(;s<i;){const r=t.charAt(i-s-1);if(r!==e||n){if(r===e||!n)break;s++}else s++}return t.substr(0,i-s)}function T(t){t&&t.sanitize&&!t.silent&&console.warn(\"marked(): sanitize and sanitizer parameters are deprecated since version 0.7.0, should not be used and will be removed in the future. Read more here: https://marked.js.org/#/USING_ADVANCED.md#options\")}function _(t,e){if(e<1)return\"\";let n=\"\";for(;e>1;)1&e&&(n+=t),e>>=1,t+=t;return n+t}function z(t,e,n,i){const s=e.href,r=e.title?o(e.title):null,a=t[1].replace(/\\\\([\\[\\]])/g,\"$1\");if(\"!\"!==t[0].charAt(0)){i.state.inLink=!0;const t={type:\"link\",raw:n,href:s,title:r,text:a,tokens:i.inlineTokens(a,[])};return i.state.inLink=!1,t}return{type:\"image\",raw:n,href:s,title:r,text:o(a)}}class A{constructor(t){this.options=t||e}space(t){const e=this.rules.block.newline.exec(t);if(e&&e[0].length>0)return{type:\"space\",raw:e[0]}}code(t){const e=this.rules.block.code.exec(t);if(e){const t=e[0].replace(/^ {1,4}/gm,\"\");return{type:\"code\",raw:e[0],codeBlockStyle:\"indented\",text:this.options.pedantic?t:S(t,\"\\n\")}}}fences(t){const e=this.rules.block.fences.exec(t);if(e){const t=e[0],n=function(t,e){const n=t.match(/^(\\s+)(?:```)/);if(null===n)return e;const i=n[1];return e.split(\"\\n\").map((t=>{const e=t.match(/^\\s+/);if(null===e)return t;const[n]=e;return n.length>=i.length?t.slice(i.length):t})).join(\"\\n\")}(t,e[3]||\"\");return{type:\"code\",raw:t,lang:e[2]?e[2].trim():e[2],text:n}}}heading(t){const e=this.rules.block.heading.exec(t);if(e){let t=e[2].trim();if(/#$/.test(t)){const e=S(t,\"#\");this.options.pedantic?t=e.trim():e&&!/ $/.test(e)||(t=e.trim())}const n={type:\"heading\",raw:e[0],depth:e[1].length,text:t,tokens:[]};return this.lexer.inline(n.text,n.tokens),n}}hr(t){const e=this.rules.block.hr.exec(t);if(e)return{type:\"hr\",raw:e[0]}}blockquote(t){const e=this.rules.block.blockquote.exec(t);if(e){const t=e[0].replace(/^ *> ?/gm,\"\");return{type:\"blockquote\",raw:e[0],tokens:this.lexer.blockTokens(t,[]),text:t}}}list(t){let e=this.rules.block.list.exec(t);if(e){let n,i,s,r,a,l,o,c,p,u,d,h,g=e[1].trim();const m=g.length>1,f={type:\"list\",raw:\"\",ordered:m,start:m?+g.slice(0,-1):\"\",loose:!1,items:[]};g=m?`\\\\d{1,9}\\\\${g.slice(-1)}`:`\\\\${g}`,this.options.pedantic&&(g=m?g:\"[*+-]\");const k=new RegExp(`^( {0,3}${g})((?: [^\\\\n]*)?(?:\\\\n|$))`);for(;t&&(h=!1,e=k.exec(t))&&!this.rules.block.hr.test(t);){if(n=e[0],t=t.substring(n.length),c=e[2].split(\"\\n\",1)[0],p=t.split(\"\\n\",1)[0],this.options.pedantic?(r=2,d=c.trimLeft()):(r=e[2].search(/[^ ]/),r=r>4?1:r,d=c.slice(r),r+=e[1].length),l=!1,!c&&/^ *$/.test(p)&&(n+=p+\"\\n\",t=t.substring(p.length+1),h=!0),!h){const e=new RegExp(`^ {0,${Math.min(3,r-1)}}(?:[*+-]|\\\\d{1,9}[.)])`);for(;t&&(u=t.split(\"\\n\",1)[0],c=u,this.options.pedantic&&(c=c.replace(/^ {1,4}(?=( {4})*[^ ])/g,\"  \")),!e.test(c));){if(c.search(/[^ ]/)>=r||!c.trim())d+=\"\\n\"+c.slice(r);else{if(l)break;d+=\"\\n\"+c}l||c.trim()||(l=!0),n+=u+\"\\n\",t=t.substring(u.length+1)}}f.loose||(o?f.loose=!0:/\\n *\\n *$/.test(n)&&(o=!0)),this.options.gfm&&(i=/^\\[[ xX]\\] /.exec(d),i&&(s=\"[ ] \"!==i[0],d=d.replace(/^\\[[ xX]\\] +/,\"\"))),f.items.push({type:\"list_item\",raw:n,task:!!i,checked:s,loose:!1,text:d}),f.raw+=n}f.items[f.items.length-1].raw=n.trimRight(),f.items[f.items.length-1].text=d.trimRight(),f.raw=f.raw.trimRight();const w=f.items.length;for(a=0;a<w;a++){this.lexer.state.top=!1,f.items[a].tokens=this.lexer.blockTokens(f.items[a].text,[]);const t=f.items[a].tokens.filter((t=>\"space\"===t.type)),e=t.every((t=>{const e=t.raw.split(\"\");let n=0;for(const t of e)if(\"\\n\"===t&&(n+=1),n>1)return!0;return!1}));!f.loose&&t.length&&e&&(f.loose=!0,f.items[a].loose=!0)}return f}}html(t){const e=this.rules.block.html.exec(t);if(e){const t={type:\"html\",raw:e[0],pre:!this.options.sanitizer&&(\"pre\"===e[1]||\"script\"===e[1]||\"style\"===e[1]),text:e[0]};return this.options.sanitize&&(t.type=\"paragraph\",t.text=this.options.sanitizer?this.options.sanitizer(e[0]):o(e[0]),t.tokens=[],this.lexer.inline(t.text,t.tokens)),t}}def(t){const e=this.rules.block.def.exec(t);if(e){e[3]&&(e[3]=e[3].substring(1,e[3].length-1));return{type:\"def\",tag:e[1].toLowerCase().replace(/\\s+/g,\" \"),raw:e[0],href:e[2],title:e[3]}}}table(t){const e=this.rules.block.table.exec(t);if(e){const t={type:\"table\",header:v(e[1]).map((t=>({text:t}))),align:e[2].replace(/^ *|\\| *$/g,\"\").split(/ *\\| */),rows:e[3]&&e[3].trim()?e[3].replace(/\\n[ \\t]*$/,\"\").split(\"\\n\"):[]};if(t.header.length===t.align.length){t.raw=e[0];let n,i,s,r,a=t.align.length;for(n=0;n<a;n++)/^ *-+: *$/.test(t.align[n])?t.align[n]=\"right\":/^ *:-+: *$/.test(t.align[n])?t.align[n]=\"center\":/^ *:-+ *$/.test(t.align[n])?t.align[n]=\"left\":t.align[n]=null;for(a=t.rows.length,n=0;n<a;n++)t.rows[n]=v(t.rows[n],t.header.length).map((t=>({text:t})));for(a=t.header.length,i=0;i<a;i++)t.header[i].tokens=[],this.lexer.inlineTokens(t.header[i].text,t.header[i].tokens);for(a=t.rows.length,i=0;i<a;i++)for(r=t.rows[i],s=0;s<r.length;s++)r[s].tokens=[],this.lexer.inlineTokens(r[s].text,r[s].tokens);return t}}}lheading(t){const e=this.rules.block.lheading.exec(t);if(e){const t={type:\"heading\",raw:e[0],depth:\"=\"===e[2].charAt(0)?1:2,text:e[1],tokens:[]};return this.lexer.inline(t.text,t.tokens),t}}paragraph(t){const e=this.rules.block.paragraph.exec(t);if(e){const t={type:\"paragraph\",raw:e[0],text:\"\\n\"===e[1].charAt(e[1].length-1)?e[1].slice(0,-1):e[1],tokens:[]};return this.lexer.inline(t.text,t.tokens),t}}text(t){const e=this.rules.block.text.exec(t);if(e){const t={type:\"text\",raw:e[0],text:e[0],tokens:[]};return this.lexer.inline(t.text,t.tokens),t}}escape(t){const e=this.rules.inline.escape.exec(t);if(e)return{type:\"escape\",raw:e[0],text:o(e[1])}}tag(t){const e=this.rules.inline.tag.exec(t);if(e)return!this.lexer.state.inLink&&/^<a /i.test(e[0])?this.lexer.state.inLink=!0:this.lexer.state.inLink&&/^<\\/a>/i.test(e[0])&&(this.lexer.state.inLink=!1),!this.lexer.state.inRawBlock&&/^<(pre|code|kbd|script)(\\s|>)/i.test(e[0])?this.lexer.state.inRawBlock=!0:this.lexer.state.inRawBlock&&/^<\\/(pre|code|kbd|script)(\\s|>)/i.test(e[0])&&(this.lexer.state.inRawBlock=!1),{type:this.options.sanitize?\"text\":\"html\",raw:e[0],inLink:this.lexer.state.inLink,inRawBlock:this.lexer.state.inRawBlock,text:this.options.sanitize?this.options.sanitizer?this.options.sanitizer(e[0]):o(e[0]):e[0]}}link(t){const e=this.rules.inline.link.exec(t);if(e){const t=e[2].trim();if(!this.options.pedantic&&/^</.test(t)){if(!/>$/.test(t))return;const e=S(t.slice(0,-1),\"\\\\\");if((t.length-e.length)%2==0)return}else{const t=function(t,e){if(-1===t.indexOf(e[1]))return-1;const n=t.length;let i=0,s=0;for(;s<n;s++)if(\"\\\\\"===t[s])s++;else if(t[s]===e[0])i++;else if(t[s]===e[1]&&(i--,i<0))return s;return-1}(e[2],\"()\");if(t>-1){const n=(0===e[0].indexOf(\"!\")?5:4)+e[1].length+t;e[2]=e[2].substring(0,t),e[0]=e[0].substring(0,n).trim(),e[3]=\"\"}}let n=e[2],i=\"\";if(this.options.pedantic){const t=/^([^'\"]*[^\\s])\\s+(['\"])(.*)\\2/.exec(n);t&&(n=t[1],i=t[3])}else i=e[3]?e[3].slice(1,-1):\"\";return n=n.trim(),/^</.test(n)&&(n=this.options.pedantic&&!/>$/.test(t)?n.slice(1):n.slice(1,-1)),z(e,{href:n?n.replace(this.rules.inline._escapes,\"$1\"):n,title:i?i.replace(this.rules.inline._escapes,\"$1\"):i},e[0],this.lexer)}}reflink(t,e){let n;if((n=this.rules.inline.reflink.exec(t))||(n=this.rules.inline.nolink.exec(t))){let t=(n[2]||n[1]).replace(/\\s+/g,\" \");if(t=e[t.toLowerCase()],!t||!t.href){const t=n[0].charAt(0);return{type:\"text\",raw:t,text:t}}return z(n,t,n[0],this.lexer)}}emStrong(t,e,n=\"\"){let i=this.rules.inline.emStrong.lDelim.exec(t);if(!i)return;if(i[3]&&n.match(/[\\p{L}\\p{N}]/u))return;const s=i[1]||i[2]||\"\";if(!s||s&&(\"\"===n||this.rules.inline.punctuation.exec(n))){const n=i[0].length-1;let s,r,a=n,l=0;const o=\"*\"===i[0][0]?this.rules.inline.emStrong.rDelimAst:this.rules.inline.emStrong.rDelimUnd;for(o.lastIndex=0,e=e.slice(-1*t.length+n);null!=(i=o.exec(e));){if(s=i[1]||i[2]||i[3]||i[4]||i[5]||i[6],!s)continue;if(r=s.length,i[3]||i[4]){a+=r;continue}if((i[5]||i[6])&&n%3&&!((n+r)%3)){l+=r;continue}if(a-=r,a>0)continue;if(r=Math.min(r,r+a+l),Math.min(n,r)%2){const e=t.slice(1,n+i.index+r);return{type:\"em\",raw:t.slice(0,n+i.index+r+1),text:e,tokens:this.lexer.inlineTokens(e,[])}}const e=t.slice(2,n+i.index+r-1);return{type:\"strong\",raw:t.slice(0,n+i.index+r+1),text:e,tokens:this.lexer.inlineTokens(e,[])}}}}codespan(t){const e=this.rules.inline.code.exec(t);if(e){let t=e[2].replace(/\\n/g,\" \");const n=/[^ ]/.test(t),i=/^ /.test(t)&&/ $/.test(t);return n&&i&&(t=t.substring(1,t.length-1)),t=o(t,!0),{type:\"codespan\",raw:e[0],text:t}}}br(t){const e=this.rules.inline.br.exec(t);if(e)return{type:\"br\",raw:e[0]}}del(t){const e=this.rules.inline.del.exec(t);if(e)return{type:\"del\",raw:e[0],text:e[2],tokens:this.lexer.inlineTokens(e[2],[])}}autolink(t,e){const n=this.rules.inline.autolink.exec(t);if(n){let t,i;return\"@\"===n[2]?(t=o(this.options.mangle?e(n[1]):n[1]),i=\"mailto:\"+t):(t=o(n[1]),i=t),{type:\"link\",raw:n[0],text:t,href:i,tokens:[{type:\"text\",raw:t,text:t}]}}}url(t,e){let n;if(n=this.rules.inline.url.exec(t)){let t,i;if(\"@\"===n[2])t=o(this.options.mangle?e(n[0]):n[0]),i=\"mailto:\"+t;else{let e;do{e=n[0],n[0]=this.rules.inline._backpedal.exec(n[0])[0]}while(e!==n[0]);t=o(n[0]),i=\"www.\"===n[1]?\"http://\"+t:t}return{type:\"link\",raw:n[0],text:t,href:i,tokens:[{type:\"text\",raw:t,text:t}]}}}inlineText(t,e){const n=this.rules.inline.text.exec(t);if(n){let t;return t=this.lexer.state.inRawBlock?this.options.sanitize?this.options.sanitizer?this.options.sanitizer(n[0]):o(n[0]):n[0]:o(this.options.smartypants?e(n[0]):n[0]),{type:\"text\",raw:n[0],text:t}}}}const E={newline:/^(?: *(?:\\n|$))+/,code:/^( {4}[^\\n]+(?:\\n(?: *(?:\\n|$))*)?)+/,fences:/^ {0,3}(`{3,}(?=[^`\\n]*\\n)|~{3,})([^\\n]*)\\n(?:|([\\s\\S]*?)\\n)(?: {0,3}\\1[~`]* *(?=\\n|$)|$)/,hr:/^ {0,3}((?:- *){3,}|(?:_ *){3,}|(?:\\* *){3,})(?:\\n+|$)/,heading:/^ {0,3}(#{1,6})(?=\\s|$)(.*)(?:\\n+|$)/,blockquote:/^( {0,3}> ?(paragraph|[^\\n]*)(?:\\n|$))+/,list:/^( {0,3}bull)( [^\\n]+?)?(?:\\n|$)/,html:\"^ {0,3}(?:<(script|pre|style|textarea)[\\\\s>][\\\\s\\\\S]*?(?:</\\\\1>[^\\\\n]*\\\\n+|$)|comment[^\\\\n]*(\\\\n+|$)|<\\\\?[\\\\s\\\\S]*?(?:\\\\?>\\\\n*|$)|<![A-Z][\\\\s\\\\S]*?(?:>\\\\n*|$)|<!\\\\[CDATA\\\\[[\\\\s\\\\S]*?(?:\\\\]\\\\]>\\\\n*|$)|</?(tag)(?: +|\\\\n|/?>)[\\\\s\\\\S]*?(?:(?:\\\\n *)+\\\\n|$)|<(?!script|pre|style|textarea)([a-z][\\\\w-]*)(?:attribute)*? */?>(?=[ \\\\t]*(?:\\\\n|$))[\\\\s\\\\S]*?(?:(?:\\\\n *)+\\\\n|$)|</(?!script|pre|style|textarea)[a-z][\\\\w-]*\\\\s*>(?=[ \\\\t]*(?:\\\\n|$))[\\\\s\\\\S]*?(?:(?:\\\\n *)+\\\\n|$))\",def:/^ {0,3}\\[(label)\\]: *(?:\\n *)?<?([^\\s>]+)>?(?:(?: +(?:\\n *)?| *\\n *)(title))? *(?:\\n+|$)/,table:b,lheading:/^([^\\n]+)\\n {0,3}(=+|-+) *(?:\\n+|$)/,_paragraph:/^([^\\n]+(?:\\n(?!hr|heading|lheading|blockquote|fences|list|html|table| +\\n)[^\\n]+)*)/,text:/^[^\\n]+/,_label:/(?!\\s*\\])(?:\\\\.|[^\\[\\]\\\\])+/,_title:/(?:\"(?:\\\\\"?|[^\"\\\\])*\"|'[^'\\n]*(?:\\n[^'\\n]+)*\\n?'|\\([^()]*\\))/};E.def=d(E.def).replace(\"label\",E._label).replace(\"title\",E._title).getRegex(),E.bullet=/(?:[*+-]|\\d{1,9}[.)])/,E.listItemStart=d(/^( *)(bull) */).replace(\"bull\",E.bullet).getRegex(),E.list=d(E.list).replace(/bull/g,E.bullet).replace(\"hr\",\"\\\\n+(?=\\\\1?(?:(?:- *){3,}|(?:_ *){3,}|(?:\\\\* *){3,})(?:\\\\n+|$))\").replace(\"def\",\"\\\\n+(?=\"+E.def.source+\")\").getRegex(),E._tag=\"address|article|aside|base|basefont|blockquote|body|caption|center|col|colgroup|dd|details|dialog|dir|div|dl|dt|fieldset|figcaption|figure|footer|form|frame|frameset|h[1-6]|head|header|hr|html|iframe|legend|li|link|main|menu|menuitem|meta|nav|noframes|ol|optgroup|option|p|param|section|source|summary|table|tbody|td|tfoot|th|thead|title|tr|track|ul\",E._comment=/<!--(?!-?>)[\\s\\S]*?(?:-->|$)/,E.html=d(E.html,\"i\").replace(\"comment\",E._comment).replace(\"tag\",E._tag).replace(\"attribute\",/ +[a-zA-Z:_][\\w.:-]*(?: *= *\"[^\"\\n]*\"| *= *'[^'\\n]*'| *= *[^\\s\"'=<>`]+)?/).getRegex(),E.paragraph=d(E._paragraph).replace(\"hr\",E.hr).replace(\"heading\",\" {0,3}#{1,6} \").replace(\"|lheading\",\"\").replace(\"|table\",\"\").replace(\"blockquote\",\" {0,3}>\").replace(\"fences\",\" {0,3}(?:`{3,}(?=[^`\\\\n]*\\\\n)|~{3,})[^\\\\n]*\\\\n\").replace(\"list\",\" {0,3}(?:[*+-]|1[.)]) \").replace(\"html\",\"</?(?:tag)(?: +|\\\\n|/?>)|<(?:script|pre|style|textarea|!--)\").replace(\"tag\",E._tag).getRegex(),E.blockquote=d(E.blockquote).replace(\"paragraph\",E.paragraph).getRegex(),E.normal=y({},E),E.gfm=y({},E.normal,{table:\"^ *([^\\\\n ].*\\\\|.*)\\\\n {0,3}(?:\\\\| *)?(:?-+:? *(?:\\\\| *:?-+:? *)*)(?:\\\\| *)?(?:\\\\n((?:(?! *\\\\n|hr|heading|blockquote|code|fences|list|html).*(?:\\\\n|$))*)\\\\n*|$)\"}),E.gfm.table=d(E.gfm.table).replace(\"hr\",E.hr).replace(\"heading\",\" {0,3}#{1,6} \").replace(\"blockquote\",\" {0,3}>\").replace(\"code\",\" {4}[^\\\\n]\").replace(\"fences\",\" {0,3}(?:`{3,}(?=[^`\\\\n]*\\\\n)|~{3,})[^\\\\n]*\\\\n\").replace(\"list\",\" {0,3}(?:[*+-]|1[.)]) \").replace(\"html\",\"</?(?:tag)(?: +|\\\\n|/?>)|<(?:script|pre|style|textarea|!--)\").replace(\"tag\",E._tag).getRegex(),E.gfm.paragraph=d(E._paragraph).replace(\"hr\",E.hr).replace(\"heading\",\" {0,3}#{1,6} \").replace(\"|lheading\",\"\").replace(\"table\",E.gfm.table).replace(\"blockquote\",\" {0,3}>\").replace(\"fences\",\" {0,3}(?:`{3,}(?=[^`\\\\n]*\\\\n)|~{3,})[^\\\\n]*\\\\n\").replace(\"list\",\" {0,3}(?:[*+-]|1[.)]) \").replace(\"html\",\"</?(?:tag)(?: +|\\\\n|/?>)|<(?:script|pre|style|textarea|!--)\").replace(\"tag\",E._tag).getRegex(),E.pedantic=y({},E.normal,{html:d(\"^ *(?:comment *(?:\\\\n|\\\\s*$)|<(tag)[\\\\s\\\\S]+?</\\\\1> *(?:\\\\n{2,}|\\\\s*$)|<tag(?:\\\"[^\\\"]*\\\"|'[^']*'|\\\\s[^'\\\"/>\\\\s]*)*?/?> *(?:\\\\n{2,}|\\\\s*$))\").replace(\"comment\",E._comment).replace(/tag/g,\"(?!(?:a|em|strong|small|s|cite|q|dfn|abbr|data|time|code|var|samp|kbd|sub|sup|i|b|u|mark|ruby|rt|rp|bdi|bdo|span|br|wbr|ins|del|img)\\\\b)\\\\w+(?!:|[^\\\\w\\\\s@]*@)\\\\b\").getRegex(),def:/^ *\\[([^\\]]+)\\]: *<?([^\\s>]+)>?(?: +([\"(][^\\n]+[\")]))? *(?:\\n+|$)/,heading:/^(#{1,6})(.*)(?:\\n+|$)/,fences:b,paragraph:d(E.normal._paragraph).replace(\"hr\",E.hr).replace(\"heading\",\" *#{1,6} *[^\\n]\").replace(\"lheading\",E.lheading).replace(\"blockquote\",\" {0,3}>\").replace(\"|fences\",\"\").replace(\"|list\",\"\").replace(\"|html\",\"\").getRegex()});const $={escape:/^\\\\([!\"#$%&'()*+,\\-./:;<=>?@\\[\\]\\\\^_`{|}~])/,autolink:/^<(scheme:[^\\s\\x00-\\x1f<>]*|email)>/,url:b,tag:\"^comment|^</[a-zA-Z][\\\\w:-]*\\\\s*>|^<[a-zA-Z][\\\\w-]*(?:attribute)*?\\\\s*/?>|^<\\\\?[\\\\s\\\\S]*?\\\\?>|^<![a-zA-Z]+\\\\s[\\\\s\\\\S]*?>|^<!\\\\[CDATA\\\\[[\\\\s\\\\S]*?\\\\]\\\\]>\",link:/^!?\\[(label)\\]\\(\\s*(href)(?:\\s+(title))?\\s*\\)/,reflink:/^!?\\[(label)\\]\\[(ref)\\]/,nolink:/^!?\\[(ref)\\](?:\\[\\])?/,reflinkSearch:\"reflink|nolink(?!\\\\()\",emStrong:{lDelim:/^(?:\\*+(?:([punct_])|[^\\s*]))|^_+(?:([punct*])|([^\\s_]))/,rDelimAst:/^[^_*]*?\\_\\_[^_*]*?\\*[^_*]*?(?=\\_\\_)|[punct_](\\*+)(?=[\\s]|$)|[^punct*_\\s](\\*+)(?=[punct_\\s]|$)|[punct_\\s](\\*+)(?=[^punct*_\\s])|[\\s](\\*+)(?=[punct_])|[punct_](\\*+)(?=[punct_])|[^punct*_\\s](\\*+)(?=[^punct*_\\s])/,rDelimUnd:/^[^_*]*?\\*\\*[^_*]*?\\_[^_*]*?(?=\\*\\*)|[punct*](\\_+)(?=[\\s]|$)|[^punct*_\\s](\\_+)(?=[punct*\\s]|$)|[punct*\\s](\\_+)(?=[^punct*_\\s])|[\\s](\\_+)(?=[punct*])|[punct*](\\_+)(?=[punct*])/},code:/^(`+)([^`]|[^`][\\s\\S]*?[^`])\\1(?!`)/,br:/^( {2,}|\\\\)\\n(?!\\s*$)/,del:b,text:/^(`+|[^`])(?:(?= {2,}\\n)|[\\s\\S]*?(?:(?=[\\\\<!\\[`*_]|\\b_|$)|[^ ](?= {2,}\\n)))/,punctuation:/^([\\spunctuation])/};function L(t){return t.replace(/---/g,\"\u2014\").replace(/--/g,\"\u2013\").replace(/(^|[-\\u2014/(\\[{\"\\s])'/g,\"$1\u2018\").replace(/'/g,\"\u2019\").replace(/(^|[-\\u2014/(\\[{\\u2018\\s])\"/g,\"$1\u201c\").replace(/\"/g,\"\u201d\").replace(/\\.{3}/g,\"\u2026\")}function R(t){let e,n,i=\"\";const s=t.length;for(e=0;e<s;e++)n=t.charCodeAt(e),Math.random()>.5&&(n=\"x\"+n.toString(16)),i+=\"&#\"+n+\";\";return i}$._punctuation=\"!\\\"#$%&'()+\\\\-.,/:;<=>?@\\\\[\\\\]`^{|}~\",$.punctuation=d($.punctuation).replace(/punctuation/g,$._punctuation).getRegex(),$.blockSkip=/\\[[^\\]]*?\\]\\([^\\)]*?\\)|`[^`]*?`|<[^>]*?>/g,$.escapedEmSt=/\\\\\\*|\\\\_/g,$._comment=d(E._comment).replace(\"(?:--\\x3e|$)\",\"--\\x3e\").getRegex(),$.emStrong.lDelim=d($.emStrong.lDelim).replace(/punct/g,$._punctuation).getRegex(),$.emStrong.rDelimAst=d($.emStrong.rDelimAst,\"g\").replace(/punct/g,$._punctuation).getRegex(),$.emStrong.rDelimUnd=d($.emStrong.rDelimUnd,\"g\").replace(/punct/g,$._punctuation).getRegex(),$._escapes=/\\\\([!\"#$%&'()*+,\\-./:;<=>?@\\[\\]\\\\^_`{|}~])/g,$._scheme=/[a-zA-Z][a-zA-Z0-9+.-]{1,31}/,$._email=/[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+(@)[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)+(?![-_])/,$.autolink=d($.autolink).replace(\"scheme\",$._scheme).replace(\"email\",$._email).getRegex(),$._attribute=/\\s+[a-zA-Z:_][\\w.:-]*(?:\\s*=\\s*\"[^\"]*\"|\\s*=\\s*'[^']*'|\\s*=\\s*[^\\s\"'=<>`]+)?/,$.tag=d($.tag).replace(\"comment\",$._comment).replace(\"attribute\",$._attribute).getRegex(),$._label=/(?:\\[(?:\\\\.|[^\\[\\]\\\\])*\\]|\\\\.|`[^`]*`|[^\\[\\]\\\\`])*?/,$._href=/<(?:\\\\.|[^\\n<>\\\\])+>|[^\\s\\x00-\\x1f]*/,$._title=/\"(?:\\\\\"?|[^\"\\\\])*\"|'(?:\\\\'?|[^'\\\\])*'|\\((?:\\\\\\)?|[^)\\\\])*\\)/,$.link=d($.link).replace(\"label\",$._label).replace(\"href\",$._href).replace(\"title\",$._title).getRegex(),$.reflink=d($.reflink).replace(\"label\",$._label).replace(\"ref\",E._label).getRegex(),$.nolink=d($.nolink).replace(\"ref\",E._label).getRegex(),$.reflinkSearch=d($.reflinkSearch,\"g\").replace(\"reflink\",$.reflink).replace(\"nolink\",$.nolink).getRegex(),$.normal=y({},$),$.pedantic=y({},$.normal,{strong:{start:/^__|\\*\\*/,middle:/^__(?=\\S)([\\s\\S]*?\\S)__(?!_)|^\\*\\*(?=\\S)([\\s\\S]*?\\S)\\*\\*(?!\\*)/,endAst:/\\*\\*(?!\\*)/g,endUnd:/__(?!_)/g},em:{start:/^_|\\*/,middle:/^()\\*(?=\\S)([\\s\\S]*?\\S)\\*(?!\\*)|^_(?=\\S)([\\s\\S]*?\\S)_(?!_)/,endAst:/\\*(?!\\*)/g,endUnd:/_(?!_)/g},link:d(/^!?\\[(label)\\]\\((.*?)\\)/).replace(\"label\",$._label).getRegex(),reflink:d(/^!?\\[(label)\\]\\s*\\[([^\\]]*)\\]/).replace(\"label\",$._label).getRegex()}),$.gfm=y({},$.normal,{escape:d($.escape).replace(\"])\",\"~|])\").getRegex(),_extended_email:/[A-Za-z0-9._+-]+(@)[a-zA-Z0-9-_]+(?:\\.[a-zA-Z0-9-_]*[a-zA-Z0-9])+(?![-_])/,url:/^((?:ftp|https?):\\/\\/|www\\.)(?:[a-zA-Z0-9\\-]+\\.?)+[^\\s<]*|^email/,_backpedal:/(?:[^?!.,:;*_~()&]+|\\([^)]*\\)|&(?![a-zA-Z0-9]+;$)|[?!.,:;*_~)]+(?!$))+/,del:/^(~~?)(?=[^\\s~])([\\s\\S]*?[^\\s~])\\1(?=[^~]|$)/,text:/^([`~]+|[^`~])(?:(?= {2,}\\n)|(?=[a-zA-Z0-9.!#$%&'*+\\/=?_`{\\|}~-]+@)|[\\s\\S]*?(?:(?=[\\\\<!\\[`*~_]|\\b_|https?:\\/\\/|ftp:\\/\\/|www\\.|$)|[^ ](?= {2,}\\n)|[^a-zA-Z0-9.!#$%&'*+\\/=?_`{\\|}~-](?=[a-zA-Z0-9.!#$%&'*+\\/=?_`{\\|}~-]+@)))/}),$.gfm.url=d($.gfm.url,\"i\").replace(\"email\",$.gfm._extended_email).getRegex(),$.breaks=y({},$.gfm,{br:d($.br).replace(\"{2,}\",\"*\").getRegex(),text:d($.gfm.text).replace(\"\\\\b_\",\"\\\\b_| {2,}\\\\n\").replace(/\\{2,\\}/g,\"*\").getRegex()});class I{constructor(t){this.tokens=[],this.tokens.links=Object.create(null),this.options=t||e,this.options.tokenizer=this.options.tokenizer||new A,this.tokenizer=this.options.tokenizer,this.tokenizer.options=this.options,this.tokenizer.lexer=this,this.inlineQueue=[],this.state={inLink:!1,inRawBlock:!1,top:!0};const n={block:E.normal,inline:$.normal};this.options.pedantic?(n.block=E.pedantic,n.inline=$.pedantic):this.options.gfm&&(n.block=E.gfm,this.options.breaks?n.inline=$.breaks:n.inline=$.gfm),this.tokenizer.rules=n}static get rules(){return{block:E,inline:$}}static lex(t,e){return new I(e).lex(t)}static lexInline(t,e){return new I(e).inlineTokens(t)}lex(t){let e;for(t=t.replace(/\\r\\n|\\r/g,\"\\n\").replace(/\\t/g,\"    \"),this.blockTokens(t,this.tokens);e=this.inlineQueue.shift();)this.inlineTokens(e.src,e.tokens);return this.tokens}blockTokens(t,e=[]){let n,i,s,r;for(this.options.pedantic&&(t=t.replace(/^ +$/gm,\"\"));t;)if(!(this.options.extensions&&this.options.extensions.block&&this.options.extensions.block.some((i=>!!(n=i.call({lexer:this},t,e))&&(t=t.substring(n.raw.length),e.push(n),!0)))))if(n=this.tokenizer.space(t))t=t.substring(n.raw.length),1===n.raw.length&&e.length>0?e[e.length-1].raw+=\"\\n\":e.push(n);else if(n=this.tokenizer.code(t))t=t.substring(n.raw.length),i=e[e.length-1],!i||\"paragraph\"!==i.type&&\"text\"!==i.type?e.push(n):(i.raw+=\"\\n\"+n.raw,i.text+=\"\\n\"+n.text,this.inlineQueue[this.inlineQueue.length-1].src=i.text);else if(n=this.tokenizer.fences(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.heading(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.hr(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.blockquote(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.list(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.html(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.def(t))t=t.substring(n.raw.length),i=e[e.length-1],!i||\"paragraph\"!==i.type&&\"text\"!==i.type?this.tokens.links[n.tag]||(this.tokens.links[n.tag]={href:n.href,title:n.title}):(i.raw+=\"\\n\"+n.raw,i.text+=\"\\n\"+n.raw,this.inlineQueue[this.inlineQueue.length-1].src=i.text);else if(n=this.tokenizer.table(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.lheading(t))t=t.substring(n.raw.length),e.push(n);else{if(s=t,this.options.extensions&&this.options.extensions.startBlock){let e=1/0;const n=t.slice(1);let i;this.options.extensions.startBlock.forEach((function(t){i=t.call({lexer:this},n),\"number\"==typeof i&&i>=0&&(e=Math.min(e,i))})),e<1/0&&e>=0&&(s=t.substring(0,e+1))}if(this.state.top&&(n=this.tokenizer.paragraph(s)))i=e[e.length-1],r&&\"paragraph\"===i.type?(i.raw+=\"\\n\"+n.raw,i.text+=\"\\n\"+n.text,this.inlineQueue.pop(),this.inlineQueue[this.inlineQueue.length-1].src=i.text):e.push(n),r=s.length!==t.length,t=t.substring(n.raw.length);else if(n=this.tokenizer.text(t))t=t.substring(n.raw.length),i=e[e.length-1],i&&\"text\"===i.type?(i.raw+=\"\\n\"+n.raw,i.text+=\"\\n\"+n.text,this.inlineQueue.pop(),this.inlineQueue[this.inlineQueue.length-1].src=i.text):e.push(n);else if(t){const e=\"Infinite loop on byte: \"+t.charCodeAt(0);if(this.options.silent){console.error(e);break}throw new Error(e)}}return this.state.top=!0,e}inline(t,e){this.inlineQueue.push({src:t,tokens:e})}inlineTokens(t,e=[]){let n,i,s,r,a,l,o=t;if(this.tokens.links){const t=Object.keys(this.tokens.links);if(t.length>0)for(;null!=(r=this.tokenizer.rules.inline.reflinkSearch.exec(o));)t.includes(r[0].slice(r[0].lastIndexOf(\"[\")+1,-1))&&(o=o.slice(0,r.index)+\"[\"+_(\"a\",r[0].length-2)+\"]\"+o.slice(this.tokenizer.rules.inline.reflinkSearch.lastIndex))}for(;null!=(r=this.tokenizer.rules.inline.blockSkip.exec(o));)o=o.slice(0,r.index)+\"[\"+_(\"a\",r[0].length-2)+\"]\"+o.slice(this.tokenizer.rules.inline.blockSkip.lastIndex);for(;null!=(r=this.tokenizer.rules.inline.escapedEmSt.exec(o));)o=o.slice(0,r.index)+\"++\"+o.slice(this.tokenizer.rules.inline.escapedEmSt.lastIndex);for(;t;)if(a||(l=\"\"),a=!1,!(this.options.extensions&&this.options.extensions.inline&&this.options.extensions.inline.some((i=>!!(n=i.call({lexer:this},t,e))&&(t=t.substring(n.raw.length),e.push(n),!0)))))if(n=this.tokenizer.escape(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.tag(t))t=t.substring(n.raw.length),i=e[e.length-1],i&&\"text\"===n.type&&\"text\"===i.type?(i.raw+=n.raw,i.text+=n.text):e.push(n);else if(n=this.tokenizer.link(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.reflink(t,this.tokens.links))t=t.substring(n.raw.length),i=e[e.length-1],i&&\"text\"===n.type&&\"text\"===i.type?(i.raw+=n.raw,i.text+=n.text):e.push(n);else if(n=this.tokenizer.emStrong(t,o,l))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.codespan(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.br(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.del(t))t=t.substring(n.raw.length),e.push(n);else if(n=this.tokenizer.autolink(t,R))t=t.substring(n.raw.length),e.push(n);else if(this.state.inLink||!(n=this.tokenizer.url(t,R))){if(s=t,this.options.extensions&&this.options.extensions.startInline){let e=1/0;const n=t.slice(1);let i;this.options.extensions.startInline.forEach((function(t){i=t.call({lexer:this},n),\"number\"==typeof i&&i>=0&&(e=Math.min(e,i))})),e<1/0&&e>=0&&(s=t.substring(0,e+1))}if(n=this.tokenizer.inlineText(s,L))t=t.substring(n.raw.length),\"_\"!==n.raw.slice(-1)&&(l=n.raw.slice(-1)),a=!0,i=e[e.length-1],i&&\"text\"===i.type?(i.raw+=n.raw,i.text+=n.text):e.push(n);else if(t){const e=\"Infinite loop on byte: \"+t.charCodeAt(0);if(this.options.silent){console.error(e);break}throw new Error(e)}}else t=t.substring(n.raw.length),e.push(n);return e}}class C{constructor(t){this.options=t||e}code(t,e,n){const i=(e||\"\").match(/\\S*/)[0];if(this.options.highlight){const e=this.options.highlight(t,i);null!=e&&e!==t&&(n=!0,t=e)}return t=t.replace(/\\n$/,\"\")+\"\\n\",i?'<pre><code class=\"'+this.options.langPrefix+o(i,!0)+'\">'+(n?t:o(t,!0))+\"</code></pre>\\n\":\"<pre><code>\"+(n?t:o(t,!0))+\"</code></pre>\\n\"}blockquote(t){return\"<blockquote>\\n\"+t+\"</blockquote>\\n\"}html(t){return t}heading(t,e,n,i){return this.options.headerIds?\"<h\"+e+' id=\"'+this.options.headerPrefix+i.slug(n)+'\">'+t+\"</h\"+e+\">\\n\":\"<h\"+e+\">\"+t+\"</h\"+e+\">\\n\"}hr(){return this.options.xhtml?\"<hr/>\\n\":\"<hr>\\n\"}list(t,e,n){const i=e?\"ol\":\"ul\";return\"<\"+i+(e&&1!==n?' start=\"'+n+'\"':\"\")+\">\\n\"+t+\"</\"+i+\">\\n\"}listitem(t){return\"<li>\"+t+\"</li>\\n\"}checkbox(t){return\"<input \"+(t?'checked=\"\" ':\"\")+'disabled=\"\" type=\"checkbox\"'+(this.options.xhtml?\" /\":\"\")+\"> \"}paragraph(t){return\"<p>\"+t+\"</p>\\n\"}table(t,e){return e&&(e=\"<tbody>\"+e+\"</tbody>\"),\"<table>\\n<thead>\\n\"+t+\"</thead>\\n\"+e+\"</table>\\n\"}tablerow(t){return\"<tr>\\n\"+t+\"</tr>\\n\"}tablecell(t,e){const n=e.header?\"th\":\"td\";return(e.align?\"<\"+n+' align=\"'+e.align+'\">':\"<\"+n+\">\")+t+\"</\"+n+\">\\n\"}strong(t){return\"<strong>\"+t+\"</strong>\"}em(t){return\"<em>\"+t+\"</em>\"}codespan(t){return\"<code>\"+t+\"</code>\"}br(){return this.options.xhtml?\"<br/>\":\"<br>\"}del(t){return\"<del>\"+t+\"</del>\"}link(t,e,n){if(null===(t=m(this.options.sanitize,this.options.baseUrl,t)))return n;let i='<a href=\"'+o(t)+'\"';return e&&(i+=' title=\"'+e+'\"'),i+=\">\"+n+\"</a>\",i}image(t,e,n){if(null===(t=m(this.options.sanitize,this.options.baseUrl,t)))return n;let i='<img src=\"'+t+'\" alt=\"'+n+'\"';return e&&(i+=' title=\"'+e+'\"'),i+=this.options.xhtml?\"/>\":\">\",i}text(t){return t}}class M{strong(t){return t}em(t){return t}codespan(t){return t}del(t){return t}html(t){return t}text(t){return t}link(t,e,n){return\"\"+n}image(t,e,n){return\"\"+n}br(){return\"\"}}class q{constructor(){this.seen={}}serialize(t){return t.toLowerCase().trim().replace(/<[!\\/a-z].*?>/gi,\"\").replace(/[\\u2000-\\u206F\\u2E00-\\u2E7F\\\\'!\"#$%&()*+,./:;<=>?@[\\]^`{|}~]/g,\"\").replace(/\\s/g,\"-\")}getNextSafeSlug(t,e){let n=t,i=0;if(this.seen.hasOwnProperty(n)){i=this.seen[t];do{i++,n=t+\"-\"+i}while(this.seen.hasOwnProperty(n))}return e||(this.seen[t]=i,this.seen[n]=0),n}slug(t,e={}){const n=this.serialize(t);return this.getNextSafeSlug(n,e.dryrun)}}class O{constructor(t){this.options=t||e,this.options.renderer=this.options.renderer||new C,this.renderer=this.options.renderer,this.renderer.options=this.options,this.textRenderer=new M,this.slugger=new q}static parse(t,e){return new O(e).parse(t)}static parseInline(t,e){return new O(e).parseInline(t)}parse(t,e=!0){let n,i,s,r,a,l,o,c,u,d,h,g,m,f,k,w,x,b,y,v=\"\";const S=t.length;for(n=0;n<S;n++)if(d=t[n],this.options.extensions&&this.options.extensions.renderers&&this.options.extensions.renderers[d.type]&&(y=this.options.extensions.renderers[d.type].call({parser:this},d),!1!==y||![\"space\",\"hr\",\"heading\",\"code\",\"table\",\"blockquote\",\"list\",\"html\",\"paragraph\",\"text\"].includes(d.type)))v+=y||\"\";else switch(d.type){case\"space\":continue;case\"hr\":v+=this.renderer.hr();continue;case\"heading\":v+=this.renderer.heading(this.parseInline(d.tokens),d.depth,p(this.parseInline(d.tokens,this.textRenderer)),this.slugger);continue;case\"code\":v+=this.renderer.code(d.text,d.lang,d.escaped);continue;case\"table\":for(c=\"\",o=\"\",r=d.header.length,i=0;i<r;i++)o+=this.renderer.tablecell(this.parseInline(d.header[i].tokens),{header:!0,align:d.align[i]});for(c+=this.renderer.tablerow(o),u=\"\",r=d.rows.length,i=0;i<r;i++){for(l=d.rows[i],o=\"\",a=l.length,s=0;s<a;s++)o+=this.renderer.tablecell(this.parseInline(l[s].tokens),{header:!1,align:d.align[s]});u+=this.renderer.tablerow(o)}v+=this.renderer.table(c,u);continue;case\"blockquote\":u=this.parse(d.tokens),v+=this.renderer.blockquote(u);continue;case\"list\":for(h=d.ordered,g=d.start,m=d.loose,r=d.items.length,u=\"\",i=0;i<r;i++)k=d.items[i],w=k.checked,x=k.task,f=\"\",k.task&&(b=this.renderer.checkbox(w),m?k.tokens.length>0&&\"paragraph\"===k.tokens[0].type?(k.tokens[0].text=b+\" \"+k.tokens[0].text,k.tokens[0].tokens&&k.tokens[0].tokens.length>0&&\"text\"===k.tokens[0].tokens[0].type&&(k.tokens[0].tokens[0].text=b+\" \"+k.tokens[0].tokens[0].text)):k.tokens.unshift({type:\"text\",text:b}):f+=b),f+=this.parse(k.tokens,m),u+=this.renderer.listitem(f,x,w);v+=this.renderer.list(u,h,g);continue;case\"html\":v+=this.renderer.html(d.text);continue;case\"paragraph\":v+=this.renderer.paragraph(this.parseInline(d.tokens));continue;case\"text\":for(u=d.tokens?this.parseInline(d.tokens):d.text;n+1<S&&\"text\"===t[n+1].type;)d=t[++n],u+=\"\\n\"+(d.tokens?this.parseInline(d.tokens):d.text);v+=e?this.renderer.paragraph(u):u;continue;default:{const t='Token with \"'+d.type+'\" type was not found.';if(this.options.silent)return void console.error(t);throw new Error(t)}}return v}parseInline(t,e){e=e||this.renderer;let n,i,s,r=\"\";const a=t.length;for(n=0;n<a;n++)if(i=t[n],this.options.extensions&&this.options.extensions.renderers&&this.options.extensions.renderers[i.type]&&(s=this.options.extensions.renderers[i.type].call({parser:this},i),!1!==s||![\"escape\",\"html\",\"link\",\"image\",\"strong\",\"em\",\"codespan\",\"br\",\"del\",\"text\"].includes(i.type)))r+=s||\"\";else switch(i.type){case\"escape\":case\"text\":r+=e.text(i.text);break;case\"html\":r+=e.html(i.text);break;case\"link\":r+=e.link(i.href,i.title,this.parseInline(i.tokens,e));break;case\"image\":r+=e.image(i.href,i.title,i.text);break;case\"strong\":r+=e.strong(this.parseInline(i.tokens,e));break;case\"em\":r+=e.em(this.parseInline(i.tokens,e));break;case\"codespan\":r+=e.codespan(i.text);break;case\"br\":r+=e.br();break;case\"del\":r+=e.del(this.parseInline(i.tokens,e));break;default:{const t='Token with \"'+i.type+'\" type was not found.';if(this.options.silent)return void console.error(t);throw new Error(t)}}return r}}function N(t,e,n){if(null==t)throw new Error(\"marked(): input parameter is undefined or null\");if(\"string\"!=typeof t)throw new Error(\"marked(): input parameter is of type \"+Object.prototype.toString.call(t)+\", string expected\");if(\"function\"==typeof e&&(n=e,e=null),T(e=y({},N.defaults,e||{})),n){const i=e.highlight;let s;try{s=I.lex(t,e)}catch(t){return n(t)}const r=function(t){let r;if(!t)try{e.walkTokens&&N.walkTokens(s,e.walkTokens),r=O.parse(s,e)}catch(e){t=e}return e.highlight=i,t?n(t):n(null,r)};if(!i||i.length<3)return r();if(delete e.highlight,!s.length)return r();let a=0;return N.walkTokens(s,(function(t){\"code\"===t.type&&(a++,setTimeout((()=>{i(t.text,t.lang,(function(e,n){if(e)return r(e);null!=n&&n!==t.text&&(t.text=n,t.escaped=!0),a--,0===a&&r()}))}),0))})),void(0===a&&r())}try{const n=I.lex(t,e);return e.walkTokens&&N.walkTokens(n,e.walkTokens),O.parse(n,e)}catch(t){if(t.message+=\"\\nPlease report this to https://github.com/markedjs/marked.\",e.silent)return\"<p>An error occurred:</p><pre>\"+o(t.message+\"\",!0)+\"</pre>\";throw t}}N.options=N.setOptions=function(t){var n;return y(N.defaults,t),n=N.defaults,e=n,N},N.getDefaults=t,N.defaults=e,N.use=function(...t){const e=y({},...t),n=N.defaults.extensions||{renderers:{},childTokens:{}};let i;t.forEach((t=>{if(t.extensions&&(i=!0,t.extensions.forEach((t=>{if(!t.name)throw new Error(\"extension name required\");if(t.renderer){const e=n.renderers?n.renderers[t.name]:null;n.renderers[t.name]=e?function(...n){let i=t.renderer.apply(this,n);return!1===i&&(i=e.apply(this,n)),i}:t.renderer}if(t.tokenizer){if(!t.level||\"block\"!==t.level&&\"inline\"!==t.level)throw new Error(\"extension level must be 'block' or 'inline'\");n[t.level]?n[t.level].unshift(t.tokenizer):n[t.level]=[t.tokenizer],t.start&&(\"block\"===t.level?n.startBlock?n.startBlock.push(t.start):n.startBlock=[t.start]:\"inline\"===t.level&&(n.startInline?n.startInline.push(t.start):n.startInline=[t.start]))}t.childTokens&&(n.childTokens[t.name]=t.childTokens)}))),t.renderer){const n=N.defaults.renderer||new C;for(const e in t.renderer){const i=n[e];n[e]=(...s)=>{let r=t.renderer[e].apply(n,s);return!1===r&&(r=i.apply(n,s)),r}}e.renderer=n}if(t.tokenizer){const n=N.defaults.tokenizer||new A;for(const e in t.tokenizer){const i=n[e];n[e]=(...s)=>{let r=t.tokenizer[e].apply(n,s);return!1===r&&(r=i.apply(n,s)),r}}e.tokenizer=n}if(t.walkTokens){const n=N.defaults.walkTokens;e.walkTokens=function(e){t.walkTokens.call(this,e),n&&n.call(this,e)}}i&&(e.extensions=n),N.setOptions(e)}))},N.walkTokens=function(t,e){for(const n of t)switch(e.call(N,n),n.type){case\"table\":for(const t of n.header)N.walkTokens(t.tokens,e);for(const t of n.rows)for(const n of t)N.walkTokens(n.tokens,e);break;case\"list\":N.walkTokens(n.items,e);break;default:N.defaults.extensions&&N.defaults.extensions.childTokens&&N.defaults.extensions.childTokens[n.type]?N.defaults.extensions.childTokens[n.type].forEach((function(t){N.walkTokens(n[t],e)})):n.tokens&&N.walkTokens(n.tokens,e)}},N.parseInline=function(t,e){if(null==t)throw new Error(\"marked.parseInline(): input parameter is undefined or null\");if(\"string\"!=typeof t)throw new Error(\"marked.parseInline(): input parameter is of type \"+Object.prototype.toString.call(t)+\", string expected\");T(e=y({},N.defaults,e||{}));try{const n=I.lexInline(t,e);return e.walkTokens&&N.walkTokens(n,e.walkTokens),O.parseInline(n,e)}catch(t){if(t.message+=\"\\nPlease report this to https://github.com/markedjs/marked.\",e.silent)return\"<p>An error occurred:</p><pre>\"+o(t.message+\"\",!0)+\"</pre>\";throw t}},N.Parser=O,N.parser=O.parse,N.Renderer=C,N.TextRenderer=M,N.Lexer=I,N.lexer=I.lex,N.Tokenizer=A,N.Slugger=q,N.parse=N;return()=>{let t,e,n=null;function i(){if(n&&!n.closed)n.focus();else{if(n=window.open(\"about:blank\",\"reveal.js - Notes\",\"width=1100,height=700\"),n.marked=N,n.document.write(\"\\x3c!--\\n\\tNOTE: You need to build the notes plugin after making changes to this file.\\n--\\x3e\\n<html lang=\\\"en\\\">\\n\\t<head>\\n\\t\\t<meta charset=\\\"utf-8\\\">\\n\\n\\t\\t<title>reveal.js - Speaker View</title>\\n\\n\\t\\t<style>\\n\\t\\t\\tbody {\\n\\t\\t\\t\\tfont-family: Helvetica;\\n\\t\\t\\t\\tfont-size: 18px;\\n\\t\\t\\t}\\n\\n\\t\\t\\t#current-slide,\\n\\t\\t\\t#upcoming-slide,\\n\\t\\t\\t#speaker-controls {\\n\\t\\t\\t\\tpadding: 6px;\\n\\t\\t\\t\\tbox-sizing: border-box;\\n\\t\\t\\t\\t-moz-box-sizing: border-box;\\n\\t\\t\\t}\\n\\n\\t\\t\\t#current-slide iframe,\\n\\t\\t\\t#upcoming-slide iframe {\\n\\t\\t\\t\\twidth: 100%;\\n\\t\\t\\t\\theight: 100%;\\n\\t\\t\\t\\tborder: 1px solid #ddd;\\n\\t\\t\\t}\\n\\n\\t\\t\\t#current-slide .label,\\n\\t\\t\\t#upcoming-slide .label {\\n\\t\\t\\t\\tposition: absolute;\\n\\t\\t\\t\\ttop: 10px;\\n\\t\\t\\t\\tleft: 10px;\\n\\t\\t\\t\\tz-index: 2;\\n\\t\\t\\t}\\n\\n\\t\\t\\t#connection-status {\\n\\t\\t\\t\\tposition: absolute;\\n\\t\\t\\t\\ttop: 0;\\n\\t\\t\\t\\tleft: 0;\\n\\t\\t\\t\\twidth: 100%;\\n\\t\\t\\t\\theight: 100%;\\n\\t\\t\\t\\tz-index: 20;\\n\\t\\t\\t\\tpadding: 30% 20% 20% 20%;\\n\\t\\t\\t\\tfont-size: 18px;\\n\\t\\t\\t\\tcolor: #222;\\n\\t\\t\\t\\tbackground: #fff;\\n\\t\\t\\t\\ttext-align: center;\\n\\t\\t\\t\\tbox-sizing: border-box;\\n\\t\\t\\t\\tline-height: 1.4;\\n\\t\\t\\t}\\n\\n\\t\\t\\t.overlay-element {\\n\\t\\t\\t\\theight: 34px;\\n\\t\\t\\t\\tline-height: 34px;\\n\\t\\t\\t\\tpadding: 0 10px;\\n\\t\\t\\t\\ttext-shadow: none;\\n\\t\\t\\t\\tbackground: rgba( 220, 220, 220, 0.8 );\\n\\t\\t\\t\\tcolor: #222;\\n\\t\\t\\t\\tfont-size: 14px;\\n\\t\\t\\t}\\n\\n\\t\\t\\t.overlay-element.interactive:hover {\\n\\t\\t\\t\\tbackground: rgba( 220, 220, 220, 1 );\\n\\t\\t\\t}\\n\\n\\t\\t\\t#current-slide {\\n\\t\\t\\t\\tposition: absolute;\\n\\t\\t\\t\\twidth: 60%;\\n\\t\\t\\t\\theight: 100%;\\n\\t\\t\\t\\ttop: 0;\\n\\t\\t\\t\\tleft: 0;\\n\\t\\t\\t\\tpadding-right: 0;\\n\\t\\t\\t}\\n\\n\\t\\t\\t#upcoming-slide {\\n\\t\\t\\t\\tposition: absolute;\\n\\t\\t\\t\\twidth: 40%;\\n\\t\\t\\t\\theight: 40%;\\n\\t\\t\\t\\tright: 0;\\n\\t\\t\\t\\ttop: 0;\\n\\t\\t\\t}\\n\\n\\t\\t\\t/* Speaker controls */\\n\\t\\t\\t#speaker-controls {\\n\\t\\t\\t\\tposition: absolute;\\n\\t\\t\\t\\ttop: 40%;\\n\\t\\t\\t\\tright: 0;\\n\\t\\t\\t\\twidth: 40%;\\n\\t\\t\\t\\theight: 60%;\\n\\t\\t\\t\\toverflow: auto;\\n\\t\\t\\t\\tfont-size: 18px;\\n\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time.hidden,\\n\\t\\t\\t\\t.speaker-controls-notes.hidden {\\n\\t\\t\\t\\t\\tdisplay: none;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time .label,\\n\\t\\t\\t\\t.speaker-controls-pace .label,\\n\\t\\t\\t\\t.speaker-controls-notes .label {\\n\\t\\t\\t\\t\\ttext-transform: uppercase;\\n\\t\\t\\t\\t\\tfont-weight: normal;\\n\\t\\t\\t\\t\\tfont-size: 0.66em;\\n\\t\\t\\t\\t\\tcolor: #666;\\n\\t\\t\\t\\t\\tmargin: 0;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time, .speaker-controls-pace {\\n\\t\\t\\t\\t\\tborder-bottom: 1px solid rgba( 200, 200, 200, 0.5 );\\n\\t\\t\\t\\t\\tmargin-bottom: 10px;\\n\\t\\t\\t\\t\\tpadding: 10px 16px;\\n\\t\\t\\t\\t\\tpadding-bottom: 20px;\\n\\t\\t\\t\\t\\tcursor: pointer;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time .reset-button {\\n\\t\\t\\t\\t\\topacity: 0;\\n\\t\\t\\t\\t\\tfloat: right;\\n\\t\\t\\t\\t\\tcolor: #666;\\n\\t\\t\\t\\t\\ttext-decoration: none;\\n\\t\\t\\t\\t}\\n\\t\\t\\t\\t.speaker-controls-time:hover .reset-button {\\n\\t\\t\\t\\t\\topacity: 1;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time .timer,\\n\\t\\t\\t\\t.speaker-controls-time .clock {\\n\\t\\t\\t\\t\\twidth: 50%;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time .timer,\\n\\t\\t\\t\\t.speaker-controls-time .clock,\\n\\t\\t\\t\\t.speaker-controls-time .pacing .hours-value,\\n\\t\\t\\t\\t.speaker-controls-time .pacing .minutes-value,\\n\\t\\t\\t\\t.speaker-controls-time .pacing .seconds-value {\\n\\t\\t\\t\\t\\tfont-size: 1.9em;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time .timer {\\n\\t\\t\\t\\t\\tfloat: left;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time .clock {\\n\\t\\t\\t\\t\\tfloat: right;\\n\\t\\t\\t\\t\\ttext-align: right;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time span.mute {\\n\\t\\t\\t\\t\\topacity: 0.3;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time .pacing-title {\\n\\t\\t\\t\\t\\tmargin-top: 5px;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time .pacing.ahead {\\n\\t\\t\\t\\t\\tcolor: blue;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time .pacing.on-track {\\n\\t\\t\\t\\t\\tcolor: green;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-time .pacing.behind {\\n\\t\\t\\t\\t\\tcolor: red;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-notes {\\n\\t\\t\\t\\t\\tpadding: 10px 16px;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t.speaker-controls-notes .value {\\n\\t\\t\\t\\t\\tmargin-top: 5px;\\n\\t\\t\\t\\t\\tline-height: 1.4;\\n\\t\\t\\t\\t\\tfont-size: 1.2em;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t/* Layout selector\u00a0*/\\n\\t\\t\\t#speaker-layout {\\n\\t\\t\\t\\tposition: absolute;\\n\\t\\t\\t\\ttop: 10px;\\n\\t\\t\\t\\tright: 10px;\\n\\t\\t\\t\\tcolor: #222;\\n\\t\\t\\t\\tz-index: 10;\\n\\t\\t\\t}\\n\\t\\t\\t\\t#speaker-layout select {\\n\\t\\t\\t\\t\\tposition: absolute;\\n\\t\\t\\t\\t\\twidth: 100%;\\n\\t\\t\\t\\t\\theight: 100%;\\n\\t\\t\\t\\t\\ttop: 0;\\n\\t\\t\\t\\t\\tleft: 0;\\n\\t\\t\\t\\t\\tborder: 0;\\n\\t\\t\\t\\t\\tbox-shadow: 0;\\n\\t\\t\\t\\t\\tcursor: pointer;\\n\\t\\t\\t\\t\\topacity: 0;\\n\\n\\t\\t\\t\\t\\tfont-size: 1em;\\n\\t\\t\\t\\t\\tbackground-color: transparent;\\n\\n\\t\\t\\t\\t\\t-moz-appearance: none;\\n\\t\\t\\t\\t\\t-webkit-appearance: none;\\n\\t\\t\\t\\t\\t-webkit-tap-highlight-color: rgba(0, 0, 0, 0);\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t#speaker-layout select:focus {\\n\\t\\t\\t\\t\\toutline: none;\\n\\t\\t\\t\\t\\tbox-shadow: none;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t.clear {\\n\\t\\t\\t\\tclear: both;\\n\\t\\t\\t}\\n\\n\\t\\t\\t/* Speaker layout: Wide */\\n\\t\\t\\tbody[data-speaker-layout=\\\"wide\\\"] #current-slide,\\n\\t\\t\\tbody[data-speaker-layout=\\\"wide\\\"] #upcoming-slide {\\n\\t\\t\\t\\twidth: 50%;\\n\\t\\t\\t\\theight: 45%;\\n\\t\\t\\t\\tpadding: 6px;\\n\\t\\t\\t}\\n\\n\\t\\t\\tbody[data-speaker-layout=\\\"wide\\\"] #current-slide {\\n\\t\\t\\t\\ttop: 0;\\n\\t\\t\\t\\tleft: 0;\\n\\t\\t\\t}\\n\\n\\t\\t\\tbody[data-speaker-layout=\\\"wide\\\"] #upcoming-slide {\\n\\t\\t\\t\\ttop: 0;\\n\\t\\t\\t\\tleft: 50%;\\n\\t\\t\\t}\\n\\n\\t\\t\\tbody[data-speaker-layout=\\\"wide\\\"] #speaker-controls {\\n\\t\\t\\t\\ttop: 45%;\\n\\t\\t\\t\\tleft: 0;\\n\\t\\t\\t\\twidth: 100%;\\n\\t\\t\\t\\theight: 50%;\\n\\t\\t\\t\\tfont-size: 1.25em;\\n\\t\\t\\t}\\n\\n\\t\\t\\t/* Speaker layout: Tall */\\n\\t\\t\\tbody[data-speaker-layout=\\\"tall\\\"] #current-slide,\\n\\t\\t\\tbody[data-speaker-layout=\\\"tall\\\"] #upcoming-slide {\\n\\t\\t\\t\\twidth: 45%;\\n\\t\\t\\t\\theight: 50%;\\n\\t\\t\\t\\tpadding: 6px;\\n\\t\\t\\t}\\n\\n\\t\\t\\tbody[data-speaker-layout=\\\"tall\\\"] #current-slide {\\n\\t\\t\\t\\ttop: 0;\\n\\t\\t\\t\\tleft: 0;\\n\\t\\t\\t}\\n\\n\\t\\t\\tbody[data-speaker-layout=\\\"tall\\\"] #upcoming-slide {\\n\\t\\t\\t\\ttop: 50%;\\n\\t\\t\\t\\tleft: 0;\\n\\t\\t\\t}\\n\\n\\t\\t\\tbody[data-speaker-layout=\\\"tall\\\"] #speaker-controls {\\n\\t\\t\\t\\tpadding-top: 40px;\\n\\t\\t\\t\\ttop: 0;\\n\\t\\t\\t\\tleft: 45%;\\n\\t\\t\\t\\twidth: 55%;\\n\\t\\t\\t\\theight: 100%;\\n\\t\\t\\t\\tfont-size: 1.25em;\\n\\t\\t\\t}\\n\\n\\t\\t\\t/* Speaker layout: Notes only */\\n\\t\\t\\tbody[data-speaker-layout=\\\"notes-only\\\"] #current-slide,\\n\\t\\t\\tbody[data-speaker-layout=\\\"notes-only\\\"] #upcoming-slide {\\n\\t\\t\\t\\tdisplay: none;\\n\\t\\t\\t}\\n\\n\\t\\t\\tbody[data-speaker-layout=\\\"notes-only\\\"] #speaker-controls {\\n\\t\\t\\t\\tpadding-top: 40px;\\n\\t\\t\\t\\ttop: 0;\\n\\t\\t\\t\\tleft: 0;\\n\\t\\t\\t\\twidth: 100%;\\n\\t\\t\\t\\theight: 100%;\\n\\t\\t\\t\\tfont-size: 1.25em;\\n\\t\\t\\t}\\n\\n\\t\\t\\t@media screen and (max-width: 1080px) {\\n\\t\\t\\t\\tbody[data-speaker-layout=\\\"default\\\"] #speaker-controls {\\n\\t\\t\\t\\t\\tfont-size: 16px;\\n\\t\\t\\t\\t}\\n\\t\\t\\t}\\n\\n\\t\\t\\t@media screen and (max-width: 900px) {\\n\\t\\t\\t\\tbody[data-speaker-layout=\\\"default\\\"] #speaker-controls {\\n\\t\\t\\t\\t\\tfont-size: 14px;\\n\\t\\t\\t\\t}\\n\\t\\t\\t}\\n\\n\\t\\t\\t@media screen and (max-width: 800px) {\\n\\t\\t\\t\\tbody[data-speaker-layout=\\\"default\\\"] #speaker-controls {\\n\\t\\t\\t\\t\\tfont-size: 12px;\\n\\t\\t\\t\\t}\\n\\t\\t\\t}\\n\\n\\t\\t</style>\\n\\t</head>\\n\\n\\t<body>\\n\\n\\t\\t<div id=\\\"connection-status\\\">Loading speaker view...</div>\\n\\n\\t\\t<div id=\\\"current-slide\\\"></div>\\n\\t\\t<div id=\\\"upcoming-slide\\\"><span class=\\\"overlay-element label\\\">Upcoming</span></div>\\n\\t\\t<div id=\\\"speaker-controls\\\">\\n\\t\\t\\t<div class=\\\"speaker-controls-time\\\">\\n\\t\\t\\t\\t<h4 class=\\\"label\\\">Time <span class=\\\"reset-button\\\">Click to Reset</span></h4>\\n\\t\\t\\t\\t<div class=\\\"clock\\\">\\n\\t\\t\\t\\t\\t<span class=\\\"clock-value\\\">0:00 AM</span>\\n\\t\\t\\t\\t</div>\\n\\t\\t\\t\\t<div class=\\\"timer\\\">\\n\\t\\t\\t\\t\\t<span class=\\\"hours-value\\\">00</span><span class=\\\"minutes-value\\\">:00</span><span class=\\\"seconds-value\\\">:00</span>\\n\\t\\t\\t\\t</div>\\n\\t\\t\\t\\t<div class=\\\"clear\\\"></div>\\n\\n\\t\\t\\t\\t<h4 class=\\\"label pacing-title\\\" style=\\\"display: none\\\">Pacing \u2013 Time to finish current slide</h4>\\n\\t\\t\\t\\t<div class=\\\"pacing\\\" style=\\\"display: none\\\">\\n\\t\\t\\t\\t\\t<span class=\\\"hours-value\\\">00</span><span class=\\\"minutes-value\\\">:00</span><span class=\\\"seconds-value\\\">:00</span>\\n\\t\\t\\t\\t</div>\\n\\t\\t\\t</div>\\n\\n\\t\\t\\t<div class=\\\"speaker-controls-notes hidden\\\">\\n\\t\\t\\t\\t<h4 class=\\\"label\\\">Notes</h4>\\n\\t\\t\\t\\t<div class=\\\"value\\\"></div>\\n\\t\\t\\t</div>\\n\\t\\t</div>\\n\\t\\t<div id=\\\"speaker-layout\\\" class=\\\"overlay-element interactive\\\">\\n\\t\\t\\t<span class=\\\"speaker-layout-label\\\"></span>\\n\\t\\t\\t<select class=\\\"speaker-layout-dropdown\\\"></select>\\n\\t\\t</div>\\n\\n\\t\\t<script>\\n\\n\\t\\t\\t(function() {\\n\\n\\t\\t\\t\\tvar notes,\\n\\t\\t\\t\\t\\tnotesValue,\\n\\t\\t\\t\\t\\tcurrentState,\\n\\t\\t\\t\\t\\tcurrentSlide,\\n\\t\\t\\t\\t\\tupcomingSlide,\\n\\t\\t\\t\\t\\tlayoutLabel,\\n\\t\\t\\t\\t\\tlayoutDropdown,\\n\\t\\t\\t\\t\\tpendingCalls = {},\\n\\t\\t\\t\\t\\tlastRevealApiCallId = 0,\\n\\t\\t\\t\\t\\tconnected = false\\n\\n\\t\\t\\t\\tvar connectionStatus = document.querySelector( '#connection-status' );\\n\\n\\t\\t\\t\\tvar SPEAKER_LAYOUTS = {\\n\\t\\t\\t\\t\\t'default': 'Default',\\n\\t\\t\\t\\t\\t'wide': 'Wide',\\n\\t\\t\\t\\t\\t'tall': 'Tall',\\n\\t\\t\\t\\t\\t'notes-only': 'Notes only'\\n\\t\\t\\t\\t};\\n\\n\\t\\t\\t\\tsetupLayout();\\n\\n\\t\\t\\t\\tlet openerOrigin;\\n\\n\\t\\t\\t\\ttry {\\n\\t\\t\\t\\t\\topenerOrigin = window.opener.location.origin;\\n\\t\\t\\t\\t}\\n\\t\\t\\t\\tcatch ( error ) { console.warn( error ) }\\n\\n\\t\\t\\t\\t// In order to prevent XSS, the speaker view will only run if its\\n\\t\\t\\t\\t// opener has the same origin as itself\\n\\t\\t\\t\\tif( window.location.origin !== openerOrigin ) {\\n\\t\\t\\t\\t\\tconnectionStatus.innerHTML = 'Cross origin error.<br>The speaker window can only be opened from the same origin.';\\n\\t\\t\\t\\t\\treturn;\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\tvar connectionTimeout = setTimeout( function() {\\n\\t\\t\\t\\t\\tconnectionStatus.innerHTML = 'Error connecting to main window.<br>Please try closing and reopening the speaker view.';\\n\\t\\t\\t\\t}, 5000 );\\n\\n\\t\\t\\t\\twindow.addEventListener( 'message', function( event ) {\\n\\n\\t\\t\\t\\t\\tclearTimeout( connectionTimeout );\\n\\t\\t\\t\\t\\tconnectionStatus.style.display = 'none';\\n\\n\\t\\t\\t\\t\\tvar data = JSON.parse( event.data );\\n\\n\\t\\t\\t\\t\\t// The overview mode is only useful to the reveal.js instance\\n\\t\\t\\t\\t\\t// where navigation occurs so we don't sync it\\n\\t\\t\\t\\t\\tif( data.state ) delete data.state.overview;\\n\\n\\t\\t\\t\\t\\t// Messages sent by the notes plugin inside of the main window\\n\\t\\t\\t\\t\\tif( data && data.namespace === 'reveal-notes' ) {\\n\\t\\t\\t\\t\\t\\tif( data.type === 'connect' ) {\\n\\t\\t\\t\\t\\t\\t\\thandleConnectMessage( data );\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\telse if( data.type === 'state' ) {\\n\\t\\t\\t\\t\\t\\t\\thandleStateMessage( data );\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\telse if( data.type === 'return' ) {\\n\\t\\t\\t\\t\\t\\t\\tpendingCalls[data.callId](data.result);\\n\\t\\t\\t\\t\\t\\t\\tdelete pendingCalls[data.callId];\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t// Messages sent by the reveal.js inside of the current slide preview\\n\\t\\t\\t\\t\\telse if( data && data.namespace === 'reveal' ) {\\n\\t\\t\\t\\t\\t\\tif( /ready/.test( data.eventName ) ) {\\n\\t\\t\\t\\t\\t\\t\\t// Send a message back to notify that the handshake is complete\\n\\t\\t\\t\\t\\t\\t\\twindow.opener.postMessage( JSON.stringify({ namespace: 'reveal-notes', type: 'connected'} ), '*' );\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\telse if( /slidechanged|fragmentshown|fragmenthidden|paused|resumed/.test( data.eventName ) && currentState !== JSON.stringify( data.state ) ) {\\n\\n\\t\\t\\t\\t\\t\\t\\tdispatchStateToMainWindow( data.state );\\n\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t} );\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Updates the presentation in the main window to match the state\\n\\t\\t\\t\\t * of the presentation in the notes window.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tconst dispatchStateToMainWindow = debounce(( state ) => {\\n\\t\\t\\t\\t\\twindow.opener.postMessage( JSON.stringify({ method: 'setState', args: [ state ]} ), '*' );\\n\\t\\t\\t\\t}, 500);\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Asynchronously calls the Reveal.js API of the main frame.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction callRevealApi( methodName, methodArguments, callback ) {\\n\\n\\t\\t\\t\\t\\tvar callId = ++lastRevealApiCallId;\\n\\t\\t\\t\\t\\tpendingCalls[callId] = callback;\\n\\t\\t\\t\\t\\twindow.opener.postMessage( JSON.stringify( {\\n\\t\\t\\t\\t\\t\\tnamespace: 'reveal-notes',\\n\\t\\t\\t\\t\\t\\ttype: 'call',\\n\\t\\t\\t\\t\\t\\tcallId: callId,\\n\\t\\t\\t\\t\\t\\tmethodName: methodName,\\n\\t\\t\\t\\t\\t\\targuments: methodArguments\\n\\t\\t\\t\\t\\t} ), '*' );\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Called when the main window is trying to establish a\\n\\t\\t\\t\\t * connection.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction handleConnectMessage( data ) {\\n\\n\\t\\t\\t\\t\\tif( connected === false ) {\\n\\t\\t\\t\\t\\t\\tconnected = true;\\n\\n\\t\\t\\t\\t\\t\\tsetupIframes( data );\\n\\t\\t\\t\\t\\t\\tsetupKeyboard();\\n\\t\\t\\t\\t\\t\\tsetupNotes();\\n\\t\\t\\t\\t\\t\\tsetupTimer();\\n\\t\\t\\t\\t\\t\\tsetupHeartbeat();\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Called when the main window sends an updated state.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction handleStateMessage( data ) {\\n\\n\\t\\t\\t\\t\\t// Store the most recently set state to avoid circular loops\\n\\t\\t\\t\\t\\t// applying the same state\\n\\t\\t\\t\\t\\tcurrentState = JSON.stringify( data.state );\\n\\n\\t\\t\\t\\t\\t// No need for updating the notes in case of fragment changes\\n\\t\\t\\t\\t\\tif ( data.notes ) {\\n\\t\\t\\t\\t\\t\\tnotes.classList.remove( 'hidden' );\\n\\t\\t\\t\\t\\t\\tnotesValue.style.whiteSpace = data.whitespace;\\n\\t\\t\\t\\t\\t\\tif( data.markdown ) {\\n\\t\\t\\t\\t\\t\\t\\tnotesValue.innerHTML = marked( data.notes );\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\telse {\\n\\t\\t\\t\\t\\t\\t\\tnotesValue.innerHTML = data.notes;\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\telse {\\n\\t\\t\\t\\t\\t\\tnotes.classList.add( 'hidden' );\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t\\t// Update the note slides\\n\\t\\t\\t\\t\\tcurrentSlide.contentWindow.postMessage( JSON.stringify({ method: 'setState', args: [ data.state ] }), '*' );\\n\\t\\t\\t\\t\\tupcomingSlide.contentWindow.postMessage( JSON.stringify({ method: 'setState', args: [ data.state ] }), '*' );\\n\\t\\t\\t\\t\\tupcomingSlide.contentWindow.postMessage( JSON.stringify({ method: 'next' }), '*' );\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t// Limit to max one state update per X ms\\n\\t\\t\\t\\thandleStateMessage = debounce( handleStateMessage, 200 );\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Forward keyboard events to the current slide window.\\n\\t\\t\\t\\t * This enables keyboard events to work even if focus\\n\\t\\t\\t\\t * isn't set on the current slide iframe.\\n\\t\\t\\t\\t *\\n\\t\\t\\t\\t * Block F5 default handling, it reloads and disconnects\\n\\t\\t\\t\\t * the speaker notes window.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction setupKeyboard() {\\n\\n\\t\\t\\t\\t\\tdocument.addEventListener( 'keydown', function( event ) {\\n\\t\\t\\t\\t\\t\\tif( event.keyCode === 116 || ( event.metaKey && event.keyCode === 82 ) ) {\\n\\t\\t\\t\\t\\t\\t\\tevent.preventDefault();\\n\\t\\t\\t\\t\\t\\t\\treturn false;\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\tcurrentSlide.contentWindow.postMessage( JSON.stringify({ method: 'triggerKey', args: [ event.keyCode ] }), '*' );\\n\\t\\t\\t\\t\\t} );\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Creates the preview iframes.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction setupIframes( data ) {\\n\\n\\t\\t\\t\\t\\tvar params = [\\n\\t\\t\\t\\t\\t\\t'receiver',\\n\\t\\t\\t\\t\\t\\t'progress=false',\\n\\t\\t\\t\\t\\t\\t'history=false',\\n\\t\\t\\t\\t\\t\\t'transition=none',\\n\\t\\t\\t\\t\\t\\t'autoSlide=0',\\n\\t\\t\\t\\t\\t\\t'backgroundTransition=none'\\n\\t\\t\\t\\t\\t].join( '&' );\\n\\n\\t\\t\\t\\t\\tvar urlSeparator = /\\\\?/.test(data.url) ? '&' : '?';\\n\\t\\t\\t\\t\\tvar hash = '#/' + data.state.indexh + '/' + data.state.indexv;\\n\\t\\t\\t\\t\\tvar currentURL = data.url + urlSeparator + params + '&postMessageEvents=true' + hash;\\n\\t\\t\\t\\t\\tvar upcomingURL = data.url + urlSeparator + params + '&controls=false' + hash;\\n\\n\\t\\t\\t\\t\\tcurrentSlide = document.createElement( 'iframe' );\\n\\t\\t\\t\\t\\tcurrentSlide.setAttribute( 'width', 1280 );\\n\\t\\t\\t\\t\\tcurrentSlide.setAttribute( 'height', 1024 );\\n\\t\\t\\t\\t\\tcurrentSlide.setAttribute( 'src', currentURL );\\n\\t\\t\\t\\t\\tdocument.querySelector( '#current-slide' ).appendChild( currentSlide );\\n\\n\\t\\t\\t\\t\\tupcomingSlide = document.createElement( 'iframe' );\\n\\t\\t\\t\\t\\tupcomingSlide.setAttribute( 'width', 640 );\\n\\t\\t\\t\\t\\tupcomingSlide.setAttribute( 'height', 512 );\\n\\t\\t\\t\\t\\tupcomingSlide.setAttribute( 'src', upcomingURL );\\n\\t\\t\\t\\t\\tdocument.querySelector( '#upcoming-slide' ).appendChild( upcomingSlide );\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Setup the notes UI.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction setupNotes() {\\n\\n\\t\\t\\t\\t\\tnotes = document.querySelector( '.speaker-controls-notes' );\\n\\t\\t\\t\\t\\tnotesValue = document.querySelector( '.speaker-controls-notes .value' );\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * We send out a heartbeat at all times to ensure we can\\n\\t\\t\\t\\t * reconnect with the main presentation window after reloads.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction setupHeartbeat() {\\n\\n\\t\\t\\t\\t\\tsetInterval( () => {\\n\\t\\t\\t\\t\\t\\twindow.opener.postMessage( JSON.stringify({ namespace: 'reveal-notes', type: 'heartbeat'} ), '*' );\\n\\t\\t\\t\\t\\t}, 1000 );\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\tfunction getTimings( callback ) {\\n\\n\\t\\t\\t\\t\\tcallRevealApi( 'getSlidesAttributes', [], function ( slideAttributes ) {\\n\\t\\t\\t\\t\\t\\tcallRevealApi( 'getConfig', [], function ( config ) {\\n\\t\\t\\t\\t\\t\\t\\tvar totalTime = config.totalTime;\\n\\t\\t\\t\\t\\t\\t\\tvar minTimePerSlide = config.minimumTimePerSlide || 0;\\n\\t\\t\\t\\t\\t\\t\\tvar defaultTiming = config.defaultTiming;\\n\\t\\t\\t\\t\\t\\t\\tif ((defaultTiming == null) && (totalTime == null)) {\\n\\t\\t\\t\\t\\t\\t\\t\\tcallback(null);\\n\\t\\t\\t\\t\\t\\t\\t\\treturn;\\n\\t\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\t\\t// Setting totalTime overrides defaultTiming\\n\\t\\t\\t\\t\\t\\t\\tif (totalTime) {\\n\\t\\t\\t\\t\\t\\t\\t\\tdefaultTiming = 0;\\n\\t\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\t\\tvar timings = [];\\n\\t\\t\\t\\t\\t\\t\\tfor ( var i in slideAttributes ) {\\n\\t\\t\\t\\t\\t\\t\\t\\tvar slide = slideAttributes[ i ];\\n\\t\\t\\t\\t\\t\\t\\t\\tvar timing = defaultTiming;\\n\\t\\t\\t\\t\\t\\t\\t\\tif( slide.hasOwnProperty( 'data-timing' )) {\\n\\t\\t\\t\\t\\t\\t\\t\\t\\tvar t = slide[ 'data-timing' ];\\n\\t\\t\\t\\t\\t\\t\\t\\t\\ttiming = parseInt(t);\\n\\t\\t\\t\\t\\t\\t\\t\\t\\tif( isNaN(timing) ) {\\n\\t\\t\\t\\t\\t\\t\\t\\t\\t\\tconsole.warn(\\\"Could not parse timing '\\\" + t + \\\"' of slide \\\" + i + \\\"; using default of \\\" + defaultTiming);\\n\\t\\t\\t\\t\\t\\t\\t\\t\\t\\ttiming = defaultTiming;\\n\\t\\t\\t\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\t\\t\\ttimings.push(timing);\\n\\t\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\t\\tif ( totalTime ) {\\n\\t\\t\\t\\t\\t\\t\\t\\t// After we've allocated time to individual slides, we summarize it and\\n\\t\\t\\t\\t\\t\\t\\t\\t// subtract it from the total time\\n\\t\\t\\t\\t\\t\\t\\t\\tvar remainingTime = totalTime - timings.reduce( function(a, b) { return a + b; }, 0 );\\n\\t\\t\\t\\t\\t\\t\\t\\t// The remaining time is divided by the number of slides that have 0 seconds\\n\\t\\t\\t\\t\\t\\t\\t\\t// allocated at the moment, giving the average time-per-slide on the remaining slides\\n\\t\\t\\t\\t\\t\\t\\t\\tvar remainingSlides = (timings.filter( function(x) { return x == 0 }) ).length\\n\\t\\t\\t\\t\\t\\t\\t\\tvar timePerSlide = Math.round( remainingTime / remainingSlides, 0 )\\n\\t\\t\\t\\t\\t\\t\\t\\t// And now we replace every zero-value timing with that average\\n\\t\\t\\t\\t\\t\\t\\t\\ttimings = timings.map( function(x) { return (x==0 ? timePerSlide : x) } );\\n\\t\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\t\\tvar slidesUnderMinimum = timings.filter( function(x) { return (x < minTimePerSlide) } ).length\\n\\t\\t\\t\\t\\t\\t\\tif ( slidesUnderMinimum ) {\\n\\t\\t\\t\\t\\t\\t\\t\\tmessage = \\\"The pacing time for \\\" + slidesUnderMinimum + \\\" slide(s) is under the configured minimum of \\\" + minTimePerSlide + \\\" seconds. Check the data-timing attribute on individual slides, or consider increasing the totalTime or minimumTimePerSlide configuration options (or removing some slides).\\\";\\n\\t\\t\\t\\t\\t\\t\\t\\talert(message);\\n\\t\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\t\\tcallback( timings );\\n\\t\\t\\t\\t\\t\\t} );\\n\\t\\t\\t\\t\\t} );\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Return the number of seconds allocated for presenting\\n\\t\\t\\t\\t * all slides up to and including this one.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction getTimeAllocated( timings, callback ) {\\n\\n\\t\\t\\t\\t\\tcallRevealApi( 'getSlidePastCount', [], function ( currentSlide ) {\\n\\t\\t\\t\\t\\t\\tvar allocated = 0;\\n\\t\\t\\t\\t\\t\\tfor (var i in timings.slice(0, currentSlide + 1)) {\\n\\t\\t\\t\\t\\t\\t\\tallocated += timings[i];\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\tcallback( allocated );\\n\\t\\t\\t\\t\\t} );\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Create the timer and clock and start updating them\\n\\t\\t\\t\\t * at an interval.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction setupTimer() {\\n\\n\\t\\t\\t\\t\\tvar start = new Date(),\\n\\t\\t\\t\\t\\ttimeEl = document.querySelector( '.speaker-controls-time' ),\\n\\t\\t\\t\\t\\tclockEl = timeEl.querySelector( '.clock-value' ),\\n\\t\\t\\t\\t\\thoursEl = timeEl.querySelector( '.hours-value' ),\\n\\t\\t\\t\\t\\tminutesEl = timeEl.querySelector( '.minutes-value' ),\\n\\t\\t\\t\\t\\tsecondsEl = timeEl.querySelector( '.seconds-value' ),\\n\\t\\t\\t\\t\\tpacingTitleEl = timeEl.querySelector( '.pacing-title' ),\\n\\t\\t\\t\\t\\tpacingEl = timeEl.querySelector( '.pacing' ),\\n\\t\\t\\t\\t\\tpacingHoursEl = pacingEl.querySelector( '.hours-value' ),\\n\\t\\t\\t\\t\\tpacingMinutesEl = pacingEl.querySelector( '.minutes-value' ),\\n\\t\\t\\t\\t\\tpacingSecondsEl = pacingEl.querySelector( '.seconds-value' );\\n\\n\\t\\t\\t\\t\\tvar timings = null;\\n\\t\\t\\t\\t\\tgetTimings( function ( _timings ) {\\n\\n\\t\\t\\t\\t\\t\\ttimings = _timings;\\n\\t\\t\\t\\t\\t\\tif (_timings !== null) {\\n\\t\\t\\t\\t\\t\\t\\tpacingTitleEl.style.removeProperty('display');\\n\\t\\t\\t\\t\\t\\t\\tpacingEl.style.removeProperty('display');\\n\\t\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t\\t\\t// Update once directly\\n\\t\\t\\t\\t\\t\\t_updateTimer();\\n\\n\\t\\t\\t\\t\\t\\t// Then update every second\\n\\t\\t\\t\\t\\t\\tsetInterval( _updateTimer, 1000 );\\n\\n\\t\\t\\t\\t\\t} );\\n\\n\\n\\t\\t\\t\\t\\tfunction _resetTimer() {\\n\\n\\t\\t\\t\\t\\t\\tif (timings == null) {\\n\\t\\t\\t\\t\\t\\t\\tstart = new Date();\\n\\t\\t\\t\\t\\t\\t\\t_updateTimer();\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\telse {\\n\\t\\t\\t\\t\\t\\t\\t// Reset timer to beginning of current slide\\n\\t\\t\\t\\t\\t\\t\\tgetTimeAllocated( timings, function ( slideEndTimingSeconds ) {\\n\\t\\t\\t\\t\\t\\t\\t\\tvar slideEndTiming = slideEndTimingSeconds * 1000;\\n\\t\\t\\t\\t\\t\\t\\t\\tcallRevealApi( 'getSlidePastCount', [], function ( currentSlide ) {\\n\\t\\t\\t\\t\\t\\t\\t\\t\\tvar currentSlideTiming = timings[currentSlide] * 1000;\\n\\t\\t\\t\\t\\t\\t\\t\\t\\tvar previousSlidesTiming = slideEndTiming - currentSlideTiming;\\n\\t\\t\\t\\t\\t\\t\\t\\t\\tvar now = new Date();\\n\\t\\t\\t\\t\\t\\t\\t\\t\\tstart = new Date(now.getTime() - previousSlidesTiming);\\n\\t\\t\\t\\t\\t\\t\\t\\t\\t_updateTimer();\\n\\t\\t\\t\\t\\t\\t\\t\\t} );\\n\\t\\t\\t\\t\\t\\t\\t} );\\n\\t\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t\\ttimeEl.addEventListener( 'click', function() {\\n\\t\\t\\t\\t\\t\\t_resetTimer();\\n\\t\\t\\t\\t\\t\\treturn false;\\n\\t\\t\\t\\t\\t} );\\n\\n\\t\\t\\t\\t\\tfunction _displayTime( hrEl, minEl, secEl, time) {\\n\\n\\t\\t\\t\\t\\t\\tvar sign = Math.sign(time) == -1 ? \\\"-\\\" : \\\"\\\";\\n\\t\\t\\t\\t\\t\\ttime = Math.abs(Math.round(time / 1000));\\n\\t\\t\\t\\t\\t\\tvar seconds = time % 60;\\n\\t\\t\\t\\t\\t\\tvar minutes = Math.floor( time / 60 ) % 60 ;\\n\\t\\t\\t\\t\\t\\tvar hours = Math.floor( time / ( 60 * 60 )) ;\\n\\t\\t\\t\\t\\t\\thrEl.innerHTML = sign + zeroPadInteger( hours );\\n\\t\\t\\t\\t\\t\\tif (hours == 0) {\\n\\t\\t\\t\\t\\t\\t\\thrEl.classList.add( 'mute' );\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\telse {\\n\\t\\t\\t\\t\\t\\t\\thrEl.classList.remove( 'mute' );\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\tminEl.innerHTML = ':' + zeroPadInteger( minutes );\\n\\t\\t\\t\\t\\t\\tif (hours == 0 && minutes == 0) {\\n\\t\\t\\t\\t\\t\\t\\tminEl.classList.add( 'mute' );\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\telse {\\n\\t\\t\\t\\t\\t\\t\\tminEl.classList.remove( 'mute' );\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\tsecEl.innerHTML = ':' + zeroPadInteger( seconds );\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t\\tfunction _updateTimer() {\\n\\n\\t\\t\\t\\t\\t\\tvar diff, hours, minutes, seconds,\\n\\t\\t\\t\\t\\t\\tnow = new Date();\\n\\n\\t\\t\\t\\t\\t\\tdiff = now.getTime() - start.getTime();\\n\\n\\t\\t\\t\\t\\t\\tclockEl.innerHTML = now.toLocaleTimeString( 'en-US', { hour12: true, hour: '2-digit', minute:'2-digit' } );\\n\\t\\t\\t\\t\\t\\t_displayTime( hoursEl, minutesEl, secondsEl, diff );\\n\\t\\t\\t\\t\\t\\tif (timings !== null) {\\n\\t\\t\\t\\t\\t\\t\\t_updatePacing(diff);\\n\\t\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t\\tfunction _updatePacing(diff) {\\n\\n\\t\\t\\t\\t\\t\\tgetTimeAllocated( timings, function ( slideEndTimingSeconds ) {\\n\\t\\t\\t\\t\\t\\t\\tvar slideEndTiming = slideEndTimingSeconds * 1000;\\n\\n\\t\\t\\t\\t\\t\\t\\tcallRevealApi( 'getSlidePastCount', [], function ( currentSlide ) {\\n\\t\\t\\t\\t\\t\\t\\t\\tvar currentSlideTiming = timings[currentSlide] * 1000;\\n\\t\\t\\t\\t\\t\\t\\t\\tvar timeLeftCurrentSlide = slideEndTiming - diff;\\n\\t\\t\\t\\t\\t\\t\\t\\tif (timeLeftCurrentSlide < 0) {\\n\\t\\t\\t\\t\\t\\t\\t\\t\\tpacingEl.className = 'pacing behind';\\n\\t\\t\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\t\\t\\telse if (timeLeftCurrentSlide < currentSlideTiming) {\\n\\t\\t\\t\\t\\t\\t\\t\\t\\tpacingEl.className = 'pacing on-track';\\n\\t\\t\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\t\\t\\telse {\\n\\t\\t\\t\\t\\t\\t\\t\\t\\tpacingEl.className = 'pacing ahead';\\n\\t\\t\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\t\\t\\t_displayTime( pacingHoursEl, pacingMinutesEl, pacingSecondsEl, timeLeftCurrentSlide );\\n\\t\\t\\t\\t\\t\\t\\t} );\\n\\t\\t\\t\\t\\t\\t} );\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Sets up the speaker view layout and layout selector.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction setupLayout() {\\n\\n\\t\\t\\t\\t\\tlayoutDropdown = document.querySelector( '.speaker-layout-dropdown' );\\n\\t\\t\\t\\t\\tlayoutLabel = document.querySelector( '.speaker-layout-label' );\\n\\n\\t\\t\\t\\t\\t// Render the list of available layouts\\n\\t\\t\\t\\t\\tfor( var id in SPEAKER_LAYOUTS ) {\\n\\t\\t\\t\\t\\t\\tvar option = document.createElement( 'option' );\\n\\t\\t\\t\\t\\t\\toption.setAttribute( 'value', id );\\n\\t\\t\\t\\t\\t\\toption.textContent = SPEAKER_LAYOUTS[ id ];\\n\\t\\t\\t\\t\\t\\tlayoutDropdown.appendChild( option );\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t\\t// Monitor the dropdown for changes\\n\\t\\t\\t\\t\\tlayoutDropdown.addEventListener( 'change', function( event ) {\\n\\n\\t\\t\\t\\t\\t\\tsetLayout( layoutDropdown.value );\\n\\n\\t\\t\\t\\t\\t}, false );\\n\\n\\t\\t\\t\\t\\t// Restore any currently persisted layout\\n\\t\\t\\t\\t\\tsetLayout( getLayout() );\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Sets a new speaker view layout. The layout is persisted\\n\\t\\t\\t\\t * in local storage.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction setLayout( value ) {\\n\\n\\t\\t\\t\\t\\tvar title = SPEAKER_LAYOUTS[ value ];\\n\\n\\t\\t\\t\\t\\tlayoutLabel.innerHTML = 'Layout' + ( title ? ( ': ' + title ) : '' );\\n\\t\\t\\t\\t\\tlayoutDropdown.value = value;\\n\\n\\t\\t\\t\\t\\tdocument.body.setAttribute( 'data-speaker-layout', value );\\n\\n\\t\\t\\t\\t\\t// Persist locally\\n\\t\\t\\t\\t\\tif( supportsLocalStorage() ) {\\n\\t\\t\\t\\t\\t\\twindow.localStorage.setItem( 'reveal-speaker-layout', value );\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Returns the ID of the most recently set speaker layout\\n\\t\\t\\t\\t * or our default layout if none has been set.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction getLayout() {\\n\\n\\t\\t\\t\\t\\tif( supportsLocalStorage() ) {\\n\\t\\t\\t\\t\\t\\tvar layout = window.localStorage.getItem( 'reveal-speaker-layout' );\\n\\t\\t\\t\\t\\t\\tif( layout ) {\\n\\t\\t\\t\\t\\t\\t\\treturn layout;\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t\\t// Default to the first record in the layouts hash\\n\\t\\t\\t\\t\\tfor( var id in SPEAKER_LAYOUTS ) {\\n\\t\\t\\t\\t\\t\\treturn id;\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\tfunction supportsLocalStorage() {\\n\\n\\t\\t\\t\\t\\ttry {\\n\\t\\t\\t\\t\\t\\tlocalStorage.setItem('test', 'test');\\n\\t\\t\\t\\t\\t\\tlocalStorage.removeItem('test');\\n\\t\\t\\t\\t\\t\\treturn true;\\n\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\tcatch( e ) {\\n\\t\\t\\t\\t\\t\\treturn false;\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\tfunction zeroPadInteger( num ) {\\n\\n\\t\\t\\t\\t\\tvar str = '00' + parseInt( num );\\n\\t\\t\\t\\t\\treturn str.substring( str.length - 2 );\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t/**\\n\\t\\t\\t\\t * Limits the frequency at which a function can be called.\\n\\t\\t\\t\\t */\\n\\t\\t\\t\\tfunction debounce( fn, ms ) {\\n\\n\\t\\t\\t\\t\\tvar lastTime = 0,\\n\\t\\t\\t\\t\\t\\ttimeout;\\n\\n\\t\\t\\t\\t\\treturn function() {\\n\\n\\t\\t\\t\\t\\t\\tvar args = arguments;\\n\\t\\t\\t\\t\\t\\tvar context = this;\\n\\n\\t\\t\\t\\t\\t\\tclearTimeout( timeout );\\n\\n\\t\\t\\t\\t\\t\\tvar timeSinceLastCall = Date.now() - lastTime;\\n\\t\\t\\t\\t\\t\\tif( timeSinceLastCall > ms ) {\\n\\t\\t\\t\\t\\t\\t\\tfn.apply( context, args );\\n\\t\\t\\t\\t\\t\\t\\tlastTime = Date.now();\\n\\t\\t\\t\\t\\t\\t}\\n\\t\\t\\t\\t\\t\\telse {\\n\\t\\t\\t\\t\\t\\t\\ttimeout = setTimeout( function() {\\n\\t\\t\\t\\t\\t\\t\\t\\tfn.apply( context, args );\\n\\t\\t\\t\\t\\t\\t\\t\\tlastTime = Date.now();\\n\\t\\t\\t\\t\\t\\t\\t}, ms - timeSinceLastCall );\\n\\t\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t\\t}\\n\\n\\t\\t\\t\\t}\\n\\n\\t\\t\\t})();\\n\\n\\t\\t<\\/script>\\n\\t</body>\\n</html>\"),!n)return void alert(\"Speaker view popup failed to open. Please make sure popups are allowed and reopen the speaker view.\");!function(){const i=e.getConfig().url,s=\"string\"==typeof i?i:window.location.protocol+\"//\"+window.location.host+window.location.pathname+window.location.search;t=setInterval((function(){n.postMessage(JSON.stringify({namespace:\"reveal-notes\",type:\"connect\",state:e.getState(),url:s}),\"*\")}),500),window.addEventListener(\"message\",r)}()}}function s(t){let i=e.getCurrentSlide(),s=i.querySelectorAll(\"aside.notes\"),r=i.querySelector(\".current-fragment\"),a={namespace:\"reveal-notes\",type:\"state\",notes:\"\",markdown:!1,whitespace:\"normal\",state:e.getState()};if(i.hasAttribute(\"data-notes\")&&(a.notes=i.getAttribute(\"data-notes\"),a.whitespace=\"pre-wrap\"),r){let t=r.querySelector(\"aside.notes\");t?(a.notes=t.innerHTML,a.markdown=\"string\"==typeof t.getAttribute(\"data-markdown\"),s=null):r.hasAttribute(\"data-notes\")&&(a.notes=r.getAttribute(\"data-notes\"),a.whitespace=\"pre-wrap\",s=null)}s&&(a.notes=Array.from(s).map((t=>t.innerHTML)).join(\"\\n\"),a.markdown=s[0]&&\"string\"==typeof s[0].getAttribute(\"data-markdown\")),n.postMessage(JSON.stringify(a),\"*\")}function r(i){if(function(t){try{return window.location.origin===t.source.location.origin}catch(t){return!1}}(i)){let s=JSON.parse(i.data);s&&\"reveal-notes\"===s.namespace&&\"connected\"===s.type?(clearInterval(t),a()):s&&\"reveal-notes\"===s.namespace&&\"call\"===s.type&&function(t,i,s){let r=e[t].apply(e,i);n.postMessage(JSON.stringify({namespace:\"reveal-notes\",type:\"return\",result:r,callId:s}),\"*\")}(s.methodName,s.arguments,s.callId)}}function a(){e.on(\"slidechanged\",s),e.on(\"fragmentshown\",s),e.on(\"fragmenthidden\",s),e.on(\"overviewhidden\",s),e.on(\"overviewshown\",s),e.on(\"paused\",s),e.on(\"resumed\",s),s()}return{id:\"notes\",init:function(t){e=t,/receiver/i.test(window.location.search)||(null!==window.location.search.match(/(\\?|\\&)notes/gi)?i():window.addEventListener(\"message\",(t=>{if(!n&&\"string\"==typeof t.data){let i;try{i=JSON.parse(t.data)}catch(t){}i&&\"reveal-notes\"===i.namespace&&\"heartbeat\"===i.type&&(e=t.source,n&&!n.closed?n.focus():(n=e,window.addEventListener(\"message\",r),a()))}var e})),e.addKeyBinding({keyCode:83,key:\"S\",description:\"Speaker notes view\"},(function(){i()})))},open:i}}}));\n",
         "!function(e,t){\"object\"==typeof exports&&\"undefined\"!=typeof module?module.exports=t():\"function\"==typeof define&&define.amd?define(t):(e=\"undefined\"!=typeof globalThis?globalThis:e||self).RevealZoom=t()}(this,(function(){\"use strict\";\n/*!\n\t * reveal.js Zoom plugin\n\t */const e={id:\"zoom\",init:function(e){e.getRevealElement().addEventListener(\"mousedown\",(function(o){var n=/Linux/.test(window.navigator.platform)?\"ctrl\":\"alt\",i=(e.getConfig().zoomKey?e.getConfig().zoomKey:n)+\"Key\",d=e.getConfig().zoomLevel?e.getConfig().zoomLevel:2;o[i]&&!e.isOverview()&&(o.preventDefault(),t.to({x:o.clientX,y:o.clientY,scale:d,pan:!1}))}))},destroy:()=>{t.reset()}};var t=function(){var e=1,o=0,n=0,i=-1,d=-1,l=\"transform\"in document.body.style;function s(t,o){var n=r();if(t.width=t.width||1,t.height=t.height||1,t.x-=(window.innerWidth-t.width*o)/2,t.y-=(window.innerHeight-t.height*o)/2,l)if(1===o)document.body.style.transform=\"\";else{var i=n.x+\"px \"+n.y+\"px\",d=\"translate(\"+-t.x+\"px,\"+-t.y+\"px) scale(\"+o+\")\";document.body.style.transformOrigin=i,document.body.style.transform=d}else 1===o?(document.body.style.position=\"\",document.body.style.left=\"\",document.body.style.top=\"\",document.body.style.width=\"\",document.body.style.height=\"\",document.body.style.zoom=\"\"):(document.body.style.position=\"relative\",document.body.style.left=-(n.x+t.x)/o+\"px\",document.body.style.top=-(n.y+t.y)/o+\"px\",document.body.style.width=100*o+\"%\",document.body.style.height=100*o+\"%\",document.body.style.zoom=o);e=o,document.documentElement.classList&&(1!==e?document.documentElement.classList.add(\"zoomed\"):document.documentElement.classList.remove(\"zoomed\"))}function c(){var t=.12*window.innerWidth,i=.12*window.innerHeight,d=r();n<i?window.scroll(d.x,d.y-14/e*(1-n/i)):n>window.innerHeight-i&&window.scroll(d.x,d.y+(1-(window.innerHeight-n)/i)*(14/e)),o<t?window.scroll(d.x-14/e*(1-o/t),d.y):o>window.innerWidth-t&&window.scroll(d.x+(1-(window.innerWidth-o)/t)*(14/e),d.y)}function r(){return{x:void 0!==window.scrollX?window.scrollX:window.pageXOffset,y:void 0!==window.scrollY?window.scrollY:window.pageYOffset}}return l&&(document.body.style.transition=\"transform 0.8s ease\"),document.addEventListener(\"keyup\",(function(o){1!==e&&27===o.keyCode&&t.out()})),document.addEventListener(\"mousemove\",(function(t){1!==e&&(o=t.clientX,n=t.clientY)})),{to:function(o){if(1!==e)t.out();else{if(o.x=o.x||0,o.y=o.y||0,o.element){var n=o.element.getBoundingClientRect();o.x=n.left-20,o.y=n.top-20,o.width=n.width+40,o.height=n.height+40}void 0!==o.width&&void 0!==o.height&&(o.scale=Math.max(Math.min(window.innerWidth/o.width,window.innerHeight/o.height),1)),o.scale>1&&(o.x*=o.scale,o.y*=o.scale,s(o,o.scale),!1!==o.pan&&(i=setTimeout((function(){d=setInterval(c,1e3/60)}),800)))}},out:function(){clearTimeout(i),clearInterval(d),s({x:0,y:0},1),e=1},magnify:function(e){this.to(e)},reset:function(){this.out()},zoomLevel:function(){return e}}}();\n/*!\n\t * zoom.js 0.3 (modified for use with reveal.js)\n\t * http://lab.hakim.se/zoom-js\n\t * MIT licensed\n\t *\n\t * Copyright (C) 2011-2014 Hakim El Hattab, http://hakim.se\n\t */return()=>e}));\n",
         "// @flow\nimport type { Interpolation } from '../types';\n\nexport default (\n  strings: Array<string>,\n  interpolations: Array<Interpolation>\n): Array<Interpolation> => {\n  const result = [strings[0]];\n\n  for (let i = 0, len = interpolations.length; i < len; i += 1) {\n    result.push(interpolations[i], strings[i + 1]);\n  }\n\n  return result;\n};\n",
         "// @flow\nimport { typeOf } from 'react-is';\n\nexport default (x: any): boolean =>\n  x !== null &&\n  typeof x === 'object' &&\n  (x.toString ? x.toString() : Object.prototype.toString.call(x)) === '[object Object]' &&\n  !typeOf(x);\n",
         "// @flow\nexport const EMPTY_ARRAY = Object.freeze([]);\nexport const EMPTY_OBJECT = Object.freeze({});\n",
```

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/main.639deb8d.chunk.js` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/main.18f5a848.chunk.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,28 @@
 (this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || []).push([
     [0], {
-        71: function(e, t, n) {
+        72: function(e, t, n) {
             var a = {
-                "./beige.css": [73, 3],
-                "./black-contrast.css": [74, 10],
-                "./black.css": [75, 11],
-                "./blood.css": [76, 12],
-                "./dracula.css": [77, 16],
-                "./fonts/league-gothic/league-gothic.css": [78, 17],
-                "./fonts/source-sans-pro/source-sans-pro.css": [79, 18],
-                "./league.css": [80, 4],
-                "./moon.css": [81, 5],
-                "./night.css": [82, 6],
-                "./serif.css": [83, 19],
-                "./simple.css": [84, 7],
-                "./sky.css": [85, 8],
-                "./solarized.css": [86, 9],
-                "./white-contrast.css": [87, 13],
-                "./white.css": [88, 14],
-                "./white_contrast_compact_verbatim_headers.css": [89, 15]
+                "./beige.css": [74, 3],
+                "./black-contrast.css": [75, 10],
+                "./black.css": [76, 11],
+                "./blood.css": [77, 12],
+                "./dracula.css": [78, 16],
+                "./fonts/league-gothic/league-gothic.css": [79, 17],
+                "./fonts/source-sans-pro/source-sans-pro.css": [80, 18],
+                "./league.css": [81, 4],
+                "./moon.css": [82, 5],
+                "./night.css": [83, 6],
+                "./serif.css": [84, 19],
+                "./simple.css": [85, 7],
+                "./sky.css": [86, 8],
+                "./solarized.css": [87, 9],
+                "./white-contrast.css": [88, 13],
+                "./white.css": [89, 14],
+                "./white_contrast_compact_verbatim_headers.css": [90, 15]
             };
 
             function s(e) {
                 if (!n.o(a, e)) return Promise.resolve().then((function() {
                     var t = new Error("Cannot find module '" + e + "'");
                     throw t.code = "MODULE_NOT_FOUND", t
                 }));
@@ -30,196 +30,197 @@
                     s = t[0];
                 return n.e(t[1]).then((function() {
                     return n.t(s, 7)
                 }))
             }
             s.keys = function() {
                 return Object.keys(a)
-            }, s.id = 71, e.exports = s
+            }, s.id = 72, e.exports = s
         },
-        72: function(e, t, n) {
+        73: function(e, t, n) {
             "use strict";
             n.r(t);
             var a = n(6),
                 s = n.n(a),
                 i = n(34),
                 o = n.n(i),
                 c = n(5),
-                r = n(39),
+                r = n(40),
                 u = n(10),
-                l = n(7),
-                f = n(15),
-                g = n.n(f),
-                h = n(35),
-                d = n.n(h),
-                m = n(20),
-                p = n.n(m),
-                v = n(36),
-                j = n.n(v),
-                b = n(37),
-                O = n.n(b),
-                y = n(38),
-                x = n.n(y),
-                w = (n(67), n(68), n(9)),
-                S = Object(r.a)(["", ""], (function(e) {
+                l = n(35),
+                f = n(7),
+                h = n(15),
+                g = n.n(h),
+                d = n(36),
+                m = n.n(d),
+                p = n(20),
+                v = n.n(p),
+                j = n(37),
+                b = n.n(j),
+                O = n(38),
+                x = n.n(O),
+                y = n(39),
+                w = n.n(y),
+                S = (n(68), n(69), n(9)),
+                _ = Object(r.a)(["", ""], (function(e) {
                     return e.inject
                 })),
-                _ = {
+                k = {
                     markdown: g.a,
-                    highlight: d.a,
-                    katex: p.a.KaTeX,
-                    mathjax2: p.a.MathJax2,
-                    mathjax3: p.a.MathJax3,
-                    search: j.a,
-                    notes: O.a,
-                    zoom: x.a
+                    highlight: m.a,
+                    katex: v.a.KaTeX,
+                    mathjax2: v.a.MathJax2,
+                    mathjax3: v.a.MathJax3,
+                    search: b.a,
+                    notes: x.a,
+                    zoom: w.a
                 },
-                k = {
+                E = {
                     width: 900,
                     height: 860,
                     margin: .05,
                     minScale: .1,
                     maxScale: 3,
                     controlsTutorial: !0,
                     controlsLayout: "edges"
                 },
-                E = Object(u.b)((function(e) {
+                C = Object(u.b)((function(e) {
                     var t = e.args,
                         s = e.disabled,
                         i = JSON.stringify(t.config),
                         o = JSON.stringify(t.initial_state),
                         r = function(e) {
-                            var n, a = Object(c.a)(Object(c.a)({}, k), JSON.parse(i));
+                            var n, a = Object(c.a)(Object(c.a)({}, E), JSON.parse(i));
                             t.allow_unsafe_html ? "plugins" in a && ((n = a.plugins).forEach((function(e, t) {
-                                n[t] = e in _ ? _[e] : null
+                                n[t] = e in k ? k[e] : null
                             })), a.plugins = n.filter((function(e) {
                                 return !!e
                             }))) : "plugins" in a ? ((n = a.plugins).forEach((function(e, t) {
-                                n[t] = e in _ ? _[e] : null
+                                n[t] = e in k ? k[e] : null
                             })), a.plugins = n.filter((function(e) {
                                 return !!e
                             })), a.plugins.includes(g.a) || a.plugins.push(g.a)) : a.plugins = [g.a];
                             return a
                         };
                     Object(a.useMemo)((function() {
-                        n(71)("./" + t.theme + ".css").then((function(e) {
+                        n(72)("./" + t.theme + ".css").then((function(e) {
                             try {
-                                l.a.layout()
+                                f.a.layout()
                             } catch (t) {
                                 console.warn("Reveal.layout() call failed.")
                             }
                         })).catch((function(e) {
                             console.warn("Failed CSS import: ", e)
                         }))
                     }), [t.theme]), Object(a.useEffect)((function() {
                         var e = r();
                         try {
-                            l.a.destroy()
+                            f.a.destroy()
                         } catch (n) {}
-                        return l.a.initialize(e).then((function() {
-                                var e = l.a.getPlugin("highlight");
-                                e && e.init(l.a);
+                        return f.a.initialize(e).then((function() {
+                                var e = f.a.getPlugin("highlight");
+                                e && e.init(f.a);
                                 var n = JSON.parse(o);
-                                if (0 !== Object.keys(n).length && l.a.setState(n), !t.display_only) {
-                                    var a = l.a.getState();
-                                    u.a.setComponentValue(a), l.a.on("slidechanged", (function(e) {
-                                        var t = l.a.getState();
+                                if (0 !== Object.keys(n).length && f.a.setState(n), !t.display_only) {
+                                    var a = f.a.getState();
+                                    u.a.setComponentValue(a), f.a.on("slidechanged", (function(e) {
+                                        var t = f.a.getState();
                                         u.a.setComponentValue({
                                             indexh: e.indexh,
                                             indexv: e.indexv,
                                             indexf: t.indexf,
                                             paused: t.paused,
                                             overview: t.overview
                                         })
-                                    })), l.a.on("fragmentshown", (function(e) {
-                                        var t = l.a.getState();
+                                    })), f.a.on("fragmentshown", (function(e) {
+                                        var t = f.a.getState();
                                         u.a.setComponentValue(t)
-                                    })), l.a.on("fragmenthidden", (function(e) {
-                                        var t = l.a.getState();
+                                    })), f.a.on("fragmenthidden", (function(e) {
+                                        var t = f.a.getState();
                                         u.a.setComponentValue(t)
-                                    })), l.a.on("overviewshown", (function(e) {
-                                        var t = l.a.getState();
+                                    })), f.a.on("overviewshown", (function(e) {
+                                        var t = f.a.getState();
                                         u.a.setComponentValue(t)
-                                    })), l.a.on("overviewhidden", (function(e) {
-                                        var t = l.a.getState();
+                                    })), f.a.on("overviewhidden", (function(e) {
+                                        var t = f.a.getState();
                                         u.a.setComponentValue(t)
-                                    })), l.a.on("paused", (function(e) {
-                                        var t = l.a.getState();
+                                    })), f.a.on("paused", (function(e) {
+                                        var t = f.a.getState();
                                         u.a.setComponentValue(t)
-                                    })), l.a.on("resumed", (function(e) {
-                                        var t = l.a.getState();
+                                    })), f.a.on("resumed", (function(e) {
+                                        var t = f.a.getState();
                                         u.a.setComponentValue(t)
                                     }))
                                 }
                             })),
                             function() {
-                                l.a.destroy()
+                                f.a.destroy()
                             }
                     }), []), Object(a.useEffect)((function() {
-                        var e = l.a.getPlugins(),
+                        var e = f.a.getPlugins(),
                             n = r(),
                             a = Object.values(e).map((function(e) {
                                 return e.id
                             }));
                         "plugins" in t.config && t.config.plugins.forEach((function(e) {
-                            e && -1 === a.indexOf(e) && l.a.registerPlugin(_[e])
+                            e && -1 === a.indexOf(e) && f.a.registerPlugin(k[e])
                         }));
-                        l.a.configure(n)
+                        f.a.configure(n)
                     }), [i, t.allow_unsafe_html]), Object(a.useEffect)((function() {
                         var e = JSON.parse(o);
-                        l.a.isReady() && 0 !== Object.keys(e).length && l.a.setState(e)
+                        f.a.isReady() && 0 !== Object.keys(e).length && f.a.setState(e)
                     }), [o]), Object(a.useEffect)((function() {
-                        if (l.a.isReady())
+                        if (f.a.isReady())
                             if (s) {
-                                l.a.togglePause(!0);
-                                var e = l.a.getViewportElement();
+                                f.a.togglePause(!0);
+                                var e = f.a.getViewportElement();
                                 e && (e.style.pointerEvents = "none")
                             } else {
-                                l.a.togglePause(!1);
-                                var t = l.a.getViewportElement();
+                                f.a.togglePause(!1);
+                                var t = f.a.getViewportElement();
                                 t && (t.style.pointerEvents = "auto")
                             }
                     }), [s]);
-                    var f = new ResizeObserver((function(e) {
+                    var h = new ResizeObserver((function(e) {
                             var n;
-                            "auto" === t.height || "number" !== typeof t.height ? (u.a.setFrameHeight(null !== (n = e[0].contentBoxSize.blockSize) && void 0 !== n ? n : e[0].contentRect.height), l.a.isReady() && l.a.layout()) : (u.a.setFrameHeight(t.height), l.a.isReady() && l.a.layout())
+                            "auto" === t.height || "number" !== typeof t.height ? (u.a.setFrameHeight(null !== (n = e[0].contentBoxSize.blockSize) && void 0 !== n ? n : e[0].contentRect.height), f.a.isReady() && f.a.layout()) : (u.a.setFrameHeight(t.height), f.a.isReady() && f.a.layout())
                         })),
-                        h = function(e) {
-                            e ? f.observe(e) : f.disconnect()
+                        d = function(e) {
+                            e ? h.observe(e) : h.disconnect()
                         };
-                    return t.allow_unsafe_html ? Object(w.jsxs)(w.Fragment, {
-                        children: [Object(w.jsx)(S, {
+                    return t.allow_unsafe_html ? Object(S.jsxs)(S.Fragment, {
+                        children: [Object(S.jsx)(_, {
                             inject: t.css
-                        }), Object(w.jsx)("div", {
-                            ref: h,
+                        }), Object(S.jsx)("div", {
+                            ref: d,
                             className: "slides",
-                            dangerouslySetInnerHTML: {
-                                __html: t.content
-                            }
+                            children: Object(S.jsx)(l.a, {
+                                html: t.content
+                            })
                         })]
-                    }) : Object(w.jsxs)(w.Fragment, {
-                        children: [Object(w.jsx)(S, {
+                    }) : Object(S.jsxs)(S.Fragment, {
+                        children: [Object(S.jsx)(_, {
                             inject: t.css
-                        }), Object(w.jsx)("div", {
-                            ref: h,
+                        }), Object(S.jsx)("div", {
+                            ref: d,
                             className: "slides",
-                            children: Object(w.jsx)("section", Object(c.a)(Object(c.a)({
+                            children: Object(S.jsx)("section", Object(c.a)(Object(c.a)({
                                 "data-markdown": ""
                             }, t.markdown_props), {}, {
-                                children: Object(w.jsx)("script", {
+                                children: Object(S.jsx)("script", {
                                     type: "text/template",
                                     children: t.content
                                 })
                             }))
                         })]
                     })
                 }));
-            o.a.render(Object(w.jsx)(s.a.StrictMode, {
-                children: Object(w.jsx)(E, {})
+            o.a.render(Object(S.jsx)(s.a.StrictMode, {
+                children: Object(S.jsx)(C, {})
             }), document.getElementById("root"))
         }
     },
     [
-        [72, 1, 2]
+        [73, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.639deb8d.chunk.js.map
+//# sourceMappingURL=main.18f5a848.chunk.js.map
```

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/main.639deb8d.chunk.js.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/main.18f5a848.chunk.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.797867803837953%*

 * *Differences: {"'file'": "'static/js/main.18f5a848.chunk.js'",*

 * * "'mappings'": "'gIAAA,IAAIA,EAAM,CACT,cAAe,CACd,GACA,GAED,uBAAwB,CACvB,GACA,IAED,cAAe,CACd,GACA,IAED,cAAe,CACd,GACA,IAED,gBAAiB,CAChB,GACA,IAED,0CAA2C,CAC1C,GACA,IAED,8CAA+C,CAC9C,GACA,IAED,eAAgB,CACf,GACA,GAED,aAAc,CACb,GACA,GAED,cAAe,CACd,GACA,GAED,cAAe,CACd,GACA,IAED,eAAgB,CACf,GACA,GAED,YAAa,CACZ,GACA,GAED,kBAAmB,CAClB,GACA,GAED,uBAAwB,CACvB,GACA,IAED,cAAe,CACd,GACA,IAED,gDAAiD,CAChD,GACA,KAGF,SAASC,EAAoBC,GAC5B,IAAIC,EAAoBC,EAAEJ,EAAKE,GAC9B,OAAOG,QAAQC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.639deb8d.chunk.js",
-    "mappings": "gIAAA,IAAIA,EAAM,CACT,cAAe,CACd,GACA,GAED,uBAAwB,CACvB,GACA,IAED,cAAe,CACd,GACA,IAED,cAAe,CACd,GACA,IAED,gBAAiB,CAChB,GACA,IAED,0CAA2C,CAC1C,GACA,IAED,8CAA+C,CAC9C,GACA,IAED,eAAgB,CACf,GACA,GAED,aAAc,CACb,GACA,GAED,cAAe,CACd,GACA,GAED,cAAe,CACd,GACA,IAED,eAAgB,CACf,GACA,GAED,YAAa,CACZ,GACA,GAED,kBAAmB,CAClB,GACA,GAED,uBAAwB,CACvB,GACA,IAED,cAAe,CACd,GACA,IAED,gDAAiD,CAChD,GACA,KAGF,SAASC,EAAoBC,GAC5B,IAAIC,EAAoBC,EAAEJ,EAAKE,GAC9B,OAAOG,QAAQC,UAAUC,MAAK,WAC7B,IAAIC,EAAI,IAAIC,MAAM,uBAAyBP,EAAM,KAEjD,MADAM,EAAEE,KAAO,mBACHF,CACP,IAGD,IAAIG,EAAMX,EAAIE,GAAMU,EAAKD,EAAI,GAC7B,OAAOR,EAAoBK,EAAEG,EAAI,IAAIJ,MAAK,WACzC,OAAOJ,EAAoBU,EAAED,EAAI,EAClC,GACD,CACAX,EAAoBa,KAAO,WAC1B,OAAOC,OAAOD,KAAKd,EACpB,EACAC,EAAoBW,GAAK,GACzBI,EAAOC,QAAUhB,C,uOC5DXiB,EAAYC,YAAiB,SAC/B,SAAAC,GAAK,OAAIA,EAAMC,MAAM,IAGnBC,EAAkB,CAAC,SAAYC,IAAgB,UAAaC,IAAiB,MAASC,IAAWC,MAAO,SAAYD,IAAWE,SAAU,SAAYF,IAAWG,SAAU,OAAUC,IAAc,MAASC,IAAa,KAAQC,KAIhOC,EAAgB,CAGrBC,MAAO,IACPC,OAAQ,IAGRC,OAAQ,IAGRC,SAAU,GACVC,SAAU,EAIVC,kBAAkB,EAGlBC,eAAgB,SAwQFC,eAjQM,SAAHC,GAA+C,IAAzCC,EAAID,EAAJC,KAAMC,EAAQF,EAARE,SAExBC,EAAYC,KAAKC,UAAUJ,EAAa,QACxCK,EAAeF,KAAKC,UAAUJ,EAAoB,eAGhDM,EAAc,SAACC,GACnB,IAkBQC,EAlBFC,EAAMC,wBAAA,GAAOpB,GAAkBa,KAAKQ,MAAMT,IAE5CF,EAAwB,kBACtB,YAAaS,KACXD,EAAMC,EAAgB,SACtBG,SAAQ,SAASC,EAAoBC,GAErCN,EAAIM,GADFD,KAAcjC,EACFA,EAAwBiC,GAGzB,IAEjB,IACAJ,EAAgB,QAAID,EAAIO,QAAO,SAACC,GAAK,QAAOA,CAAC,KAI3C,YAAaP,IACXD,EAAMC,EAAgB,SACtBG,SAAQ,SAASC,EAAoBC,GAErCN,EAAIM,GADFD,KAAcjC,EACFA,EAAwBiC,GAGzB,IAEjB,IACAJ,EAAgB,QAAID,EAAIO,QAAO,SAACC,GAAK,QAAOA,CAAC,IACzCP,EAAgB,QAAEQ,SAASpC,MAC7B4B,EAAgB,QAAES,KAAKrC,MAIzB4B,EAAgB,QAAI,CAAC5B,KAGzB,OAAO4B,CACT,EAEAU,mBAAQ,WAKN,MAAO,KAA0CnB,EAAKoB,MAAQ,QAAQvD,MAAK,SAACwD,GAC1E,IACEC,IAAOC,QACT,CACA,MAAOzD,GACL0D,QAAQC,KAAK,+BACf,CACF,IAAGC,OAAM,SAACC,GACRH,QAAQC,KAAK,sBAAuBE,EACtC,GAEF,GAAG,CAAC3B,EAAKoB,QAETQ,qBAAU,WACR,IAAMnB,EAASH,IAEf,IACEgB,IAAOO,SACT,CACA,MAAO/D,GACP,CA+DA,OA9DAwD,IAAOQ,WAAWrB,GAAQ5C,MAAK,WAQ7B,IAAIkE,EAAcT,IAAOU,UAAU,aAC/BD,GACFA,EAAYE,KAAKX,KAGnB,IAAMY,EAAY/B,KAAKQ,MAAMN,GAK7B,GAJqC,IAAlChC,OAAOD,KAAK8D,GAAWC,QACxBb,IAAOc,SAASF,IAGdlC,EAAmB,aAAE,CAEvB,IAAMqC,EAAYf,IAAOgB,WACzBC,IAAUC,kBAAkBH,GAC5Bf,IAAOmB,GAAI,gBAAgB,SAAAC,GAEzB,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkB,CAACI,OAASF,EAAcE,OAAQC,OAASH,EAAcG,OAAQC,OAAQH,EAAUG,OAAQC,OAAQJ,EAAUI,OAAQC,SAAUL,EAAUK,UACrK,IAEA1B,IAAOmB,GAAI,iBAAiB,SAAAC,GAE1B,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,IACArB,IAAOmB,GAAI,kBAAkB,SAAAC,GAE3B,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,IACArB,IAAOmB,GAAI,iBAAiB,SAAAC,GAE1B,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,IACArB,IAAOmB,GAAI,kBAAkB,SAAAC,GAE3B,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,IACArB,IAAOmB,GAAI,UAAU,SAAAC,GAEnB,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,IACArB,IAAOmB,GAAI,WAAW,SAAAC,GAEpB,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,GACF,CAEF,IAEO,WAELrB,IAAOO,SACT,CACF,GAAG,IAGHD,qBAAU,WACR,IAAMqB,EAAkB3B,IAAO4B,aACzBzC,EAASH,IAGX6C,EAAiC9E,OAAO+E,OAAOH,GAAiB3F,KAAI,SAAC+F,GAAW,OAAKA,EAAOnF,EAAE,IAC/F,YAAa8B,EAAa,QACXA,EAAa,OAAW,QAClBY,SAAQ,SAACyC,GACzBA,IAAmD,IAAzCF,EAAoBG,QAAQD,IACxC/B,IAAOiC,eAAgB3E,EAAwByE,GAEnD,IAaF/B,IAAOkC,UAAU/C,EACnB,GAAG,CAACP,EAAWF,EAAwB,oBAEvC4B,qBAAU,WACR,IAAMM,EAAY/B,KAAKQ,MAAMN,GACzBiB,IAAOmC,WAA+C,IAAlCpF,OAAOD,KAAK8D,GAAWC,QAC7Cb,IAAOc,SAASF,EAEpB,GAAG,CAAC7B,IAEJuB,qBAAU,WACR,GAAIN,IAAOmC,UACT,GAAIxD,EAAS,CACXqB,IAAOoC,aAAY,GACnB,IAAIC,EAAWrC,IAAOsC,qBAClBD,IACFA,EAASE,MAAMC,cAAgB,OAEnC,KACK,CACHxC,IAAOoC,aAAY,GACnB,IAAIC,EAAWrC,IAAOsC,qBAClBD,IACFA,EAASE,MAAMC,cAAgB,OAEnC,CAEJ,GAAG,CAAC7D,IAYJ,IAAM8D,EAAiB,IAAIC,gBAAe,SAACC,GAG4B,IAADC,EAA7C,SAAnBlE,EAAa,QAA0C,kBAAnBA,EAAa,QACnDuC,IAAU4B,eAAmD,QAArCD,EAAED,EAAQ,GAAGG,eAAeC,iBAAS,IAAAH,IAAID,EAAQ,GAAGK,YAAY9E,QACpF8B,IAAOmC,WACTnC,IAAOC,WAITgB,IAAU4B,eAAenE,EAAa,QAClCsB,IAAOmC,WACTnC,IAAOC,SAIb,IAEMgD,EAAU,SAACC,GACfA,EAAUT,EAAeQ,QAAQC,GAA6BT,EAAeU,YAC/E,EAEA,OAAIzE,EAAwB,kBAExB0E,eAAAC,WAAA,CAAAC,SAAA,CACEC,cAACrG,EAAS,CAACG,OAAQqB,EAAKqB,MACxBwD,cAAA,OAAKC,IAAKP,EAASQ,UAAU,SAASC,wBAAyB,CAACC,OAAQjF,EAAc,cAOxF0E,eAAAC,WAAA,CAAAC,SAAA,CACEC,cAACrG,EAAS,CAACG,OAAQqB,EAAKqB,MACxBwD,cAAA,OAAKC,IAAKP,EAASQ,UAAU,SAAQH,SACnCC,cAAA,UAAAnE,wBAAA,CAAS,gBAAe,IAAQV,EAAqB,gBAAC,IAAA4E,SACpDC,cAAA,UAAQK,KAAM,gBAAgBN,SAC3B5E,EAAc,iBAO7B,ICnTAmF,IAASC,OACPP,cAACQ,IAAMC,WAAU,CAAAV,SACfC,cAACU,EAAY,MAEfC,SAASC,eAAe,Q",
+    "file": "static/js/main.18f5a848.chunk.js",
+    "mappings": "gIAAA,IAAIA,EAAM,CACT,cAAe,CACd,GACA,GAED,uBAAwB,CACvB,GACA,IAED,cAAe,CACd,GACA,IAED,cAAe,CACd,GACA,IAED,gBAAiB,CAChB,GACA,IAED,0CAA2C,CAC1C,GACA,IAED,8CAA+C,CAC9C,GACA,IAED,eAAgB,CACf,GACA,GAED,aAAc,CACb,GACA,GAED,cAAe,CACd,GACA,GAED,cAAe,CACd,GACA,IAED,eAAgB,CACf,GACA,GAED,YAAa,CACZ,GACA,GAED,kBAAmB,CAClB,GACA,GAED,uBAAwB,CACvB,GACA,IAED,cAAe,CACd,GACA,IAED,gDAAiD,CAChD,GACA,KAGF,SAASC,EAAoBC,GAC5B,IAAIC,EAAoBC,EAAEJ,EAAKE,GAC9B,OAAOG,QAAQC,UAAUC,MAAK,WAC7B,IAAIC,EAAI,IAAIC,MAAM,uBAAyBP,EAAM,KAEjD,MADAM,EAAEE,KAAO,mBACHF,CACP,IAGD,IAAIG,EAAMX,EAAIE,GAAMU,EAAKD,EAAI,GAC7B,OAAOR,EAAoBK,EAAEG,EAAI,IAAIJ,MAAK,WACzC,OAAOJ,EAAoBU,EAAED,EAAI,EAClC,GACD,CACAX,EAAoBa,KAAO,WAC1B,OAAOC,OAAOD,KAAKd,EACpB,EACAC,EAAoBW,GAAK,GACzBI,EAAOC,QAAUhB,C,+OC3DXiB,EAAYC,YAAiB,SAC/B,SAAAC,GAAK,OAAIA,EAAMC,MAAM,IAGnBC,EAAkB,CAAC,SAAYC,IAAgB,UAAaC,IAAiB,MAASC,IAAWC,MAAO,SAAYD,IAAWE,SAAU,SAAYF,IAAWG,SAAU,OAAUC,IAAc,MAASC,IAAa,KAAQC,KAIhOC,EAAgB,CAGrBC,MAAO,IACPC,OAAQ,IAGRC,OAAQ,IAGRC,SAAU,GACVC,SAAU,EAIVC,kBAAkB,EAGlBC,eAAgB,SAyQFC,eAlQM,SAAHC,GAA+C,IAAzCC,EAAID,EAAJC,KAAMC,EAAQF,EAARE,SAExBC,EAAYC,KAAKC,UAAUJ,EAAa,QACxCK,EAAeF,KAAKC,UAAUJ,EAAoB,eAGhDM,EAAc,SAACC,GACnB,IAkBQC,EAlBFC,EAAMC,wBAAA,GAAOpB,GAAkBa,KAAKQ,MAAMT,IAE5CF,EAAwB,kBACtB,YAAaS,KACXD,EAAMC,EAAgB,SACtBG,SAAQ,SAASC,EAAoBC,GAErCN,EAAIM,GADFD,KAAcjC,EACFA,EAAwBiC,GAGzB,IAEjB,IACAJ,EAAgB,QAAID,EAAIO,QAAO,SAACC,GAAK,QAAOA,CAAC,KAI3C,YAAaP,IACXD,EAAMC,EAAgB,SACtBG,SAAQ,SAASC,EAAoBC,GAErCN,EAAIM,GADFD,KAAcjC,EACFA,EAAwBiC,GAGzB,IAEjB,IACAJ,EAAgB,QAAID,EAAIO,QAAO,SAACC,GAAK,QAAOA,CAAC,IACzCP,EAAgB,QAAEQ,SAASpC,MAC7B4B,EAAgB,QAAES,KAAKrC,MAIzB4B,EAAgB,QAAI,CAAC5B,KAGzB,OAAO4B,CACT,EAEAU,mBAAQ,WAKN,MAAO,KAA0CnB,EAAKoB,MAAQ,QAAQvD,MAAK,SAACwD,GAC1E,IACEC,IAAOC,QACT,CACA,MAAOzD,GACL0D,QAAQC,KAAK,+BACf,CACF,IAAGC,OAAM,SAACC,GACRH,QAAQC,KAAK,sBAAuBE,EACtC,GAEF,GAAG,CAAC3B,EAAKoB,QAETQ,qBAAU,WACR,IAAMnB,EAASH,IAEf,IACEgB,IAAOO,SACT,CACA,MAAO/D,GACP,CA+DA,OA9DAwD,IAAOQ,WAAWrB,GAAQ5C,MAAK,WAQ7B,IAAIkE,EAAcT,IAAOU,UAAU,aAC/BD,GACFA,EAAYE,KAAKX,KAGnB,IAAMY,EAAY/B,KAAKQ,MAAMN,GAK7B,GAJqC,IAAlChC,OAAOD,KAAK8D,GAAWC,QACxBb,IAAOc,SAASF,IAGdlC,EAAmB,aAAE,CAEvB,IAAMqC,EAAYf,IAAOgB,WACzBC,IAAUC,kBAAkBH,GAC5Bf,IAAOmB,GAAI,gBAAgB,SAAAC,GAEzB,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkB,CAACI,OAASF,EAAcE,OAAQC,OAASH,EAAcG,OAAQC,OAAQH,EAAUG,OAAQC,OAAQJ,EAAUI,OAAQC,SAAUL,EAAUK,UACrK,IAEA1B,IAAOmB,GAAI,iBAAiB,SAAAC,GAE1B,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,IACArB,IAAOmB,GAAI,kBAAkB,SAAAC,GAE3B,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,IACArB,IAAOmB,GAAI,iBAAiB,SAAAC,GAE1B,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,IACArB,IAAOmB,GAAI,kBAAkB,SAAAC,GAE3B,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,IACArB,IAAOmB,GAAI,UAAU,SAAAC,GAEnB,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,IACArB,IAAOmB,GAAI,WAAW,SAAAC,GAEpB,IAAMC,EAAYrB,IAAOgB,WACzBC,IAAUC,kBAAkBG,EAC9B,GACF,CAEF,IAEO,WAELrB,IAAOO,SACT,CACF,GAAG,IAGHD,qBAAU,WACR,IAAMqB,EAAkB3B,IAAO4B,aACzBzC,EAASH,IAGX6C,EAAiC9E,OAAO+E,OAAOH,GAAiB3F,KAAI,SAAC+F,GAAW,OAAKA,EAAOnF,EAAE,IAC/F,YAAa8B,EAAa,QACXA,EAAa,OAAW,QAClBY,SAAQ,SAACyC,GACzBA,IAAmD,IAAzCF,EAAoBG,QAAQD,IACxC/B,IAAOiC,eAAgB3E,EAAwByE,GAEnD,IAaF/B,IAAOkC,UAAU/C,EACnB,GAAG,CAACP,EAAWF,EAAwB,oBAEvC4B,qBAAU,WACR,IAAMM,EAAY/B,KAAKQ,MAAMN,GACzBiB,IAAOmC,WAA+C,IAAlCpF,OAAOD,KAAK8D,GAAWC,QAC7Cb,IAAOc,SAASF,EAEpB,GAAG,CAAC7B,IAEJuB,qBAAU,WACR,GAAIN,IAAOmC,UACT,GAAIxD,EAAS,CACXqB,IAAOoC,aAAY,GACnB,IAAIC,EAAWrC,IAAOsC,qBAClBD,IACFA,EAASE,MAAMC,cAAgB,OAEnC,KACK,CACHxC,IAAOoC,aAAY,GACnB,IAAIC,EAAWrC,IAAOsC,qBAClBD,IACFA,EAASE,MAAMC,cAAgB,OAEnC,CAEJ,GAAG,CAAC7D,IAYJ,IAAM8D,EAAiB,IAAIC,gBAAe,SAACC,GAG4B,IAADC,EAA7C,SAAnBlE,EAAa,QAA0C,kBAAnBA,EAAa,QACnDuC,IAAU4B,eAAmD,QAArCD,EAAED,EAAQ,GAAGG,eAAeC,iBAAS,IAAAH,IAAID,EAAQ,GAAGK,YAAY9E,QACpF8B,IAAOmC,WACTnC,IAAOC,WAITgB,IAAU4B,eAAenE,EAAa,QAClCsB,IAAOmC,WACTnC,IAAOC,SAIb,IAEMgD,EAAU,SAACC,GACfA,EAAUT,EAAeQ,QAAQC,GAA6BT,EAAeU,YAC/E,EAEA,OAAIzE,EAAwB,kBAExB0E,eAAAC,WAAA,CAAAC,SAAA,CACEC,cAACrG,EAAS,CAACG,OAAQqB,EAAKqB,MACxBwD,cAAA,OAAKC,IAAKP,EAASQ,UAAU,SAAQH,SACnCC,cAACG,IAAS,CAACC,KAAMjF,EAAc,eAOnC0E,eAAAC,WAAA,CAAAC,SAAA,CACEC,cAACrG,EAAS,CAACG,OAAQqB,EAAKqB,MACxBwD,cAAA,OAAKC,IAAKP,EAASQ,UAAU,SAAQH,SACnCC,cAAA,UAAAnE,wBAAA,CAAS,gBAAe,IAAQV,EAAqB,gBAAC,IAAA4E,SACpDC,cAAA,UAAQK,KAAM,gBAAgBN,SAC3B5E,EAAc,iBAO7B,ICrTAmF,IAASC,OACPP,cAACQ,IAAMC,WAAU,CAAAV,SACfC,cAACU,EAAY,MAEfC,SAASC,eAAe,Q",
     "names": [
         "map",
         "webpackAsyncContext",
         "req",
         "__webpack_require__",
         "o",
         "Promise",
@@ -120,16 +120,16 @@
         "disconnect",
         "_jsxs",
         "_Fragment",
         "children",
         "_jsx",
         "ref",
         "className",
-        "dangerouslySetInnerHTML",
-        "__html",
+        "InnerHTML",
+        "html",
         "type",
         "ReactDOM",
         "render",
         "React",
         "StrictMode",
         "RevealSlides",
         "document",
@@ -138,13 +138,13 @@
     "sourceRoot": "",
     "sources": [
         "../node_modules/reveal.js/dist/theme lazy /^/.//.*/.css$/ groupOptions: {} namespace object",
         "RevealSlides.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "var map = {\n\t\"./beige.css\": [\n\t\t73,\n\t\t3\n\t],\n\t\"./black-contrast.css\": [\n\t\t74,\n\t\t10\n\t],\n\t\"./black.css\": [\n\t\t75,\n\t\t11\n\t],\n\t\"./blood.css\": [\n\t\t76,\n\t\t12\n\t],\n\t\"./dracula.css\": [\n\t\t77,\n\t\t16\n\t],\n\t\"./fonts/league-gothic/league-gothic.css\": [\n\t\t78,\n\t\t17\n\t],\n\t\"./fonts/source-sans-pro/source-sans-pro.css\": [\n\t\t79,\n\t\t18\n\t],\n\t\"./league.css\": [\n\t\t80,\n\t\t4\n\t],\n\t\"./moon.css\": [\n\t\t81,\n\t\t5\n\t],\n\t\"./night.css\": [\n\t\t82,\n\t\t6\n\t],\n\t\"./serif.css\": [\n\t\t83,\n\t\t19\n\t],\n\t\"./simple.css\": [\n\t\t84,\n\t\t7\n\t],\n\t\"./sky.css\": [\n\t\t85,\n\t\t8\n\t],\n\t\"./solarized.css\": [\n\t\t86,\n\t\t9\n\t],\n\t\"./white-contrast.css\": [\n\t\t87,\n\t\t13\n\t],\n\t\"./white.css\": [\n\t\t88,\n\t\t14\n\t],\n\t\"./white_contrast_compact_verbatim_headers.css\": [\n\t\t89,\n\t\t15\n\t]\n};\nfunction webpackAsyncContext(req) {\n\tif(!__webpack_require__.o(map, req)) {\n\t\treturn Promise.resolve().then(function() {\n\t\t\tvar e = new Error(\"Cannot find module '\" + req + \"'\");\n\t\t\te.code = 'MODULE_NOT_FOUND';\n\t\t\tthrow e;\n\t\t});\n\t}\n\n\tvar ids = map[req], id = ids[0];\n\treturn __webpack_require__.e(ids[1]).then(function() {\n\t\treturn __webpack_require__.t(id, 7);\n\t});\n}\nwebpackAsyncContext.keys = function webpackAsyncContextKeys() {\n\treturn Object.keys(map);\n};\nwebpackAsyncContext.id = 71;\nmodule.exports = webpackAsyncContext;",
-        "import {\n  Streamlit,\n  ComponentProps,\n  withStreamlitConnection,\n  Theme,\n} from \"streamlit-component-lib\"\nimport { useEffect, useMemo, useRef } from \"react\"\nimport { createGlobalStyle } from \"styled-components/macro\"\n\nimport Reveal from 'reveal.js';\nimport RevealMarkdown from 'reveal.js/plugin/markdown/markdown';\nimport RevealHighlight from 'reveal.js/plugin/highlight/highlight';\nimport RevealMath from 'reveal.js/plugin/math/math';\nimport RevealSearch from 'reveal.js/plugin/search/search';\nimport RevealNotes from 'reveal.js/plugin/notes/notes';\nimport RevealZoom from 'reveal.js/plugin/zoom/zoom';\n\n\nimport 'reveal.js/dist/reveal.css';\nimport 'reveal.js/plugin/highlight/monokai.css';\n\ninterface RevealSlidesProps extends ComponentProps {\n  args: any\n  width: number\n  disabled: boolean\n  theme?: Theme\n}\n\nconst GlobalCSS = createGlobalStyle<{ inject: string}>`\n  ${props => props.inject}\n`\n\nconst includedPlugins = {\"markdown\": RevealMarkdown, \"highlight\": RevealHighlight, \"katex\": RevealMath.KaTeX, \"mathjax2\": RevealMath.MathJax2, \"mathjax3\": RevealMath.MathJax3, \"search\": RevealSearch, \"notes\": RevealNotes, \"zoom\": RevealZoom}\n// const simpleCommands = {\"left\": Reveal.left, \"right\": () => {Reveal.right()}, \"up\": Reveal.up, \"down\": Reveal.down, \"prev\": Reveal.prev, \"next\": Reveal.next, \"prevFragment\": Reveal.prevFragment, \"nextFragment\": Reveal.nextFragment, \"togglePause\": Reveal.togglePause, \"toggleAutoSlide\": Reveal.toggleAutoSlide, \"toggleHelp\": Reveal.toggleHelp, \"toggleOverview\": Reveal.toggleOverview, \"shuffle\": Reveal.shuffle}\n// const commandsWithArgs = {slide: Reveal.slide, togglePause: Reveal.togglePause, toggleAutoSlide: Reveal.toggleAutoSlide, toggleHelp: Reveal.toggleHelp, toggleOverview: Reveal.toggleOverview}\n\nconst defaultConfig = {\n  // The \"normal\" size of the presentation, aspect ratio will be preserved\n\t// when the presentation is scaled to fit different resolutions\n\twidth: 900,\n\theight: 860,\n\t\n\t// Factor of the display size that should remain empty around the content\n\tmargin: 0.05,\n\n\t// Bounds for smallest/largest possible scale to apply to content\n\tminScale: 0.1,\n\tmaxScale: 3.0,\n\n\t// Help the user learn the controls by providing hints, for example by\n\t// bouncing the down arrow when they first encounter a vertical slide\n\tcontrolsTutorial: true,\n\n\t// Determines where controls appear, \"edges\" or \"bottom-right\"\n\tcontrolsLayout: 'edges',\n}\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nconst RevealSlides = ({ args, disabled }: RevealSlidesProps) => {   \n\n  let configStr = JSON.stringify(args[\"config\"])\n  let initStateStr = JSON.stringify(args[\"initial_state\"])\n  // const commandStr = JSON.stringify(args[\"commands\"])\n\n  const setupConfig = (configString: string) : object => {\n    const config = {...defaultConfig, ...JSON.parse(configStr)}\n    // code to run after render goes here\n    if (args[\"allow_unsafe_html\"]) {\n      if ('plugins' in config){\n        var arr = config['plugins'];\n        arr.forEach(function(moduleName: string, index: number) {\n          if (moduleName in includedPlugins){\n            arr[index] = (includedPlugins as any)[moduleName];\n          }\n          else {\n            arr[index] = null;\n          }\n        });\n        config['plugins'] = arr.filter((x:any) => !!x) as any[];\n      }\n    }\n    else {\n      if ('plugins' in config){\n        var arr = config['plugins'];\n        arr.forEach(function(moduleName: string, index: number) {\n          if (moduleName in includedPlugins){\n            arr[index] = (includedPlugins as any)[moduleName];\n          }\n          else {\n            arr[index] = null;\n          }\n        });\n        config['plugins'] = arr.filter((x:any) => !!x) as any[];\n        if(!config['plugins'].includes(RevealMarkdown)){\n          config['plugins'].push(RevealMarkdown);\n        }\n      }\n      else {\n        config['plugins'] = [RevealMarkdown];\n      }\n    }\n    return config;\n  }\n\n  useMemo(()=>{\n    // code to run on component mount goes here\n\n    // To do: remove or disable previously imported css. When the list of\n    // css imports exceed about 25, the page no longer updates.\n    import('../node_modules/reveal.js/dist/theme/' + args.theme + '.css').then((css) => {\n      try{\n        Reveal.layout();\n      }\n      catch (e){\n        console.warn(\"Reveal.layout() call failed.\")\n      }\n    }).catch((err) => {\n      console.warn(\"Failed CSS import: \", err);\n    });\n\n  }, [args.theme]);\n\n  useEffect(() => {\n    const config = setupConfig(configStr)\n    \n    try {\n      Reveal.destroy();\n    }\n    catch (e) {\n    }\n    Reveal.initialize(config).then(() => {\n      // reveal.js is ready\n      \n      // For some yet to be determined reason, the highlight plugin is not initialized.\n      // Setting highlight config option highlightOnLoad to true (before passing to initialize function)\n      // does not work\n      // To Do: make sure the highlight plugin only changes the HTML involving the code once instead of many times.\n      // Possible solution is to make a change to the plugin init function.\n      let highlighter = Reveal.getPlugin('highlight') as any;\n      if (highlighter){\n        highlighter.init(Reveal);\n      }\n      \n      const initState = JSON.parse(initStateStr);\n      if(Object.keys(initState).length !== 0){\n        Reveal.setState(initState);\n      }\n\n      if(!args['display_only']){\n        // Send slide position indecies back to Streamlit on initialization and on slide change\n        const currState = Reveal.getState();\n        Streamlit.setComponentValue(currState);\n        Reveal.on( 'slidechanged', event => {\n\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue({indexh: (event as any).indexh, indexv: (event as any).indexv, indexf: tempState.indexf, paused: tempState.paused, overview: tempState.overview});\n        });\n        \n        Reveal.on( 'fragmentshown', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'fragmenthidden', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'overviewshown', event => {\n          // event.overview = the overview DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'overviewhidden', event => {\n          // event.overview = the overview DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'paused', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'resumed', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n      }\n\n    });\n\n    return () => {\n      // code to run on component unmount goes here\n      Reveal.destroy();  \n    }\n  }, []);\n\n  // Reconfigure reveal.js if config changes\n  useEffect(() => {\n    const existingPlugins = Reveal.getPlugins();\n    const config = setupConfig(configStr)\n\n    // Add and register plugins that are not already loaded\n    let existingPluginsList : string[] = Object.values(existingPlugins).map((plugin: any) => plugin.id);\n    if('plugins' in args[\"config\"]){\n      const plugins = args[\"config\"][\"plugins\"];\n      (plugins as string[]).forEach((plugin: string) => {\n        if (plugin && existingPluginsList.indexOf(plugin) === -1){\n          Reveal.registerPlugin((includedPlugins as any)[plugin]);\n        }\n      });\n\n      //// Remove plugins that are no longer in the list (does not work yet..some signs there is a bug in Reveal.Plugin)\n      // Object.values(existingPlugins as {[id: string]: Reveal.Plugin;}).forEach((plugin: any) => {\n      //   if (plugin.id && plugin.id !=='markdown' && plugins.indexOf(plugin.id) === -1){\n      //     console.log(\"destroy plugin: \" + plugin.id);\n      //     if( typeof plugin.destroy === 'function' ) {\n      //       plugin.destroy();\n      //     }\n      //   }\n      // });\n    }\n    // Reconfigure reveal.js\n    Reveal.configure(config);\n  }, [configStr, args[\"allow_unsafe_html\"]]);\n\n  useEffect(() => {\n    const initState = JSON.parse(initStateStr);\n    if (Reveal.isReady() && Object.keys(initState).length !== 0){\n      Reveal.setState(initState);\n    }\n  }, [initStateStr]);\n\n  useEffect(() => {\n    if (Reveal.isReady()){\n      if (disabled){\n        Reveal.togglePause(true);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"none\";\n        }\n      }\n      else {  \n        Reveal.togglePause(false);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"auto\";\n        }\n      }\n    }\n  }, [disabled]);\n\n  //To do: add support for commands (i.e. control slides from Streamlit)\n  //-----------------\n  //\n\n\n  /**\n   * resizeObserver observes changes in elements its given to observe and is used here\n   * to communicate to streamlit the height of the component that has changed\n   * so that streamlit can adjust the iframe containing the component accordingly.\n   */\n  const resizeObserver = new ResizeObserver((entries: any) => {\n    // If we know that the body will always fully contain our component (without cutting it off)\n    // then we can use docuemnt.body height instead\n    if (args[\"height\"] === \"auto\" || typeof args[\"height\"] !== \"number\"){\n      Streamlit.setFrameHeight((entries[0].contentBoxSize.blockSize ?? entries[0].contentRect.height)); \n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    else {\n      Streamlit.setFrameHeight(args[\"height\"]);\n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    \n  })\n\n  const observe = (divElem: any) => {\n    divElem ? resizeObserver.observe(divElem as HTMLDivElement) : resizeObserver.disconnect();\n  }\n\n  if (args[\"allow_unsafe_html\"]) {\n    return (\n      <>\n        <GlobalCSS inject={args.css}/>\n        <div ref={observe} className=\"slides\" dangerouslySetInnerHTML={{__html: args[\"content\"]}}>\n        </div>\n      </>\n    )\n  }\n  else {\n    return (\n      <>\n        <GlobalCSS inject={args.css}/>\n        <div ref={observe} className=\"slides\">\n          <section data-markdown={\"\"} {...args[\"markdown_props\"]}>\n            <script type={\"text/template\"}>\n              {args[\"content\"]}\n            </script>\n          </section>\n        </div>\n      </>\n    )\n  }\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(RevealSlides)\n",
+        "var map = {\n\t\"./beige.css\": [\n\t\t74,\n\t\t3\n\t],\n\t\"./black-contrast.css\": [\n\t\t75,\n\t\t10\n\t],\n\t\"./black.css\": [\n\t\t76,\n\t\t11\n\t],\n\t\"./blood.css\": [\n\t\t77,\n\t\t12\n\t],\n\t\"./dracula.css\": [\n\t\t78,\n\t\t16\n\t],\n\t\"./fonts/league-gothic/league-gothic.css\": [\n\t\t79,\n\t\t17\n\t],\n\t\"./fonts/source-sans-pro/source-sans-pro.css\": [\n\t\t80,\n\t\t18\n\t],\n\t\"./league.css\": [\n\t\t81,\n\t\t4\n\t],\n\t\"./moon.css\": [\n\t\t82,\n\t\t5\n\t],\n\t\"./night.css\": [\n\t\t83,\n\t\t6\n\t],\n\t\"./serif.css\": [\n\t\t84,\n\t\t19\n\t],\n\t\"./simple.css\": [\n\t\t85,\n\t\t7\n\t],\n\t\"./sky.css\": [\n\t\t86,\n\t\t8\n\t],\n\t\"./solarized.css\": [\n\t\t87,\n\t\t9\n\t],\n\t\"./white-contrast.css\": [\n\t\t88,\n\t\t13\n\t],\n\t\"./white.css\": [\n\t\t89,\n\t\t14\n\t],\n\t\"./white_contrast_compact_verbatim_headers.css\": [\n\t\t90,\n\t\t15\n\t]\n};\nfunction webpackAsyncContext(req) {\n\tif(!__webpack_require__.o(map, req)) {\n\t\treturn Promise.resolve().then(function() {\n\t\t\tvar e = new Error(\"Cannot find module '\" + req + \"'\");\n\t\t\te.code = 'MODULE_NOT_FOUND';\n\t\t\tthrow e;\n\t\t});\n\t}\n\n\tvar ids = map[req], id = ids[0];\n\treturn __webpack_require__.e(ids[1]).then(function() {\n\t\treturn __webpack_require__.t(id, 7);\n\t});\n}\nwebpackAsyncContext.keys = function webpackAsyncContextKeys() {\n\treturn Object.keys(map);\n};\nwebpackAsyncContext.id = 72;\nmodule.exports = webpackAsyncContext;",
+        "import {\n  Streamlit,\n  ComponentProps,\n  withStreamlitConnection,\n  Theme,\n} from \"streamlit-component-lib\"\nimport { useEffect, useMemo, useRef } from \"react\"\nimport { createGlobalStyle } from \"styled-components/macro\"\nimport InnerHTML from 'dangerously-set-html-content'\n\nimport Reveal from 'reveal.js';\nimport RevealMarkdown from 'reveal.js/plugin/markdown/markdown';\nimport RevealHighlight from 'reveal.js/plugin/highlight/highlight';\nimport RevealMath from 'reveal.js/plugin/math/math';\nimport RevealSearch from 'reveal.js/plugin/search/search';\nimport RevealNotes from 'reveal.js/plugin/notes/notes';\nimport RevealZoom from 'reveal.js/plugin/zoom/zoom';\n\n\nimport 'reveal.js/dist/reveal.css';\nimport 'reveal.js/plugin/highlight/monokai.css';\n\ninterface RevealSlidesProps extends ComponentProps {\n  args: any\n  width: number\n  disabled: boolean\n  theme?: Theme\n}\n\nconst GlobalCSS = createGlobalStyle<{ inject: string}>`\n  ${props => props.inject}\n`\n\nconst includedPlugins = {\"markdown\": RevealMarkdown, \"highlight\": RevealHighlight, \"katex\": RevealMath.KaTeX, \"mathjax2\": RevealMath.MathJax2, \"mathjax3\": RevealMath.MathJax3, \"search\": RevealSearch, \"notes\": RevealNotes, \"zoom\": RevealZoom}\n// const simpleCommands = {\"left\": Reveal.left, \"right\": () => {Reveal.right()}, \"up\": Reveal.up, \"down\": Reveal.down, \"prev\": Reveal.prev, \"next\": Reveal.next, \"prevFragment\": Reveal.prevFragment, \"nextFragment\": Reveal.nextFragment, \"togglePause\": Reveal.togglePause, \"toggleAutoSlide\": Reveal.toggleAutoSlide, \"toggleHelp\": Reveal.toggleHelp, \"toggleOverview\": Reveal.toggleOverview, \"shuffle\": Reveal.shuffle}\n// const commandsWithArgs = {slide: Reveal.slide, togglePause: Reveal.togglePause, toggleAutoSlide: Reveal.toggleAutoSlide, toggleHelp: Reveal.toggleHelp, toggleOverview: Reveal.toggleOverview}\n\nconst defaultConfig = {\n  // The \"normal\" size of the presentation, aspect ratio will be preserved\n\t// when the presentation is scaled to fit different resolutions\n\twidth: 900,\n\theight: 860,\n\t\n\t// Factor of the display size that should remain empty around the content\n\tmargin: 0.05,\n\n\t// Bounds for smallest/largest possible scale to apply to content\n\tminScale: 0.1,\n\tmaxScale: 3.0,\n\n\t// Help the user learn the controls by providing hints, for example by\n\t// bouncing the down arrow when they first encounter a vertical slide\n\tcontrolsTutorial: true,\n\n\t// Determines where controls appear, \"edges\" or \"bottom-right\"\n\tcontrolsLayout: 'edges',\n}\n\n/**\n * This is a React-based component template. The `render()` function is called\n * automatically when your component should be re-rendered.\n */\nconst RevealSlides = ({ args, disabled }: RevealSlidesProps) => {   \n\n  let configStr = JSON.stringify(args[\"config\"])\n  let initStateStr = JSON.stringify(args[\"initial_state\"])\n  // const commandStr = JSON.stringify(args[\"commands\"])\n\n  const setupConfig = (configString: string) : object => {\n    const config = {...defaultConfig, ...JSON.parse(configStr)}\n    // code to run after render goes here\n    if (args[\"allow_unsafe_html\"]) {\n      if ('plugins' in config){\n        var arr = config['plugins'];\n        arr.forEach(function(moduleName: string, index: number) {\n          if (moduleName in includedPlugins){\n            arr[index] = (includedPlugins as any)[moduleName];\n          }\n          else {\n            arr[index] = null;\n          }\n        });\n        config['plugins'] = arr.filter((x:any) => !!x) as any[];\n      }\n    }\n    else {\n      if ('plugins' in config){\n        var arr = config['plugins'];\n        arr.forEach(function(moduleName: string, index: number) {\n          if (moduleName in includedPlugins){\n            arr[index] = (includedPlugins as any)[moduleName];\n          }\n          else {\n            arr[index] = null;\n          }\n        });\n        config['plugins'] = arr.filter((x:any) => !!x) as any[];\n        if(!config['plugins'].includes(RevealMarkdown)){\n          config['plugins'].push(RevealMarkdown);\n        }\n      }\n      else {\n        config['plugins'] = [RevealMarkdown];\n      }\n    }\n    return config;\n  }\n\n  useMemo(()=>{\n    // code to run on component mount goes here\n\n    // To do: remove or disable previously imported css. When the list of\n    // css imports exceed about 25, the page no longer updates.\n    import('../node_modules/reveal.js/dist/theme/' + args.theme + '.css').then((css) => {\n      try{\n        Reveal.layout();\n      }\n      catch (e){\n        console.warn(\"Reveal.layout() call failed.\")\n      }\n    }).catch((err) => {\n      console.warn(\"Failed CSS import: \", err);\n    });\n\n  }, [args.theme]);\n\n  useEffect(() => {\n    const config = setupConfig(configStr)\n    \n    try {\n      Reveal.destroy();\n    }\n    catch (e) {\n    }\n    Reveal.initialize(config).then(() => {\n      // reveal.js is ready\n      \n      // For some yet to be determined reason, the highlight plugin is not initialized.\n      // Setting highlight config option highlightOnLoad to true (before passing to initialize function)\n      // does not work\n      // To Do: make sure the highlight plugin only changes the HTML involving the code once instead of many times.\n      // Possible solution is to make a change to the plugin init function.\n      let highlighter = Reveal.getPlugin('highlight') as any;\n      if (highlighter){\n        highlighter.init(Reveal);\n      }\n      \n      const initState = JSON.parse(initStateStr);\n      if(Object.keys(initState).length !== 0){\n        Reveal.setState(initState);\n      }\n\n      if(!args['display_only']){\n        // Send slide position indecies back to Streamlit on initialization and on slide change\n        const currState = Reveal.getState();\n        Streamlit.setComponentValue(currState);\n        Reveal.on( 'slidechanged', event => {\n\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue({indexh: (event as any).indexh, indexv: (event as any).indexv, indexf: tempState.indexf, paused: tempState.paused, overview: tempState.overview});\n        });\n        \n        Reveal.on( 'fragmentshown', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'fragmenthidden', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'overviewshown', event => {\n          // event.overview = the overview DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'overviewhidden', event => {\n          // event.overview = the overview DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'paused', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n        Reveal.on( 'resumed', event => {\n          // event.fragment = the fragment DOM element\n          const tempState = Reveal.getState();\n          Streamlit.setComponentValue(tempState);\n        } );\n      }\n\n    });\n\n    return () => {\n      // code to run on component unmount goes here\n      Reveal.destroy();  \n    }\n  }, []);\n\n  // Reconfigure reveal.js if config changes\n  useEffect(() => {\n    const existingPlugins = Reveal.getPlugins();\n    const config = setupConfig(configStr)\n\n    // Add and register plugins that are not already loaded\n    let existingPluginsList : string[] = Object.values(existingPlugins).map((plugin: any) => plugin.id);\n    if('plugins' in args[\"config\"]){\n      const plugins = args[\"config\"][\"plugins\"];\n      (plugins as string[]).forEach((plugin: string) => {\n        if (plugin && existingPluginsList.indexOf(plugin) === -1){\n          Reveal.registerPlugin((includedPlugins as any)[plugin]);\n        }\n      });\n\n      //// Remove plugins that are no longer in the list (does not work yet..some signs there is a bug in Reveal.Plugin)\n      // Object.values(existingPlugins as {[id: string]: Reveal.Plugin;}).forEach((plugin: any) => {\n      //   if (plugin.id && plugin.id !=='markdown' && plugins.indexOf(plugin.id) === -1){\n      //     console.log(\"destroy plugin: \" + plugin.id);\n      //     if( typeof plugin.destroy === 'function' ) {\n      //       plugin.destroy();\n      //     }\n      //   }\n      // });\n    }\n    // Reconfigure reveal.js\n    Reveal.configure(config);\n  }, [configStr, args[\"allow_unsafe_html\"]]);\n\n  useEffect(() => {\n    const initState = JSON.parse(initStateStr);\n    if (Reveal.isReady() && Object.keys(initState).length !== 0){\n      Reveal.setState(initState);\n    }\n  }, [initStateStr]);\n\n  useEffect(() => {\n    if (Reveal.isReady()){\n      if (disabled){\n        Reveal.togglePause(true);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"none\";\n        }\n      }\n      else {  \n        Reveal.togglePause(false);\n        let viewport = Reveal.getViewportElement();\n        if (viewport){\n          viewport.style.pointerEvents = \"auto\";\n        }\n      }\n    }\n  }, [disabled]);\n\n  //To do: add support for commands (i.e. control slides from Streamlit)\n  //-----------------\n  //\n\n\n  /**\n   * resizeObserver observes changes in elements its given to observe and is used here\n   * to communicate to streamlit the height of the component that has changed\n   * so that streamlit can adjust the iframe containing the component accordingly.\n   */\n  const resizeObserver = new ResizeObserver((entries: any) => {\n    // If we know that the body will always fully contain our component (without cutting it off)\n    // then we can use docuemnt.body height instead\n    if (args[\"height\"] === \"auto\" || typeof args[\"height\"] !== \"number\"){\n      Streamlit.setFrameHeight((entries[0].contentBoxSize.blockSize ?? entries[0].contentRect.height)); \n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    else {\n      Streamlit.setFrameHeight(args[\"height\"]);\n      if (Reveal.isReady()){\n        Reveal.layout();\n      }\n    }\n    \n  })\n\n  const observe = (divElem: any) => {\n    divElem ? resizeObserver.observe(divElem as HTMLDivElement) : resizeObserver.disconnect();\n  }\n\n  if (args[\"allow_unsafe_html\"]) {\n    return (\n      <>\n        <GlobalCSS inject={args.css}/>\n        <div ref={observe} className=\"slides\" >\n          <InnerHTML html={args[\"content\"]} />\n        </div>\n      </>\n    )\n  }\n  else {\n    return (\n      <>\n        <GlobalCSS inject={args.css}/>\n        <div ref={observe} className=\"slides\">\n          <section data-markdown={\"\"} {...args[\"markdown_props\"]}>\n            <script type={\"text/template\"}>\n              {args[\"content\"]}\n            </script>\n          </section>\n        </div>\n      </>\n    )\n  }\n}\n\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\n// connection between your component and the Streamlit app, and handles\n// passing arguments from Python -> Component.\n//\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\nexport default withStreamlitConnection(RevealSlides)\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport RevealSlides from \"./RevealSlides\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <RevealSlides />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/runtime-main.887ff237.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 ! function(e) {
     function t(t) {
-        for (var n, o, c = t[0], i = t[1], f = t[2], l = 0, d = []; l < c.length; l++) o = c[l], Object.prototype.hasOwnProperty.call(a, o) && a[o] && d.push(a[o][0]), a[o] = 0;
+        for (var n, o, c = t[0], i = t[1], l = t[2], f = 0, d = []; f < c.length; f++) o = c[f], Object.prototype.hasOwnProperty.call(a, o) && a[o] && d.push(a[o][0]), a[o] = 0;
         for (n in i) Object.prototype.hasOwnProperty.call(i, n) && (e[n] = i[n]);
         for (s && s(t); d.length;) d.shift()();
-        return u.push.apply(u, f || []), r()
+        return u.push.apply(u, l || []), r()
     }
 
     function r() {
         for (var e, t = 0; t < u.length; t++) {
             for (var r = u[t], n = !0, o = 1; o < r.length; o++) {
                 var i = r[o];
                 0 !== a[i] && (n = !1)
@@ -70,21 +70,21 @@
                     14: "e64fc659",
                     15: "3adba626",
                     16: "b573d318",
                     17: "10a8300f",
                     18: "4eb3e38a",
                     19: "74b97645"
                 } [e] + ".chunk.css", a = c.p + n, u = document.getElementsByTagName("link"), i = 0; i < u.length; i++) {
-                var f = (s = u[i]).getAttribute("data-href") || s.getAttribute("href");
-                if ("stylesheet" === s.rel && (f === n || f === a)) return t()
+                var l = (s = u[i]).getAttribute("data-href") || s.getAttribute("href");
+                if ("stylesheet" === s.rel && (l === n || l === a)) return t()
             }
-            var l = document.getElementsByTagName("style");
-            for (i = 0; i < l.length; i++) {
+            var f = document.getElementsByTagName("style");
+            for (i = 0; i < f.length; i++) {
                 var s;
-                if ((f = (s = l[i]).getAttribute("data-href")) === n || f === a) return t()
+                if ((l = (s = f[i]).getAttribute("data-href")) === n || l === a) return t()
             }
             var d = document.createElement("link");
             d.rel = "stylesheet", d.type = "text/css", d.onload = t, d.onerror = function(t) {
                 var n = t && t.target && t.target.src || a,
                     u = new Error("Loading CSS chunk " + e + " failed.\n(" + n + ")");
                 u.code = "CSS_CHUNK_LOAD_FAILED", u.request = n, delete o[e], d.parentNode.removeChild(d), r(u)
             }, d.href = a, document.getElementsByTagName("head")[0].appendChild(d)
@@ -98,47 +98,47 @@
                 var n = new Promise((function(t, n) {
                     r = a[e] = [t, n]
                 }));
                 t.push(r[2] = n);
                 var u, i = document.createElement("script");
                 i.charset = "utf-8", i.timeout = 120, c.nc && i.setAttribute("nonce", c.nc), i.src = function(e) {
                     return c.p + "static/js/" + ({} [e] || e) + "." + {
-                        3: "d30f1cfd",
-                        4: "ec7a53ea",
-                        5: "e42b3133",
-                        6: "e9192981",
-                        7: "be794506",
-                        8: "15dd3b20",
-                        9: "119f08fa",
-                        10: "18fc5a6d",
-                        11: "e2b8452b",
-                        12: "6c6d4448",
-                        13: "c5f703d1",
-                        14: "39efed4e",
-                        15: "7665d197",
-                        16: "4a5a2671",
-                        17: "e0e3c073",
-                        18: "b265fc2b",
-                        19: "5ba3da56"
+                        3: "a17c1b63",
+                        4: "c8e4936c",
+                        5: "ab74786f",
+                        6: "7f9bbd64",
+                        7: "887bb0a8",
+                        8: "0121e917",
+                        9: "e6c78b5a",
+                        10: "442a54e9",
+                        11: "6dd2762e",
+                        12: "b5132789",
+                        13: "155b252b",
+                        14: "124342a7",
+                        15: "1df3933b",
+                        16: "e98baccf",
+                        17: "f47ed1b3",
+                        18: "bbe30a24",
+                        19: "63982437"
                     } [e] + ".chunk.js"
                 }(e);
-                var f = new Error;
+                var l = new Error;
                 u = function(t) {
-                    i.onerror = i.onload = null, clearTimeout(l);
+                    i.onerror = i.onload = null, clearTimeout(f);
                     var r = a[e];
                     if (0 !== r) {
                         if (r) {
                             var n = t && ("load" === t.type ? "missing" : t.type),
                                 o = t && t.target && t.target.src;
-                            f.message = "Loading chunk " + e + " failed.\n(" + n + ": " + o + ")", f.name = "ChunkLoadError", f.type = n, f.request = o, r[1](f)
+                            l.message = "Loading chunk " + e + " failed.\n(" + n + ": " + o + ")", l.name = "ChunkLoadError", l.type = n, l.request = o, r[1](l)
                         }
                         a[e] = void 0
                     }
                 };
-                var l = setTimeout((function() {
+                var f = setTimeout((function() {
                     u({
                         type: "timeout",
                         target: i
                     })
                 }), 12e4);
                 i.onerror = i.onload = u, document.head.appendChild(i)
             } return Promise.all(t)
@@ -174,14 +174,14 @@
         return c.d(t, "a", t), t
     }, c.o = function(e, t) {
         return Object.prototype.hasOwnProperty.call(e, t)
     }, c.p = "./", c.oe = function(e) {
         throw console.error(e), e
     };
     var i = this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || [],
-        f = i.push.bind(i);
+        l = i.push.bind(i);
     i.push = t, i = i.slice();
-    for (var l = 0; l < i.length; l++) t(i[l]);
-    var s = f;
+    for (var f = 0; f < i.length; f++) t(i[f]);
+    var s = l;
     r()
 }([]);
-//# sourceMappingURL=runtime-main.eaac28ce.js.map
+//# sourceMappingURL=runtime-main.887ff237.js.map
```

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/js/runtime-main.887ff237.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'file'": "'static/js/runtime-main.887ff237.js'",*

 * * "'sourcesContent'": "[' \\t// install a JSONP callback for chunk loading\\n \\tfunction "*

 * *                     'webpackJsonpCallback(data) {\\n \\t\\tvar chunkIds = data[0];\\n \\t\\tvar '*

 * *                     'moreModules = data[1];\\n \\t\\tvar executeModules = data[2];\\n\\n \\t\\t// '*

 * *                     'add "moreModules" to the modules object,\\n \\t\\t// then flag all '*

 * *                     '"chunkIds" as loaded and fire callback\\n \\t\\tvar modul […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "static/js/runtime-main.eaac28ce.js",
+    "file": "static/js/runtime-main.887ff237.js",
     "mappings": "aACE,SAASA,EAAqBC,GAQ7B,IAPA,IAMIC,EAAUC,EANVC,EAAWH,EAAK,GAChBI,EAAcJ,EAAK,GACnBK,EAAiBL,EAAK,GAIHM,EAAI,EAAGC,EAAW,GACpCD,EAAIH,EAASK,OAAQF,IACzBJ,EAAUC,EAASG,GAChBG,OAAOC,UAAUC,eAAeC,KAAKC,EAAiBX,IAAYW,EAAgBX,IACpFK,EAASO,KAAKD,EAAgBX,GAAS,IAExCW,EAAgBX,GAAW,EAE5B,IAAID,KAAYG,EACZK,OAAOC,UAAUC,eAAeC,KAAKR,EAAaH,KACpDc,EAAQd,GAAYG,EAAYH,IAKlC,IAFGe,GAAqBA,EAAoBhB,GAEtCO,EAASC,QACdD,EAASU,OAATV,GAOD,OAHAW,EAAgBJ,KAAKK,MAAMD,EAAiBb,GAAkB,IAGvDe,GACR,CACA,SAASA,IAER,IADA,IAAIC,EACIf,EAAI,EAAGA,EAAIY,EAAgBV,OAAQF,IAAK,CAG/C,IAFA,IAAIgB,EAAiBJ,EAAgBZ,GACjCiB,GAAY,EACRC,EAAI,EAAGA,EAAIF,EAAed,OAAQgB,IAAK,CAC9C,IAAIC,EAAQH,EAAeE,GACG,IAA3BX,EAAgBY,KAAcF,GAAY,EAC9C,CACGA,IACFL,EAAgBQ,OAAOpB,IAAK,GAC5Be,EAASM,EAAoBA,EAAoBC,EAAIN,EAAe,IAEtE,CAEA,OAAOD,CACR,CAGA,IAAIQ,EAAmB,CAAC,EAGpBC,EAAqB,CACxB,EAAG,GAMAjB,EAAkB,CACrB,EAAG,GAGAK,EAAkB,GAQtB,SAASS,EAAoB1B,GAG5B,GAAG4B,EAAiB5B,GACnB,OAAO4B,EAAiB5B,GAAU8B,QAGnC,IAAIC,EAASH,EAAiB5B,GAAY,CACzCK,EAAGL,EACHgC,GAAG,EACHF,QAAS,CAAC,GAUX,OANAhB,EAAQd,GAAUW,KAAKoB,EAAOD,QAASC,EAAQA,EAAOD,QAASJ,GAG/DK,EAAOC,GAAI,EAGJD,EAAOD,OACf,CAIAJ,EAAoBO,EAAI,SAAuBhC,GAC9C,IAAIiC,EAAW,GAKZL,EAAmB5B,GAAUiC,EAASrB,KAAKgB,EAAmB5B,IACzB,IAAhC4B,EAAmB5B,IAFX,CAAC,EAAI,EAAE,EAAI,EAAE,EAAI,EAAE,EAAI,EAAE,EAAI,EAAE,EAAI,EAAE,EAAI,EAAE,GAAK,EAAE,GAAK,EAAE,GAAK,EAAE,GAAK,EAAE,GAAK,EAAE,GAAK,EAAE,GAAK,EAAE,GAAK,EAAE,GAAK,EAAE,GAAK,GAExEA,IACtDiC,EAASrB,KAAKgB,EAAmB5B,GAAW,IAAIkC,SAAQ,SAASC,EAASC,GAIzE,IAHA,IAAIC,EAAO,eAAiB,CAAC,EAAErC,IAAUA,GAAW,IAAM,CAAC,EAAI,WAAW,EAAI,WAAW,EAAI,WAAW,EAAI,WAAW,EAAI,WAAW,EAAI,WAAW,EAAI,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,YAAYA,GAAW,aAC5UsC,EAAWb,EAAoBc,EAAIF,EACnCG,EAAmBC,SAASC,qBAAqB,QAC7CtC,EAAI,EAAGA,EAAIoC,EAAiBlC,OAAQF,IAAK,CAChD,IACIuC,GADAC,EAAMJ,EAAiBpC,IACRyC,aAAa,cAAgBD,EAAIC,aAAa,QACjE,GAAe,eAAZD,EAAIE,MAAyBH,IAAaN,GAAQM,IAAaL,GAAW,OAAOH,GACrF,CACA,IAAIY,EAAoBN,SAASC,qBAAqB,SACtD,IAAQtC,EAAI,EAAGA,EAAI2C,EAAkBzC,OAAQF,IAAK,CACjD,IAAIwC,EAEJ,IADID,GADAC,EAAMG,EAAkB3C,IACTyC,aAAa,gBAChBR,GAAQM,IAAaL,EAAU,OAAOH,GACvD,CACA,IAAIa,EAAUP,SAASQ,cAAc,QACrCD,EAAQF,IAAM,aACdE,EAAQE,KAAO,WACfF,EAAQG,OAAShB,EACjBa,EAAQI,QAAU,SAASC,GAC1B,IAAIC,EAAUD,GAASA,EAAME,QAAUF,EAAME,OAAOC,KAAOlB,EACvDmB,EAAM,IAAIC,MAAM,qBAAuB1D,EAAU,cAAgBsD,EAAU,KAC/EG,EAAIE,KAAO,wBACXF,EAAIH,QAAUA,SACP1B,EAAmB5B,GAC1BgD,EAAQY,WAAWC,YAAYb,GAC/BZ,EAAOqB,EACR,EACAT,EAAQX,KAAOC,EAEJG,SAASC,qBAAqB,QAAQ,GAC5CoB,YAAYd,EAClB,IAAGe,MAAK,WACPnC,EAAmB5B,GAAW,CAC/B,KAKD,IAAIgE,EAAqBrD,EAAgBX,GACzC,GAA0B,IAAvBgE,EAGF,GAAGA,EACF/B,EAASrB,KAAKoD,EAAmB,QAC3B,CAEN,IAAIC,EAAU,IAAI/B,SAAQ,SAASC,EAASC,GAC3C4B,EAAqBrD,EAAgBX,GAAW,CAACmC,EAASC,EAC3D,IACAH,EAASrB,KAAKoD,EAAmB,GAAKC,GAGtC,IACIC,EADAC,EAAS1B,SAASQ,cAAc,UAGpCkB,EAAOC,QAAU,QACjBD,EAAOE,QAAU,IACb5C,EAAoB6C,IACvBH,EAAOI,aAAa,QAAS9C,EAAoB6C,IAElDH,EAAOX,IAnGV,SAAwBxD,GACvB,OAAOyB,EAAoBc,EAAI,cAAgB,CAAC,EAAEvC,IAAUA,GAAW,IAAM,CAAC,EAAI,WAAW,EAAI,WAAW,EAAI,WAAW,EAAI,WAAW,EAAI,WAAW,EAAI,WAAW,EAAI,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,WAAW,GAAK,YAAYA,GAAW,WACpW,CAiGgBwE,CAAexE,GAG5B,IAAIyE,EAAQ,IAAIf,MAChBQ,EAAmB,SAAUb,GAE5Bc,EAAOf,QAAUe,EAAOhB,OAAS,KACjCuB,aAAaL,GACb,IAAIM,EAAQhE,EAAgBX,GAC5B,GAAa,IAAV2E,EAAa,CACf,GAAGA,EAAO,CACT,IAAIC,EAAYvB,IAAyB,SAAfA,EAAMH,KAAkB,UAAYG,EAAMH,MAChE2B,EAAUxB,GAASA,EAAME,QAAUF,EAAME,OAAOC,IACpDiB,EAAMK,QAAU,iBAAmB9E,EAAU,cAAgB4E,EAAY,KAAOC,EAAU,IAC1FJ,EAAMM,KAAO,iBACbN,EAAMvB,KAAO0B,EACbH,EAAMnB,QAAUuB,EAChBF,EAAM,GAAGF,EACV,CACA9D,EAAgBX,QAAWgF,CAC5B,CACD,EACA,IAAIX,EAAUY,YAAW,WACxBf,EAAiB,CAAEhB,KAAM,UAAWK,OAAQY,GAC7C,GAAG,MACHA,EAAOf,QAAUe,EAAOhB,OAASe,EACjCzB,SAASyC,KAAKpB,YAAYK,EAC3B,CAED,OAAOjC,QAAQiD,IAAIlD,EACpB,EAGAR,EAAoB2D,EAAIvE,EAGxBY,EAAoB4D,EAAI1D,EAGxBF,EAAoB6D,EAAI,SAASzD,EAASkD,EAAMQ,GAC3C9D,EAAoB+D,EAAE3D,EAASkD,IAClCxE,OAAOkF,eAAe5D,EAASkD,EAAM,CAAEW,YAAY,EAAMC,IAAKJ,GAEhE,EAGA9D,EAAoBmE,EAAI,SAAS/D,GACX,qBAAXgE,QAA0BA,OAAOC,aAC1CvF,OAAOkF,eAAe5D,EAASgE,OAAOC,YAAa,CAAEC,MAAO,WAE7DxF,OAAOkF,eAAe5D,EAAS,aAAc,CAAEkE,OAAO,GACvD,EAOAtE,EAAoBuE,EAAI,SAASD,EAAOE,GAEvC,GADU,EAAPA,IAAUF,EAAQtE,EAAoBsE,IAC/B,EAAPE,EAAU,OAAOF,EACpB,GAAW,EAAPE,GAA8B,kBAAVF,GAAsBA,GAASA,EAAMG,WAAY,OAAOH,EAChF,IAAII,EAAK5F,OAAO6F,OAAO,MAGvB,GAFA3E,EAAoBmE,EAAEO,GACtB5F,OAAOkF,eAAeU,EAAI,UAAW,CAAET,YAAY,EAAMK,MAAOA,IACtD,EAAPE,GAA4B,iBAATF,EAAmB,IAAI,IAAIM,KAAON,EAAOtE,EAAoB6D,EAAEa,EAAIE,EAAK,SAASA,GAAO,OAAON,EAAMM,EAAM,EAAEC,KAAK,KAAMD,IAC9I,OAAOF,CACR,EAGA1E,EAAoB8E,EAAI,SAASzE,GAChC,IAAIyD,EAASzD,GAAUA,EAAOoE,WAC7B,WAAwB,OAAOpE,EAAgB,OAAG,EAClD,WAA8B,OAAOA,CAAQ,EAE9C,OADAL,EAAoB6D,EAAEC,EAAQ,IAAKA,GAC5BA,CACR,EAGA9D,EAAoB+D,EAAI,SAASgB,EAAQC,GAAY,OAAOlG,OAAOC,UAAUC,eAAeC,KAAK8F,EAAQC,EAAW,EAGpHhF,EAAoBc,EAAI,KAGxBd,EAAoBiF,GAAK,SAASjD,GAA2B,MAApBkD,QAAQlC,MAAMhB,GAAYA,CAAK,EAExE,IAAImD,EAAaC,KAA+C,yCAAIA,KAA+C,0CAAK,GACpHC,EAAmBF,EAAWhG,KAAK0F,KAAKM,GAC5CA,EAAWhG,KAAOf,EAClB+G,EAAaA,EAAWG,QACxB,IAAI,IAAI3G,EAAI,EAAGA,EAAIwG,EAAWtG,OAAQF,IAAKP,EAAqB+G,EAAWxG,IAC3E,IAAIU,EAAsBgG,EAI1B5F,G",
     "names": [
         "webpackJsonpCallback",
         "data",
         "moduleId",
         "chunkId",
         "chunkIds",
@@ -119,11 +119,11 @@
         "slice"
     ],
     "sourceRoot": "",
     "sources": [
         "../webpack/bootstrap"
     ],
     "sourcesContent": [
-        " \t// install a JSONP callback for chunk loading\n \tfunction webpackJsonpCallback(data) {\n \t\tvar chunkIds = data[0];\n \t\tvar moreModules = data[1];\n \t\tvar executeModules = data[2];\n\n \t\t// add \"moreModules\" to the modules object,\n \t\t// then flag all \"chunkIds\" as loaded and fire callback\n \t\tvar moduleId, chunkId, i = 0, resolves = [];\n \t\tfor(;i < chunkIds.length; i++) {\n \t\t\tchunkId = chunkIds[i];\n \t\t\tif(Object.prototype.hasOwnProperty.call(installedChunks, chunkId) && installedChunks[chunkId]) {\n \t\t\t\tresolves.push(installedChunks[chunkId][0]);\n \t\t\t}\n \t\t\tinstalledChunks[chunkId] = 0;\n \t\t}\n \t\tfor(moduleId in moreModules) {\n \t\t\tif(Object.prototype.hasOwnProperty.call(moreModules, moduleId)) {\n \t\t\t\tmodules[moduleId] = moreModules[moduleId];\n \t\t\t}\n \t\t}\n \t\tif(parentJsonpFunction) parentJsonpFunction(data);\n\n \t\twhile(resolves.length) {\n \t\t\tresolves.shift()();\n \t\t}\n\n \t\t// add entry modules from loaded chunk to deferred list\n \t\tdeferredModules.push.apply(deferredModules, executeModules || []);\n\n \t\t// run deferred modules when all chunks ready\n \t\treturn checkDeferredModules();\n \t};\n \tfunction checkDeferredModules() {\n \t\tvar result;\n \t\tfor(var i = 0; i < deferredModules.length; i++) {\n \t\t\tvar deferredModule = deferredModules[i];\n \t\t\tvar fulfilled = true;\n \t\t\tfor(var j = 1; j < deferredModule.length; j++) {\n \t\t\t\tvar depId = deferredModule[j];\n \t\t\t\tif(installedChunks[depId] !== 0) fulfilled = false;\n \t\t\t}\n \t\t\tif(fulfilled) {\n \t\t\t\tdeferredModules.splice(i--, 1);\n \t\t\t\tresult = __webpack_require__(__webpack_require__.s = deferredModule[0]);\n \t\t\t}\n \t\t}\n\n \t\treturn result;\n \t}\n\n \t// The module cache\n \tvar installedModules = {};\n\n \t// object to store loaded CSS chunks\n \tvar installedCssChunks = {\n \t\t1: 0\n \t};\n\n \t// object to store loaded and loading chunks\n \t// undefined = chunk not loaded, null = chunk preloaded/prefetched\n \t// Promise = chunk loading, 0 = chunk loaded\n \tvar installedChunks = {\n \t\t1: 0\n \t};\n\n \tvar deferredModules = [];\n\n \t// script path function\n \tfunction jsonpScriptSrc(chunkId) {\n \t\treturn __webpack_require__.p + \"static/js/\" + ({}[chunkId]||chunkId) + \".\" + {\"3\":\"d30f1cfd\",\"4\":\"ec7a53ea\",\"5\":\"e42b3133\",\"6\":\"e9192981\",\"7\":\"be794506\",\"8\":\"15dd3b20\",\"9\":\"119f08fa\",\"10\":\"18fc5a6d\",\"11\":\"e2b8452b\",\"12\":\"6c6d4448\",\"13\":\"c5f703d1\",\"14\":\"39efed4e\",\"15\":\"7665d197\",\"16\":\"4a5a2671\",\"17\":\"e0e3c073\",\"18\":\"b265fc2b\",\"19\":\"5ba3da56\"}[chunkId] + \".chunk.js\"\n \t}\n\n \t// The require function\n \tfunction __webpack_require__(moduleId) {\n\n \t\t// Check if module is in cache\n \t\tif(installedModules[moduleId]) {\n \t\t\treturn installedModules[moduleId].exports;\n \t\t}\n \t\t// Create a new module (and put it into the cache)\n \t\tvar module = installedModules[moduleId] = {\n \t\t\ti: moduleId,\n \t\t\tl: false,\n \t\t\texports: {}\n \t\t};\n\n \t\t// Execute the module function\n \t\tmodules[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n \t\t// Flag the module as loaded\n \t\tmodule.l = true;\n\n \t\t// Return the exports of the module\n \t\treturn module.exports;\n \t}\n\n \t// This file contains only the entry chunk.\n \t// The chunk loading function for additional chunks\n \t__webpack_require__.e = function requireEnsure(chunkId) {\n \t\tvar promises = [];\n\n\n \t\t// mini-css-extract-plugin CSS loading\n \t\tvar cssChunks = {\"3\":1,\"4\":1,\"5\":1,\"6\":1,\"7\":1,\"8\":1,\"9\":1,\"10\":1,\"11\":1,\"12\":1,\"13\":1,\"14\":1,\"15\":1,\"16\":1,\"17\":1,\"18\":1,\"19\":1};\n \t\tif(installedCssChunks[chunkId]) promises.push(installedCssChunks[chunkId]);\n \t\telse if(installedCssChunks[chunkId] !== 0 && cssChunks[chunkId]) {\n \t\t\tpromises.push(installedCssChunks[chunkId] = new Promise(function(resolve, reject) {\n \t\t\t\tvar href = \"static/css/\" + ({}[chunkId]||chunkId) + \".\" + {\"3\":\"11f8848d\",\"4\":\"2fe0cb1b\",\"5\":\"5a2b8ee3\",\"6\":\"1b9cee33\",\"7\":\"4e275de2\",\"8\":\"eb5abf62\",\"9\":\"1253a161\",\"10\":\"1f3244e3\",\"11\":\"cb699f02\",\"12\":\"158b51eb\",\"13\":\"74908590\",\"14\":\"e64fc659\",\"15\":\"3adba626\",\"16\":\"b573d318\",\"17\":\"10a8300f\",\"18\":\"4eb3e38a\",\"19\":\"74b97645\"}[chunkId] + \".chunk.css\";\n \t\t\t\tvar fullhref = __webpack_require__.p + href;\n \t\t\t\tvar existingLinkTags = document.getElementsByTagName(\"link\");\n \t\t\t\tfor(var i = 0; i < existingLinkTags.length; i++) {\n \t\t\t\t\tvar tag = existingLinkTags[i];\n \t\t\t\t\tvar dataHref = tag.getAttribute(\"data-href\") || tag.getAttribute(\"href\");\n \t\t\t\t\tif(tag.rel === \"stylesheet\" && (dataHref === href || dataHref === fullhref)) return resolve();\n \t\t\t\t}\n \t\t\t\tvar existingStyleTags = document.getElementsByTagName(\"style\");\n \t\t\t\tfor(var i = 0; i < existingStyleTags.length; i++) {\n \t\t\t\t\tvar tag = existingStyleTags[i];\n \t\t\t\t\tvar dataHref = tag.getAttribute(\"data-href\");\n \t\t\t\t\tif(dataHref === href || dataHref === fullhref) return resolve();\n \t\t\t\t}\n \t\t\t\tvar linkTag = document.createElement(\"link\");\n \t\t\t\tlinkTag.rel = \"stylesheet\";\n \t\t\t\tlinkTag.type = \"text/css\";\n \t\t\t\tlinkTag.onload = resolve;\n \t\t\t\tlinkTag.onerror = function(event) {\n \t\t\t\t\tvar request = event && event.target && event.target.src || fullhref;\n \t\t\t\t\tvar err = new Error(\"Loading CSS chunk \" + chunkId + \" failed.\\n(\" + request + \")\");\n \t\t\t\t\terr.code = \"CSS_CHUNK_LOAD_FAILED\";\n \t\t\t\t\terr.request = request;\n \t\t\t\t\tdelete installedCssChunks[chunkId]\n \t\t\t\t\tlinkTag.parentNode.removeChild(linkTag)\n \t\t\t\t\treject(err);\n \t\t\t\t};\n \t\t\t\tlinkTag.href = fullhref;\n\n \t\t\t\tvar head = document.getElementsByTagName(\"head\")[0];\n \t\t\t\thead.appendChild(linkTag);\n \t\t\t}).then(function() {\n \t\t\t\tinstalledCssChunks[chunkId] = 0;\n \t\t\t}));\n \t\t}\n\n \t\t// JSONP chunk loading for javascript\n\n \t\tvar installedChunkData = installedChunks[chunkId];\n \t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n \t\t\t// a Promise means \"currently loading\".\n \t\t\tif(installedChunkData) {\n \t\t\t\tpromises.push(installedChunkData[2]);\n \t\t\t} else {\n \t\t\t\t// setup Promise in chunk cache\n \t\t\t\tvar promise = new Promise(function(resolve, reject) {\n \t\t\t\t\tinstalledChunkData = installedChunks[chunkId] = [resolve, reject];\n \t\t\t\t});\n \t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n \t\t\t\t// start chunk loading\n \t\t\t\tvar script = document.createElement('script');\n \t\t\t\tvar onScriptComplete;\n\n \t\t\t\tscript.charset = 'utf-8';\n \t\t\t\tscript.timeout = 120;\n \t\t\t\tif (__webpack_require__.nc) {\n \t\t\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n \t\t\t\t}\n \t\t\t\tscript.src = jsonpScriptSrc(chunkId);\n\n \t\t\t\t// create error before stack unwound to get useful stacktrace later\n \t\t\t\tvar error = new Error();\n \t\t\t\tonScriptComplete = function (event) {\n \t\t\t\t\t// avoid mem leaks in IE.\n \t\t\t\t\tscript.onerror = script.onload = null;\n \t\t\t\t\tclearTimeout(timeout);\n \t\t\t\t\tvar chunk = installedChunks[chunkId];\n \t\t\t\t\tif(chunk !== 0) {\n \t\t\t\t\t\tif(chunk) {\n \t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n \t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n \t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n \t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n \t\t\t\t\t\t\terror.type = errorType;\n \t\t\t\t\t\t\terror.request = realSrc;\n \t\t\t\t\t\t\tchunk[1](error);\n \t\t\t\t\t\t}\n \t\t\t\t\t\tinstalledChunks[chunkId] = undefined;\n \t\t\t\t\t}\n \t\t\t\t};\n \t\t\t\tvar timeout = setTimeout(function(){\n \t\t\t\t\tonScriptComplete({ type: 'timeout', target: script });\n \t\t\t\t}, 120000);\n \t\t\t\tscript.onerror = script.onload = onScriptComplete;\n \t\t\t\tdocument.head.appendChild(script);\n \t\t\t}\n \t\t}\n \t\treturn Promise.all(promises);\n \t};\n\n \t// expose the modules object (__webpack_modules__)\n \t__webpack_require__.m = modules;\n\n \t// expose the module cache\n \t__webpack_require__.c = installedModules;\n\n \t// define getter function for harmony exports\n \t__webpack_require__.d = function(exports, name, getter) {\n \t\tif(!__webpack_require__.o(exports, name)) {\n \t\t\tObject.defineProperty(exports, name, { enumerable: true, get: getter });\n \t\t}\n \t};\n\n \t// define __esModule on exports\n \t__webpack_require__.r = function(exports) {\n \t\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n \t\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n \t\t}\n \t\tObject.defineProperty(exports, '__esModule', { value: true });\n \t};\n\n \t// create a fake namespace object\n \t// mode & 1: value is a module id, require it\n \t// mode & 2: merge all properties of value into the ns\n \t// mode & 4: return value when already ns object\n \t// mode & 8|1: behave like require\n \t__webpack_require__.t = function(value, mode) {\n \t\tif(mode & 1) value = __webpack_require__(value);\n \t\tif(mode & 8) return value;\n \t\tif((mode & 4) && typeof value === 'object' && value && value.__esModule) return value;\n \t\tvar ns = Object.create(null);\n \t\t__webpack_require__.r(ns);\n \t\tObject.defineProperty(ns, 'default', { enumerable: true, value: value });\n \t\tif(mode & 2 && typeof value != 'string') for(var key in value) __webpack_require__.d(ns, key, function(key) { return value[key]; }.bind(null, key));\n \t\treturn ns;\n \t};\n\n \t// getDefaultExport function for compatibility with non-harmony modules\n \t__webpack_require__.n = function(module) {\n \t\tvar getter = module && module.__esModule ?\n \t\t\tfunction getDefault() { return module['default']; } :\n \t\t\tfunction getModuleExports() { return module; };\n \t\t__webpack_require__.d(getter, 'a', getter);\n \t\treturn getter;\n \t};\n\n \t// Object.prototype.hasOwnProperty.call\n \t__webpack_require__.o = function(object, property) { return Object.prototype.hasOwnProperty.call(object, property); };\n\n \t// __webpack_public_path__\n \t__webpack_require__.p = \"./\";\n\n \t// on error function for async loading\n \t__webpack_require__.oe = function(err) { console.error(err); throw err; };\n\n \tvar jsonpArray = this[\"webpackJsonpstreamlit_component_template\"] = this[\"webpackJsonpstreamlit_component_template\"] || [];\n \tvar oldJsonpFunction = jsonpArray.push.bind(jsonpArray);\n \tjsonpArray.push = webpackJsonpCallback;\n \tjsonpArray = jsonpArray.slice();\n \tfor(var i = 0; i < jsonpArray.length; i++) webpackJsonpCallback(jsonpArray[i]);\n \tvar parentJsonpFunction = oldJsonpFunction;\n\n\n \t// run deferred modules from other chunks\n \tcheckDeferredModules();\n"
+        " \t// install a JSONP callback for chunk loading\n \tfunction webpackJsonpCallback(data) {\n \t\tvar chunkIds = data[0];\n \t\tvar moreModules = data[1];\n \t\tvar executeModules = data[2];\n\n \t\t// add \"moreModules\" to the modules object,\n \t\t// then flag all \"chunkIds\" as loaded and fire callback\n \t\tvar moduleId, chunkId, i = 0, resolves = [];\n \t\tfor(;i < chunkIds.length; i++) {\n \t\t\tchunkId = chunkIds[i];\n \t\t\tif(Object.prototype.hasOwnProperty.call(installedChunks, chunkId) && installedChunks[chunkId]) {\n \t\t\t\tresolves.push(installedChunks[chunkId][0]);\n \t\t\t}\n \t\t\tinstalledChunks[chunkId] = 0;\n \t\t}\n \t\tfor(moduleId in moreModules) {\n \t\t\tif(Object.prototype.hasOwnProperty.call(moreModules, moduleId)) {\n \t\t\t\tmodules[moduleId] = moreModules[moduleId];\n \t\t\t}\n \t\t}\n \t\tif(parentJsonpFunction) parentJsonpFunction(data);\n\n \t\twhile(resolves.length) {\n \t\t\tresolves.shift()();\n \t\t}\n\n \t\t// add entry modules from loaded chunk to deferred list\n \t\tdeferredModules.push.apply(deferredModules, executeModules || []);\n\n \t\t// run deferred modules when all chunks ready\n \t\treturn checkDeferredModules();\n \t};\n \tfunction checkDeferredModules() {\n \t\tvar result;\n \t\tfor(var i = 0; i < deferredModules.length; i++) {\n \t\t\tvar deferredModule = deferredModules[i];\n \t\t\tvar fulfilled = true;\n \t\t\tfor(var j = 1; j < deferredModule.length; j++) {\n \t\t\t\tvar depId = deferredModule[j];\n \t\t\t\tif(installedChunks[depId] !== 0) fulfilled = false;\n \t\t\t}\n \t\t\tif(fulfilled) {\n \t\t\t\tdeferredModules.splice(i--, 1);\n \t\t\t\tresult = __webpack_require__(__webpack_require__.s = deferredModule[0]);\n \t\t\t}\n \t\t}\n\n \t\treturn result;\n \t}\n\n \t// The module cache\n \tvar installedModules = {};\n\n \t// object to store loaded CSS chunks\n \tvar installedCssChunks = {\n \t\t1: 0\n \t};\n\n \t// object to store loaded and loading chunks\n \t// undefined = chunk not loaded, null = chunk preloaded/prefetched\n \t// Promise = chunk loading, 0 = chunk loaded\n \tvar installedChunks = {\n \t\t1: 0\n \t};\n\n \tvar deferredModules = [];\n\n \t// script path function\n \tfunction jsonpScriptSrc(chunkId) {\n \t\treturn __webpack_require__.p + \"static/js/\" + ({}[chunkId]||chunkId) + \".\" + {\"3\":\"a17c1b63\",\"4\":\"c8e4936c\",\"5\":\"ab74786f\",\"6\":\"7f9bbd64\",\"7\":\"887bb0a8\",\"8\":\"0121e917\",\"9\":\"e6c78b5a\",\"10\":\"442a54e9\",\"11\":\"6dd2762e\",\"12\":\"b5132789\",\"13\":\"155b252b\",\"14\":\"124342a7\",\"15\":\"1df3933b\",\"16\":\"e98baccf\",\"17\":\"f47ed1b3\",\"18\":\"bbe30a24\",\"19\":\"63982437\"}[chunkId] + \".chunk.js\"\n \t}\n\n \t// The require function\n \tfunction __webpack_require__(moduleId) {\n\n \t\t// Check if module is in cache\n \t\tif(installedModules[moduleId]) {\n \t\t\treturn installedModules[moduleId].exports;\n \t\t}\n \t\t// Create a new module (and put it into the cache)\n \t\tvar module = installedModules[moduleId] = {\n \t\t\ti: moduleId,\n \t\t\tl: false,\n \t\t\texports: {}\n \t\t};\n\n \t\t// Execute the module function\n \t\tmodules[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n \t\t// Flag the module as loaded\n \t\tmodule.l = true;\n\n \t\t// Return the exports of the module\n \t\treturn module.exports;\n \t}\n\n \t// This file contains only the entry chunk.\n \t// The chunk loading function for additional chunks\n \t__webpack_require__.e = function requireEnsure(chunkId) {\n \t\tvar promises = [];\n\n\n \t\t// mini-css-extract-plugin CSS loading\n \t\tvar cssChunks = {\"3\":1,\"4\":1,\"5\":1,\"6\":1,\"7\":1,\"8\":1,\"9\":1,\"10\":1,\"11\":1,\"12\":1,\"13\":1,\"14\":1,\"15\":1,\"16\":1,\"17\":1,\"18\":1,\"19\":1};\n \t\tif(installedCssChunks[chunkId]) promises.push(installedCssChunks[chunkId]);\n \t\telse if(installedCssChunks[chunkId] !== 0 && cssChunks[chunkId]) {\n \t\t\tpromises.push(installedCssChunks[chunkId] = new Promise(function(resolve, reject) {\n \t\t\t\tvar href = \"static/css/\" + ({}[chunkId]||chunkId) + \".\" + {\"3\":\"11f8848d\",\"4\":\"2fe0cb1b\",\"5\":\"5a2b8ee3\",\"6\":\"1b9cee33\",\"7\":\"4e275de2\",\"8\":\"eb5abf62\",\"9\":\"1253a161\",\"10\":\"1f3244e3\",\"11\":\"cb699f02\",\"12\":\"158b51eb\",\"13\":\"74908590\",\"14\":\"e64fc659\",\"15\":\"3adba626\",\"16\":\"b573d318\",\"17\":\"10a8300f\",\"18\":\"4eb3e38a\",\"19\":\"74b97645\"}[chunkId] + \".chunk.css\";\n \t\t\t\tvar fullhref = __webpack_require__.p + href;\n \t\t\t\tvar existingLinkTags = document.getElementsByTagName(\"link\");\n \t\t\t\tfor(var i = 0; i < existingLinkTags.length; i++) {\n \t\t\t\t\tvar tag = existingLinkTags[i];\n \t\t\t\t\tvar dataHref = tag.getAttribute(\"data-href\") || tag.getAttribute(\"href\");\n \t\t\t\t\tif(tag.rel === \"stylesheet\" && (dataHref === href || dataHref === fullhref)) return resolve();\n \t\t\t\t}\n \t\t\t\tvar existingStyleTags = document.getElementsByTagName(\"style\");\n \t\t\t\tfor(var i = 0; i < existingStyleTags.length; i++) {\n \t\t\t\t\tvar tag = existingStyleTags[i];\n \t\t\t\t\tvar dataHref = tag.getAttribute(\"data-href\");\n \t\t\t\t\tif(dataHref === href || dataHref === fullhref) return resolve();\n \t\t\t\t}\n \t\t\t\tvar linkTag = document.createElement(\"link\");\n \t\t\t\tlinkTag.rel = \"stylesheet\";\n \t\t\t\tlinkTag.type = \"text/css\";\n \t\t\t\tlinkTag.onload = resolve;\n \t\t\t\tlinkTag.onerror = function(event) {\n \t\t\t\t\tvar request = event && event.target && event.target.src || fullhref;\n \t\t\t\t\tvar err = new Error(\"Loading CSS chunk \" + chunkId + \" failed.\\n(\" + request + \")\");\n \t\t\t\t\terr.code = \"CSS_CHUNK_LOAD_FAILED\";\n \t\t\t\t\terr.request = request;\n \t\t\t\t\tdelete installedCssChunks[chunkId]\n \t\t\t\t\tlinkTag.parentNode.removeChild(linkTag)\n \t\t\t\t\treject(err);\n \t\t\t\t};\n \t\t\t\tlinkTag.href = fullhref;\n\n \t\t\t\tvar head = document.getElementsByTagName(\"head\")[0];\n \t\t\t\thead.appendChild(linkTag);\n \t\t\t}).then(function() {\n \t\t\t\tinstalledCssChunks[chunkId] = 0;\n \t\t\t}));\n \t\t}\n\n \t\t// JSONP chunk loading for javascript\n\n \t\tvar installedChunkData = installedChunks[chunkId];\n \t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n \t\t\t// a Promise means \"currently loading\".\n \t\t\tif(installedChunkData) {\n \t\t\t\tpromises.push(installedChunkData[2]);\n \t\t\t} else {\n \t\t\t\t// setup Promise in chunk cache\n \t\t\t\tvar promise = new Promise(function(resolve, reject) {\n \t\t\t\t\tinstalledChunkData = installedChunks[chunkId] = [resolve, reject];\n \t\t\t\t});\n \t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n \t\t\t\t// start chunk loading\n \t\t\t\tvar script = document.createElement('script');\n \t\t\t\tvar onScriptComplete;\n\n \t\t\t\tscript.charset = 'utf-8';\n \t\t\t\tscript.timeout = 120;\n \t\t\t\tif (__webpack_require__.nc) {\n \t\t\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n \t\t\t\t}\n \t\t\t\tscript.src = jsonpScriptSrc(chunkId);\n\n \t\t\t\t// create error before stack unwound to get useful stacktrace later\n \t\t\t\tvar error = new Error();\n \t\t\t\tonScriptComplete = function (event) {\n \t\t\t\t\t// avoid mem leaks in IE.\n \t\t\t\t\tscript.onerror = script.onload = null;\n \t\t\t\t\tclearTimeout(timeout);\n \t\t\t\t\tvar chunk = installedChunks[chunkId];\n \t\t\t\t\tif(chunk !== 0) {\n \t\t\t\t\t\tif(chunk) {\n \t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n \t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n \t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n \t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n \t\t\t\t\t\t\terror.type = errorType;\n \t\t\t\t\t\t\terror.request = realSrc;\n \t\t\t\t\t\t\tchunk[1](error);\n \t\t\t\t\t\t}\n \t\t\t\t\t\tinstalledChunks[chunkId] = undefined;\n \t\t\t\t\t}\n \t\t\t\t};\n \t\t\t\tvar timeout = setTimeout(function(){\n \t\t\t\t\tonScriptComplete({ type: 'timeout', target: script });\n \t\t\t\t}, 120000);\n \t\t\t\tscript.onerror = script.onload = onScriptComplete;\n \t\t\t\tdocument.head.appendChild(script);\n \t\t\t}\n \t\t}\n \t\treturn Promise.all(promises);\n \t};\n\n \t// expose the modules object (__webpack_modules__)\n \t__webpack_require__.m = modules;\n\n \t// expose the module cache\n \t__webpack_require__.c = installedModules;\n\n \t// define getter function for harmony exports\n \t__webpack_require__.d = function(exports, name, getter) {\n \t\tif(!__webpack_require__.o(exports, name)) {\n \t\t\tObject.defineProperty(exports, name, { enumerable: true, get: getter });\n \t\t}\n \t};\n\n \t// define __esModule on exports\n \t__webpack_require__.r = function(exports) {\n \t\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n \t\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n \t\t}\n \t\tObject.defineProperty(exports, '__esModule', { value: true });\n \t};\n\n \t// create a fake namespace object\n \t// mode & 1: value is a module id, require it\n \t// mode & 2: merge all properties of value into the ns\n \t// mode & 4: return value when already ns object\n \t// mode & 8|1: behave like require\n \t__webpack_require__.t = function(value, mode) {\n \t\tif(mode & 1) value = __webpack_require__(value);\n \t\tif(mode & 8) return value;\n \t\tif((mode & 4) && typeof value === 'object' && value && value.__esModule) return value;\n \t\tvar ns = Object.create(null);\n \t\t__webpack_require__.r(ns);\n \t\tObject.defineProperty(ns, 'default', { enumerable: true, value: value });\n \t\tif(mode & 2 && typeof value != 'string') for(var key in value) __webpack_require__.d(ns, key, function(key) { return value[key]; }.bind(null, key));\n \t\treturn ns;\n \t};\n\n \t// getDefaultExport function for compatibility with non-harmony modules\n \t__webpack_require__.n = function(module) {\n \t\tvar getter = module && module.__esModule ?\n \t\t\tfunction getDefault() { return module['default']; } :\n \t\t\tfunction getModuleExports() { return module; };\n \t\t__webpack_require__.d(getter, 'a', getter);\n \t\treturn getter;\n \t};\n\n \t// Object.prototype.hasOwnProperty.call\n \t__webpack_require__.o = function(object, property) { return Object.prototype.hasOwnProperty.call(object, property); };\n\n \t// __webpack_public_path__\n \t__webpack_require__.p = \"./\";\n\n \t// on error function for async loading\n \t__webpack_require__.oe = function(err) { console.error(err); throw err; };\n\n \tvar jsonpArray = this[\"webpackJsonpstreamlit_component_template\"] = this[\"webpackJsonpstreamlit_component_template\"] || [];\n \tvar oldJsonpFunction = jsonpArray.push.bind(jsonpArray);\n \tjsonpArray.push = webpackJsonpCallback;\n \tjsonpArray = jsonpArray.slice();\n \tfor(var i = 0; i < jsonpArray.length; i++) webpackJsonpCallback(jsonpArray[i]);\n \tvar parentJsonpFunction = oldJsonpFunction;\n\n\n \t// run deferred modules from other chunks\n \tcheckDeferredModules();\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-regular.45c54810.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-regular.d1653550.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.6ebea875.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.83db537e.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibold.f11ba60a.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.522a9ee9.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.a43f56ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot` & `streamlit-reveal-slides-0.1.9/reveal_slides/frontend/build/static/media/source-sans-pro-semibolditalic.fb03c660.eot`

 * *Files identical despite different names*

### Comparing `streamlit-reveal-slides-0.1.8/setup.py` & `streamlit-reveal-slides-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-reveal-slides",
-    version="0.1.8",
+    version="0.1.9",
     author="Anas Bouzid",
     author_email="",
     description="reveal.js HTML presentations for streamlit",
     long_description="create and add reveal.js HTML presentations to your streamlit app",
     long_description_content_type="text/plain",
     url="https://github.com/bouzidanas/streamlit.io/tree/master/streamlit-reveal-slides",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-reveal-slides-0.1.8/streamlit_reveal_slides.egg-info/SOURCES.txt` & `streamlit-reveal-slides-0.1.9/streamlit_reveal_slides.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,55 +38,55 @@
 reveal_slides/frontend/build/static/css/6.1b9cee33.chunk.css.map
 reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css
 reveal_slides/frontend/build/static/css/7.4e275de2.chunk.css.map
 reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css
 reveal_slides/frontend/build/static/css/8.eb5abf62.chunk.css.map
 reveal_slides/frontend/build/static/css/9.1253a161.chunk.css
 reveal_slides/frontend/build/static/css/9.1253a161.chunk.css.map
-reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js
-reveal_slides/frontend/build/static/js/10.18fc5a6d.chunk.js.map
-reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js
-reveal_slides/frontend/build/static/js/11.e2b8452b.chunk.js.map
-reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js
-reveal_slides/frontend/build/static/js/12.6c6d4448.chunk.js.map
-reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js
-reveal_slides/frontend/build/static/js/13.c5f703d1.chunk.js.map
-reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js
-reveal_slides/frontend/build/static/js/14.39efed4e.chunk.js.map
-reveal_slides/frontend/build/static/js/15.7665d197.chunk.js
-reveal_slides/frontend/build/static/js/15.7665d197.chunk.js.map
-reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js
-reveal_slides/frontend/build/static/js/16.4a5a2671.chunk.js.map
-reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js
-reveal_slides/frontend/build/static/js/17.e0e3c073.chunk.js.map
-reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js
-reveal_slides/frontend/build/static/js/18.b265fc2b.chunk.js.map
-reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js
-reveal_slides/frontend/build/static/js/19.5ba3da56.chunk.js.map
-reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js
-reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.LICENSE.txt
-reveal_slides/frontend/build/static/js/2.5c1e1a04.chunk.js.map
-reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js
-reveal_slides/frontend/build/static/js/3.d30f1cfd.chunk.js.map
-reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js
-reveal_slides/frontend/build/static/js/4.ec7a53ea.chunk.js.map
-reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js
-reveal_slides/frontend/build/static/js/5.e42b3133.chunk.js.map
-reveal_slides/frontend/build/static/js/6.e9192981.chunk.js
-reveal_slides/frontend/build/static/js/6.e9192981.chunk.js.map
-reveal_slides/frontend/build/static/js/7.be794506.chunk.js
-reveal_slides/frontend/build/static/js/7.be794506.chunk.js.map
-reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js
-reveal_slides/frontend/build/static/js/8.15dd3b20.chunk.js.map
-reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js
-reveal_slides/frontend/build/static/js/9.119f08fa.chunk.js.map
-reveal_slides/frontend/build/static/js/main.639deb8d.chunk.js
-reveal_slides/frontend/build/static/js/main.639deb8d.chunk.js.map
-reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js
-reveal_slides/frontend/build/static/js/runtime-main.eaac28ce.js.map
+reveal_slides/frontend/build/static/js/10.442a54e9.chunk.js
+reveal_slides/frontend/build/static/js/10.442a54e9.chunk.js.map
+reveal_slides/frontend/build/static/js/11.6dd2762e.chunk.js
+reveal_slides/frontend/build/static/js/11.6dd2762e.chunk.js.map
+reveal_slides/frontend/build/static/js/12.b5132789.chunk.js
+reveal_slides/frontend/build/static/js/12.b5132789.chunk.js.map
+reveal_slides/frontend/build/static/js/13.155b252b.chunk.js
+reveal_slides/frontend/build/static/js/13.155b252b.chunk.js.map
+reveal_slides/frontend/build/static/js/14.124342a7.chunk.js
+reveal_slides/frontend/build/static/js/14.124342a7.chunk.js.map
+reveal_slides/frontend/build/static/js/15.1df3933b.chunk.js
+reveal_slides/frontend/build/static/js/15.1df3933b.chunk.js.map
+reveal_slides/frontend/build/static/js/16.e98baccf.chunk.js
+reveal_slides/frontend/build/static/js/16.e98baccf.chunk.js.map
+reveal_slides/frontend/build/static/js/17.f47ed1b3.chunk.js
+reveal_slides/frontend/build/static/js/17.f47ed1b3.chunk.js.map
+reveal_slides/frontend/build/static/js/18.bbe30a24.chunk.js
+reveal_slides/frontend/build/static/js/18.bbe30a24.chunk.js.map
+reveal_slides/frontend/build/static/js/19.63982437.chunk.js
+reveal_slides/frontend/build/static/js/19.63982437.chunk.js.map
+reveal_slides/frontend/build/static/js/2.971d039e.chunk.js
+reveal_slides/frontend/build/static/js/2.971d039e.chunk.js.LICENSE.txt
+reveal_slides/frontend/build/static/js/2.971d039e.chunk.js.map
+reveal_slides/frontend/build/static/js/3.a17c1b63.chunk.js
+reveal_slides/frontend/build/static/js/3.a17c1b63.chunk.js.map
+reveal_slides/frontend/build/static/js/4.c8e4936c.chunk.js
+reveal_slides/frontend/build/static/js/4.c8e4936c.chunk.js.map
+reveal_slides/frontend/build/static/js/5.ab74786f.chunk.js
+reveal_slides/frontend/build/static/js/5.ab74786f.chunk.js.map
+reveal_slides/frontend/build/static/js/6.7f9bbd64.chunk.js
+reveal_slides/frontend/build/static/js/6.7f9bbd64.chunk.js.map
+reveal_slides/frontend/build/static/js/7.887bb0a8.chunk.js
+reveal_slides/frontend/build/static/js/7.887bb0a8.chunk.js.map
+reveal_slides/frontend/build/static/js/8.0121e917.chunk.js
+reveal_slides/frontend/build/static/js/8.0121e917.chunk.js.map
+reveal_slides/frontend/build/static/js/9.e6c78b5a.chunk.js
+reveal_slides/frontend/build/static/js/9.e6c78b5a.chunk.js.map
+reveal_slides/frontend/build/static/js/main.18f5a848.chunk.js
+reveal_slides/frontend/build/static/js/main.18f5a848.chunk.js.map
+reveal_slides/frontend/build/static/js/runtime-main.887ff237.js
+reveal_slides/frontend/build/static/js/runtime-main.887ff237.js.map
 reveal_slides/frontend/build/static/media/league-gothic.080eee2a.woff
 reveal_slides/frontend/build/static/media/league-gothic.12baac5d.eot
 reveal_slides/frontend/build/static/media/league-gothic.6ae91382.ttf
 reveal_slides/frontend/build/static/media/source-sans-pro-italic.10a5cb40.ttf
 reveal_slides/frontend/build/static/media/source-sans-pro-italic.97e79d3e.eot
 reveal_slides/frontend/build/static/media/source-sans-pro-italic.983d97ca.woff
 reveal_slides/frontend/build/static/media/source-sans-pro-regular.36443d24.eot
```
